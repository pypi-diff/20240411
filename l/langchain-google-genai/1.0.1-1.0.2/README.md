# Comparing `tmp/langchain_google_genai-1.0.1.tar.gz` & `tmp/langchain_google_genai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_genai-1.0.1.tar", max compression
+gzip compressed data, was "langchain_google_genai-1.0.2.tar", max compression
```

## Comparing `langchain_google_genai-1.0.1.tar` & `langchain_google_genai-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/LICENSE
--rw-r--r--   0        0        0     2875 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/README.md
--rw-r--r--   0        0        0     2762 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/__init__.py
--rw-r--r--   0        0        0      136 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/_common.py
--rw-r--r--   0        0        0      163 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/_enums.py
--rw-r--r--   0        0        0     3640 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/_function_utils.py
--rw-r--r--   0        0        0    18736 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/_genai_extension.py
--rw-r--r--   0        0        0    23680 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/chat_models.py
--rw-r--r--   0        0        0     4562 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/embeddings.py
--rw-r--r--   0        0        0     4303 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/genai_aqa.py
--rw-r--r--   0        0        0    16139 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/google_vector_store.py
--rw-r--r--   0        0        0    12994 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/llms.py
--rw-r--r--   0        0        0        0 2024-03-27 10:34:12.211817 langchain_google_genai-1.0.1/langchain_google_genai/py.typed
--rw-r--r--   0        0        0     2700 2024-03-27 10:34:12.215817 langchain_google_genai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2875 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/README.md
+-rw-r--r--   0        0        0     2762 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/__init__.py
+-rw-r--r--   0        0        0      136 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_common.py
+-rw-r--r--   0        0        0      163 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_enums.py
+-rw-r--r--   0        0        0     3640 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_function_utils.py
+-rw-r--r--   0        0        0    18736 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/_genai_extension.py
+-rw-r--r--   0        0        0    23557 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/chat_models.py
+-rw-r--r--   0        0        0     4562 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/embeddings.py
+-rw-r--r--   0        0        0     4303 2024-04-11 17:35:33.148180 langchain_google_genai-1.0.2/langchain_google_genai/genai_aqa.py
+-rw-r--r--   0        0        0    16139 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/langchain_google_genai/google_vector_store.py
+-rw-r--r--   0        0        0    13193 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/langchain_google_genai/llms.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/langchain_google_genai/py.typed
+-rw-r--r--   0        0        0     3012 2024-04-11 17:35:33.152180 langchain_google_genai-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.2/PKG-INFO
```

### Comparing `langchain_google_genai-1.0.1/LICENSE` & `langchain_google_genai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/README.md` & `langchain_google_genai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/__init__.py` & `langchain_google_genai-1.0.2/langchain_google_genai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/_function_utils.py` & `langchain_google_genai-1.0.2/langchain_google_genai/_function_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/_genai_extension.py` & `langchain_google_genai-1.0.2/langchain_google_genai/_genai_extension.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/chat_models.py` & `langchain_google_genai-1.0.2/langchain_google_genai/chat_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import base64
 import json
 import logging
 import os
+import warnings
 from io import BytesIO
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
@@ -296,35 +297,24 @@
                 "Gemini only supports text and inline_data parts."
             )
     return parts
 
 
 def _parse_chat_history(
     input_messages: Sequence[BaseMessage], convert_system_message_to_human: bool = False
-) -> List[genai.types.ContentDict]:
+) -> Tuple[Optional[genai.types.ContentDict], List[genai.types.ContentDict]]:
     messages: List[genai.types.MessageDict] = []
 
-    raw_system_message: Optional[SystemMessage] = None
-    for i, message in enumerate(input_messages):
-        if (
-            i == 0
-            and isinstance(message, SystemMessage)
-            and not convert_system_message_to_human
-        ):
-            raise ValueError(
-                """SystemMessages are not yet supported!
-
-To automatically convert the leading SystemMessage to a HumanMessage,
-set  `convert_system_message_to_human` to True. Example:
+    if convert_system_message_to_human:
+        warnings.warn("Convert_system_message_to_human will be deprecated!")
 
-llm = ChatGoogleGenerativeAI(model="gemini-pro", convert_system_message_to_human=True)
-"""
-            )
-        elif i == 0 and isinstance(message, SystemMessage):
-            raw_system_message = message
+    system_instruction: Optional[genai.types.ContentDict] = None
+    for i, message in enumerate(input_messages):
+        if i == 0 and isinstance(message, SystemMessage):
+            system_instruction = _convert_to_parts(message.content)
             continue
         elif isinstance(message, AIMessage):
             role = "model"
             raw_function_call = message.additional_kwargs.get("function_call")
             if raw_function_call:
                 function_call = glm.FunctionCall(
                     {
@@ -361,24 +351,16 @@
                 )
             ]
         else:
             raise ValueError(
                 f"Unexpected message with type {type(message)} at the position {i}."
             )
 
-        if raw_system_message:
-            if role == "model":
-                raise ValueError(
-                    "SystemMessage should be followed by a HumanMessage and "
-                    "not by AIMessage."
-                )
-            parts = _convert_to_parts(raw_system_message.content) + parts
-            raw_system_message = None
         messages.append({"role": role, "parts": parts})
-    return messages
+    return system_instruction, messages
 
 
 def _parse_response_candidate(
     response_candidate: glm.Candidate, stream: bool
 ) -> AIMessage:
     first_part = response_candidate.content.parts[0]
     if first_part.function_call:
@@ -479,31 +461,36 @@
     @classmethod
     def is_lc_serializable(self) -> bool:
         return True
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validates params and passes them to google-generativeai package."""
+        additional_headers = values.get("additional_headers") or {}
+        default_metadata = tuple(additional_headers.items())
+
         if values.get("credentials"):
             genai.configure(
                 credentials=values.get("credentials"),
                 transport=values.get("transport"),
                 client_options=values.get("client_options"),
+                default_metadata=default_metadata,
             )
         else:
             google_api_key = get_from_dict_or_env(
                 values, "google_api_key", "GOOGLE_API_KEY"
             )
             if isinstance(google_api_key, SecretStr):
                 google_api_key = google_api_key.get_secret_value()
 
             genai.configure(
                 api_key=google_api_key,
                 transport=values.get("transport"),
                 client_options=values.get("client_options"),
+                default_metadata=default_metadata,
             )
         if (
             values.get("temperature") is not None
             and not 0 <= values["temperature"] <= 1
         ):
             raise ValueError("temperature must be in the range [0.0, 1.0]")
 
@@ -650,19 +637,23 @@
                 convert_to_genai_function_declarations(functions) if functions else None
             )
             client = genai.GenerativeModel(
                 model_name=self.model, tools=tools, safety_settings=safety_settings
             )
 
         params = self._prepare_params(stop, **kwargs)
-        history = _parse_chat_history(
+        system_instruction, history = _parse_chat_history(
             messages,
             convert_system_message_to_human=self.convert_system_message_to_human,
         )
         message = history.pop()
+        if self.client._system_instruction != system_instruction:
+            self.client = genai.GenerativeModel(
+                model_name=self.model, system_instruction=system_instruction
+            )
         chat = client.start_chat(history=history)
         return params, chat, message
 
     def get_num_tokens(self, text: str) -> int:
         """Get the number of tokens present in the text.
 
         Useful for checking if an input will fit in a model's context window.
```

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/embeddings.py` & `langchain_google_genai-1.0.2/langchain_google_genai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/genai_aqa.py` & `langchain_google_genai-1.0.2/langchain_google_genai/genai_aqa.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/google_vector_store.py` & `langchain_google_genai-1.0.2/langchain_google_genai/google_vector_store.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.1/langchain_google_genai/llms.py` & `langchain_google_genai-1.0.2/langchain_google_genai/llms.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,14 +150,20 @@
             "such as `api_endpoint`."
         ),
     )
     transport: Optional[str] = Field(
         None,
         description="A string, one of: [`rest`, `grpc`, `grpc_asyncio`].",
     )
+    additional_headers: Optional[Dict[str, str]] = Field(
+        None,
+        description=(
+            "A key-value dictionary representing additional headers for the model call"
+        ),
+    )
 
     safety_settings: Optional[Dict[HarmCategory, HarmBlockThreshold]] = None
     """The default safety settings to use for all generations. 
     
         For example: 
 
             from google.generativeai.types.safety_types import HarmBlockThreshold, HarmCategory
```

### Comparing `langchain_google_genai-1.0.1/pyproject.toml` & `langchain_google_genai-1.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-google-genai"
-version = "1.0.1"
+version = "1.0.2"
 description = "An integration package connecting Google's genai package and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-google/tree/main/libs/genai"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = "^0.1"
-google-generativeai = "^0.4.1"
+langchain-core = ">=0.1.27,<0.2"
+google-generativeai = "^0.5.0"
 pillow = { version = "^10.1.0", optional = true }
 
 [tool.poetry.extras]
 images = ["pillow"]
 
 [tool.poetry.group.test]
 optional = true
@@ -26,14 +26,15 @@
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 numpy = "^1.26.2"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -52,23 +53,25 @@
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
 types-requests = "^2.28.11.5"
 types-google-cloud-ndb = "^2.2.0.1"
 types-pillow = "^10.1.0.2"
 types-protobuf = "^4.24.0.20240302"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pillow = "^10.1.0"
 types-requests = "^2.31.0.10"
 types-pillow = "^10.1.0.2"
 types-google-cloud-ndb = "^2.2.0.1"
+langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
```

### Comparing `langchain_google_genai-1.0.1/PKG-INFO` & `langchain_google_genai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-google-genai
-Version: 1.0.1
+Version: 1.0.2
 Summary: An integration package connecting Google's genai package and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: images
-Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
-Requires-Dist: langchain-core (>=0.1,<0.2)
+Requires-Dist: google-generativeai (>=0.5.0,<0.6.0)
+Requires-Dist: langchain-core (>=0.1.27,<0.2)
 Requires-Dist: pillow (>=10.1.0,<11.0.0) ; extra == "images"
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/genai
 Description-Content-Type: text/markdown
 
 # langchain-google-genai
```

