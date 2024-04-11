# Comparing `tmp/langchain_mistralai-0.1.2.tar.gz` & `tmp/langchain_mistralai-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.2.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.2rc1.tar", max compression
```

## Comparing `langchain_mistralai-0.1.2.tar` & `langchain_mistralai-0.1.2rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/LICENSE
--rw-r--r--   0        0        0     1336 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/README.md
--rw-r--r--   0        0        0      173 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    26751 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     5961 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2391 2024-04-11 16:21:10.043685 langchain_mistralai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/LICENSE
+-rw-r--r--   0        0        0     1336 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/README.md
+-rw-r--r--   0        0        0      173 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    26092 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     5961 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2437 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2247 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.2rc1/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.2/LICENSE` & `langchain_mistralai-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.2/README.md` & `langchain_mistralai-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.2/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.2rc1/langchain_mistralai/chat_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import logging
-import uuid
 from operator import itemgetter
 from typing import (
     Any,
     AsyncContextManager,
     AsyncIterator,
     Callable,
     Dict,
@@ -88,26 +87,22 @@
     tool_calls = []
     invalid_tool_calls = []
     if raw_tool_calls := _message.get("tool_calls"):
         additional_kwargs["tool_calls"] = raw_tool_calls
         for raw_tool_call in raw_tool_calls:
             try:
                 parsed: dict = cast(
-                    dict, parse_tool_call(raw_tool_call, return_id=True)
+                    dict, parse_tool_call(raw_tool_call, return_id=False)
+                )
+                tool_calls.append(
+                    {
+                        **parsed,
+                        **{"id": None},
+                    },
                 )
-                if not parsed["id"]:
-                    tool_call_id = uuid.uuid4().hex[:]
-                    tool_calls.append(
-                        {
-                            **parsed,
-                            **{"id": tool_call_id},
-                        },
-                    )
-                else:
-                    tool_calls.append(parsed)
             except Exception as e:
                 invalid_tool_calls.append(
                     dict(make_invalid_tool_call(raw_tool_call, str(e)))
                 )
     return AIMessage(
         content=content,
         additional_kwargs=additional_kwargs,
@@ -161,28 +156,23 @@
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         additional_kwargs: Dict = {}
         if raw_tool_calls := _delta.get("tool_calls"):
             additional_kwargs["tool_calls"] = raw_tool_calls
             try:
-                tool_call_chunks = []
-                for raw_tool_call in raw_tool_calls:
-                    if not raw_tool_call.get("index") and not raw_tool_call.get("id"):
-                        tool_call_id = uuid.uuid4().hex[:]
-                    else:
-                        tool_call_id = raw_tool_call.get("id")
-                    tool_call_chunks.append(
-                        {
-                            "name": raw_tool_call["function"].get("name"),
-                            "args": raw_tool_call["function"].get("arguments"),
-                            "id": tool_call_id,
-                            "index": raw_tool_call.get("index"),
-                        }
-                    )
+                tool_call_chunks = [
+                    {
+                        "name": rtc["function"].get("name"),
+                        "args": rtc["function"].get("arguments"),
+                        "id": rtc.get("id"),
+                        "index": rtc.get("index"),
+                    }
+                    for rtc in raw_tool_calls
+                ]
             except KeyError:
                 pass
         else:
             tool_call_chunks = []
         return AIMessageChunk(
             content=content,
             additional_kwargs=additional_kwargs,
@@ -201,25 +191,23 @@
 ) -> Dict:
     if isinstance(message, ChatMessage):
         return dict(role=message.role, content=message.content)
     elif isinstance(message, HumanMessage):
         return dict(role="user", content=message.content)
     elif isinstance(message, AIMessage):
         if "tool_calls" in message.additional_kwargs:
-            tool_calls = []
-            for tc in message.additional_kwargs["tool_calls"]:
-                chunk = {
+            tool_calls = [
+                {
                     "function": {
                         "name": tc["function"]["name"],
                         "arguments": tc["function"]["arguments"],
                     }
                 }
-                if _id := tc.get("id"):
-                    chunk["id"] = _id
-                tool_calls.append(chunk)
+                for tc in message.additional_kwargs["tool_calls"]
+            ]
         else:
             tool_calls = []
         return {
             "role": "assistant",
             "content": message.content,
             "tool_calls": tool_calls,
         }
```

### Comparing `langchain_mistralai-0.1.2/langchain_mistralai/embeddings.py` & `langchain_mistralai-0.1.2rc1/langchain_mistralai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.2/pyproject.toml` & `langchain_mistralai-0.1.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.2"
+version = "0.1.2rc1"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.42"
+langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 tokenizers = "^0.15.1"
 httpx = ">=0.25.2,<1"
 httpx-sse = ">=0.3.1,<1"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_mistralai-0.1.2/PKG-INFO` & `langchain_mistralai-0.1.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.2
+Version: 0.1.2rc1
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: httpx-sse (>=0.3.1,<1)
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
 Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai
 Description-Content-Type: text/markdown
 
 # langchain-mistralai
```

