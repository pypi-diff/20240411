# Comparing `tmp/gigachain_openai-0.1.1.tar.gz` & `tmp/gigachain_openai-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_openai-0.1.1.tar", max compression
+gzip compressed data, was "gigachain_openai-0.1.3rc1.tar", max compression
```

## Comparing `gigachain_openai-0.1.1.tar` & `gigachain_openai-0.1.3rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-03-14 13:23:47.499850 gigachain_openai-0.1.1/LICENSE
--rw-r--r--   0        0        0     1627 2024-03-14 13:23:47.500394 gigachain_openai-0.1.1/README.md
--rw-r--r--   0        0        0      371 2024-03-14 13:23:47.500651 gigachain_openai-0.1.1/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-03-14 13:23:47.501088 gigachain_openai-0.1.1/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10508 2024-03-27 08:44:31.340657 gigachain_openai-0.1.1/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    42224 2024-03-27 08:44:31.341482 gigachain_openai-0.1.1/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-03-14 13:23:47.502629 gigachain_openai-0.1.1/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6689 2024-03-27 08:44:31.341955 gigachain_openai-0.1.1/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    23294 2024-03-27 08:44:31.342374 gigachain_openai-0.1.1/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-03-14 13:23:47.503827 gigachain_openai-0.1.1/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-03-27 08:44:31.342702 gigachain_openai-0.1.1/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24043 2024-03-27 08:44:31.343090 gigachain_openai-0.1.1/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-03-14 13:23:47.505070 gigachain_openai-0.1.1/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-03-14 13:23:47.505344 gigachain_openai-0.1.1/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:47.505460 gigachain_openai-0.1.1/langchain_openai/py.typed
--rw-r--r--   0        0        0     2792 2024-03-27 09:35:23.359621 gigachain_openai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 gigachain_openai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-18 15:16:41.009869 gigachain_openai-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     1627 2024-01-18 15:16:41.010661 gigachain_openai-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      371 2024-01-18 15:16:41.011302 gigachain_openai-0.1.3rc1/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-01-18 15:16:41.012203 gigachain_openai-0.1.3rc1/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10508 2024-03-28 12:44:20.752636 gigachain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    44617 2024-04-11 07:23:40.046099 gigachain_openai-0.1.3rc1/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-01-18 15:16:41.014232 gigachain_openai-0.1.3rc1/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-10 15:22:17.494741 gigachain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    23294 2024-03-28 12:44:20.755225 gigachain_openai-0.1.3rc1/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-01-18 15:16:41.016012 gigachain_openai-0.1.3rc1/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8008 2024-03-28 12:44:20.756153 gigachain_openai-0.1.3rc1/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24477 2024-04-10 15:22:17.495379 gigachain_openai-0.1.3rc1/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-03-28 12:44:20.757798 gigachain_openai-0.1.3rc1/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-28 12:44:20.758114 gigachain_openai-0.1.3rc1/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:16:41.017389 gigachain_openai-0.1.3rc1/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2915 2024-04-11 09:52:44.491735 gigachain_openai-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 gigachain_openai-0.1.3rc1/PKG-INFO
```

### Comparing `gigachain_openai-0.1.1/LICENSE` & `gigachain_openai-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.1/README.md` & `gigachain_openai-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.1/langchain_openai/chat_models/azure.py` & `gigachain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.1/langchain_openai/chat_models/base.py` & `gigachain_openai-0.1.3rc1/langchain_openai/chat_models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     JsonOutputParser,
     PydanticOutputParser,
 )
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
@@ -99,18 +101,32 @@
     elif role == "assistant":
         # Fix for azure
         # Also OpenAI returns None for tool invocations
         content = _dict.get("content", "") or ""
         additional_kwargs: Dict = {}
         if function_call := _dict.get("function_call"):
             additional_kwargs["function_call"] = dict(function_call)
-        if tool_calls := _dict.get("tool_calls"):
-            additional_kwargs["tool_calls"] = tool_calls
+        tool_calls = []
+        invalid_tool_calls = []
+        if raw_tool_calls := _dict.get("tool_calls"):
+            additional_kwargs["tool_calls"] = raw_tool_calls
+            for raw_tool_call in raw_tool_calls:
+                try:
+                    tool_calls.append(parse_tool_call(raw_tool_call, return_id=True))
+                except Exception as e:
+                    invalid_tool_calls.append(
+                        make_invalid_tool_call(raw_tool_call, str(e))
+                    )
         return AIMessage(
-            content=content, additional_kwargs=additional_kwargs, name=name, id=id_
+            content=content,
+            additional_kwargs=additional_kwargs,
+            name=name,
+            id=id_,
+            tool_calls=tool_calls,
+            invalid_tool_calls=invalid_tool_calls,
         )
     elif role == "system":
         return SystemMessage(content=_dict.get("content", ""), name=name, id=id_)
     elif role == "function":
         return FunctionMessage(
             content=_dict.get("content", ""), name=cast(str, _dict.get("name")), id=id_
         )
@@ -184,22 +200,38 @@
     content = cast(str, _dict.get("content") or "")
     additional_kwargs: Dict = {}
     if _dict.get("function_call"):
         function_call = dict(_dict["function_call"])
         if "name" in function_call and function_call["name"] is None:
             function_call["name"] = ""
         additional_kwargs["function_call"] = function_call
-    if _dict.get("tool_calls"):
-        additional_kwargs["tool_calls"] = _dict["tool_calls"]
+    tool_call_chunks = []
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
 
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content, id=id_)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(
-            content=content, additional_kwargs=additional_kwargs, id=id_
+            content=content,
+            additional_kwargs=additional_kwargs,
+            id=id_,
+            tool_call_chunks=tool_call_chunks,
         )
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content, id=id_)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"], id=id_)
     elif role == "tool" or default_class == ToolMessageChunk:
         return ToolMessageChunk(
@@ -236,15 +268,15 @@
     in, even if not explicitly saved on this class.
 
     Example:
         .. code-block:: python
 
             from langchain_openai import ChatOpenAI
 
-            model = ChatOpenAI(model_name="gpt-3.5-turbo")
+            model = ChatOpenAI(model="gpt-3.5-turbo")
     """
 
     @property
     def lc_secrets(self) -> Dict[str, str]:
         return {"openai_api_key": "OPENAI_API_KEY"}
 
     @classmethod
@@ -376,20 +408,39 @@
             "base_url": values["openai_api_base"],
             "timeout": values["request_timeout"],
             "max_retries": values["max_retries"],
             "default_headers": values["default_headers"],
             "default_query": values["default_query"],
         }
 
+        openai_proxy = values["openai_proxy"]
         if not values.get("client"):
+            if openai_proxy and not values["http_client"]:
+                try:
+                    import httpx
+                except ImportError as e:
+                    raise ImportError(
+                        "Could not import httpx python package. "
+                        "Please install it with `pip install httpx`."
+                    ) from e
+                values["http_client"] = httpx.Client(proxy=openai_proxy)
             sync_specific = {"http_client": values["http_client"]}
             values["client"] = openai.OpenAI(
                 **client_params, **sync_specific
             ).chat.completions
         if not values.get("async_client"):
+            if openai_proxy and not values["http_async_client"]:
+                try:
+                    import httpx
+                except ImportError as e:
+                    raise ImportError(
+                        "Could not import httpx python package. "
+                        "Please install it with `pip install httpx`."
+                    ) from e
+                values["http_async_client"] = httpx.AsyncClient(proxy=openai_proxy)
             async_specific = {"http_client": values["http_async_client"]}
             values["async_client"] = openai.AsyncOpenAI(
                 **client_params, **async_specific
             ).chat.completions
         return values
 
     @property
@@ -434,57 +485,56 @@
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs, "stream": True}
 
         default_chunk_class = AIMessageChunk
-        for chunk in self.client.create(messages=message_dicts, **params):
-            if not isinstance(chunk, dict):
-                chunk = chunk.model_dump()
-            if len(chunk["choices"]) == 0:
-                continue
-            choice = chunk["choices"][0]
-            chunk = _convert_delta_to_message_chunk(
-                choice["delta"], default_chunk_class
-            )
-            generation_info = {}
-            if finish_reason := choice.get("finish_reason"):
-                generation_info["finish_reason"] = finish_reason
-            logprobs = choice.get("logprobs")
-            if logprobs:
-                generation_info["logprobs"] = logprobs
-            default_chunk_class = chunk.__class__
-            chunk = ChatGenerationChunk(
-                message=chunk, generation_info=generation_info or None
-            )
-            if run_manager:
-                run_manager.on_llm_new_token(chunk.text, chunk=chunk, logprobs=logprobs)
-            yield chunk
+        with self.client.create(messages=message_dicts, **params) as response:
+            for chunk in response:
+                if not isinstance(chunk, dict):
+                    chunk = chunk.model_dump()
+                if len(chunk["choices"]) == 0:
+                    continue
+                choice = chunk["choices"][0]
+                if choice["delta"] is None:
+                    continue
+                chunk = _convert_delta_to_message_chunk(
+                    choice["delta"], default_chunk_class
+                )
+                generation_info = {}
+                if finish_reason := choice.get("finish_reason"):
+                    generation_info["finish_reason"] = finish_reason
+                logprobs = choice.get("logprobs")
+                if logprobs:
+                    generation_info["logprobs"] = logprobs
+                default_chunk_class = chunk.__class__
+                chunk = ChatGenerationChunk(
+                    message=chunk, generation_info=generation_info or None
+                )
+                if run_manager:
+                    run_manager.on_llm_new_token(
+                        chunk.text, chunk=chunk, logprobs=logprobs
+                    )
+                yield chunk
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
-        stream: Optional[bool] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        should_stream = stream if stream is not None else self.streaming
-        if should_stream:
+        if self.streaming:
             stream_iter = self._stream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return generate_from_stream(stream_iter)
         message_dicts, params = self._create_message_dicts(messages, stop)
-        params = {
-            **params,
-            **({"stream": stream} if stream is not None else {}),
-            **kwargs,
-        }
+        params = {**params, **kwargs}
         response = self.client.create(messages=message_dicts, **params)
         return self._create_chat_result(response)
 
     def _create_message_dicts(
         self, messages: List[BaseMessage], stop: Optional[List[str]]
     ) -> Tuple[List[Dict[str, Any]], Dict[str, Any]]:
         params = self._default_params
@@ -497,14 +547,22 @@
 
     def _create_chat_result(
         self, response: Union[dict, openai.BaseModel]
     ) -> ChatResult:
         generations = []
         if not isinstance(response, dict):
             response = response.model_dump()
+
+        # Sometimes the AI Model calling will get error, we should raise it.
+        # Otherwise, the next code 'choices.extend(response["choices"])'
+        # will throw a "TypeError: 'NoneType' object is not iterable" error
+        # to mask the true error. Because 'response["choices"]' is None.
+        if response.get("error"):
+            raise ValueError(response.get("error"))
+
         for res in response["choices"]:
             message = _convert_dict_to_message(res["message"])
             generation_info = dict(finish_reason=res.get("finish_reason"))
             if "logprobs" in res:
                 generation_info["logprobs"] = res["logprobs"]
             gen = ChatGeneration(
                 message=message,
@@ -526,62 +584,58 @@
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs, "stream": True}
 
         default_chunk_class = AIMessageChunk
-        async for chunk in await self.async_client.create(
-            messages=message_dicts, **params
-        ):
-            if not isinstance(chunk, dict):
-                chunk = chunk.model_dump()
-            if len(chunk["choices"]) == 0:
-                continue
-            choice = chunk["choices"][0]
-            chunk = _convert_delta_to_message_chunk(
-                choice["delta"], default_chunk_class
-            )
-            generation_info = {}
-            if finish_reason := choice.get("finish_reason"):
-                generation_info["finish_reason"] = finish_reason
-            logprobs = choice.get("logprobs")
-            if logprobs:
-                generation_info["logprobs"] = logprobs
-            default_chunk_class = chunk.__class__
-            chunk = ChatGenerationChunk(
-                message=chunk, generation_info=generation_info or None
-            )
-            if run_manager:
-                await run_manager.on_llm_new_token(
-                    token=chunk.text, chunk=chunk, logprobs=logprobs
+        response = await self.async_client.create(messages=message_dicts, **params)
+        async with response:
+            async for chunk in response:
+                if not isinstance(chunk, dict):
+                    chunk = chunk.model_dump()
+                if len(chunk["choices"]) == 0:
+                    continue
+                choice = chunk["choices"][0]
+                if choice["delta"] is None:
+                    continue
+                chunk = _convert_delta_to_message_chunk(
+                    choice["delta"], default_chunk_class
+                )
+                generation_info = {}
+                if finish_reason := choice.get("finish_reason"):
+                    generation_info["finish_reason"] = finish_reason
+                logprobs = choice.get("logprobs")
+                if logprobs:
+                    generation_info["logprobs"] = logprobs
+                default_chunk_class = chunk.__class__
+                chunk = ChatGenerationChunk(
+                    message=chunk, generation_info=generation_info or None
                 )
-            yield chunk
+                if run_manager:
+                    await run_manager.on_llm_new_token(
+                        token=chunk.text, chunk=chunk, logprobs=logprobs
+                    )
+                yield chunk
 
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
-        stream: Optional[bool] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        should_stream = stream if stream is not None else self.streaming
-        if should_stream:
+        if self.streaming:
             stream_iter = self._astream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return await agenerate_from_stream(stream_iter)
 
         message_dicts, params = self._create_message_dicts(messages, stop)
-        params = {
-            **params,
-            **({"stream": stream} if stream is not None else {}),
-            **kwargs,
-        }
+        params = {**params, **kwargs}
         response = await self.async_client.create(messages=message_dicts, **params)
         return self._create_chat_result(response)
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return {"model_name": self.model_name, **self._default_params}
```

### Comparing `gigachain_openai-0.1.1/langchain_openai/embeddings/azure.py` & `gigachain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Azure OpenAI embeddings wrapper."""
+
 from __future__ import annotations
 
 import os
 from typing import Callable, Dict, Optional, Union
 
 import openai
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
@@ -53,14 +54,16 @@
     """A function that returns an Azure Active Directory token.
 
         Will be invoked on every request.
     """
     openai_api_version: Optional[str] = Field(default=None, alias="api_version")
     """Automatically inferred from env var `OPENAI_API_VERSION` if not provided."""
     validate_base_url: bool = True
+    chunk_size: int = 2048
+    """Maximum number of texts to embed in each batch"""
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         # Check OPENAI_KEY for backwards compatibility.
         # TODO: Remove OPENAI_API_KEY support to avoid possible conflict when using
         # other forms of azure credentials.
@@ -95,18 +98,14 @@
         values["azure_endpoint"] = values["azure_endpoint"] or os.getenv(
             "AZURE_OPENAI_ENDPOINT"
         )
         azure_ad_token = values["azure_ad_token"] or os.getenv("AZURE_OPENAI_AD_TOKEN")
         values["azure_ad_token"] = (
             convert_to_secret_str(azure_ad_token) if azure_ad_token else None
         )
-        # Azure OpenAI embedding models allow a maximum of 2048 texts
-        # at a time in each batch
-        # See: https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/embeddings?tabs=console#best-practices
-        values["chunk_size"] = min(values["chunk_size"], 2048)
         # For backwards compatibility. Before openai v1, no distinction was made
         # between azure_endpoint and base_url (openai_api_base).
         openai_api_base = values["openai_api_base"]
         if openai_api_base and values["validate_base_url"]:
             if "/openai" not in openai_api_base:
                 values["openai_api_base"] += "/openai"
                 raise ValueError(
@@ -122,20 +121,24 @@
                     "Instead use `deployment` (or alias `azure_deployment`) "
                     "and `azure_endpoint`."
                 )
         client_params = {
             "api_version": values["openai_api_version"],
             "azure_endpoint": values["azure_endpoint"],
             "azure_deployment": values["deployment"],
-            "api_key": values["openai_api_key"].get_secret_value()
-            if values["openai_api_key"]
-            else None,
-            "azure_ad_token": values["azure_ad_token"].get_secret_value()
-            if values["azure_ad_token"]
-            else None,
+            "api_key": (
+                values["openai_api_key"].get_secret_value()
+                if values["openai_api_key"]
+                else None
+            ),
+            "azure_ad_token": (
+                values["azure_ad_token"].get_secret_value()
+                if values["azure_ad_token"]
+                else None
+            ),
             "azure_ad_token_provider": values["azure_ad_token_provider"],
             "organization": values["openai_organization"],
             "base_url": values["openai_api_base"],
             "timeout": values["request_timeout"],
             "max_retries": values["max_retries"],
             "default_headers": values["default_headers"],
             "default_query": values["default_query"],
```

### Comparing `gigachain_openai-0.1.1/langchain_openai/embeddings/base.py` & `gigachain_openai-0.1.3rc1/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.1/langchain_openai/llms/azure.py` & `gigachain_openai-0.1.3rc1/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.1/langchain_openai/llms/base.py` & `gigachain_openai-0.1.3rc1/langchain_openai/llms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,21 @@
             else:
                 response = self.client.create(prompt=_prompts, **params)
                 if not isinstance(response, dict):
                     # V1 client returns the response in an PyDantic object instead of
                     # dict. For the transition period, we deep convert it to dict.
                     response = response.model_dump()
 
+                # Sometimes the AI Model calling will get error, we should raise it.
+                # Otherwise, the next code 'choices.extend(response["choices"])'
+                # will throw a "TypeError: 'NoneType' object is not iterable" error
+                # to mask the true error. Because 'response["choices"]' is None.
+                if response.get("error"):
+                    raise ValueError(response.get("error"))
+
                 choices.extend(response["choices"])
                 _update_token_usage(_keys, response, token_usage)
                 if not system_fingerprint:
                     system_fingerprint = response.get("system_fingerprint")
         return self.create_llm_result(
             choices,
             prompts,
```

### Comparing `gigachain_openai-0.1.1/pyproject.toml` & `gigachain_openai-0.1.3rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "gigachain-openai"
-version = "0.1.1"
+version = "0.1.3rc1"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 packages = [
     {include = "langchain_openai"}
 ]
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = "^0.1.33"
+gigachain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 openai = "^1.10.0"
 tiktoken = ">=0.5.2,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -27,14 +27,15 @@
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 gigachain-core = { path = "../../core", develop = true }
 pytest-cov = "^4.1.0"
+gigachain-standard-tests = { path = "../../standard-tests", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `gigachain_openai-0.1.1/PKG-INFO` & `gigachain_openai-0.1.3rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gigachain-openai
-Version: 0.1.1
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
-Requires-Dist: gigachain-core (>=0.1.33,<0.2.0)
+Requires-Dist: gigachain-core (>=0.1.42rc1,<0.2.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

