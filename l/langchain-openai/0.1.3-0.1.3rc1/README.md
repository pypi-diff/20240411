# Comparing `tmp/langchain_openai-0.1.3.tar.gz` & `tmp/langchain_openai-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.3.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.3rc1.tar", max compression
```

## Comparing `langchain_openai-0.1.3.tar` & `langchain_openai-0.1.3rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/LICENSE
--rw-r--r--   0        0        0     1627 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/README.md
--rw-r--r--   0        0        0      371 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10508 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    45927 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    23294 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24477 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/langchain_openai/py.typed
--rw-r--r--   0        0        0     2819 2024-04-11 16:20:35.124399 langchain_openai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     1627 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      371 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10508 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    44617 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    23294 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8008 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24477 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2865 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 langchain_openai-0.1.3rc1/PKG-INFO
```

### Comparing `langchain_openai-0.1.3/LICENSE` & `langchain_openai-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/README.md` & `langchain_openai-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.3rc1/langchain_openai/chat_models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """OpenAI chat wrapper."""
 
 from __future__ import annotations
 
-import json
 import logging
 import os
 import sys
 from operator import itemgetter
 from typing import (
     Any,
     AsyncIterator,
@@ -47,18 +46,16 @@
     BaseMessageChunk,
     ChatMessage,
     ChatMessageChunk,
     FunctionMessage,
     FunctionMessageChunk,
     HumanMessage,
     HumanMessageChunk,
-    InvalidToolCall,
     SystemMessage,
     SystemMessageChunk,
-    ToolCall,
     ToolMessage,
     ToolMessageChunk,
 )
 from langchain_core.output_parsers import (
     JsonOutputParser,
     PydanticOutputParser,
 )
@@ -168,33 +165,22 @@
         message_dict["role"] = message.role
     elif isinstance(message, HumanMessage):
         message_dict["role"] = "user"
     elif isinstance(message, AIMessage):
         message_dict["role"] = "assistant"
         if "function_call" in message.additional_kwargs:
             message_dict["function_call"] = message.additional_kwargs["function_call"]
-        if message.tool_calls or message.invalid_tool_calls:
-            message_dict["tool_calls"] = [
-                _lc_tool_call_to_openai_tool_call(tc) for tc in message.tool_calls
-            ] + [
-                _lc_invalid_tool_call_to_openai_tool_call(tc)
-                for tc in message.invalid_tool_calls
-            ]
-        elif "tool_calls" in message.additional_kwargs:
+            # If function call only, content is None not empty string
+            if message_dict["content"] == "":
+                message_dict["content"] = None
+        if "tool_calls" in message.additional_kwargs:
             message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
-            tool_call_supported_props = {"id", "type", "function"}
-            message_dict["tool_calls"] = [
-                {k: v for k, v in tool_call.items() if k in tool_call_supported_props}
-                for tool_call in message_dict["tool_calls"]
-            ]
-        else:
-            pass
-        # If tool calls present, content null value should be None not empty string.
-        if "function_call" in message_dict or "tool_calls" in message_dict:
-            message_dict["content"] = message_dict["content"] or None
+            # If tool calls only, content is None not empty string
+            if message_dict["content"] == "":
+                message_dict["content"] = None
     elif isinstance(message, SystemMessage):
         message_dict["role"] = "system"
     elif isinstance(message, FunctionMessage):
         message_dict["role"] = "function"
     elif isinstance(message, ToolMessage):
         message_dict["role"] = "tool"
         message_dict["tool_call_id"] = message.tool_call_id
@@ -818,18 +804,15 @@
             if isinstance(tool_choice, str):
                 if tool_choice not in ("auto", "none"):
                     tool_choice = {
                         "type": "function",
                         "function": {"name": tool_choice},
                     }
             elif isinstance(tool_choice, bool):
-                tool_choice = {
-                    "type": "function",
-                    "function": {"name": formatted_tools[0]["function"]["name"]},
-                }
+                tool_choice = formatted_tools[0]
             elif isinstance(tool_choice, dict):
                 if (
                     formatted_tools[0]["function"]["name"]
                     != tool_choice["function"]["name"]
                 ):
                     raise ValueError(
                         f"Tool choice {tool_choice} was specified, but the only "
@@ -1071,31 +1054,7 @@
             return RunnableMap(raw=llm) | parser_with_fallback
         else:
             return llm | output_parser
 
 
 def _is_pydantic_class(obj: Any) -> bool:
     return isinstance(obj, type) and issubclass(obj, BaseModel)
-
-
-def _lc_tool_call_to_openai_tool_call(tool_call: ToolCall) -> dict:
-    return {
-        "type": "function",
-        "id": tool_call["id"],
-        "function": {
-            "name": tool_call["name"],
-            "arguments": json.dumps(tool_call["args"]),
-        },
-    }
-
-
-def _lc_invalid_tool_call_to_openai_tool_call(
-    invalid_tool_call: InvalidToolCall,
-) -> dict:
-    return {
-        "type": "function",
-        "id": invalid_tool_call["id"],
-        "function": {
-            "name": invalid_tool_call["name"],
-            "arguments": invalid_tool_call["args"],
-        },
-    }
```

### Comparing `langchain_openai-0.1.3/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.3rc1/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/langchain_openai/llms/azure.py` & `langchain_openai-0.1.3rc1/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/langchain_openai/llms/base.py` & `langchain_openai-0.1.3rc1/langchain_openai/llms/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.3/pyproject.toml` & `langchain_openai-0.1.3rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.3"
+version = "0.1.3rc1"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.42"
+langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 openai = "^1.10.0"
 tiktoken = ">=0.5.2,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_openai-0.1.3/PKG-INFO` & `langchain_openai-0.1.3rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.3
+Version: 0.1.3rc1
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

