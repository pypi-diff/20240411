# Comparing `tmp/langchain_fireworks-0.1.1.tar.gz` & `tmp/langchain_fireworks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_fireworks-0.1.1.tar", max compression
+gzip compressed data, was "langchain_fireworks-0.1.2.tar", max compression
```

## Comparing `langchain_fireworks-0.1.1.tar` & `langchain_fireworks-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-03-01 17:21:25.472242 langchain_fireworks-0.1.1/LICENSE
--rw-r--r--   0        0        0     2929 2024-03-01 17:21:25.472242 langchain_fireworks-0.1.1/README.md
--rw-r--r--   0        0        0      319 2024-03-01 17:21:25.472242 langchain_fireworks-0.1.1/langchain_fireworks/__init__.py
--rw-r--r--   0        0        0    36132 2024-03-01 17:21:25.472242 langchain_fireworks-0.1.1/langchain_fireworks/chat_models.py
--rw-r--r--   0        0        0    64929 2024-03-01 17:21:25.476242 langchain_fireworks-0.1.1/langchain_fireworks/docs/embeddings.ipynb
--rw-r--r--   0        0        0     1788 2024-03-01 17:21:25.476242 langchain_fireworks-0.1.1/langchain_fireworks/embeddings.py
--rw-r--r--   0        0        0     7962 2024-03-01 17:21:25.476242 langchain_fireworks-0.1.1/langchain_fireworks/llms.py
--rw-r--r--   0        0        0        0 2024-03-01 17:21:25.476242 langchain_fireworks-0.1.1/langchain_fireworks/py.typed
--rw-r--r--   0        0        0      232 2024-03-01 17:21:25.476242 langchain_fireworks-0.1.1/langchain_fireworks/version.py
--rw-r--r--   0        0        0     2593 2024-03-01 17:21:25.476242 langchain_fireworks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 langchain_fireworks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2929 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/README.md
+-rw-r--r--   0        0        0      319 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/__init__.py
+-rw-r--r--   0        0        0    37383 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/chat_models.py
+-rw-r--r--   0        0        0     1788 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/embeddings.py
+-rw-r--r--   0        0        0     7962 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/llms.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/py.typed
+-rw-r--r--   0        0        0      232 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/version.py
+-rw-r--r--   0        0        0     2593 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 langchain_fireworks-0.1.2/PKG-INFO
```

### Comparing `langchain_fireworks-0.1.1/LICENSE` & `langchain_fireworks-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.1/README.md` & `langchain_fireworks-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.1/langchain_fireworks/chat_models.py` & `langchain_fireworks-0.1.2/langchain_fireworks/chat_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     ToolMessageChunk,
 )
 from langchain_core.output_parsers import JsonOutputParser, PydanticOutputParser
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
     PydanticToolsParser,
+    make_invalid_tool_call,
+    parse_tool_call,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
 from langchain_core.runnables import Runnable, RunnableMap, RunnablePassthrough
 from langchain_core.tools import BaseTool
 from langchain_core.utils import (
     convert_to_secret_str,
@@ -90,17 +92,31 @@
     elif role == "assistant":
         # Fix for azure
         # Also Fireworks returns None for tool invocations
         content = _dict.get("content", "") or ""
         additional_kwargs: Dict = {}
         if function_call := _dict.get("function_call"):
             additional_kwargs["function_call"] = dict(function_call)
-        if tool_calls := _dict.get("tool_calls"):
-            additional_kwargs["tool_calls"] = tool_calls
-        return AIMessage(content=content, additional_kwargs=additional_kwargs)
+        tool_calls = []
+        invalid_tool_calls = []
+        if raw_tool_calls := _dict.get("tool_calls"):
+            additional_kwargs["tool_calls"] = raw_tool_calls
+            for raw_tool_call in raw_tool_calls:
+                try:
+                    tool_calls.append(parse_tool_call(raw_tool_call, return_id=True))
+                except Exception as e:
+                    invalid_tool_calls.append(
+                        dict(make_invalid_tool_call(raw_tool_call, str(e)))
+                    )
+        return AIMessage(
+            content=content,
+            additional_kwargs=additional_kwargs,
+            tool_calls=tool_calls,
+            invalid_tool_calls=invalid_tool_calls,
+        )
     elif role == "system":
         return SystemMessage(content=_dict.get("content", ""))
     elif role == "function":
         return FunctionMessage(
             content=_dict.get("content", ""), name=_dict.get("name", "")
         )
     elif role == "tool":
@@ -170,21 +186,39 @@
     content = cast(str, _dict.get("content") or "")
     additional_kwargs: Dict = {}
     if _dict.get("function_call"):
         function_call = dict(_dict["function_call"])
         if "name" in function_call and function_call["name"] is None:
             function_call["name"] = ""
         additional_kwargs["function_call"] = function_call
-    if _dict.get("tool_calls"):
-        additional_kwargs["tool_calls"] = _dict["tool_calls"]
+    if raw_tool_calls := _dict.get("tool_calls"):
+        additional_kwargs["tool_calls"] = raw_tool_calls
+        try:
+            tool_call_chunks = [
+                {
+                    "name": rtc["function"].get("name"),
+                    "args": rtc["function"].get("arguments"),
+                    "id": rtc.get("id"),
+                    "index": rtc["index"],
+                }
+                for rtc in raw_tool_calls
+            ]
+        except KeyError:
+            pass
+    else:
+        tool_call_chunks = []
 
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
-        return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
+        return AIMessageChunk(
+            content=content,
+            additional_kwargs=additional_kwargs,
+            tool_call_chunks=tool_call_chunks,
+        )
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"])
     elif role == "tool" or default_class == ToolMessageChunk:
         return ToolMessageChunk(content=content, tool_call_id=_dict["tool_call_id"])
     elif role or default_class == ChatMessageChunk:
@@ -575,38 +609,43 @@
             **kwargs,
         )
 
     def bind_tools(
         self,
         tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
         *,
-        tool_choice: Optional[Union[dict, str, Literal["auto", "none"], bool]] = None,
+        tool_choice: Optional[
+            Union[dict, str, Literal["auto", "any", "none"], bool]
+        ] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
         Assumes model is compatible with Fireworks tool-calling API.
 
         Args:
             tools: A list of tool definitions to bind to this chat model.
                 Can be  a dictionary, pydantic model, callable, or BaseTool. Pydantic
                 models, callables, and BaseTools will be automatically converted to
                 their schema dictionary representation.
             tool_choice: Which tool to require the model to call.
-                Must be the name of the single provided function or
+                Must be the name of the single provided function,
                 "auto" to automatically determine which function to call
-                (if any), or a dict of the form:
+                with the option to not call any function, "any" to enforce that some
+                function is called, or a dict of the form:
                 {"type": "function", "function": {"name": <<tool_name>>}}.
             **kwargs: Any additional parameters to pass to the
                 :class:`~langchain.runnable.Runnable` constructor.
         """
 
         formatted_tools = [convert_to_openai_tool(tool) for tool in tools]
         if tool_choice is not None and tool_choice:
-            if isinstance(tool_choice, str) and (tool_choice not in ("auto", "none")):
+            if isinstance(tool_choice, str) and (
+                tool_choice not in ("auto", "any", "none")
+            ):
                 tool_choice = {"type": "function", "function": {"name": tool_choice}}
             if isinstance(tool_choice, dict) and (len(formatted_tools) != 1):
                 raise ValueError(
                     "When specifying `tool_choice`, you must provide exactly one "
                     f"tool. Received {len(formatted_tools)} tools."
                 )
             if isinstance(tool_choice, dict) and (
```

### Comparing `langchain_fireworks-0.1.1/langchain_fireworks/embeddings.py` & `langchain_fireworks-0.1.2/langchain_fireworks/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.1/langchain_fireworks/llms.py` & `langchain_fireworks-0.1.2/langchain_fireworks/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.1/pyproject.toml` & `langchain_fireworks-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-fireworks"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting Fireworks and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/fireworks"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.27"
+langchain-core = "^0.1.42"
 fireworks-ai = ">=0.13.0"
 openai = "^1.10.0"
 requests = "^2"
 aiohttp = "^3.9.1"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_fireworks-0.1.1/PKG-INFO` & `langchain_fireworks-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-fireworks
-Version: 0.1.1
+Version: 0.1.2
 Summary: An integration package connecting Fireworks and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: fireworks-ai (>=0.13.0)
-Requires-Dist: langchain-core (>=0.1.27,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2,<3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/fireworks
 Description-Content-Type: text/markdown
 
 # LangChain-Fireworks
```

