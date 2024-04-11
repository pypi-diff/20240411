# Comparing `tmp/langchain_google_vertexai-0.1.2.tar.gz` & `tmp/langchain_google_vertexai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_vertexai-0.1.2.tar", max compression
+gzip compressed data, was "langchain_google_vertexai-0.1.3.tar", max compression
```

## Comparing `langchain_google_vertexai-0.1.2.tar` & `langchain_google_vertexai-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1072 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/LICENSE
--rw-r--r--   0        0        0     2594 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/README.md
--rw-r--r--   0        0        0     1558 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/__init__.py
--rw-r--r--   0        0        0    11390 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/_base.py
--rw-r--r--   0        0        0      151 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/_enums.py
--rw-r--r--   0        0        0     6282 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/_image_utils.py
--rw-r--r--   0        0        0     6591 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/_utils.py
--rw-r--r--   0        0        0     2511 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/callbacks.py
--rw-r--r--   0        0        0     4346 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/chains.py
--rw-r--r--   0        0        0    30613 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/chat_models.py
--rw-r--r--   0        0        0    16400 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/embeddings.py
--rw-r--r--   0        0        0     5912 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/functions_utils.py
--rw-r--r--   0        0        0    12748 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/gemma.py
--rw-r--r--   0        0        0    11414 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/llms.py
--rw-r--r--   0        0        0     2577 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/model_garden.py
--rw-r--r--   0        0        0        0 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/py.typed
--rw-r--r--   0        0        0      287 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/__init__.py
--rw-r--r--   0        0        0     8490 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_document_storage.py
--rw-r--r--   0        0        0     4679 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_sdk_manager.py
--rw-r--r--   0        0        0     6103 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_searcher.py
--rw-r--r--   0        0        0     5436 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_utils.py
--rw-r--r--   0        0        0    15651 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/vectorstores.py
--rw-r--r--   0        0        0    16906 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/langchain_google_vertexai/vision_models.py
--rw-r--r--   0        0        0     2880 2024-03-26 14:42:59.609444 langchain_google_vertexai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 langchain_google_vertexai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2594 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/README.md
+-rw-r--r--   0        0        0     1853 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/__init__.py
+-rw-r--r--   0        0        0     3255 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_anthropic_utils.py
+-rw-r--r--   0        0        0    11390 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_base.py
+-rw-r--r--   0        0        0      151 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_enums.py
+-rw-r--r--   0        0        0     8169 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_image_utils.py
+-rw-r--r--   0        0        0     6591 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_utils.py
+-rw-r--r--   0        0        0     2511 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/callbacks.py
+-rw-r--r--   0        0        0     5471 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/chains.py
+-rw-r--r--   0        0        0    37792 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/chat_models.py
+-rw-r--r--   0        0        0    16400 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/embeddings.py
+-rw-r--r--   0        0        0     6304 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/functions_utils.py
+-rw-r--r--   0        0        0    12748 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/gemma.py
+-rw-r--r--   0        0        0    11414 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/llms.py
+-rw-r--r--   0        0        0     8224 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/model_garden.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/py.typed
+-rw-r--r--   0        0        0      471 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     4679 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_sdk_manager.py
+-rw-r--r--   0        0        0     6103 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_searcher.py
+-rw-r--r--   0        0        0     5436 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_utils.py
+-rw-r--r--   0        0        0     8050 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/document_storage.py
+-rw-r--r--   0        0        0    15958 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/vectorstores.py
+-rw-r--r--   0        0        0    18548 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vision_models.py
+-rw-r--r--   0        0        0     3366 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-0.1.3/PKG-INFO
```

### Comparing `langchain_google_vertexai-0.1.2/LICENSE` & `langchain_google_vertexai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/README.md` & `langchain_google_vertexai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/__init__.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from langchain_google_vertexai._enums import HarmBlockThreshold, HarmCategory
 from langchain_google_vertexai.chains import create_structured_runnable
 from langchain_google_vertexai.chat_models import ChatVertexAI
 from langchain_google_vertexai.embeddings import VertexAIEmbeddings
-from langchain_google_vertexai.functions_utils import PydanticFunctionsOutputParser
+from langchain_google_vertexai.functions_utils import (
+    PydanticFunctionsOutputParser,
+    ToolConfig,
+)
 from langchain_google_vertexai.gemma import (
     GemmaChatLocalHF,
     GemmaChatLocalKaggle,
     GemmaChatVertexAIModelGarden,
     GemmaLocalHF,
     GemmaLocalKaggle,
     GemmaVertexAIModelGarden,
 )
 from langchain_google_vertexai.llms import VertexAI
 from langchain_google_vertexai.model_garden import VertexAIModelGarden
-from langchain_google_vertexai.vectorstores.vectorstores import VectorSearchVectorStore
+from langchain_google_vertexai.vectorstores import (
+    DataStoreDocumentStorage,
+    GCSDocumentStorage,
+    VectorSearchVectorStore,
+    VectorSearchVectorStoreDatastore,
+    VectorSearchVectorStoreGCS,
+)
 from langchain_google_vertexai.vision_models import (
     VertexAIImageCaptioning,
     VertexAIImageCaptioningChat,
     VertexAIImageEditorChat,
     VertexAIImageGeneratorChat,
     VertexAIVisualQnAChat,
 )
@@ -32,15 +41,20 @@
     "GemmaChatLocalHF",
     "VertexAIEmbeddings",
     "VertexAI",
     "VertexAIModelGarden",
     "HarmBlockThreshold",
     "HarmCategory",
     "PydanticFunctionsOutputParser",
+    "ToolConfig",
     "create_structured_runnable",
-    "VectorSearchVectorStore",
     "VertexAIImageCaptioning",
     "VertexAIImageCaptioningChat",
     "VertexAIImageEditorChat",
     "VertexAIImageGeneratorChat",
     "VertexAIVisualQnAChat",
+    "DataStoreDocumentStorage",
+    "GCSDocumentStorage",
+    "VectorSearchVectorStore",
+    "VectorSearchVectorStoreDatastore",
+    "VectorSearchVectorStoreGCS",
 ]
```

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/_base.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_base.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/_image_utils.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_image_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 from __future__ import annotations
 
 import base64
 import os
 import re
+from enum import Enum
 from typing import Dict, Union
 from urllib.parse import urlparse
 
 import requests
 from google.cloud import storage
+from vertexai.generative_models import Image, Part  # type: ignore
+
+
+class Route(Enum):
+    """Image Loading Route"""
+
+    GOOGLE_CLOUD_STORAGE = 1
+    BASE64 = 2
+    LOCAL_FILE = 3
+    URL = 4
 
 
 class ImageBytesLoader:
     """Loads image bytes from multiple sources given a string.
 
     Currently supported:
         - Google cloud storage URI
@@ -41,25 +52,77 @@
                     - Local file path
                     - URL
 
         Returns:
             Image bytes.
         """
 
+        route = self._route(image_string)
+
+        if route == Route.GOOGLE_CLOUD_STORAGE:
+            blob = self._blob_from_gcs(image_string)
+            return blob.download_as_bytes()
+
+        if route == Route.BASE64:
+            return self._bytes_from_b64(image_string)
+
+        if route == Route.URL:
+            return self._bytes_from_url(image_string)
+
+        if route == Route.LOCAL_FILE:
+            return self._bytes_from_file(image_string)
+
+        raise ValueError(
+            "Image string must be one of: Google Cloud Storage URI, "
+            "b64 encoded image string (data:image/...), valid image url, "
+            f"or existing local image file. Instead got '{image_string}'."
+        )
+
+    def load_part(self, image_string: str) -> Part:
+        """Gets Part for loading from Gemini.
+
+        Args:
+            image_string: Can be either:
+                    - Google cloud storage URI
+                    - B64 Encoded image string
+                    - Local file path
+                    - URL
+
+        Returns:
+            generative_models.Part
+        """
+        route = self._route(image_string)
+
+        if route == Route.GOOGLE_CLOUD_STORAGE:
+            blob = self._blob_from_gcs(image_string)
+            return Part.from_uri(uri=image_string, mime_type=blob.content_type)
+
+        if route == Route.BASE64:
+            bytes_ = self._bytes_from_b64(image_string)
+
+        if route == Route.URL:
+            bytes_ = self._bytes_from_url(image_string)
+
+        if route == Route.LOCAL_FILE:
+            bytes_ = self._bytes_from_file(image_string)
+
+        return Part.from_image(Image.from_bytes(bytes_))
+
+    def _route(self, image_string: str) -> Route:
         if image_string.startswith("gs://"):
-            return self._bytes_from_gcs(image_string)
+            return Route.GOOGLE_CLOUD_STORAGE
 
         if image_string.startswith("data:image/"):
-            return self._bytes_from_b64(image_string)
+            return Route.BASE64
 
         if self._is_url(image_string):
-            return self._bytes_from_url(image_string)
+            return Route.URL
 
         if os.path.exists(image_string):
-            return self._bytes_from_file(image_string)
+            return Route.LOCAL_FILE
 
         raise ValueError(
             "Image string must be one of: Google Cloud Storage URI, "
             "b64 encoded image string (data:image/...), valid image url, "
             f"or existing local image file. Instead got '{image_string}'."
         )
 
@@ -111,29 +174,31 @@
         response = requests.get(url)
 
         if not response.ok:
             response.raise_for_status()
 
         return response.content
 
-    def _bytes_from_gcs(self, gcs_uri: str) -> bytes:
-        """Gets image bytes from a Google Cloud Storage uri.
+    def _blob_from_gcs(self, gcs_uri: str) -> storage.Blob:
+        """Gets image Blob from a Google Cloud Storage uri.
 
         Args:
             gcs_uri: Valid gcs uri.
 
         Raises:
             ValueError if there are more than one blob matching the uri.
 
         Returns:
-            Image bytes
+            storage.Blob
         """
 
         gcs_client = storage.Client(project=self._project)
-        return storage.Blob.from_string(gcs_uri, gcs_client).download_as_bytes()
+        blob = storage.Blob.from_string(gcs_uri, gcs_client)
+        blob.reload(client=gcs_client)
+        return blob
 
     def _is_url(self, url_string: str) -> bool:
         """Checks if a url is valid.
 
         Args:
             url_string: Url to check.
```

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/_utils.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/callbacks.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/chains.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/chains.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,17 @@
     Type,
     Union,
 )
 
 from langchain_core.output_parsers import (
     BaseGenerationOutputParser,
     BaseOutputParser,
+    StrOutputParser,
 )
-from langchain_core.prompts import BasePromptTemplate
+from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable
 
 from langchain_google_vertexai.functions_utils import PydanticFunctionsOutputParser
 
 
 def get_output_parser(
@@ -39,30 +40,55 @@
         pydantic_schema = functions[0]
     output_parser: Union[
         BaseOutputParser, BaseGenerationOutputParser
     ] = PydanticFunctionsOutputParser(pydantic_schema=pydantic_schema)
     return output_parser
 
 
+def _create_structured_runnable_extra_step(
+    functions: Sequence[Type[BaseModel]],
+    llm: Runnable,
+    *,
+    prompt: Optional[BasePromptTemplate] = None,
+) -> Runnable:
+    llm_with_functions = llm.bind(functions=functions)
+    parsing_prompt = ChatPromptTemplate.from_template(
+        "You are a world class algorithm for recording entities.\nMake calls "
+        "to the relevant function to record the entities in the following "
+        "input:\n{output}\nTip: Make sure to answer in the correct format."
+    )
+    output_parser = get_output_parser(functions)
+    if prompt:
+        initial_chain = (
+            prompt | llm | StrOutputParser() | parsing_prompt | llm_with_functions
+        )
+    else:
+        initial_chain = parsing_prompt | llm_with_functions
+
+    return initial_chain | output_parser
+
+
 def create_structured_runnable(
     function: Union[Type[BaseModel], Sequence[Type[BaseModel]]],
     llm: Runnable,
     *,
     prompt: Optional[BasePromptTemplate] = None,
+    use_extra_step: bool = False,
 ) -> Runnable:
     """Create a runnable sequence that uses OpenAI functions.
 
     Args:
         function: Either a single pydantic.BaseModel class or a sequence
             of pydantic.BaseModels classes.
             For best results, pydantic.BaseModels
             should have descriptions of the parameters.
         llm: Language model to use,
             assumed to support the Google Vertex function-calling API.
         prompt: BasePromptTemplate to pass to the model.
+        use_extra_step: whether to make an extra step to parse output into a function
 
     Returns:
         A runnable sequence that will pass in the given functions to the model when run.
 
     Example:
         .. code-block:: python
 
@@ -98,14 +124,18 @@
                 chain = create_structured_runnable([RecordPerson, RecordDog], llm, prompt=prompt)
                 chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
                 # -> RecordDog(name="Harry", color="brown", fav_food="chicken")
     """  # noqa: E501
     if not function:
         raise ValueError("Need to pass in at least one function. Received zero.")
     functions = function if isinstance(function, Sequence) else [function]
+    if use_extra_step:
+        return _create_structured_runnable_extra_step(
+            functions=functions, llm=llm, prompt=prompt
+        )
     output_parser = get_output_parser(functions)
     llm_with_functions = llm.bind(functions=functions)
     if prompt is None:
         initial_chain = llm_with_functions
     else:
         initial_chain = prompt | llm_with_functions
     return initial_chain | output_parser
```

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/chat_models.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/chat_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,28 @@
 
 from __future__ import annotations  # noqa
 
 import json
 import logging
 from dataclasses import dataclass, field
 from operator import itemgetter
-from typing import Any, AsyncIterator, Dict, Iterator, List, Optional, Type, Union, cast
+import uuid
+from typing import (
+    Any,
+    AsyncIterator,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+    cast,
+)
 
 import proto  # type: ignore[import-untyped]
 from google.cloud.aiplatform_v1beta1.types.content import Part as GapicPart
 from google.cloud.aiplatform_v1beta1.types.tool import FunctionCall
 from google.cloud.aiplatform import telemetry
 
 from langchain_core.callbacks import (
@@ -24,29 +37,34 @@
 )
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     FunctionMessage,
     HumanMessage,
+    InvalidToolCall,
     SystemMessage,
+    ToolCall,
+    ToolCallChunk,
+    ToolMessage,
 )
+from langchain_core.tools import BaseTool, tool as tool_from_callable
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_functions import (
     JsonOutputFunctionsParser,
     PydanticOutputFunctionsParser,
 )
+from langchain_core.output_parsers.openai_tools import parse_tool_calls
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, root_validator
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from vertexai.generative_models import (  # type: ignore
     Candidate,
     Content,
     GenerativeModel,
-    Image,
     Part,
 )
 from vertexai.language_models import (  # type: ignore
     ChatMessage,
     ChatModel,
     ChatSession,
     CodeChatModel,
@@ -66,14 +84,15 @@
 from langchain_google_vertexai._image_utils import ImageBytesLoader
 from langchain_google_vertexai._utils import (
     get_generation_info,
     is_codey_model,
     is_gemini_model,
 )
 from langchain_google_vertexai.functions_utils import (
+    _format_tool_config,
     _format_tools_to_vertex_tool,
 )
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -115,58 +134,67 @@
     return chat_history
 
 
 def _parse_chat_history_gemini(
     history: List[BaseMessage],
     project: Optional[str] = None,
     convert_system_message_to_human: Optional[bool] = False,
-) -> List[Content]:
+) -> tuple[Content | None, list[Content]]:
     def _convert_to_prompt(part: Union[str, Dict]) -> Part:
         if isinstance(part, str):
             return Part.from_text(part)
 
         if not isinstance(part, Dict):
             raise ValueError(
                 f"Message's content is expected to be a dict, got {type(part)}!"
             )
         if part["type"] == "text":
             return Part.from_text(part["text"])
-        elif part["type"] == "image_url":
+        if part["type"] == "image_url":
             path = part["image_url"]["url"]
-            image_bytes = ImageBytesLoader(project=project).load_bytes(path)
-            image = Image.from_bytes(image_bytes)
-        else:
-            raise ValueError("Only text and image_url types are supported!")
-        return Part.from_image(image)
+            return ImageBytesLoader(project=project).load_part(path)
+
+        raise ValueError("Only text and image_url types are supported!")
 
     def _convert_to_parts(message: BaseMessage) -> List[Part]:
         raw_content = message.content
         if isinstance(raw_content, str):
             raw_content = [raw_content]
         return [_convert_to_prompt(part) for part in raw_content]
 
     vertex_messages = []
-    raw_system_message = None
+    convert_system_message_to_human_content = None
+    system_instruction = None
     for i, message in enumerate(history):
-        if (
+        if isinstance(message, SystemMessage):
+            if system_instruction is not None:
+                raise ValueError(
+                    "Detected more than one SystemMessage in the list of messages."
+                    "Gemini APIs support the insertion of only one SystemMessage."
+                )
+            else:
+                if convert_system_message_to_human:
+                    logger.warning(
+                        "gemini models released from April 2024 support"
+                        "SystemMessages natively. For best performances,"
+                        "when working with these models,"
+                        "set convert_system_message_to_human to False"
+                    )
+                    convert_system_message_to_human_content = message
+                    continue
+                system_instruction = Content(
+                    role="user", parts=_convert_to_parts(message)
+                )
+                continue
+        elif (
             i == 0
             and isinstance(message, SystemMessage)
-            and not convert_system_message_to_human
+            and convert_system_message_to_human
         ):
-            raise ValueError(
-                """SystemMessages are not yet supported!
-                
-To automatically convert the leading SystemMessage to a HumanMessage,
-set  `convert_system_message_to_human` to True. Example:
-
-llm = ChatVertexAI(model_name="gemini-pro", convert_system_message_to_human=True)
-"""
-            )
-        elif i == 0 and isinstance(message, SystemMessage):
-            raw_system_message = message
+            convert_system_message_to_human_content = message
             continue
         elif isinstance(message, AIMessage):
             raw_function_call = message.additional_kwargs.get("function_call")
             role = "model"
             if raw_function_call:
                 function_call = FunctionCall(
                     {
@@ -178,40 +206,58 @@
                 parts = [Part._from_gapic(gapic_part)]
             else:
                 parts = _convert_to_parts(message)
         elif isinstance(message, HumanMessage):
             role = "user"
             parts = _convert_to_parts(message)
         elif isinstance(message, FunctionMessage):
-            role = "user"
+            role = "function"
             parts = [
                 Part.from_function_response(
                     name=message.name,
                     response={
                         "content": message.content,
                     },
                 )
             ]
+        elif isinstance(message, ToolMessage):
+            role = "function"
+            if (i > 0) and isinstance(history[i - 1], AIMessage):
+                # message.name can be null for ToolMessage
+                if history[i - 1].tool_calls:  # type: ignore
+                    name = history[i - 1].tool_calls[0]["name"]  # type: ignore
+                else:
+                    name = message.name
+            else:
+                name = message.name
+            parts = [
+                Part.from_function_response(
+                    name=name,
+                    response={
+                        "content": message.content,
+                    },
+                )
+            ]
         else:
             raise ValueError(
                 f"Unexpected message with type {type(message)} at the position {i}."
             )
 
-        if raw_system_message:
+        if convert_system_message_to_human_content:
             if role == "model":
                 raise ValueError(
                     "SystemMessage should be followed by a HumanMessage and "
                     "not by AIMessage."
                 )
-            parts = _convert_to_parts(raw_system_message) + parts
-            raw_system_message = None
+            parts = _convert_to_parts(convert_system_message_to_human_content) + parts
+            convert_system_message_to_human_content = None
 
         vertex_message = Content(role=role, parts=parts)
         vertex_messages.append(vertex_message)
-    return vertex_messages
+    return system_instruction, vertex_messages
 
 
 def _parse_examples(examples: List[BaseMessage]) -> List[InputOutputTextPair]:
     if len(examples) % 2 != 0:
         raise ValueError(
             f"Expect examples to have an even amount of messages, got {len(examples)}."
         )
@@ -246,15 +292,30 @@
     if not isinstance(question, HumanMessage):
         raise ValueError(
             f"Last message in the list should be from human, got {question.type}."
         )
     return question
 
 
-def _parse_response_candidate(response_candidate: "Candidate") -> AIMessage:
+def _get_client_with_sys_instruction(
+    client: GenerativeModel,
+    system_instruction: Content,
+    model_name: str,
+):
+    if client._system_instruction != system_instruction:
+        client = GenerativeModel(
+            model_name=model_name,
+            system_instruction=system_instruction,
+        )
+    return client
+
+
+def _parse_response_candidate(
+    response_candidate: "Candidate", streaming: bool = False
+) -> AIMessage:
     try:
         content = response_candidate.text
     except AttributeError:
         content = ""
 
     additional_kwargs = {}
     first_part = response_candidate.content.parts[0]
@@ -264,28 +325,73 @@
         function_call_args_dict = proto.Message.to_dict(first_part.function_call)[
             "args"
         ]
         function_call["arguments"] = json.dumps(
             {k: function_call_args_dict[k] for k in function_call_args_dict}
         )
         additional_kwargs["function_call"] = function_call
+        if streaming:
+            tool_call_chunks = [
+                ToolCallChunk(
+                    name=function_call.get("name"),
+                    args=function_call.get("arguments"),
+                    id=function_call.get("id", str(uuid.uuid4())),
+                    index=function_call.get("index"),
+                )
+            ]
+            return AIMessageChunk(
+                content=content,
+                additional_kwargs=additional_kwargs,
+                tool_call_chunks=tool_call_chunks,
+            )
+        else:
+            tool_calls = []
+            invalid_tool_calls = []
+            try:
+                tool_calls_dicts = parse_tool_calls(
+                    [{"function": function_call}],
+                    return_id=False,
+                )
+                tool_calls = [
+                    ToolCall(
+                        name=tool_call["name"],
+                        args=tool_call["args"],
+                        id=tool_call.get("id", str(uuid.uuid4())),
+                    )
+                    for tool_call in tool_calls_dicts
+                ]
+            except Exception as e:
+                invalid_tool_calls = [
+                    InvalidToolCall(
+                        name=function_call.get("name"),
+                        args=function_call.get("arguments"),
+                        id=function_call.get("id", str(uuid.uuid4())),
+                        error=str(e),
+                    )
+                ]
+
+            return AIMessage(
+                content=content,
+                additional_kwargs=additional_kwargs,
+                tool_calls=tool_calls,
+                invalid_tool_calls=invalid_tool_calls,
+            )
     return AIMessage(content=content, additional_kwargs=additional_kwargs)
 
 
 class ChatVertexAI(_VertexAICommon, BaseChatModel):
     """`Vertex AI` Chat large language models API."""
 
     model_name: str = "chat-bison"
     "Underlying model name."
     examples: Optional[List[BaseMessage]] = None
     convert_system_message_to_human: bool = False
-    """Whether to merge any leading SystemMessage into the following HumanMessage.
-    
-    Gemini does not support system messages; any unsupported messages will 
-    raise an error."""
+    """[Deprecated] Since new Gemini models support setting a System Message,
+    setting this parameter to True is discouraged.
+    """
 
     @classmethod
     def is_lc_serializable(self) -> bool:
         return True
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
@@ -356,31 +462,40 @@
 
         params = self._prepare_params(stop=stop, stream=False, **kwargs)
         msg_params = {}
         if "candidate_count" in params:
             msg_params["candidate_count"] = params.pop("candidate_count")
 
         if self._is_gemini_model:
-            history_gemini = _parse_chat_history_gemini(
+            system_instruction, history_gemini = _parse_chat_history_gemini(
                 messages,
                 project=self.project,
                 convert_system_message_to_human=self.convert_system_message_to_human,
             )
-            message = history_gemini.pop()
-            with telemetry.tool_context_manager(self._user_agent):
-                chat = self.client.start_chat(history=history_gemini)
+            self.client = _get_client_with_sys_instruction(
+                client=self.client,
+                system_instruction=system_instruction,
+                model_name=self.model_name,
+            )
 
             # set param to `functions` until core tool/function calling implemented
             raw_tools = params.pop("functions") if "functions" in params else None
             tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
+            raw_tool_config = (
+                params.pop("tool_config") if "tool_config" in params else None
+            )
+            tool_config = (
+                _format_tool_config(raw_tool_config) if raw_tool_config else None
+            )
             with telemetry.tool_context_manager(self._user_agent):
-                response = chat.send_message(
-                    message,
+                response = self.client.generate_content(
+                    history_gemini,
                     generation_config=params,
                     tools=tools,
+                    tool_config=tool_config,
                     safety_settings=safety_settings,
                 )
             generations = [
                 ChatGeneration(
                     message=_parse_response_candidate(candidate),
                     generation_info=get_generation_info(
                         candidate,
@@ -440,30 +555,40 @@
         params = self._prepare_params(stop=stop, **kwargs)
         safety_settings = kwargs.pop("safety_settings", None)
         msg_params = {}
         if "candidate_count" in params:
             msg_params["candidate_count"] = params.pop("candidate_count")
 
         if self._is_gemini_model:
-            history_gemini = _parse_chat_history_gemini(
+            system_instruction, history_gemini = _parse_chat_history_gemini(
                 messages,
                 project=self.project,
                 convert_system_message_to_human=self.convert_system_message_to_human,
             )
-            message = history_gemini.pop()
-            with telemetry.tool_context_manager(self._user_agent):
-                chat = self.client.start_chat(history=history_gemini)
+
+            self.client = _get_client_with_sys_instruction(
+                client=self.client,
+                system_instruction=system_instruction,
+                model_name=self.model_name,
+            )
             # set param to `functions` until core tool/function calling implemented
             raw_tools = params.pop("functions") if "functions" in params else None
             tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
+            raw_tool_config = (
+                params.pop("tool_config") if "tool_config" in params else None
+            )
+            tool_config = (
+                _format_tool_config(raw_tool_config) if raw_tool_config else None
+            )
             with telemetry.tool_context_manager(self._user_agent):
-                response = await chat.send_message_async(
-                    message,
+                response = await self.client.generate_content_async(
+                    history_gemini,
                     generation_config=params,
                     tools=tools,
+                    tool_config=tool_config,
                     safety_settings=safety_settings,
                 )
             generations = [
                 ChatGeneration(
                     message=_parse_response_candidate(c),
                     generation_info=get_generation_info(
                         c,
@@ -500,49 +625,67 @@
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         params = self._prepare_params(stop=stop, stream=True, **kwargs)
         if self._is_gemini_model:
-            history_gemini = _parse_chat_history_gemini(
+            safety_settings = params.pop("safety_settings", None)
+            system_instruction, history_gemini = _parse_chat_history_gemini(
                 messages,
                 project=self.project,
                 convert_system_message_to_human=self.convert_system_message_to_human,
             )
-            message = history_gemini.pop()
-            with telemetry.tool_context_manager(self._user_agent):
-                chat = self.client.start_chat(history=history_gemini)
+            self.client = _get_client_with_sys_instruction(
+                client=self.client,
+                system_instruction=system_instruction,
+                model_name=self.model_name,
+            )
             # set param to `functions` until core tool/function calling implemented
             raw_tools = params.pop("functions") if "functions" in params else None
             tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
-            safety_settings = params.pop("safety_settings", None)
+            raw_tool_config = (
+                params.pop("tool_config") if "tool_config" in params else None
+            )
+            tool_config = (
+                _format_tool_config(raw_tool_config) if raw_tool_config else None
+            )
             with telemetry.tool_context_manager(self._user_agent):
-                responses = chat.send_message(
-                    message,
+                responses = self.client.generate_content(
+                    history_gemini,
                     stream=True,
                     generation_config=params,
-                    safety_settings=safety_settings,
                     tools=tools,
+                    tool_config=tool_config,
+                    safety_settings=safety_settings,
                 )
                 for response in responses:
-                    message = _parse_response_candidate(response.candidates[0])
-                    if run_manager:
-                        run_manager.on_llm_new_token(message.content)
-                    yield ChatGenerationChunk(
-                        message=AIMessageChunk(
-                            content=message.content,
-                            additional_kwargs=message.additional_kwargs,
-                        ),
-                        generation_info=get_generation_info(
-                            response.candidates[0],
-                            self._is_gemini_model,
-                            usage_metadata=response.to_dict().get("usage_metadata"),
-                        ),
+                    message = _parse_response_candidate(
+                        response.candidates[0], streaming=True
                     )
+                    generation_info = get_generation_info(
+                        response.candidates[0],
+                        self._is_gemini_model,
+                        usage_metadata=response.to_dict().get("usage_metadata"),
+                    )
+                    if run_manager and isinstance(message.content, str):
+                        run_manager.on_llm_new_token(message.content)
+                    if isinstance(message, AIMessageChunk):
+                        yield ChatGenerationChunk(
+                            message=message,
+                            generation_info=generation_info,
+                        )
+                    else:
+                        yield ChatGenerationChunk(
+                            message=AIMessageChunk(
+                                content=message.content,
+                                additional_kwargs=message.additional_kwargs,
+                            ),
+                            generation_info=generation_info,
+                        )
         else:
             question = _get_question(messages)
             history = _parse_chat_history(messages[:-1])
             examples = kwargs.get("examples", None)
             if examples:
                 params["examples"] = _parse_examples(examples)
             with telemetry.tool_context_manager(self._user_agent):
@@ -566,47 +709,60 @@
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         if not self._is_gemini_model:
             raise NotImplementedError()
         params = self._prepare_params(stop=stop, stream=True, **kwargs)
-        history_gemini = _parse_chat_history_gemini(
+        safety_settings = params.pop("safety_settings", None)
+        system_instruction, history_gemini = _parse_chat_history_gemini(
             messages,
             project=self.project,
             convert_system_message_to_human=self.convert_system_message_to_human,
         )
         message = history_gemini.pop()
-        with telemetry.tool_context_manager(self._user_agent):
-            chat = self.client.start_chat(history=history_gemini)
+        self.client = _get_client_with_sys_instruction(
+            client=self.client,
+            system_instruction=system_instruction,
+            model_name=self.model_name,
+        )
         raw_tools = params.pop("functions") if "functions" in params else None
         tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
-        safety_settings = params.pop("safety_settings", None)
+        raw_tool_config = params.pop("tool_config") if "tool_config" in params else None
+        tool_config = _format_tool_config(raw_tool_config) if raw_tool_config else None
         with telemetry.tool_context_manager(self._user_agent):
-            async for chunk in await chat.send_message_async(
-                message,
+            async for chunk in await self.client.generate_content_async(
+                history_gemini,
                 stream=True,
                 generation_config=params,
-                safety_settings=safety_settings,
                 tools=tools,
+                tool_config=tool_config,
+                safety_settings=safety_settings,
             ):
-                message = _parse_response_candidate(chunk.candidates[0])
-                if run_manager:
-                    await run_manager.on_llm_new_token(message.content)
-                yield ChatGenerationChunk(
-                    message=AIMessageChunk(
-                        content=message.content,
-                        additional_kwargs=message.additional_kwargs,
-                    ),
-                    generation_info=get_generation_info(
-                        chunk.candidates[0],
-                        self._is_gemini_model,
-                        usage_metadata=chunk.to_dict().get("usage_metadata"),
-                    ),
+                message = _parse_response_candidate(chunk.candidates[0], streaming=True)
+                generation_info = get_generation_info(
+                    chunk.candidates[0],
+                    self._is_gemini_model,
+                    usage_metadata=chunk.to_dict().get("usage_metadata"),
                 )
+                if run_manager and isinstance(message.content, str):
+                    await run_manager.on_llm_new_token(message.content)
+                if isinstance(message, AIMessageChunk):
+                    yield ChatGenerationChunk(
+                        message=message,
+                        generation_info=generation_info,
+                    )
+                else:
+                    yield ChatGenerationChunk(
+                        message=AIMessageChunk(
+                            content=message.content,
+                            additional_kwargs=message.additional_kwargs,
+                        ),
+                        generation_info=generation_info,
+                    )
 
     def with_structured_output(
         self,
         schema: Union[Dict, Type[BaseModel]],
         *,
         include_raw: bool = False,
         **kwargs: Any,
@@ -714,14 +870,45 @@
                 [RunnablePassthrough.assign(parsed=lambda _: None)],
                 exception_key="parsing_error",
             )
             return {"raw": llm} | parser_with_fallback
         else:
             return llm | parser
 
+    def bind_tools(
+        self,
+        tools: Sequence[Union[Type[BaseModel], Callable, BaseTool]],
+        **kwargs: Any,
+    ) -> Runnable[LanguageModelInput, BaseMessage]:
+        """Bind tool-like objects to this chat model.
+
+        Assumes model is compatible with Vertex tool-calling API.
+
+        Args:
+            tools: A list of tool definitions to bind to this chat model.
+                Can be a pydantic model, callable, or BaseTool. Pydantic
+                models, callables, and BaseTools will be automatically converted to
+                their schema dictionary representation.
+            **kwargs: Any additional parameters to pass to the
+                :class:`~langchain.runnable.Runnable` constructor.
+        """
+        formatted_tools = []
+        for schema in tools:
+            if isinstance(schema, BaseTool) or (
+                isinstance(schema, type) and issubclass(schema, BaseModel)
+            ):
+                formatted_tools.append(schema)
+            elif callable(schema):
+                formatted_tools.append(tool_from_callable(schema))  # type: ignore
+            else:
+                raise ValueError(
+                    "Tool must be a BaseTool, Pydantic model, or callable."
+                )
+        return super().bind(functions=formatted_tools, **kwargs)
+
     def _start_chat(
         self, history: _ChatHistory, **kwargs: Any
     ) -> Union[ChatSession, CodeChatSession]:
         if not self.is_codey_model:
             return self.client.start_chat(
                 context=history.context, message_history=history.history, **kwargs
             )
```

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/embeddings.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/functions_utils.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/functions_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from vertexai.generative_models import (  # type: ignore
     FunctionDeclaration,
 )
 from vertexai.generative_models import (
     Tool as VertexTool,
 )
 
+# FIXME: vertexai is not exporting ToolConfig
+from vertexai.generative_models._generative_models import (  # type: ignore
+    ToolConfig,
+)
+
 
 def _format_pydantic_to_vertex_function(
     pydantic_model: Type[BaseModel],
 ) -> FunctionDescription:
     schema = pydantic_model.schema()
 
     return {
@@ -71,25 +76,34 @@
         else:
             raise ValueError(f"Unsupported tool call type {tool}")
         function_declarations.append(FunctionDeclaration(**func))
 
     return [VertexTool(function_declarations=function_declarations)]
 
 
+def _format_tool_config(tool_config: Dict[str, Any]) -> Union[ToolConfig, None]:
+    if "function_calling_config" not in tool_config:
+        return None
+    return ToolConfig(
+        function_calling_config=ToolConfig.FunctionCallingConfig(
+            **tool_config["function_calling_config"]
+        )
+    )
+
+
 class ParametersSchema(BaseModel):
     """
     This is a schema of currently supported definitions in function calling.
-    We need explicitly exclude `title` and `definitions` fields as they
-    are not currently supported.
+    We need explicitly exclude `definitions` field
+    as it is not currently supported.
 
     All other fields will be passed through (as extra fields are allowed)
     and intercepted on `google.cloud.aiplatform` level
     """
 
-    title: Optional[str] = Field(exclude=True)
     definitions: Optional[Any] = Field(exclude=True)
     items: Optional["ParametersSchema"]
     properties: Optional[Dict[str, "ParametersSchema"]]
 
     class Config:
         extra = "allow"
```

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/gemma.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/gemma.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/llms.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_sdk_manager.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_sdk_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_searcher.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_searcher.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/_utils.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/vectorstores/vectorstores.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/vectorstores.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     Namespace,
     NumericNamespace,
 )
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
-from langchain_google_vertexai.vectorstores._document_storage import (
-    DataStoreDocumentStorage,
-    DocumentStorage,
-    GCSDocumentStorage,
-)
 from langchain_google_vertexai.vectorstores._sdk_manager import VectorSearchSDKManager
 from langchain_google_vertexai.vectorstores._searcher import (
     Searcher,
     VectorSearchSearcher,
 )
+from langchain_google_vertexai.vectorstores.document_storage import (
+    DataStoreDocumentStorage,
+    DocumentStorage,
+    GCSDocumentStorage,
+)
 
 
 class _BaseVertexAIVectorStore(VectorStore):
     """Represents a base vector store based on VertexAI."""
 
     def __init__(
         self,
@@ -111,27 +111,27 @@
             Lower score represents more similarity.
         """
 
         neighbors_list = self._searcher.find_neighbors(
             embeddings=[embedding], k=k, filter_=filter, numeric_filter=numeric_filter
         )
 
-        results = []
-
-        for neighbor_id, distance in neighbors_list[0]:
-            document = self._document_storage.get_by_id(neighbor_id)
-
-            if document is None:
-                raise ValueError(
-                    f"Document with id {neighbor_id} not found in document" "storage."
-                )
-
-            results.append((document, distance))
-
-        return results
+        keys = [key for key, _ in neighbors_list[0]]
+        distances = [distance for _, distance in neighbors_list[0]]
+        documents = self._document_storage.mget(keys)
+
+        if all(document is not None for document in documents):
+            # Ignore typing because mypy doesn't seem to be able to identify that
+            # in documents there is no possibility to have None values with the
+            # check above.
+            return list(zip(documents, distances))  # type: ignore
+        else:
+            missing_docs = [key for key, doc in zip(keys, documents) if doc is None]
+            message = f"Documents with ids: {missing_docs} not found in the storage"
+            raise ValueError(message)
 
     def similarity_search(
         self,
         query: str,
         k: int = 4,
         filter: Optional[List[Namespace]] = None,
         numeric_filter: Optional[List[NumericNamespace]] = None,
@@ -193,15 +193,15 @@
             )
 
         documents = [
             Document(page_content=text, metadata=metadata)
             for text, metadata in zip(texts, metadatas)
         ]
 
-        self._document_storage.batch_store_by_id(ids=ids, documents=documents)
+        self._document_storage.mset(list(zip(ids, documents)))
 
         embeddings = self._embeddings.embed_documents(texts)
 
         self._searcher.add_to_index(
             ids, embeddings, metadatas, is_complete_overwrite, **kwargs
         )
```

### Comparing `langchain_google_vertexai-0.1.2/langchain_google_vertexai/vision_models.py` & `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vision_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 from google.cloud.aiplatform import telemetry
 from langchain_core.callbacks import CallbackManagerForLLMRun
 from langchain_core.language_models import BaseChatModel, BaseLLM
 from langchain_core.messages import AIMessage, BaseMessage
 from langchain_core.outputs import ChatResult, LLMResult
 from langchain_core.outputs.chat_generation import ChatGeneration
@@ -25,26 +25,31 @@
 )
 from langchain_google_vertexai._utils import get_user_agent
 
 
 class _BaseImageTextModel(BaseModel):
     """Base class for all integrations that use ImageTextModel"""
 
+    cached_client: Any = Field(default=None)
     model_name: str = Field(default="imagetext@001")
     """ Name of the model to use"""
     number_of_results: int = Field(default=1)
     """Number of results to return from one query"""
     language: str = Field(default="en")
     """Language of the query"""
     project: Union[str, None] = Field(default=None)
     """Google cloud project"""
 
-    def _create_model(self) -> ImageTextModel:
-        """Builds the model object from the class attributes."""
-        return ImageTextModel.from_pretrained(model_name=self.model_name)
+    @property
+    def client(self) -> ImageTextModel:
+        if self.cached_client is None:
+            self.cached_client = ImageTextModel.from_pretrained(
+                model_name=self.model_name,
+            )
+        return self.cached_client
 
     def _get_image_from_message_part(self, message_part: str | Dict) -> Image | None:
         """Given a message part obtain a image if the part represents it.
 
         Args:
             message_part: Item of a message content.
 
@@ -79,34 +84,50 @@
 
     @property
     def _user_agent(self) -> str:
         """Gets the User Agent."""
         _, user_agent = get_user_agent(f"{type(self).__name__}_{self.model_name}")
         return user_agent
 
+    @property
+    def _default_params(self) -> Dict[str, Any]:
+        return {"number_of_results": self.number_of_results, "language": self.language}
+
+    def _prepare_params(self, **kwargs: Any) -> Dict[str, Any]:
+        params = self._default_params
+        for key, value in kwargs.items():
+            if key in params and value is not None:
+                params[key] = value
+        return params
+
 
 class _BaseVertexAIImageCaptioning(_BaseImageTextModel):
     """Base class for Image Captioning models."""
 
-    def _get_captions(self, image: Image) -> List[str]:
+    def _get_captions(
+        self,
+        image: Image,
+        number_of_results: Optional[int] = None,
+        language: Optional[str] = None,
+    ) -> List[str]:
         """Uses the sdk methods to generate a list of captions.
 
         Args:
             image: Image to get the captions for.
+            number_of_results: Number of results to return from one query.
+            language: Language of the query.
 
         Returns:
             List of captions obtained from the image.
         """
         with telemetry.tool_context_manager(self._user_agent):
-            model = self._create_model()
-            captions = model.get_captions(
-                image=image,
-                number_of_results=self.number_of_results,
-                language=self.language,
+            params = self._prepare_params(
+                number_of_results=number_of_results, language=language
             )
+            captions = self.client.get_captions(image=image, **params)
             return captions
 
 
 class VertexAIImageCaptioning(_BaseVertexAIImageCaptioning, BaseLLM):
     """Implementation of the Image Captioning model as an LLM."""
 
     def _generate(
@@ -126,31 +147,33 @@
                 - Local file path
                 - Remote url
 
         Returns:
             Captions generated from every prompt.
         """
 
-        generations = [self._generate_one(prompt=prompt) for prompt in prompts]
+        generations = [
+            self._generate_one(prompt=prompt, **kwargs) for prompt in prompts
+        ]
 
         return LLMResult(generations=generations)
 
-    def _generate_one(self, prompt: str) -> List[Generation]:
+    def _generate_one(self, prompt: str, **kwargs) -> List[Generation]:
         """Generates the captions for a single prompt.
 
         Args:
             prompt: Image url for the generation.
 
         Returns:
             List of generations
         """
         image_loader = ImageBytesLoader(project=self.project)
         image_bytes = image_loader.load_bytes(prompt)
         image = Image(image_bytes=image_bytes)
-        caption_list = self._get_captions(image=image)
+        caption_list = self._get_captions(image=image, **kwargs)
         return [Generation(text=caption) for caption in caption_list]
 
 
 class VertexAIImageCaptioningChat(_BaseVertexAIImageCaptioning, BaseChatModel):
     """Implementation of the Image Captioning model as a chat."""
 
     def _generate(
@@ -195,26 +218,30 @@
             raise ValueError(
                 f"{self.__class__.__name__} messages should be a list with "
                 "only one message. This message content must be a list with "
                 "one dictionary with the format: "
                 "{'type': 'image_url', 'image_url': {'image': <image_str>}}"
             )
 
-        captions = self._get_captions(image)
+        captions = self._get_captions(image, **messages[0].additional_kwargs)
 
         generations = [
             ChatGeneration(message=AIMessage(content=caption)) for caption in captions
         ]
 
         return ChatResult(generations=generations)
 
 
 class VertexAIVisualQnAChat(_BaseImageTextModel, BaseChatModel):
     """Chat implementation of a visual QnA model"""
 
+    @property
+    def _default_params(self) -> Dict[str, Any]:
+        return {"number_of_results": self.number_of_results}
+
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: List[str] | None = None,
         run_manager: CallbackManagerForLLMRun | None = None,
         **kwargs: Any,
     ) -> ChatResult:
@@ -253,113 +280,127 @@
                 "two elements. The first element should be the image, a dictionary "
                 "with format"
                 "{'type': 'image_url', 'image_url': {'image': <image_str>}}."
                 "The second one should be the user question. Either a simple string"
                 "or a dictionary with format {'type': 'text', 'text': <message>}"
             )
 
-        answers = self._ask_questions(image=image, query=user_question)
+        answers = self._ask_questions(
+            image=image, query=user_question, **messages[0].additional_kwargs
+        )
 
         generations = [
             ChatGeneration(message=AIMessage(content=answer)) for answer in answers
         ]
 
         return ChatResult(generations=generations)
 
-    def _ask_questions(self, image: Image, query: str) -> List[str]:
+    def _ask_questions(
+        self, image: Image, query: str, number_of_results: Optional[int] = None
+    ) -> List[str]:
         """Interfaces with the sdk to get the question.
 
         Args:
             image: Image to question about.
             query: User query.
 
         Returns:
             List of responses to the query.
         """
         with telemetry.tool_context_manager(self._user_agent):
-            model = self._create_model()
-            answers = model.ask_question(
-                image=image, question=query, number_of_results=self.number_of_results
-            )
+            params = self._prepare_params(number_of_results=number_of_results)
+            answers = self.client.ask_question(image=image, question=query, **params)
             return answers
 
 
 class _BaseVertexAIImageGenerator(BaseModel):
     """Base class form generation and edition of images."""
 
+    cached_client: Any = Field(default=None)
     model_name: str = Field(default="imagegeneration@002")
     """Name of the base model"""
     negative_prompt: Union[str, None] = Field(default=None)
     """A description of what you want to omit in
         the generated images"""
-    number_of_images: int = Field(default=1)
+    number_of_results: int = Field(default=1)
     """Number of images to generate"""
     guidance_scale: Union[float, None] = Field(default=None)
     """Controls the strength of the prompt"""
     language: Union[str, None] = Field(default=None)
     """Language of the text prompt for the image Supported values are "en" for English, 
     "hi" for Hindi, "ja" for Japanese, "ko" for Korean, and "auto" for automatic 
     language detection"""
     seed: Union[int, None] = Field(default=None)
     """Random seed for the image generation"""
     project: Union[str, None] = Field(default=None)
     """Google cloud project id"""
 
-    def _generate_images(self, prompt: str) -> List[str]:
+    @property
+    def client(self) -> ImageGenerationModel:
+        if not self.cached_client:
+            self.cached_client = ImageGenerationModel.from_pretrained(
+                model_name=self.model_name,
+            )
+        return self.cached_client
+
+    @property
+    def _default_params(self) -> Dict[str, Any]:
+        return {
+            "number_of_images": self.number_of_results,
+            "language": self.language,
+            "negative_prompt": self.negative_prompt,
+            "guidance_scale": self.guidance_scale,
+            "seed": self.seed,
+        }
+
+    def _prepare_params(self, **kwargs: Any) -> Dict[str, Any]:
+        params = self._default_params
+        mapping = {"number_of_results": "number_of_images"}
+        for key, value in kwargs.items():
+            key = mapping.get(key, key)
+            if key in params and value is not None:
+                params[key] = value
+        return {k: v for k, v in params.items() if v is not None}
+
+    def _generate_images(self, prompt: str, **kwargs: Any) -> List[str]:
         """Generates images given a prompt.
 
         Args:
             prompt: Description of what the image should look like.
 
         Returns:
             List of b64 encoded strings.
         """
         with telemetry.tool_context_manager(self._user_agent):
-            model = ImageGenerationModel.from_pretrained(self.model_name)
-
-            generation_result = model.generate_images(
-                prompt=prompt,
-                negative_prompt=self.negative_prompt,
-                number_of_images=self.number_of_images,
-                language=self.language,
-                guidance_scale=self.guidance_scale,
-                seed=self.seed,
+            generation_result = self.client.generate_images(
+                prompt=prompt, **self._prepare_params(**kwargs)
             )
 
         image_str_list = [
             self._to_b64_string(image) for image in generation_result.images
         ]
 
         return image_str_list
 
-    def _edit_images(self, image_str: str, prompt: str) -> List[str]:
+    def _edit_images(self, image_str: str, prompt: str, **kwargs: Any) -> List[str]:
         """Edit an image given a image and a prompt.
 
         Args:
             image_str: String representation of the image.
             prompt: Description of what the image should look like.
 
         Returns:
             List of b64 encoded strings.
         """
         with telemetry.tool_context_manager(self._user_agent):
-            model = ImageGenerationModel.from_pretrained(self.model_name)
-
             image_loader = ImageBytesLoader(project=self.project)
             image_bytes = image_loader.load_bytes(image_str)
             image = Image(image_bytes=image_bytes)
-
-            generation_result = model.edit_image(
-                prompt=prompt,
-                base_image=image,
-                negative_prompt=self.negative_prompt,
-                number_of_images=self.number_of_images,
-                language=self.language,
-                guidance_scale=self.guidance_scale,
-                seed=self.seed,
+            generation_result = self.client.edit_image(
+                prompt=prompt, base_image=image, **self._prepare_params(**kwargs)
             )
 
         image_str_list = [
             self._to_b64_string(image) for image in generation_result.images
         ]
 
         return image_str_list
@@ -423,15 +464,17 @@
             user_query = get_text_str_from_content_part(messages[0].content[0])
         if user_query is None:
             raise ValueError(
                 "Only one message with one text part allowed for image generation"
                 " Must The prompt of the image"
             )
 
-        image_str_list = self._generate_images(prompt=user_query)
+        image_str_list = self._generate_images(
+            prompt=user_query, **messages[0].additional_kwargs
+        )
         image_content_part_list = [
             create_image_content_part(image_str=image_str)
             for image_str in image_str_list
         ]
 
         generations = [
             ChatGeneration(message=AIMessage(content=[content_part]))
@@ -470,15 +513,17 @@
             user_query = get_text_str_from_content_part(messages[0].content[1])
         if (user_query is None) or (image_str is None):
             raise ValueError(
                 "Only one message allowed for image edition. The message must have"
                 "two parts: First the image and then the user prompt."
             )
 
-        image_str_list = self._edit_images(image_str=image_str, prompt=user_query)
+        image_str_list = self._edit_images(
+            image_str=image_str, prompt=user_query, **messages[0].additional_kwargs
+        )
         image_content_part_list = [
             create_image_content_part(image_str=image_str)
             for image_str in image_str_list
         ]
 
         generations = [
             ChatGeneration(message=AIMessage(content=[content_part]))
```

### Comparing `langchain_google_vertexai-0.1.2/PKG-INFO` & `langchain_google_vertexai-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: langchain-google-vertexai
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integration package connecting Google VertexAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: google-cloud-aiplatform (>=1.44.0,<2.0.0)
+Provides-Extra: anthropic
+Requires-Dist: anthropic[vertexai] (>=0.23.0,<1) ; extra == "anthropic"
+Requires-Dist: google-cloud-aiplatform (>=1.47.0,<2.0.0)
 Requires-Dist: google-cloud-storage (>=2.14.0,<3.0.0)
-Requires-Dist: langchain-core (>=0.1.27,<0.2)
+Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
 Requires-Dist: types-protobuf (>=4.24.0.4,<5.0.0.0)
 Requires-Dist: types-requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/vertexai
 Description-Content-Type: text/markdown
 
 # langchain-google-vertexai
```

