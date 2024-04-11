# Comparing `tmp/llama_index_vector_stores_elasticsearch-0.1.6.tar.gz` & `tmp/llama_index_vector_stores_elasticsearch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_elasticsearch-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_elasticsearch-0.1.7.tar", max compression
```

## Comparing `llama_index_vector_stores_elasticsearch-0.1.6.tar` & `llama_index_vector_stores_elasticsearch-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       54 2024-03-21 21:20:40.228748 llama_index_vector_stores_elasticsearch-0.1.6/README.md
--rw-r--r--   0        0        0      110 2024-03-21 21:20:40.228748 llama_index_vector_stores_elasticsearch-0.1.6/llama_index/vector_stores/elasticsearch/__init__.py
--rw-r--r--   0        0        0    20593 2024-03-21 21:20:40.228748 llama_index_vector_stores_elasticsearch-0.1.6/llama_index/vector_stores/elasticsearch/base.py
--rw-r--r--   0        0        0     1533 2024-03-21 21:20:40.228748 llama_index_vector_stores_elasticsearch-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 llama_index_vector_stores_elasticsearch-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-11 03:38:48.366242 llama_index_vector_stores_elasticsearch-0.1.7/README.md
+-rw-r--r--   0        0        0      110 2024-04-11 03:38:48.366242 llama_index_vector_stores_elasticsearch-0.1.7/llama_index/vector_stores/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    21853 2024-04-11 03:38:48.366242 llama_index_vector_stores_elasticsearch-0.1.7/llama_index/vector_stores/elasticsearch/base.py
+-rw-r--r--   0        0        0     1533 2024-04-11 03:38:48.366242 llama_index_vector_stores_elasticsearch-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 llama_index_vector_stores_elasticsearch-0.1.7/PKG-INFO
```

### Comparing `llama_index_vector_stores_elasticsearch-0.1.6/llama_index/vector_stores/elasticsearch/base.py` & `llama_index_vector_stores_elasticsearch-0.1.7/llama_index/vector_stores/elasticsearch/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -152,14 +152,50 @@
         distance_strategy: Optional. Distance strategy to use for similarity search.
                         Defaults to "COSINE".
 
     Raises:
         ConnectionError: If AsyncElasticsearch client cannot connect to Elasticsearch.
         ValueError: If neither es_client nor es_url nor es_cloud_id is provided.
 
+    Examples:
+        `pip install llama-index-vector-stores-elasticsearch`
+
+        ```python
+        from llama_index.vector_stores import ElasticsearchStore
+
+        # Additional setup for ElasticsearchStore class
+        index_name = "my_index"
+        es_url = "http://localhost:9200"
+        es_cloud_id = "<cloud-id>"  # Found within the deployment page
+        es_user = "elastic"
+        es_password = "<password>"  # Provided when creating deployment or can be reset
+        es_api_key = "<api-key>"  # Create an API key within Kibana (Security -> API Keys)
+
+        # Connecting to ElasticsearchStore locally
+        es_local = ElasticsearchStore(
+            index_name=index_name,
+            es_url=es_url,
+        )
+
+        # Connecting to Elastic Cloud with username and password
+        es_cloud_user_pass = ElasticsearchStore(
+            index_name=index_name,
+            es_cloud_id=es_cloud_id,
+            es_user=es_user,
+            es_password=es_password,
+        )
+
+        # Connecting to Elastic Cloud with API Key
+        es_cloud_api_key = ElasticsearchStore(
+            index_name=index_name,
+            es_cloud_id=es_cloud_id,
+            es_api_key=es_api_key,
+        )
+        ```
+
     """
 
     stores_text: bool = True
     index_name: str
     es_client: Optional[Any]
     es_url: Optional[str]
     es_cloud_id: Optional[str]
@@ -524,15 +560,15 @@
                 "bool": {
                     "must": {"match": {self.text_field: {"query": query.query_str}}},
                     "filter": filter,
                 }
             }
 
         if query.mode == VectorStoreQueryMode.HYBRID:
-            es_query["rank"] = {"rrf": {}}
+            es_query["rank"] = {"rrf": {"window_size": query.similarity_top_k}}
 
         if custom_query is not None:
             es_query = custom_query(es_query, query)
             logger.debug(f"Calling custom_query, Query body now: {es_query}")
 
         async with self.client as client:
             response = await client.search(
```

### Comparing `llama_index_vector_stores_elasticsearch-0.1.6/pyproject.toml` & `llama_index_vector_stores_elasticsearch-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores elasticsearch integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-elasticsearch"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 elasticsearch = "^8.12.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_elasticsearch-0.1.6/PKG-INFO` & `llama_index_vector_stores_elasticsearch-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-elasticsearch
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index vector_stores elasticsearch integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

