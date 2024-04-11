# Comparing `tmp/langchain_cohere-0.1.1rc0.tar.gz` & `tmp/langchain_cohere-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.1rc0.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.2.tar", max compression
```

## Comparing `langchain_cohere-0.1.1rc0.tar` & `langchain_cohere-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/LICENSE
--rw-r--r--   0        0        0     3796 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/README.md
--rw-r--r--   0        0        0      608 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    13374 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     8089 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     1215 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/common.py
--rw-r--r--   0        0        0     5366 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     8050 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/py.typed
--rw-r--r--   0        0        0     3349 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0        0 2024-04-05 21:17:20.030871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/__init__.py
--rw-r--r--   0        0        0     4899 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/agent.py
--rw-r--r--   0        0        0     4059 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py
--rw-r--r--   0        0        0    10974 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/parsing.py
--rw-r--r--   0        0        0     9635 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/prompt.py
--rw-r--r--   0        0        0     3995 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/rerank.py
--rw-r--r--   0        0        0     1655 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2331 2024-04-05 21:17:20.034871 langchain_cohere-0.1.1rc0/pyproject.toml
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 langchain_cohere-0.1.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3796 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/README.md
+-rw-r--r--   0        0        0      608 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    15842 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8089 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1215 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5366 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8050 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:26:58.684860 langchain_cohere-0.1.2/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3349 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4899 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4059 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    10974 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9635 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     3995 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2328 2024-04-11 16:26:58.688860 langchain_cohere-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4623 1970-01-01 00:00:00.000000 langchain_cohere-0.1.2/PKG-INFO
```

### Comparing `langchain_cohere-0.1.1rc0/LICENSE` & `langchain_cohere-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/README.md` & `langchain_cohere-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/__init__.py` & `langchain_cohere-0.1.2/langchain_cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.2/langchain_cohere/chat_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     ChatMessage,
     HumanMessage,
     SystemMessage,
 )
+from langchain_core.messages import (
+    ToolCall as LC_ToolCall,
+)
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
     PydanticToolsParser,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel
@@ -246,18 +249,35 @@
                 delta = data.text
                 chunk = ChatGenerationChunk(message=AIMessageChunk(content=delta))
                 if run_manager:
                     run_manager.on_llm_new_token(delta, chunk=chunk)
                 yield chunk
             elif data.event_type == "stream-end":
                 generation_info = self._get_generation_info(data.response)
+                tool_call_chunks = []
+                if tool_calls := generation_info.get("tool_calls"):
+                    try:
+                        tool_call_chunks = [
+                            {
+                                "name": tool_call["function"].get("name"),
+                                "args": tool_call["function"].get("arguments"),
+                                "id": tool_call.get("id"),
+                                "index": tool_call.get("index"),
+                            }
+                            for tool_call in tool_calls
+                        ]
+                    except KeyError:
+                        pass
+                message = AIMessageChunk(
+                    content="",
+                    additional_kwargs=generation_info,
+                    tool_call_chunks=tool_call_chunks,
+                )
                 yield ChatGenerationChunk(
-                    message=AIMessageChunk(
-                        content="", additional_kwargs=generation_info
-                    ),
+                    message=message,
                     generation_info=generation_info,
                 )
 
     async def _astream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
@@ -278,18 +298,35 @@
                 delta = data.text
                 chunk = ChatGenerationChunk(message=AIMessageChunk(content=delta))
                 if run_manager:
                     await run_manager.on_llm_new_token(delta, chunk=chunk)
                 yield chunk
             elif data.event_type == "stream-end":
                 generation_info = self._get_generation_info(data.response)
+                tool_call_chunks = []
+                if tool_calls := generation_info.get("tool_calls"):
+                    try:
+                        tool_call_chunks = [
+                            {
+                                "name": tool_call["function"].get("name"),
+                                "args": tool_call["function"].get("arguments"),
+                                "id": tool_call.get("id"),
+                                "index": tool_call.get("index"),
+                            }
+                            for tool_call in tool_calls
+                        ]
+                    except KeyError:
+                        pass
+                message = AIMessageChunk(
+                    content="",
+                    additional_kwargs=generation_info,
+                    tool_call_chunks=tool_call_chunks,
+                )
                 yield ChatGenerationChunk(
-                    message=AIMessageChunk(
-                        content="", additional_kwargs=generation_info
-                    ),
+                    message=message,
                     generation_info=generation_info,
                 )
 
     def _get_generation_info(self, response: NonStreamedChatResponse) -> Dict[str, Any]:
         """Get the generation info from cohere API response."""
         generation_info = {
             "documents": response.documents,
@@ -324,15 +361,26 @@
 
         request = get_cohere_chat_request(
             messages, stop_sequences=stop, **self._default_params, **kwargs
         )
         response = self.client.chat(**request)
 
         generation_info = self._get_generation_info(response)
-        message = AIMessage(content=response.text, additional_kwargs=generation_info)
+        if "tool_calls" in generation_info:
+            tool_calls = [
+                _convert_cohere_tool_call_to_langchain(tool_call)
+                for tool_call in response.tool_calls
+            ]
+        else:
+            tool_calls = []
+        message = AIMessage(
+            content=response.text,
+            additional_kwargs=generation_info,
+            tool_calls=tool_calls,
+        )
         return ChatResult(
             generations=[
                 ChatGeneration(message=message, generation_info=generation_info)
             ]
         )
 
     async def _agenerate(
@@ -350,15 +398,26 @@
 
         request = get_cohere_chat_request(
             messages, stop_sequences=stop, **self._default_params, **kwargs
         )
         response = self.client.chat(**request)
 
         generation_info = self._get_generation_info(response)
-        message = AIMessage(content=response.text, additional_kwargs=generation_info)
+        if "tool_calls" in generation_info:
+            tool_calls = [
+                _convert_cohere_tool_call_to_langchain(tool_call)
+                for tool_call in response.tool_calls
+            ]
+        else:
+            tool_calls = []
+        message = AIMessage(
+            content=response.text,
+            additional_kwargs=generation_info,
+            tool_calls=tool_calls,
+        )
         return ChatResult(
             generations=[
                 ChatGeneration(message=message, generation_info=generation_info)
             ]
         )
 
     def get_num_tokens(self, text: str) -> int:
@@ -384,7 +443,12 @@
                     "name": tool_call.name,
                     "arguments": json.dumps(tool_call.parameters),
                 },
                 "type": "function",
             }
         )
     return formatted_tool_calls
+
+
+def _convert_cohere_tool_call_to_langchain(tool_call: ToolCall) -> LC_ToolCall:
+    """Convert a Cohere tool call into langchain_core.messages.ToolCall"""
+    return LC_ToolCall(name=tool_call.name, args=tool_call.parameters, id=None)
```

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.2/langchain_cohere/cohere_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/common.py` & `langchain_cohere-0.1.2/langchain_cohere/common.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.2/langchain_cohere/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/llms.py` & `langchain_cohere-0.1.2/langchain_cohere/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.2/langchain_cohere/rag_retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/agent.py` & `langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py` & `langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/default_prompt_constants.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/parsing.py` & `langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/parsing.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/react_multi_hop/prompt.py` & `langchain_cohere-0.1.2/langchain_cohere/react_multi_hop/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/rerank.py` & `langchain_cohere-0.1.2/langchain_cohere/rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/langchain_cohere/utils.py` & `langchain_cohere-0.1.2/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.1rc0/pyproject.toml` & `langchain_cohere-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.1rc0"
+version = "0.1.2"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-cohere/tree/main/libs/cohere"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.32"
+langchain-core = "^0.1.42"
 cohere = ">=5.1.8,<5.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_cohere-0.1.1rc0/PKG-INFO` & `langchain_cohere-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-cohere
-Version: 0.1.1rc0
+Version: 0.1.2
 Summary: An integration package connecting Cohere and LangChain
 Home-page: https://github.com/langchain-ai/langchain-cohere
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cohere (>=5.1.8,<5.2)
-Requires-Dist: langchain-core (>=0.1.32,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-cohere
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-cohere/tree/main/libs/cohere
 Description-Content-Type: text/markdown
 
 # Cohere
 
 >[Cohere](https://cohere.ai/about) is a Canadian startup that provides natural language processing models
```

