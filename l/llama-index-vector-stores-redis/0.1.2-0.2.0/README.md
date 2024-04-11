# Comparing `tmp/llama_index_vector_stores_redis-0.1.2.tar.gz` & `tmp/llama_index_vector_stores_redis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_redis-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_redis-0.2.0.tar", max compression
```

## Comparing `llama_index_vector_stores_redis-0.1.2.tar` & `llama_index_vector_stores_redis-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       46 2024-02-13 13:53:02.021667 llama_index_vector_stores_redis-0.1.2/README.md
--rw-r--r--   0        0        0       98 2024-02-13 13:53:02.021911 llama_index_vector_stores_redis-0.1.2/llama_index/vector_stores/redis/__init__.py
--rw-r--r--   0        0        0    16950 2024-02-13 13:53:02.021988 llama_index_vector_stores_redis-0.1.2/llama_index/vector_stores/redis/base.py
--rw-r--r--   0        0        0     3406 2024-02-13 13:53:02.022067 llama_index_vector_stores_redis-0.1.2/llama_index/vector_stores/redis/utils.py
--rw-r--r--   0        0        0     1472 2024-02-21 23:38:30.845634 llama_index_vector_stores_redis-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 llama_index_vector_stores_redis-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-11 00:58:34.615904 llama_index_vector_stores_redis-0.2.0/README.md
+-rw-r--r--   0        0        0       98 2024-04-11 00:58:34.615904 llama_index_vector_stores_redis-0.2.0/llama_index/vector_stores/redis/__init__.py
+-rw-r--r--   0        0        0    17470 2024-04-11 00:58:34.615904 llama_index_vector_stores_redis-0.2.0/llama_index/vector_stores/redis/base.py
+-rw-r--r--   0        0        0     1592 2024-04-11 00:58:34.615904 llama_index_vector_stores_redis-0.2.0/llama_index/vector_stores/redis/schema.py
+-rw-r--r--   0        0        0      917 2024-04-11 00:58:34.615904 llama_index_vector_stores_redis-0.2.0/llama_index/vector_stores/redis/utils.py
+-rw-r--r--   0        0        0     1486 2024-04-11 00:58:34.615904 llama_index_vector_stores_redis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 llama_index_vector_stores_redis-0.2.0/PKG-INFO
```

### Comparing `llama_index_vector_stores_redis-0.1.2/llama_index/vector_stores/redis/base.py` & `llama_index_vector_stores_redis-0.2.0/llama_index/vector_stores/redis/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,443 +14,461 @@
     NodeRelationship,
     RelatedNodeInfo,
     TextNode,
 )
 from llama_index.core.vector_stores.types import (
     BasePydanticVectorStore,
     MetadataFilters,
+    MetadataFilter,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 from llama_index.core.vector_stores.utils import (
     metadata_dict_to_node,
     node_to_metadata_dict,
 )
-from llama_index.vector_stores.redis.utils import (
-    TokenEscaper,
-    array_to_buffer,
-    check_redis_modules_exist,
-    convert_bytes,
-    get_redis_query,
+from llama_index.vector_stores.redis.schema import (
+    NODE_ID_FIELD_NAME,
+    NODE_CONTENT_FIELD_NAME,
+    DOC_ID_FIELD_NAME,
+    TEXT_FIELD_NAME,
+    VECTOR_FIELD_NAME,
+    RedisVectorStoreSchema,
 )
+from llama_index.vector_stores.redis.utils import REDIS_LLAMA_FIELD_SPEC
 
-import redis
-from redis import DataError
-from redis.client import Redis as RedisType
-from redis.commands.search.field import VectorField
+from redis import Redis
 from redis.exceptions import RedisError
 from redis.exceptions import TimeoutError as RedisTimeoutError
 
-_logger = logging.getLogger(__name__)
+from redisvl.index import SearchIndex
+from redisvl.schema import IndexSchema
+from redisvl.query import VectorQuery, FilterQuery, CountQuery
+from redisvl.query.filter import Tag, FilterExpression
+from redisvl.schema.fields import BaseField
+from redisvl.redis.utils import array_to_buffer
+
+
+logger = logging.getLogger(__name__)
 
 
 class RedisVectorStore(BasePydanticVectorStore):
+    """RedisVectorStore.
+
+    The RedisVectorStore takes a user-defined schema object and a Redis connection
+    client or URL string. The schema is optional, but useful for:
+    - Defining a custom index name, key prefix, and key separator.
+    - Defining *additional* metadata fields to use as query filters.
+    - Setting custom specifications on fields to improve search quality, e.g
+    which vector index algorithm to use.
+
+    Other Notes:
+    - All embeddings and docs are stored in Redis. During query time, the index
+    uses Redis to query for the top k most similar nodes.
+    - Redis & LlamaIndex expect at least 4 *required* fields for any schema, default or custom,
+    `id`, `doc_id`, `text`, `vector`.
+
+    Args:
+        schema (IndexSchema, optional): Redis index schema object.
+        redis_client (Redis, optional): Redis client connection.
+        redis_url (str, optional): Redis server URL.
+            Defaults to "redis://localhost:6379".
+        overwrite (bool, optional): Whether to overwrite the index if it already exists.
+            Defaults to False.
+
+    Raises:
+        ValueError: If your Redis server does not have search or JSON enabled.
+        ValueError: If a Redis connection failed to be established.
+        ValueError: If an invalid schema is provided.
+
+    Example:
+        from redisvl.schema import IndexSchema
+        from llama_index.vector_stores.redis import RedisVectorStore
+
+        # Use default schema
+        rds = RedisVectorStore(redis_url="redis://localhost:6379")
+
+        # Use custom schema from dict
+        schema = IndexSchema.from_dict({
+            "index": {"name": "my-index", "prefix": "docs"},
+            "fields": [
+                {"name": "id", "type": "tag"},
+                {"name": "doc_id", "type": "tag},
+                {"name": "text", "type": "text"},
+                {"name": "vector", "type": "vector", "attrs": {"dims": 1536, "algorithm": "flat"}}
+            ]
+        })
+        vector_store = RedisVectorStore(
+            schema=schema,
+            redis_url="redis://localhost:6379"
+        )
+    """
+
     stores_text = True
     stores_node = True
     flat_metadata = False
 
-    _tokenizer: Any = PrivateAttr()
-    _redis_client: Any = PrivateAttr()
-    _prefix: str = PrivateAttr()
-    _index_name: str = PrivateAttr()
-    _index_args: Dict[str, Any] = PrivateAttr()
-    _metadata_fields: List[str] = PrivateAttr()
+    _index: SearchIndex = PrivateAttr()
     _overwrite: bool = PrivateAttr()
-    _vector_field: str = PrivateAttr()
-    _vector_key: str = PrivateAttr()
+    _return_fields: List[str] = PrivateAttr()
 
     def __init__(
         self,
-        index_name: str,
-        index_prefix: str = "llama_index",
-        prefix_ending: str = "/vector",
-        index_args: Optional[Dict[str, Any]] = None,
-        metadata_fields: Optional[List[str]] = None,
-        redis_url: str = "redis://localhost:6379",
+        schema: Optional[IndexSchema] = None,
+        redis_client: Optional[Redis] = None,
+        redis_url: Optional[str] = None,
         overwrite: bool = False,
+        return_fields: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
-        """Initialize RedisVectorStore.
-
-        For index arguments that can be passed to RediSearch, see
-        https://redis.io/docs/stack/search/reference/vectors/
+        # check for indicators of old schema
+        self._flag_old_kwargs(**kwargs)
 
-        The index arguments will depend on the index type chosen. There
-        are two available index types
-            - FLAT: a flat index that uses brute force search
-            - HNSW: a hierarchical navigable small world graph index
+        # Setup schema
+        if not schema:
+            logger.info("Using default RedisVectorStore schema.")
+            schema = RedisVectorStoreSchema()
+
+        self._validate_schema(schema)
+        self._return_fields = return_fields or [
+            NODE_ID_FIELD_NAME,
+            DOC_ID_FIELD_NAME,
+            TEXT_FIELD_NAME,
+            NODE_CONTENT_FIELD_NAME,
+        ]
+        self._index = SearchIndex(schema=schema)
+        self._overwrite = overwrite
 
-        Args:
-            index_name (str): Name of the index.
-            index_prefix (str): Prefix for the index. Defaults to "llama_index".
-                The actual prefix used by Redis will be
-                "{index_prefix}{prefix_ending}".
-            prefix_ending (str): Prefix ending for the index. Be careful when
-                changing this: https://github.com/jerryjliu/llama_index/pull/6665.
-                Defaults to "/vector".
-            index_args (Dict[str, Any]): Arguments for the index. Defaults to None.
-            metadata_fields (List[str]): List of metadata fields to store in the index
-                (only supports TAG fields).
-            redis_url (str): URL for the redis instance.
-                Defaults to "redis://localhost:6379".
-            overwrite (bool): Whether to overwrite the index if it already exists.
-                Defaults to False.
-            kwargs (Any): Additional arguments to pass to the redis client.
+        # Establish redis connection
+        if redis_client:
+            self._index.set_client(redis_client)
+        elif redis_url:
+            self._index.connect(redis_url)
+        else:
+            raise ValueError(
+                "Failed to connect to Redis. Must provide a valid redis client or url"
+            )
 
-        Raises:
-            ValueError: If redis-py is not installed
-            ValueError: If RediSearch is not installed
+        # Create index
+        self.create_index()
 
-        Examples:
-            >>> from llama_index.core.vector_stores.redis import RedisVectorStore
-            >>> # Create a RedisVectorStore
-            >>> vector_store = RedisVectorStore(
-            >>>     index_name="my_index",
-            >>>     index_prefix="llama_index",
-            >>>     index_args={"algorithm": "HNSW", "m": 16, "ef_construction": 200,
-                "distance_metric": "cosine"},
-            >>>     redis_url="redis://localhost:6379/",
-            >>>     overwrite=True)
-        """
-        try:
-            # connect to redis from url
-            self._redis_client = redis.from_url(redis_url, **kwargs)
-            # check if redis has redisearch module installed
-            check_redis_modules_exist(self._redis_client)
-        except ValueError as e:
-            raise ValueError(f"Redis failed to connect: {e}")
-
-        # index identifiers
-        self._prefix = index_prefix + prefix_ending
-        self._index_name = index_name
-        self._index_args = index_args if index_args is not None else {}
-        self._metadata_fields = metadata_fields if metadata_fields is not None else []
-        self._overwrite = overwrite
-        self._vector_field = str(self._index_args.get("vector_field", "vector"))
-        self._vector_key = str(self._index_args.get("vector_key", "vector"))
-        self._tokenizer = TokenEscaper()
         super().__init__()
 
+    def _flag_old_kwargs(self, **kwargs):
+        old_kwargs = [
+            "index_name",
+            "index_prefix",
+            "prefix_ending",
+            "index_args",
+            "metadata_fields",
+        ]
+        for kwarg in old_kwargs:
+            if kwarg in kwargs:
+                raise ValueError(
+                    f"Deprecated kwarg, {kwarg}, found upon initialization. "
+                    "RedisVectorStore now requires an IndexSchema object. "
+                    "See the documentation for a complete example: https://docs.llamaindex.ai/en/stable/examples/vector_stores/RedisIndexDemo/"
+                )
+
+    def _validate_schema(self, schema: IndexSchema) -> str:
+        base_schema = RedisVectorStoreSchema()
+        for name, field in base_schema.fields.items():
+            if (name not in schema.fields) or (
+                not schema.fields[name].type == field.type
+            ):
+                raise ValueError(
+                    f"Required field {name} must be present in the index "
+                    f"and of type {schema.fields[name].type}"
+                )
+
     @property
-    def client(self) -> "RedisType":
+    def client(self) -> "Redis":
         """Return the redis client instance."""
-        return self._redis_client
+        return self._index.client
+
+    @property
+    def index_name(self) -> str:
+        """Return the name of the index based on the schema."""
+        return self._index.name
+
+    @property
+    def schema(self) -> IndexSchema:
+        """Return the index schema."""
+        return self._index.schema
+
+    def set_return_fields(self, return_fields: List[str]) -> None:
+        """Update the return fields for the query response."""
+        self._return_fields = return_fields
+
+    def index_exists(self) -> bool:
+        """Check whether the index exists in Redis.
+
+        Returns:
+            bool: True or False.
+        """
+        return self._index.exists()
+
+    def create_index(self, overwrite: Optional[bool] = None) -> None:
+        """Create an index in Redis."""
+        if overwrite is None:
+            overwrite = self._overwrite
+        # Create index honoring overwrite policy
+        if overwrite:
+            self._index.create(overwrite=True, drop=True)
+        else:
+            self._index.create()
 
     def add(self, nodes: List[BaseNode], **add_kwargs: Any) -> List[str]:
         """Add nodes to the index.
 
         Args:
             nodes (List[BaseNode]): List of nodes with embeddings
 
         Returns:
             List[str]: List of ids of the documents added to the index.
 
         Raises:
             ValueError: If the index already exists and overwrite is False.
         """
-        # check to see if empty document list was passed
+        # Check to see if empty document list was passed
         if len(nodes) == 0:
             return []
 
-        # set vector dim for creation if index doesn't exist
-        self._index_args["dims"] = len(nodes[0].get_embedding())
-
-        if self._index_exists():
-            if self._overwrite:
-                self.delete_index()
-                self._create_index()
-            else:
-                logging.info(f"Adding document to existing index {self._index_name}")
-        else:
-            self._create_index()
+        # Now check for the scenario where user is trying to index embeddings that don't align with schema
+        embedding_len = len(nodes[0].get_embedding())
+        expected_dims = self._index.schema.fields[VECTOR_FIELD_NAME].attrs.dims
+        if expected_dims != embedding_len:
+            raise ValueError(
+                f"Attempting to index embeddings of dim {embedding_len} "
+                f"which doesn't match the index schema expectation of {expected_dims}. "
+                "Please review the Redis integration example to learn how to customize schema. "
+                ""
+            )
 
-        ids = []
+        data: List[Dict[str, Any]] = []
         for node in nodes:
-            mapping = {
-                "id": node.node_id,
-                "doc_id": node.ref_doc_id,
-                "text": node.get_content(metadata_mode=MetadataMode.NONE),
-                self._vector_key: array_to_buffer(node.get_embedding()),
+            embedding = node.get_embedding()
+            record = {
+                NODE_ID_FIELD_NAME: node.node_id,
+                DOC_ID_FIELD_NAME: node.ref_doc_id,
+                TEXT_FIELD_NAME: node.get_content(metadata_mode=MetadataMode.NONE),
+                VECTOR_FIELD_NAME: array_to_buffer(embedding),
             }
+            # parse and append metadata
             additional_metadata = node_to_metadata_dict(
                 node, remove_text=True, flat_metadata=self.flat_metadata
             )
-            mapping.update(additional_metadata)
-
-            ids.append(node.node_id)
-            key = "_".join([self._prefix, str(node.node_id)])
-            self._redis_client.hset(key, mapping=mapping)  # type: ignore
+            data.append({**record, **additional_metadata})
 
-        _logger.info(f"Added {len(ids)} documents to index {self._index_name}")
-        return ids
+        # Load nodes to Redis
+        keys = self._index.load(data, id_field=NODE_ID_FIELD_NAME, **add_kwargs)
+        logger.info(f"Added {len(keys)} documents to index {self._index.name}")
+        return [
+            key.strip(self._index.prefix + self._index.key_separator) for key in keys
+        ]
 
     def delete(self, ref_doc_id: str, **delete_kwargs: Any) -> None:
         """
         Delete nodes using with ref_doc_id.
 
         Args:
             ref_doc_id (str): The doc_id of the document to delete.
 
         """
-        # use tokenizer to escape dashes in query
-        query_str = "@doc_id:{%s}" % self._tokenizer.escape(ref_doc_id)
-        # find all documents that match a doc_id
-        results = self._redis_client.ft(self._index_name).search(query_str)
-        if len(results.docs) == 0:
-            # don't raise an error but warn the user that document wasn't found
-            # could be a result of eviction policy
-            _logger.warning(
-                f"Document with doc_id {ref_doc_id} not found "
-                f"in index {self._index_name}"
-            )
-            return
+        # build a filter to target specific docs by doc ID
+        doc_filter = Tag(DOC_ID_FIELD_NAME) == ref_doc_id
+        total = self._index.query(CountQuery(doc_filter))
+        delete_query = FilterQuery(
+            return_fields=[NODE_ID_FIELD_NAME],
+            filter_expression=doc_filter,
+            num_results=total,
+        )
+        # fetch docs to delete and flush them
+        docs_to_delete = self._index.search(delete_query.query, delete_query.params)
+        with self._index.client.pipeline(transaction=False) as pipe:
+            for doc in docs_to_delete.docs:
+                pipe.delete(doc.id)
+            res = pipe.execute()
 
-        for doc in results.docs:
-            self._redis_client.delete(doc.id)
-        _logger.info(
-            f"Deleted {len(results.docs)} documents from index {self._index_name}"
+        logger.info(
+            f"Deleted {len(docs_to_delete.docs)} documents from index {self._index.name}"
         )
 
     def delete_index(self) -> None:
         """Delete the index and all documents."""
-        _logger.info(f"Deleting index {self._index_name}")
-        self._redis_client.ft(self._index_name).dropindex(delete_documents=True)
+        logger.info(f"Deleting index {self._index.name}")
+        self._index.delete(drop=True)
+
+    @staticmethod
+    def _to_redis_filter(field: BaseField, filter: MetadataFilter) -> FilterExpression:
+        """
+        Translate a standard metadata filter to a Redis specific filter expression.
+
+        Args:
+            field (BaseField): The field to be filtered on, must have a type attribute.
+            filter (MetadataFilter): The filter to apply, must have operator and value attributes.
+
+        Returns:
+            FilterExpression: A Redis-specific filter expression constructed from the input.
+
+        Raises:
+            ValueError: If the field type is unsupported or if the operator is not supported for the field type.
+        """
+        # Check for unsupported field type
+        if field.type not in REDIS_LLAMA_FIELD_SPEC:
+            raise ValueError(f"Unsupported field type {field.type} for {field.name}")
+
+        field_info = REDIS_LLAMA_FIELD_SPEC[field.type]
+
+        # Check for unsupported operator
+        if filter.operator not in field_info["operators"]:
+            raise ValueError(
+                f"Filter operator {filter.operator} not supported for {field.name} of type {field.type}"
+            )
+
+        # Create field instance and apply the operator function
+        field_instance = field_info["class"](field.name)
+        return field_info["operators"][filter.operator](field_instance, filter.value)
+
+    def _create_redis_filter_expression(
+        self, metadata_filters: MetadataFilters
+    ) -> FilterExpression:
+        """
+        Generate a Redis Filter Expression as a combination of metadata filters.
+
+        Args:
+            metadata_filters (MetadataFilters): List of metadata filters to use.
+
+        Returns:
+            FilterExpression: A Redis filter expression.
+        """
+        filter_expression = FilterExpression("*")
+        if metadata_filters:
+            if metadata_filters.filters:
+                for filter in metadata_filters.filters:
+                    # Index must be created with the metadata field in the index schema
+                    field = self._index.schema.fields.get(filter.key)
+                    if not field:
+                        logger.warning(
+                            f"{filter.key} field was not included as part of the index schema, and thus cannot be used as a filter condition."
+                        )
+                        continue
+                    # Extract redis filter
+                    redis_filter = self._to_redis_filter(field, filter)
+                    # Combine with conditional
+                    if metadata_filters.condition == "and":
+                        filter_expression = filter_expression & redis_filter
+                    else:
+                        filter_expression = filter_expression | redis_filter
+        return filter_expression
+
+    def _to_redis_query(self, query: VectorStoreQuery) -> VectorQuery:
+        """Creates a RedisQuery from a VectorStoreQuery."""
+        filter_expression = self._create_redis_filter_expression(query.filters)
+        return_fields = self._return_fields.copy()
+        return VectorQuery(
+            vector=query.query_embedding,
+            vector_field_name=VECTOR_FIELD_NAME,
+            num_results=query.similarity_top_k,
+            filter_expression=filter_expression,
+            return_fields=return_fields,
+        )
+
+    def _extract_node_and_score(self, doc, redis_query: VectorQuery):
+        """Extracts a node and its score from a document."""
+        try:
+            node = metadata_dict_to_node(
+                {NODE_CONTENT_FIELD_NAME: doc[NODE_CONTENT_FIELD_NAME]}
+            )
+            node.text = doc[TEXT_FIELD_NAME]
+        except Exception:
+            # Handle legacy metadata format
+            node = TextNode(
+                text=doc[TEXT_FIELD_NAME],
+                id_=doc[NODE_ID_FIELD_NAME],
+                embedding=None,
+                relationships={
+                    NodeRelationship.SOURCE: RelatedNodeInfo(
+                        node_id=doc[DOC_ID_FIELD_NAME]
+                    )
+                },
+            )
+        score = 1 - float(doc[redis_query.DISTANCE_ID])
+        return node, score
+
+    def _process_query_results(
+        self, results, redis_query: VectorQuery
+    ) -> VectorStoreQueryResult:
+        """Processes query results and returns a VectorStoreQueryResult."""
+        ids, nodes, scores = [], [], []
+        for doc in results:
+            node, score = self._extract_node_and_score(doc, redis_query)
+            ids.append(doc[NODE_ID_FIELD_NAME])
+            nodes.append(node)
+            scores.append(score)
+        logger.info(f"Found {len(nodes)} results for query with id {ids}")
+        return VectorStoreQueryResult(nodes=nodes, ids=ids, similarities=scores)
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """Query the index.
 
         Args:
             query (VectorStoreQuery): query object
 
         Returns:
             VectorStoreQueryResult: query result
 
         Raises:
             ValueError: If query.query_embedding is None.
             redis.exceptions.RedisError: If there is an error querying the index.
             redis.exceptions.TimeoutError: If there is a timeout querying the index.
-            ValueError: If no documents are found when querying the index.
         """
-        return_fields = [
-            "id",
-            "doc_id",
-            "text",
-            self._vector_key,
-            "vector_score",
-            "_node_content",
-        ]
-
-        filters = _to_redis_filters(query.filters) if query.filters is not None else "*"
-
-        _logger.info(f"Using filters: {filters}")
-
-        redis_query = get_redis_query(
-            return_fields=return_fields,
-            top_k=query.similarity_top_k,
-            vector_field=self._vector_field,
-            filters=filters,
-        )
-
         if not query.query_embedding:
             raise ValueError("Query embedding is required for querying.")
 
-        query_params = {
-            "vector": array_to_buffer(query.query_embedding),
-        }
-        _logger.info(f"Querying index {self._index_name}")
+        redis_query = self._to_redis_query(query)
+        logger.info(
+            f"Querying index {self._index.name} with filters {redis_query.get_filter()}"
+        )
 
         try:
-            results = self._redis_client.ft(self._index_name).search(
-                redis_query, query_params=query_params  # type: ignore
-            )
+            results = self._index.query(redis_query)
         except RedisTimeoutError as e:
-            _logger.error(f"Query timed out on {self._index_name}: {e}")
+            logger.error(f"Query timed out on {self._index.name}: {e}")
             raise
         except RedisError as e:
-            _logger.error(f"Error querying {self._index_name}: {e}")
+            logger.error(f"Error querying {self._index.name}: {e}")
             raise
 
-        if len(results.docs) == 0:
-            raise ValueError(
-                f"No docs found on index '{self._index_name}' with "
-                f"prefix '{self._prefix}' and filters '{filters}'. "
-                "* Did you originally create the index with a different prefix? "
-                "* Did you index your metadata fields when you created the index?"
-            )
-
-        ids = []
-        nodes = []
-        scores = []
-        for doc in results.docs:
-            try:
-                node = metadata_dict_to_node({"_node_content": doc._node_content})
-                node.text = doc.text
-            except Exception:
-                # TODO: Legacy support for old metadata format
-                node = TextNode(
-                    text=doc.text,
-                    id_=doc.id,
-                    embedding=None,
-                    relationships={
-                        NodeRelationship.SOURCE: RelatedNodeInfo(node_id=doc.doc_id)
-                    },
-                )
-            ids.append(doc.id.replace(self._prefix + "_", ""))
-            nodes.append(node)
-            scores.append(1 - float(doc.vector_score))
-        _logger.info(f"Found {len(nodes)} results for query with id {ids}")
-
-        return VectorStoreQueryResult(nodes=nodes, ids=ids, similarities=scores)
+        return self._process_query_results(results, redis_query)
 
     def persist(
         self,
-        persist_path: str,
+        persist_path: Optional[str] = None,
         fs: Optional[fsspec.AbstractFileSystem] = None,
         in_background: bool = True,
     ) -> None:
         """Persist the vector store to disk.
 
+        For Redis, more notes here: https://redis.io/docs/management/persistence/
+
         Args:
             persist_path (str): Path to persist the vector store to. (doesn't apply)
             in_background (bool, optional): Persist in background. Defaults to True.
             fs (fsspec.AbstractFileSystem, optional): Filesystem to persist to.
                 (doesn't apply)
 
         Raises:
             redis.exceptions.RedisError: If there is an error
                                          persisting the index to disk.
         """
         try:
             if in_background:
-                _logger.info("Saving index to disk in background")
-                self._redis_client.bgsave()
+                logger.info("Saving index to disk in background")
+                self._index.client.bgsave()
             else:
-                _logger.info("Saving index to disk")
-                self._redis_client.save()
+                logger.info("Saving index to disk")
+                self._index.client.save()
 
         except RedisError as e:
-            _logger.error(f"Error saving index to disk: {e}")
+            logger.error(f"Error saving index to disk: {e}")
             raise
-
-    def _create_index(self) -> None:
-        # should never be called outside class and hence should not raise importerror
-        from redis.commands.search.field import TagField, TextField
-        from redis.commands.search.indexDefinition import IndexDefinition, IndexType
-
-        # Create Index
-        default_fields = [
-            TextField("text", weight=1.0),
-            TagField("doc_id", sortable=False),
-            TagField("id", sortable=False),
-        ]
-        # add vector field to list of index fields. Create lazily to allow user
-        # to specify index and search attributes in creation.
-
-        fields = [
-            *default_fields,
-            self._create_vector_field(self._vector_field, **self._index_args),
-        ]
-
-        # add metadata fields to list of index fields or we won't be able to search them
-        for metadata_field in self._metadata_fields:
-            # TODO: allow addition of text fields as metadata
-            # TODO: make sure we're preventing overwriting other keys (e.g. text,
-            #   doc_id, id, and other vector fields)
-            fields.append(TagField(metadata_field, sortable=False))
-
-        _logger.info(f"Creating index {self._index_name}")
-        self._redis_client.ft(self._index_name).create_index(
-            fields=fields,
-            definition=IndexDefinition(
-                prefix=[self._prefix], index_type=IndexType.HASH
-            ),  # TODO support JSON
-        )
-
-    def _index_exists(self) -> bool:
-        # use FT._LIST to check if index exists
-        indices = convert_bytes(self._redis_client.execute_command("FT._LIST"))
-        return self._index_name in indices
-
-    def _create_vector_field(
-        self,
-        name: str,
-        dims: int = 1536,
-        algorithm: str = "FLAT",
-        datatype: str = "FLOAT32",
-        distance_metric: str = "COSINE",
-        initial_cap: int = 20000,
-        block_size: int = 1000,
-        m: int = 16,
-        ef_construction: int = 200,
-        ef_runtime: int = 10,
-        epsilon: float = 0.8,
-        **kwargs: Any,
-    ) -> "VectorField":
-        """Create a RediSearch VectorField.
-
-        Args:
-            name (str): The name of the field.
-            algorithm (str): The algorithm used to index the vector.
-            dims (int): The dimensionality of the vector.
-            datatype (str): The type of the vector. default: FLOAT32
-            distance_metric (str): The distance metric used to compare vectors.
-            initial_cap (int): The initial capacity of the index.
-            block_size (int): The block size of the index.
-            m (int): The number of outgoing edges in the HNSW graph.
-            ef_construction (int): Number of maximum allowed potential outgoing edges
-                            candidates for each node in the graph,
-                            during the graph building.
-            ef_runtime (int): The umber of maximum top candidates to hold during the
-                KNN search
-
-        Returns:
-            A RediSearch VectorField.
-        """
-        try:
-            if algorithm.upper() == "HNSW":
-                return VectorField(
-                    name,
-                    "HNSW",
-                    {
-                        "TYPE": datatype.upper(),
-                        "DIM": dims,
-                        "DISTANCE_METRIC": distance_metric.upper(),
-                        "INITIAL_CAP": initial_cap,
-                        "M": m,
-                        "EF_CONSTRUCTION": ef_construction,
-                        "EF_RUNTIME": ef_runtime,
-                        "EPSILON": epsilon,
-                    },
-                )
-            else:
-                return VectorField(
-                    name,
-                    "FLAT",
-                    {
-                        "TYPE": datatype.upper(),
-                        "DIM": dims,
-                        "DISTANCE_METRIC": distance_metric.upper(),
-                        "INITIAL_CAP": initial_cap,
-                        "BLOCK_SIZE": block_size,
-                    },
-                )
-        except DataError as e:
-            raise ValueError(
-                f"Failed to create Redis index vector field with error: {e}"
-            )
-
-
-# currently only supports exact tag match - {} denotes a tag
-# must create the index with the correct metadata field before using a field as a
-#   filter, or it will return no results
-def _to_redis_filters(metadata_filters: MetadataFilters) -> str:
-    tokenizer = TokenEscaper()
-
-    filter_strings = []
-    for filter in metadata_filters.legacy_filters():
-        # adds quotes around the value to ensure that the filter is treated as an
-        #   exact match
-        filter_string = f"@{filter.key}:{{{tokenizer.escape(str(filter.value))}}}"
-        filter_strings.append(filter_string)
-
-    joined_filter_strings = " & ".join(filter_strings)
-    return f"({joined_filter_strings})"
```

### Comparing `llama_index_vector_stores_redis-0.1.2/pyproject.toml` & `llama_index_vector_stores_redis-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.vector_stores.redis"
 
 [tool.llamahub.class_authors]
-RedisVectorStore = "llama-index"
+RedisVectorStore = "redis"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = ["Tyler Hutcherson <tyler.hutcherson@redis.com>"]
 description = "llama-index vector_stores redis integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-redis"
 readme = "README.md"
-version = "0.1.2"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-redis = "^5.0.1"
+redisvl = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_vector_stores_redis-0.1.2/PKG-INFO` & `llama_index_vector_stores_redis-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-redis
-Version: 0.1.2
+Version: 0.2.0
 Summary: llama-index vector_stores redis integration
 License: MIT
-Author: Your Name
-Author-email: you@example.com
+Author: Tyler Hutcherson
+Author-email: tyler.hutcherson@redis.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Requires-Dist: redis (>=5.0.1,<6.0.0)
+Requires-Dist: redisvl (>=0.1.3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Redis
```

