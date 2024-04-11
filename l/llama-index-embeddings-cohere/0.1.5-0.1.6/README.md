# Comparing `tmp/llama_index_embeddings_cohere-0.1.5.tar.gz` & `tmp/llama_index_embeddings_cohere-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_cohere-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_embeddings_cohere-0.1.6.tar", max compression
```

## Comparing `llama_index_embeddings_cohere-0.1.5.tar` & `llama_index_embeddings_cohere-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-03-27 17:43:22.126524 llama_index_embeddings_cohere-0.1.5/README.md
--rw-r--r--   0        0        0       94 2024-03-27 17:43:22.126524 llama_index_embeddings_cohere-0.1.5/llama_index/embeddings/cohere/__init__.py
--rw-r--r--   0        0        0     7756 2024-03-27 17:43:22.126524 llama_index_embeddings_cohere-0.1.5/llama_index/embeddings/cohere/base.py
--rw-r--r--   0        0        0     1466 2024-03-27 17:43:22.126524 llama_index_embeddings_cohere-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_embeddings_cohere-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-11 16:23:15.552394 llama_index_embeddings_cohere-0.1.6/README.md
+-rw-r--r--   0        0        0       94 2024-04-11 16:23:15.552394 llama_index_embeddings_cohere-0.1.6/llama_index/embeddings/cohere/__init__.py
+-rw-r--r--   0        0        0     9416 2024-04-11 16:23:15.552394 llama_index_embeddings_cohere-0.1.6/llama_index/embeddings/cohere/base.py
+-rw-r--r--   0        0        0     1466 2024-04-11 16:23:15.552394 llama_index_embeddings_cohere-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_embeddings_cohere-0.1.6/PKG-INFO
```

### Comparing `llama_index_embeddings_cohere-0.1.5/llama_index/embeddings/cohere/base.py` & `llama_index_embeddings_cohere-0.1.6/llama_index/embeddings/cohere/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from enum import Enum
-from typing import Any, List, Optional
+from typing import List, Optional
 
 from llama_index.core.base.embeddings.base import (
     DEFAULT_EMBED_BATCH_SIZE,
     BaseEmbedding,
 )
 from llama_index.core.bridge.pydantic import Field
 from llama_index.core.callbacks import CallbackManager
+import cohere
+import httpx
 
 
 # Enums for validation and type safety
 class CohereAIModelName(str, Enum):
     ENGLISH_V3 = "embed-english-v3.0"
     ENGLISH_LIGHT_V3 = "embed-english-light-v3.0"
     MULTILINGUAL_V3 = "embed-multilingual-v3.0"
@@ -70,14 +72,23 @@
         CAIT.CLUSTERING,
     ],
     CAMN.ENGLISH_V2: [None],
     CAMN.ENGLISH_LIGHT_V2: [None],
     CAMN.MULTILINGUAL_V2: [None],
 }
 
+# v3 models require an input_type field
+V3_MODELS = [
+    CAMN.ENGLISH_V3,
+    CAMN.ENGLISH_LIGHT_V3,
+    CAMN.MULTILINGUAL_V3,
+    CAMN.MULTILINGUAL_LIGHT_V3,
+]
+
+
 # This list would be used for model name and embedding types validation
 # Embedding type can be float/ int8/ uint8/ binary/ ubinary based on model.
 VALID_MODEL_EMBEDDING_TYPES = {
     CAMN.ENGLISH_V3: ["float", "int8", "uint8", "binary", "ubinary"],
     CAMN.ENGLISH_LIGHT_V3: ["float", "int8", "uint8", "binary", "ubinary"],
     CAMN.MULTILINGUAL_V3: ["float", "int8", "uint8", "binary", "ubinary"],
     CAMN.MULTILINGUAL_LIGHT_V3: ["float", "int8", "uint8", "binary", "ubinary"],
@@ -90,15 +101,18 @@
 
 
 # Assuming BaseEmbedding is a Pydantic model and handles its own initializations
 class CohereEmbedding(BaseEmbedding):
     """CohereEmbedding uses the Cohere API to generate embeddings for text."""
 
     # Instance variables initialized via Pydantic's mechanism
-    cohere_client: Any = Field(description="CohereAI client")
+    _cohere_client: cohere.Client = Field(description="CohereAI client")
+    _cohere_async_client: cohere.AsyncClient = Field(
+        description="CohereAI Async client"
+    )
     truncate: str = Field(description="Truncation type - START/ END/ NONE")
     input_type: Optional[str] = Field(
         description="Model Input type. If not provided, search_document and search_query are used when needed."
     )
     embedding_type: str = Field(
         description="Embedding type. If not provided float embedding_type is used when needed."
     )
@@ -108,35 +122,31 @@
         cohere_api_key: Optional[str] = None,
         model_name: str = "embed-english-v3.0",
         truncate: str = "END",
         input_type: Optional[str] = None,
         embedding_type: str = "float",
         embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
         callback_manager: Optional[CallbackManager] = None,
+        base_url: Optional[str] = None,
+        timeout: Optional[float] = None,
+        httpx_client: Optional[httpx.AsyncClient] = None,
     ):
         """
         A class representation for generating embeddings using the Cohere API.
 
         Args:
             cohere_client (Any): An instance of the Cohere client, which is used to communicate with the Cohere API.
             truncate (str): A string indicating the truncation strategy to be applied to input text. Possible values
                         are 'START', 'END', or 'NONE'.
             input_type (Optional[str]): An optional string that specifies the type of input provided to the model.
                                     This is model-dependent and could be one of the following: 'search_query',
                                     'search_document', 'classification', or 'clustering'.
             model_name (str): The name of the model to be used for generating embeddings. The class ensures that
                           this model is supported and that the input type provided is compatible with the model.
         """
-        try:
-            import cohere
-        except ImportError:
-            raise ImportError(
-                "`cohere` package not found. Please run `pip install 'cohere>=5.1.1,<6.0.0'."
-            )
-
         # Validate model_name and input_type
         if model_name not in VALID_MODEL_INPUT_TYPES:
             raise ValueError(f"{model_name} is not a valid model name")
 
         if input_type not in VALID_MODEL_INPUT_TYPES[model_name]:
             raise ValueError(
                 f"{input_type} is not a valid input type for the provided model."
@@ -146,15 +156,28 @@
                 f"{embedding_type} is not a embedding type for the provided model."
             )
 
         if truncate not in VALID_TRUNCATE_OPTIONS:
             raise ValueError(f"truncate must be one of {VALID_TRUNCATE_OPTIONS}")
 
         super().__init__(
-            cohere_client=cohere.Client(cohere_api_key, client_name="llama_index"),
+            _cohere_client=cohere.Client(
+                cohere_api_key,
+                client_name="llama_index",
+                base_url=base_url,
+                timeout=timeout,
+                httpx_client=httpx_client,
+            ),
+            _cohere_async_client=cohere.AsyncClient(
+                cohere_api_key,
+                client_name="llama_index",
+                base_url=base_url,
+                timeout=timeout,
+                httpx_client=httpx_client,
+            ),
             cohere_api_key=cohere_api_key,
             model_name=model_name,
             input_type=input_type,
             embedding_type=embedding_type,
             truncate=truncate,
             embed_batch_size=embed_batch_size,
             callback_manager=callback_manager,
@@ -162,48 +185,70 @@
 
     @classmethod
     def class_name(cls) -> str:
         return "CohereEmbedding"
 
     def _embed(self, texts: List[str], input_type: str) -> List[List[float]]:
         """Embed sentences using Cohere."""
-        if self.model_name in [
-            CAMN.ENGLISH_V3,
-            CAMN.ENGLISH_LIGHT_V3,
-            CAMN.MULTILINGUAL_V3,
-            CAMN.MULTILINGUAL_LIGHT_V3,
-        ]:
-            result = self.cohere_client.embed(
+        if self.model_name in V3_MODELS:
+            result = self._cohere_client.embed(
                 texts=texts,
                 input_type=self.input_type or input_type,
                 embedding_types=[self.embedding_type],
                 model=self.model_name,
                 truncate=self.truncate,
             ).embeddings
         else:
-            result = self.cohere_client.embed(
+            result = self._cohere_client.embed(
                 texts=texts,
                 model=self.model_name,
                 embedding_types=[self.embedding_type],
                 truncate=self.truncate,
             ).embeddings
         return getattr(result, self.embedding_type, None)
 
+    async def _aembed(self, texts: List[str], input_type: str) -> List[List[float]]:
+        """Embed sentences using Cohere."""
+        if self.model_name in V3_MODELS:
+            result = (
+                await self._cohere_async_client.embed(
+                    texts=texts,
+                    input_type=self.input_type or input_type,
+                    embedding_types=[self.embedding_type],
+                    model=self.model_name,
+                    truncate=self.truncate,
+                )
+            ).embeddings
+        else:
+            result = (
+                await self._cohere_async_client.embed(
+                    texts=texts,
+                    model=self.model_name,
+                    embedding_types=[self.embedding_type],
+                    truncate=self.truncate,
+                )
+            ).embeddings
+        return getattr(result, self.embedding_type, None)
+
     def _get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding. For query embeddings, input_type='search_query'."""
         return self._embed([query], input_type="search_query")[0]
 
     async def _aget_query_embedding(self, query: str) -> List[float]:
         """Get query embedding async. For query embeddings, input_type='search_query'."""
-        return self._get_query_embedding(query)
+        return (await self._aembed([query], input_type="search_query"))[0]
 
     def _get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
         return self._embed([text], input_type="search_document")[0]
 
     async def _aget_text_embedding(self, text: str) -> List[float]:
         """Get text embedding async."""
-        return self._get_text_embedding(text)
+        return (await self._aembed([text], input_type="search_document"))[0]
 
     def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Get text embeddings."""
         return self._embed(texts, input_type="search_document")
+
+    async def _aget_text_embeddings(self, texts: List[str]) -> List[List[float]]:
+        """Get text embeddings."""
+        return await self._aembed(texts, input_type="search_document")
```

### Comparing `llama_index_embeddings_cohere-0.1.5/pyproject.toml` & `llama_index_embeddings_cohere-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings cohere integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-cohere"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-cohere = "^5.1.1"
+cohere = "^5.2.5"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

