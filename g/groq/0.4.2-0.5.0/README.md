# Comparing `tmp/groq-0.4.2.tar.gz` & `tmp/groq-0.5.0.tar.gz`

## Comparing `groq-0.4.2.tar` & `groq-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/__init__.py
--rw-r--r--   0        0        0    61906 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_base_client.py
--rw-r--r--   0        0        0    14884 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_compat.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_constants.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_exceptions.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_files.py
--rw-r--r--   0        0        0    16432 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_qs.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_resource.py
--rw-r--r--   0        0        0    27743 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_response.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_streaming.py
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_types.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/py.typed
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_sync.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/lib/.keep
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/lib/chat_completion_chunk.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/resources/__init__.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/resources/models.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/resources/chat/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/resources/chat/chat.py
--rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/resources/chat/completions.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/types/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/types/model.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/types/model_list.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/types/chat/__init__.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/types/chat/chat_completion.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 groq-0.4.2/src/groq/types/chat/completion_create_params.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 groq-0.4.2/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 groq-0.4.2/LICENSE
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 groq-0.4.2/README.md
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 groq-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 groq-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/__init__.py
+-rw-r--r--   0        0        0    62500 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_base_client.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_compat.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_constants.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_files.py
+-rw-r--r--   0        0        0    16432 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_qs.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_resource.py
+-rw-r--r--   0        0        0    27935 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_response.py
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_types.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/py.typed
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_logs.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_sync.py
+-rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_typing.py
+-rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/lib/.keep
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/lib/chat_completion_chunk.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/__init__.py
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/models.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/__init__.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/audio.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/translations.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/chat/chat.py
+-rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/chat/completions.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/model.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/model_list.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/translation.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/transcription.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/chat/__init__.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 groq-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 groq-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 groq-0.5.0/README.md
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 groq-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 groq-0.5.0/PKG-INFO
```

### Comparing `groq-0.4.2/src/groq/__init__.py` & `groq-0.5.0/src/groq/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_base_client.py` & `groq-0.5.0/src/groq/_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,14 +775,19 @@
             # as this check is structural, meaning that we'll think they didn't
             # pass in a timeout and will ignore it
             if http_client and http_client.timeout != HTTPX_DEFAULT_TIMEOUT:
                 timeout = http_client.timeout
             else:
                 timeout = DEFAULT_TIMEOUT
 
+        if http_client is not None and not isinstance(http_client, httpx.Client):  # pyright: ignore[reportUnnecessaryIsInstance]
+            raise TypeError(
+                f"Invalid `http_client` argument; Expected an instance of `httpx.Client` but got {type(http_client)}"
+            )
+
         super().__init__(
             version=version,
             limits=limits,
             # cast to a valid type because mypy doesn't understand our type narrowing
             timeout=cast(Timeout, timeout),
             proxies=proxies,
             base_url=base_url,
@@ -1304,14 +1309,19 @@
             # as this check is structural, meaning that we'll think they didn't
             # pass in a timeout and will ignore it
             if http_client and http_client.timeout != HTTPX_DEFAULT_TIMEOUT:
                 timeout = http_client.timeout
             else:
                 timeout = DEFAULT_TIMEOUT
 
+        if http_client is not None and not isinstance(http_client, httpx.AsyncClient):  # pyright: ignore[reportUnnecessaryIsInstance]
+            raise TypeError(
+                f"Invalid `http_client` argument; Expected an instance of `httpx.AsyncClient` but got {type(http_client)}"
+            )
+
         super().__init__(
             version=version,
             base_url=base_url,
             limits=limits,
             # cast to a valid type because mypy doesn't understand our type narrowing
             timeout=cast(Timeout, timeout),
             proxies=proxies,
```

### Comparing `groq-0.4.2/src/groq/_client.py` & `groq-0.5.0/src/groq/_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "Client",
     "AsyncClient",
 ]
 
 
 class Groq(SyncAPIClient):
     chat: resources.Chat
+    audio: resources.Audio
     models: resources.Models
     with_raw_response: GroqWithRawResponse
     with_streaming_response: GroqWithStreamedResponse
 
     # client options
     api_key: str
 
@@ -100,14 +101,15 @@
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
         self.chat = resources.Chat(self)
+        self.audio = resources.Audio(self)
         self.models = resources.Models(self)
         self.with_raw_response = GroqWithRawResponse(self)
         self.with_streaming_response = GroqWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
@@ -211,14 +213,15 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncGroq(AsyncAPIClient):
     chat: resources.AsyncChat
+    audio: resources.AsyncAudio
     models: resources.AsyncModels
     with_raw_response: AsyncGroqWithRawResponse
     with_streaming_response: AsyncGroqWithStreamedResponse
 
     # client options
     api_key: str
 
@@ -268,14 +271,15 @@
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
         self.chat = resources.AsyncChat(self)
+        self.audio = resources.AsyncAudio(self)
         self.models = resources.AsyncModels(self)
         self.with_raw_response = AsyncGroqWithRawResponse(self)
         self.with_streaming_response = AsyncGroqWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
@@ -380,31 +384,35 @@
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class GroqWithRawResponse:
     def __init__(self, client: Groq) -> None:
         self.chat = resources.ChatWithRawResponse(client.chat)
+        self.audio = resources.AudioWithRawResponse(client.audio)
         self.models = resources.ModelsWithRawResponse(client.models)
 
 
 class AsyncGroqWithRawResponse:
     def __init__(self, client: AsyncGroq) -> None:
         self.chat = resources.AsyncChatWithRawResponse(client.chat)
+        self.audio = resources.AsyncAudioWithRawResponse(client.audio)
         self.models = resources.AsyncModelsWithRawResponse(client.models)
 
 
 class GroqWithStreamedResponse:
     def __init__(self, client: Groq) -> None:
         self.chat = resources.ChatWithStreamingResponse(client.chat)
+        self.audio = resources.AudioWithStreamingResponse(client.audio)
         self.models = resources.ModelsWithStreamingResponse(client.models)
 
 
 class AsyncGroqWithStreamedResponse:
     def __init__(self, client: AsyncGroq) -> None:
         self.chat = resources.AsyncChatWithStreamingResponse(client.chat)
+        self.audio = resources.AsyncAudioWithStreamingResponse(client.audio)
         self.models = resources.AsyncModelsWithStreamingResponse(client.models)
 
 
 Client = Groq
 
 AsyncClient = AsyncGroq
```

### Comparing `groq-0.4.2/src/groq/_compat.py` & `groq-0.5.0/src/groq/_compat.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_exceptions.py` & `groq-0.5.0/src/groq/_exceptions.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_files.py` & `groq-0.5.0/src/groq/_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 import anyio
 
 from ._types import (
     FileTypes,
     FileContent,
     RequestFiles,
     HttpxFileTypes,
+    Base64FileInput,
     HttpxFileContent,
     HttpxRequestFiles,
 )
 from ._utils import is_tuple_t, is_mapping_t, is_sequence_t
 
 
+def is_base64_file_input(obj: object) -> TypeGuard[Base64FileInput]:
+    return isinstance(obj, io.IOBase) or isinstance(obj, os.PathLike)
+
+
 def is_file_content(obj: object) -> TypeGuard[FileContent]:
     return (
         isinstance(obj, bytes) or isinstance(obj, tuple) or isinstance(obj, io.IOBase) or isinstance(obj, os.PathLike)
     )
 
 
 def assert_is_file_content(obj: object, *, key: str | None = None) -> None:
```

### Comparing `groq-0.4.2/src/groq/_models.py` & `groq-0.5.0/src/groq/_models.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_qs.py` & `groq-0.5.0/src/groq/_qs.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_resource.py` & `groq-0.5.0/src/groq/_resource.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_response.py` & `groq-0.5.0/src/groq/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,20 @@
         response = self.http_response
         if cast_to == str:
             return cast(R, response.text)
 
         if cast_to == bytes:
             return cast(R, response.content)
 
+        if cast_to == int:
+            return cast(R, int(response.text))
+
+        if cast_to == float:
+            return cast(R, float(response.text))
+
         origin = get_origin(cast_to) or cast_to
 
         if origin == APIResponse:
             raise RuntimeError("Unexpected state - cast_to is `APIResponse`")
 
         if inspect.isclass(origin) and issubclass(origin, httpx.Response):
             # Because of the invariance of our ResponseT TypeVar, users can subclass httpx.Response
@@ -269,14 +275,16 @@
 
         We support parsing:
           - `BaseModel`
           - `dict`
           - `list`
           - `Union`
           - `str`
+          - `int`
+          - `float`
           - `httpx.Response`
         """
         cache_key = to if to is not None else self._cast_to
         cached = self._parsed_by_type.get(cache_key)
         if cached is not None:
             return cached  # type: ignore[no-any-return]
```

### Comparing `groq-0.4.2/src/groq/_streaming.py` & `groq-0.5.0/src/groq/_streaming.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_types.py` & `groq-0.5.0/src/groq/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 
 
 # Approximates httpx internal ProxiesTypes and RequestFiles types
 # while adding support for `PathLike` instances
 ProxiesDict = Dict["str | URL", Union[None, str, URL, Proxy]]
 ProxiesTypes = Union[str, Proxy, ProxiesDict]
 if TYPE_CHECKING:
+    Base64FileInput = Union[IO[bytes], PathLike[str]]
     FileContent = Union[IO[bytes], bytes, PathLike[str]]
 else:
+    Base64FileInput = Union[IO[bytes], PathLike]
     FileContent = Union[IO[bytes], bytes, PathLike]  # PathLike is not subscriptable in Python 3.8.
 FileTypes = Union[
     # file (or bytes)
     FileContent,
     # (filename, file (or bytes))
     Tuple[Optional[str], FileContent],
     # (filename, file (or bytes), content_type)
```

### Comparing `groq-0.4.2/src/groq/_utils/__init__.py` & `groq-0.5.0/src/groq/_utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,9 +40,11 @@
     strip_annotated_type as strip_annotated_type,
     extract_type_var_from_base as extract_type_var_from_base,
 )
 from ._streams import consume_sync_iterator as consume_sync_iterator, consume_async_iterator as consume_async_iterator
 from ._transform import (
     PropertyInfo as PropertyInfo,
     transform as transform,
+    async_transform as async_transform,
     maybe_transform as maybe_transform,
+    async_maybe_transform as async_maybe_transform,
 )
```

### Comparing `groq-0.4.2/src/groq/_utils/_logs.py` & `groq-0.5.0/src/groq/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_utils/_proxy.py` & `groq-0.5.0/src/groq/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_utils/_sync.py` & `groq-0.5.0/src/groq/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_utils/_transform.py` & `groq-0.5.0/src/groq/_utils/_transform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
 
+import io
+import base64
+import pathlib
 from typing import Any, Mapping, TypeVar, cast
 from datetime import date, datetime
 from typing_extensions import Literal, get_args, override, get_type_hints
 
+import anyio
 import pydantic
 
 from ._utils import (
     is_list,
     is_mapping,
     is_iterable,
 )
+from .._files import is_base64_file_input
 from ._typing import (
     is_list_type,
     is_union_type,
     extract_type_arg,
     is_iterable_type,
     is_required_type,
     is_annotated_type,
@@ -25,15 +30,15 @@
 _T = TypeVar("_T")
 
 
 # TODO: support for drilling globals() and locals()
 # TODO: ensure works correctly with forward references in all cases
 
 
-PropertyFormat = Literal["iso8601", "custom"]
+PropertyFormat = Literal["iso8601", "base64", "custom"]
 
 
 class PropertyInfo:
     """Metadata class to be used in Annotated types to provide information about a given type.
 
     For example:
 
@@ -176,19 +181,15 @@
         for subtype in get_args(stripped_type):
             data = _transform_recursive(data, annotation=annotation, inner_type=subtype)
         return data
 
     if isinstance(data, pydantic.BaseModel):
         return model_dump(data, exclude_unset=True)
 
-    return _transform_value(data, annotation)
-
-
-def _transform_value(data: object, type_: type) -> object:
-    annotated_type = _get_annotated_type(type_)
+    annotated_type = _get_annotated_type(annotation)
     if annotated_type is None:
         return data
 
     # ignore the first argument as it is the actual type
     annotations = get_args(annotated_type)[1:]
     for annotation in annotations:
         if isinstance(annotation, PropertyInfo) and annotation.format is not None:
@@ -201,14 +202,30 @@
     if isinstance(data, (date, datetime)):
         if format_ == "iso8601":
             return data.isoformat()
 
         if format_ == "custom" and format_template is not None:
             return data.strftime(format_template)
 
+    if format_ == "base64" and is_base64_file_input(data):
+        binary: str | bytes | None = None
+
+        if isinstance(data, pathlib.Path):
+            binary = data.read_bytes()
+        elif isinstance(data, io.IOBase):
+            binary = data.read()
+
+            if isinstance(binary, str):  # type: ignore[unreachable]
+                binary = binary.encode()
+
+        if not isinstance(binary, bytes):
+            raise RuntimeError(f"Could not read bytes from {data}; Received {type(binary)}")
+
+        return base64.b64encode(binary).decode("ascii")
+
     return data
 
 
 def _transform_typeddict(
     data: Mapping[str, object],
     expected_type: type,
 ) -> Mapping[str, object]:
@@ -218,7 +235,145 @@
         type_ = annotations.get(key)
         if type_ is None:
             # we do not have a type annotation for this field, leave it as is
             result[key] = value
         else:
             result[_maybe_transform_key(key, type_)] = _transform_recursive(value, annotation=type_)
     return result
+
+
+async def async_maybe_transform(
+    data: object,
+    expected_type: object,
+) -> Any | None:
+    """Wrapper over `async_transform()` that allows `None` to be passed.
+
+    See `async_transform()` for more details.
+    """
+    if data is None:
+        return None
+    return await async_transform(data, expected_type)
+
+
+async def async_transform(
+    data: _T,
+    expected_type: object,
+) -> _T:
+    """Transform dictionaries based off of type information from the given type, for example:
+
+    ```py
+    class Params(TypedDict, total=False):
+        card_id: Required[Annotated[str, PropertyInfo(alias="cardID")]]
+
+
+    transformed = transform({"card_id": "<my card ID>"}, Params)
+    # {'cardID': '<my card ID>'}
+    ```
+
+    Any keys / data that does not have type information given will be included as is.
+
+    It should be noted that the transformations that this function does are not represented in the type system.
+    """
+    transformed = await _async_transform_recursive(data, annotation=cast(type, expected_type))
+    return cast(_T, transformed)
+
+
+async def _async_transform_recursive(
+    data: object,
+    *,
+    annotation: type,
+    inner_type: type | None = None,
+) -> object:
+    """Transform the given data against the expected type.
+
+    Args:
+        annotation: The direct type annotation given to the particular piece of data.
+            This may or may not be wrapped in metadata types, e.g. `Required[T]`, `Annotated[T, ...]` etc
+
+        inner_type: If applicable, this is the "inside" type. This is useful in certain cases where the outside type
+            is a container type such as `List[T]`. In that case `inner_type` should be set to `T` so that each entry in
+            the list can be transformed using the metadata from the container type.
+
+            Defaults to the same value as the `annotation` argument.
+    """
+    if inner_type is None:
+        inner_type = annotation
+
+    stripped_type = strip_annotated_type(inner_type)
+    if is_typeddict(stripped_type) and is_mapping(data):
+        return await _async_transform_typeddict(data, stripped_type)
+
+    if (
+        # List[T]
+        (is_list_type(stripped_type) and is_list(data))
+        # Iterable[T]
+        or (is_iterable_type(stripped_type) and is_iterable(data) and not isinstance(data, str))
+    ):
+        inner_type = extract_type_arg(stripped_type, 0)
+        return [await _async_transform_recursive(d, annotation=annotation, inner_type=inner_type) for d in data]
+
+    if is_union_type(stripped_type):
+        # For union types we run the transformation against all subtypes to ensure that everything is transformed.
+        #
+        # TODO: there may be edge cases where the same normalized field name will transform to two different names
+        # in different subtypes.
+        for subtype in get_args(stripped_type):
+            data = await _async_transform_recursive(data, annotation=annotation, inner_type=subtype)
+        return data
+
+    if isinstance(data, pydantic.BaseModel):
+        return model_dump(data, exclude_unset=True)
+
+    annotated_type = _get_annotated_type(annotation)
+    if annotated_type is None:
+        return data
+
+    # ignore the first argument as it is the actual type
+    annotations = get_args(annotated_type)[1:]
+    for annotation in annotations:
+        if isinstance(annotation, PropertyInfo) and annotation.format is not None:
+            return await _async_format_data(data, annotation.format, annotation.format_template)
+
+    return data
+
+
+async def _async_format_data(data: object, format_: PropertyFormat, format_template: str | None) -> object:
+    if isinstance(data, (date, datetime)):
+        if format_ == "iso8601":
+            return data.isoformat()
+
+        if format_ == "custom" and format_template is not None:
+            return data.strftime(format_template)
+
+    if format_ == "base64" and is_base64_file_input(data):
+        binary: str | bytes | None = None
+
+        if isinstance(data, pathlib.Path):
+            binary = await anyio.Path(data).read_bytes()
+        elif isinstance(data, io.IOBase):
+            binary = data.read()
+
+            if isinstance(binary, str):  # type: ignore[unreachable]
+                binary = binary.encode()
+
+        if not isinstance(binary, bytes):
+            raise RuntimeError(f"Could not read bytes from {data}; Received {type(binary)}")
+
+        return base64.b64encode(binary).decode("ascii")
+
+    return data
+
+
+async def _async_transform_typeddict(
+    data: Mapping[str, object],
+    expected_type: type,
+) -> Mapping[str, object]:
+    result: dict[str, object] = {}
+    annotations = get_type_hints(expected_type, include_extras=True)
+    for key, value in data.items():
+        type_ = annotations.get(key)
+        if type_ is None:
+            # we do not have a type annotation for this field, leave it as is
+            result[key] = value
+        else:
+            result[_maybe_transform_key(key, type_)] = await _async_transform_recursive(value, annotation=type_)
+    return result
```

### Comparing `groq-0.4.2/src/groq/_utils/_typing.py` & `groq-0.5.0/src/groq/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/_utils/_utils.py` & `groq-0.5.0/src/groq/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/lib/chat_completion_chunk.py` & `groq-0.5.0/src/groq/lib/chat_completion_chunk.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # File Manually added to support streaming
 # File is in libs instead of models to avoid conflicts with stainless bot
 
 from typing import List, Optional
-from ..types.chat.chat_completion import Usage
 
 from .._models import BaseModel
+from ..types.chat.chat_completion import Usage
 
 __all__ = [
     "ChatCompletionChunk",
     "Choice",
     "ChoiceLogprobs",
     "ChoiceLogprobsContent",
     "ChoiceLogprobsContentTopLogprob",
```

### Comparing `groq-0.4.2/src/groq/resources/__init__.py` & `groq-0.5.0/src/groq/resources/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,22 @@
     Chat,
     AsyncChat,
     ChatWithRawResponse,
     AsyncChatWithRawResponse,
     ChatWithStreamingResponse,
     AsyncChatWithStreamingResponse,
 )
+from .audio import (
+    Audio,
+    AsyncAudio,
+    AudioWithRawResponse,
+    AsyncAudioWithRawResponse,
+    AudioWithStreamingResponse,
+    AsyncAudioWithStreamingResponse,
+)
 from .models import (
     Models,
     AsyncModels,
     ModelsWithRawResponse,
     AsyncModelsWithRawResponse,
     ModelsWithStreamingResponse,
     AsyncModelsWithStreamingResponse,
@@ -20,14 +28,20 @@
 __all__ = [
     "Chat",
     "AsyncChat",
     "ChatWithRawResponse",
     "AsyncChatWithRawResponse",
     "ChatWithStreamingResponse",
     "AsyncChatWithStreamingResponse",
+    "Audio",
+    "AsyncAudio",
+    "AudioWithRawResponse",
+    "AsyncAudioWithRawResponse",
+    "AudioWithStreamingResponse",
+    "AsyncAudioWithStreamingResponse",
     "Models",
     "AsyncModels",
     "ModelsWithRawResponse",
     "AsyncModelsWithRawResponse",
     "ModelsWithStreamingResponse",
     "AsyncModelsWithStreamingResponse",
 ]
```

### Comparing `groq-0.4.2/src/groq/resources/models.py` & `groq-0.5.0/src/groq/resources/models.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/resources/chat/__init__.py` & `groq-0.5.0/src/groq/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/resources/chat/chat.py` & `groq-0.5.0/src/groq/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/resources/chat/completions.py` & `groq-0.5.0/src/groq/resources/chat/completions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 from typing import Dict, List, Union, Iterable, Optional, overload
 from typing_extensions import Literal
 
 import httpx
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import maybe_transform
+from ..._utils import (
+    maybe_transform,
+    async_maybe_transform,
+)
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
@@ -349,15 +352,15 @@
 
           extra_body: Add additional JSON properties to the request
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
             "/openai/v1/chat/completions",
-            body=maybe_transform(
+            body=await async_maybe_transform(
                 {
                     "messages": messages,
                     "model": model,
                     "frequency_penalty": frequency_penalty,
                     "logit_bias": logit_bias,
                     "logprobs": logprobs,
                     "max_tokens": max_tokens,
```

### Comparing `groq-0.4.2/src/groq/types/chat/chat_completion.py` & `groq-0.5.0/src/groq/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/src/groq/types/chat/completion_create_params.py` & `groq-0.5.0/src/groq/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/LICENSE` & `groq-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/README.md` & `groq-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `groq-0.4.2/pyproject.toml` & `groq-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "groq"
-version = "0.4.2"
+version = "0.5.0"
 description = "The official Python library for the groq API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Groq", email = "support@groq.com" },
 ]
 dependencies = [
```

### Comparing `groq-0.4.2/PKG-INFO` & `groq-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: groq
-Version: 0.4.2
+Version: 0.5.0
 Summary: The official Python library for the groq API
 Project-URL: Homepage, https://github.com/groq/groq-python
 Project-URL: Repository, https://github.com/groq/groq-python
 Author-email: Groq <support@groq.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

