# Comparing `tmp/quickapiclient-0.0.8.tar.gz` & `tmp/quickapiclient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickapiclient-0.0.8.tar", max compression
+gzip compressed data, was "quickapiclient-0.0.9.tar", max compression
```

## Comparing `quickapiclient-0.0.8.tar` & `quickapiclient-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      580 2024-03-19 06:41:37.434686 quickapiclient-0.0.8/LICENSE
--rw-r--r--   0        0        0     7484 2024-03-19 06:41:37.434686 quickapiclient-0.0.8/README.md
--rw-r--r--   0        0        0     2205 2024-03-19 06:41:54.886863 quickapiclient-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      448 2024-03-19 06:41:37.434686 quickapiclient-0.0.8/quickapi/__init__.py
--rw-r--r--   0        0        0     7497 2024-03-19 06:41:37.434686 quickapiclient-0.0.8/quickapi/client.py
--rw-r--r--   0        0        0     1383 2024-03-19 06:41:37.434686 quickapiclient-0.0.8/quickapi/exceptions.py
--rw-r--r--   0        0        0     3684 2024-03-19 06:41:37.434686 quickapiclient-0.0.8/quickapi/http_client.py
--rw-r--r--   0        0        0     8367 1970-01-01 00:00:00.000000 quickapiclient-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      580 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9291 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/README.md
+-rw-r--r--   0        0        0     2529 2024-03-27 05:50:44.422422 quickapiclient-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      499 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/quickapi/__init__.py
+-rw-r--r--   0        0        0     7141 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/quickapi/client.py
+-rw-r--r--   0        0        0     2182 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/quickapi/exceptions.py
+-rw-r--r--   0        0        0     3915 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/quickapi/http_client.py
+-rw-r--r--   0        0        0     5142 2024-03-27 05:50:25.282314 quickapiclient-0.0.9/quickapi/serializers.py
+-rw-r--r--   0        0        0    10322 1970-01-01 00:00:00.000000 quickapiclient-0.0.9/PKG-INFO
```

### Comparing `quickapiclient-0.0.8/LICENSE` & `quickapiclient-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quickapiclient-0.0.8/pyproject.toml` & `quickapiclient-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 [tool.poetry]
 name = "quickapiclient"
-version = "v0.0.8"
+version = "v0.0.9"
 description = "A library for creating fully typed declarative API clients quickly and easily."
 authors = ["Martin N. <martinn@users.noreply.github.com>"]
 repository = "https://github.com/martinn/quickapiclient"
 documentation = "https://martinn.github.io/quickapiclient/"
 readme = "README.md"
 packages = [{ include = "quickapi" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 httpx = "^0.27.0"
 requests = { version = "^2.31.0", optional = true }
 attrs = "^23.2.0"
 cattrs = "^23.2.3"
+pydantic = { version = "^2.6.4", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-httpx = "^0.30.0"
 deptry = "^0.12.0"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
 tox = "^4.11.1"
 httpx-auth = "^0.22.0"
 responses = "^0.25.0"
 types-requests = "^2.31.0.20240311"
+pydantic = "^2.6.4"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.2.7"
 mkdocstrings = { extras = ["python"], version = "^0.24.1" }
 markdown-checklist = "^0.4.4"
 
 [tool.poetry.extras]
 requests = ["requests"]
+attrs = ["attrs", "cattrs"]
+pydantic = ["pydantic"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 files = ["quickapi"]
@@ -99,15 +103,25 @@
 ]
 
 [tool.ruff.format]
 preview = true
 
 [tool.coverage.report]
 skip_empty = true
+exclude_also = [
+    "if TYPE_CHECKING:",
+    "raise AssertionError",
+    "raise NotImplementedError",
+    "@(abc\\.)?abstractmethod",
+    "case _:",
+]
 
 [tool.coverage.run]
 branch = true
 source = ["quickapi"]
 
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
+
+[tool.deptry]
+known_first_party = ["_typeshed"]
```

### Comparing `quickapiclient-0.0.8/quickapi/client.py` & `quickapiclient-0.0.9/quickapi/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,38 @@
-from contextlib import suppress
+from dataclasses import dataclass
 from enum import Enum
-from typing import TYPE_CHECKING, Generic, TypeVar, get_args
+from typing import Generic, TypeVar, get_args
 
-import attrs
-import cattrs
-import httpx
-
-from .exceptions import ClientSetupError, HTTPError, ResponseSerializationError
-from .http_client import BaseAuth, BaseHttpClient, HTTPxClient
-
-if TYPE_CHECKING:
-    with suppress(ImportError):
-        pass
+from .exceptions import (
+    ClientSetupError,
+    DictDeserializationError,
+    DictSerializationError,
+    HTTPError,
+    RequestSerializationError,
+    ResponseSerializationError,
+)
+from .http_client import (
+    BaseHttpClient,
+    BaseHttpClientAuth,
+    BaseHttpClientResponse,
+    HTTPxClient,
+)
+from .serializers import (
+    DictSerializable,
+    DictSerializableT,
+)
 
 USE_DEFAULT = object()
 
+ResponseBodyT = TypeVar("ResponseBodyT")
 
-@attrs.define
-class BaseRequestParams:
-    def to_dict(self: "BaseRequestParams") -> dict:
-        return attrs.asdict(self)
 
-
-@attrs.define
-class BaseRequestBody:
-    def to_dict(self: "BaseRequestBody") -> dict:
-        return attrs.asdict(self)
-
-
-ResponseBodyT = TypeVar("ResponseBodyT", bound="BaseResponseBody")
-
-
-# TODO: Needs to support differebt response body types (json, text, xml, etc)
-class BaseResponseBody(Generic[ResponseBodyT]):
-    @classmethod
-    def from_dict(cls: type[ResponseBodyT], value: dict) -> ResponseBodyT:
-        try:
-            return cattrs.structure(value, cls)
-        except cattrs.ClassValidationError as e:
-            raise ResponseSerializationError(expected_type=cls.__name__) from e
-
-
-@attrs.define
+@dataclass
 class BaseResponse(Generic[ResponseBodyT]):
-    client_response: httpx.Response
+    client_response: BaseHttpClientResponse
     body: ResponseBodyT
 
 
 class BaseApiMethod(str, Enum):
     """Supported HTTP methods."""
 
     GET = "GET"
@@ -65,23 +50,23 @@
 
 
 class BaseApi(Generic[ResponseBodyT]):
     """Base class for all API clients."""
 
     url: str
     method: BaseApiMethod = BaseApiMethod.GET
-    auth: BaseAuth = None
-    request_params: type[BaseRequestParams] | None = None
-    request_body: type[BaseRequestBody] | None = None
+    auth: BaseHttpClientAuth = None
+    request_params: type[DictSerializableT] | None = None
+    request_body: type[DictSerializableT] | None = None
     response_body: type[ResponseBodyT]
-    http_client: type[BaseHttpClient] | BaseHttpClient | None = None
+    http_client: BaseHttpClient | None = None
 
     _http_client: BaseHttpClient = HTTPxClient()
-    _request_params: BaseRequestParams = BaseRequestParams()
-    _request_body: BaseRequestBody = BaseRequestBody()
+    _request_params: "DictSerializableT | None" = None
+    _request_body: "DictSerializableT | None" = None
     _response_body_cls: type[ResponseBodyT]
     _response: BaseResponse[ResponseBodyT] | None = None
 
     @classmethod
     def __init_subclass__(cls, **kwargs: object) -> None:
         super().__init_subclass__(**kwargs)
         cls._validate_subclass()
@@ -91,19 +76,15 @@
 
         if cls.request_body is not None:
             cls._request_body = cls.request_body()
 
         cls._response_body_cls = cls.response_body  # pyright: ignore [reportGeneralTypeIssues]
 
         if cls.http_client is not None:
-            cls._http_client = (
-                cls.http_client
-                if isinstance(cls.http_client, BaseHttpClient)
-                else cls.http_client()
-            )
+            cls._http_client = cls.http_client
 
     @classmethod
     def _validate_subclass(cls) -> None:
         if getattr(cls, "url", None) is None:
             raise ClientSetupError(attribute="url")
 
         if getattr(cls, "response_body", None) is None:
@@ -113,102 +94,120 @@
             getattr(cls, "method", None) is not None
             and cls.method not in BaseApiMethod.values()
         ):
             raise ClientSetupError(attribute="method")
 
         if getattr(cls, "http_client", None) is not None and not (
             isinstance(cls.http_client, BaseHttpClient)
-            or issubclass(cls.http_client, BaseHttpClient)  # type: ignore [arg-type]
         ):
             raise ClientSetupError(attribute="http_client")
 
         if getattr(cls, "__orig_bases__", None) is not None:
             response_body_generic_type = get_args(cls.__orig_bases__[0])[0]  # type: ignore [attr-defined]
             if (
                 isinstance(response_body_generic_type, TypeVar)
                 and response_body_generic_type.__name__ == "ResponseBodyT"
             ):
                 raise ClientSetupError(attribute="ResponseBodyT")
 
     def __init__(
         self,
-        request_params: BaseRequestParams | None = None,
-        request_body: BaseRequestBody | None = None,
+        request_params: "DictSerializableT | None" = None,
+        request_body: "DictSerializableT | None" = None,
         http_client: BaseHttpClient | None = None,
-        auth: BaseAuth = USE_DEFAULT,
+        auth: BaseHttpClientAuth = USE_DEFAULT,
     ) -> None:
         self._request_params = request_params or self._request_params
         self._request_body = request_body or self._request_body
         self._http_client = http_client or self._http_client
         self.auth = auth if auth != USE_DEFAULT else self.auth
 
     def execute(
         self,
-        request_params: BaseRequestParams | None = None,
-        request_body: BaseRequestBody | None = None,
+        request_params: "DictSerializableT | None" = None,
+        request_body: "DictSerializableT | None" = None,
         http_client: BaseHttpClient | None = None,
-        auth: BaseAuth = USE_DEFAULT,
+        auth: BaseHttpClientAuth = USE_DEFAULT,
     ) -> BaseResponse[ResponseBodyT]:
         """Execute the API request and return the response."""
 
         self._request_params = request_params or self._request_params
         self._request_body = request_body or self._request_body
         self._http_client = http_client or self._http_client
         self.auth = auth if auth != USE_DEFAULT else self.auth
+        try:
+            params = (
+                DictSerializable.to_dict(self._request_params)
+                if self._request_params
+                else {}
+            )
+            json = (
+                DictSerializable.to_dict(self._request_body)
+                if self._request_body
+                else {}
+            )
+        except DictDeserializationError as e:
+            raise RequestSerializationError(expected_type=e.expected_type) from e
 
         match self.method:
             case BaseApiMethod.GET:
                 client_response = self._http_client.get(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
+                    params=params,
                 )
             case BaseApiMethod.OPTIONS:
                 client_response = self._http_client.options(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
+                    params=params,
                 )
             case BaseApiMethod.HEAD:
                 client_response = self._http_client.head(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
+                    params=params,
                 )
             case BaseApiMethod.POST:
                 client_response = self._http_client.post(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
-                    json=self._request_body.to_dict(),
+                    params=params,
+                    json=json,
                 )
             case BaseApiMethod.PUT:
                 client_response = self._http_client.put(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
-                    json=self._request_body.to_dict(),
+                    params=params,
+                    json=json,
                 )
             case BaseApiMethod.PATCH:
                 client_response = self._http_client.patch(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
-                    json=self._request_body.to_dict(),
+                    params=params,
+                    json=json,
                 )
             case BaseApiMethod.DELETE:
                 client_response = self._http_client.delete(
                     url=self.url,
                     auth=self.auth,
-                    params=self._request_params.to_dict(),
+                    params=params,
                 )
             case _:
                 raise NotImplementedError(f"Method {self.method} not implemented.")
 
         # TODO: Add support for handling different response status codes
         if client_response.status_code != 200:
             raise HTTPError(client_response.status_code)
 
-        body = self._response_body_cls.from_dict(client_response.json())
+        try:
+            body = DictSerializable.from_dict(
+                self._response_body_cls, client_response.json()
+            )
+        except DictSerializationError as e:
+            raise ResponseSerializationError(expected_type=e.expected_type) from e
+
         self._response = BaseResponse(client_response=client_response, body=body)
 
         return self._response
```

### Comparing `quickapiclient-0.0.8/quickapi/exceptions.py` & `quickapiclient-0.0.9/quickapi/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,22 +14,52 @@
     """The response received a non `200` response status code."""
 
     def __init__(self, status_code: int):
         message = f"HTTP request received a non `HTTP 200 (OK)` response. The response status code was `{status_code}`."
         super().__init__(message)
 
 
+class DictSerializationError(QuickApiException):
+    """Dict serialization failed."""
+
+    expected_type = ""
+
+    def __init__(self, expected_type: str):
+        self.expected_type = expected_type
+        super().__init__(self.__doc__)
+
+
+class DictDeserializationError(QuickApiException):
+    """Dict deserialization failed."""
+
+    expected_type = ""
+
+    def __init__(self, expected_type: str):
+        self.expected_type = expected_type
+        super().__init__(self.__doc__)
+
+
 class ResponseSerializationError(QuickApiException):
     """The response received was not serializable to the configured `response_body` type."""
 
     def __init__(self, expected_type: str):
         message = f"HTTP response body did not match expected type `{expected_type}`."
         super().__init__(message)
 
 
+class RequestSerializationError(QuickApiException):
+    """The request was not serializable to the configured type."""
+
+    def __init__(self, expected_type: str):
+        message = (
+            f"HTTP request params/body did not match expected type `{expected_type}`."
+        )
+        super().__init__(message)
+
+
 class MissingDependencyError(QuickApiException):
     """Trying to use an optional dependency without installing it first."""
 
     def __init__(self, dependency: str):
         message = (
             f"Using an optional dependecy without installing it first `{dependency}`."
             f"Please install the dependency using `pip install quickapiclient[{dependency}]`."
```

### Comparing `quickapiclient-0.0.8/quickapi/http_client.py` & `quickapiclient-0.0.9/quickapi/http_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-from contextlib import suppress
-from typing import TYPE_CHECKING, TypeAlias
+from abc import ABC, abstractmethod
+from typing import TypeAlias
 
 import httpx
 
 from .exceptions import MissingDependencyError
 
-if TYPE_CHECKING:
-    with suppress(ImportError):
-        import requests
+try:
+    import requests
+except ImportError:
+    requests_installed = False
+else:
+    requests_installed = True
 
 # TODO: Fix types
-BaseAuth: TypeAlias = httpx.Auth | type["requests.auth.AuthBase"] | object | None
+BaseHttpClientAuth: TypeAlias = "httpx.Auth | requests.auth.AuthBase | object | None"
+BaseHttpClientResponse: TypeAlias = "httpx.Response | requests.Response | None"
 
 
-class BaseHttpClient:
+class BaseHttpClient(ABC):
     """Base interface for all HTTP clients."""
 
+    @abstractmethod
     def __init__(self, *args, **kwargs): ...  # type: ignore [no-untyped-def]
 
+    @abstractmethod
     def get(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
+    @abstractmethod
     def options(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
+    @abstractmethod
     def head(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
+    @abstractmethod
     def post(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
+    @abstractmethod
     def put(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
+    @abstractmethod
     def patch(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
+    @abstractmethod
     def delete(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         raise NotImplementedError
 
 
 class HTTPxClient(BaseHttpClient):
     """A thin wrapper around HTTPx. This is the default client."""
 
@@ -74,18 +86,16 @@
 
     This client is only available if the requests library is installed with:
     `pip install quickapiclient[requests]`
     or `poetry add quickapiclient[requests]`.
     """
 
     def __init__(self, client: type["requests.sessions.Session"] | None = None):
-        try:
-            import requests
-        except ImportError as exc:
-            raise MissingDependencyError(dependency="requests") from exc
+        if requests_installed is False:
+            raise MissingDependencyError(dependency="requests")
 
         self._client = client or requests.sessions.Session()
 
     def get(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         return self._client.get(*args, **kwargs)
 
     def options(self, *args, **kwargs):  # type: ignore [no-untyped-def]
```

### Comparing `quickapiclient-0.0.8/PKG-INFO` & `quickapiclient-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: quickapiclient
-Version: 0.0.8
-Summary: A library for creating fully typed declarative API clients quickly and easily.
-Home-page: https://github.com/martinn/quickapiclient
-Author: Martin N.
-Author-email: martinn@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: requests
-Requires-Dist: attrs (>=23.2.0,<24.0.0)
-Requires-Dist: cattrs (>=23.2.3,<24.0.0)
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "requests"
-Project-URL: Documentation, https://martinn.github.io/quickapiclient/
-Project-URL: Repository, https://github.com/martinn/quickapiclient
-Description-Content-Type: text/markdown
-
 # Quick Api Client
 
 [![Release](https://img.shields.io/github/v/release/martinn/quickapiclient)](https://img.shields.io/github/v/release/martinn/quickapiclient)
 [![Build status](https://img.shields.io/github/actions/workflow/status/martinn/quickapiclient/main.yml?branch=main)](https://github.com/martinn/quickapiclient/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/martinn/quickapiclient/branch/main/graph/badge.svg)](https://codecov.io/gh/martinn/quickapiclient)
 
 A library for creating fully typed declarative API clients quickly and easily.
@@ -31,28 +10,28 @@
 - **Documentation** <https://martinn.github.io/quickapiclient/>
 
 ## A quick example
 
 An API definition for a simple service could look like this:
 
 ```python
-import attrs
+from dataclasses import dataclass
 import quickapi
 
 
 # An example type that will be part of the API response
-@attrs.define
+@dataclass
 class Fact:
     fact: str
     length: int
 
 
 # What the API response should look like
-@attrs.define
-class ResponseBody(quickapi.BaseResponseBody):
+@dataclass
+class ResponseBody:
     current_page: int
     data: list[Fact]
 
 
 # Now we can define our API
 class MyApi(quickapi.BaseApi[ResponseBody]):
     url = "https://catfact.ninja/facts"
@@ -62,99 +41,134 @@
 And you would use it like this:
 
 ```python
 api_client = MyApi()
 response = api_client.execute()
 
 # That's it! Now `response` is fully typed and conforms to our `ResponseBody` definition
-assert isinstance(response.body, ResponseBody) == True
-assert isinstance(response.body.data[0], Fact) == True
+assert isinstance(response.body, ResponseBody)
+assert isinstance(response.body.data[0], Fact)
 ```
 
+There's also support for `attrs` or `pydantic` for more complex modeling, validation or serialization support.
+
+Scroll down [here](#a-post-request-with-validation-and-conversion-using-attrs) for examples using those.
+
 ## Features
 
-It's still early development and this is currently tightly coupled with `attrs`,
-but could expand to support others in the future if there's interest.
+It's still early development but so far we have support for:
 
 - Write fully typed declarative API clients quickly and easily
   - [x] Fully typed request params / body
   - [x] Fully typed response body
-  - [x] Built in serialization/deserialization with `attrs`
+  - [x] Serialization/deserialization support
   - [x] Basic error and serialization handling
   - [ ] Nested/inner class definitions
   - [ ] Improved HTTP status codes error handling
   - [ ] Sessions support and/or allow building several related APIs through a single interface
-  - [ ] Generate API boilerplate from OpenAPI specs?
+  - [ ] Generate API boilerplate from OpenAPI specs
+  - [ ] Full async support
 - HTTP client libraries
   - [x] httpx
   - [x] requests
   - [ ] aiohttp
 - Authentication mechanisms
   - [x] Basic Auth
   - [x] Token / JWT
   - [x] Digest
   - [x] NetRC
-  - [x] Any auth supported by `httpx` or [httpx_auth](https://github.com/Colin-b/httpx_auth) or `requests`,
-        including custom schemes
+  - [x] Any auth supported by `httpx` or [httpx_auth](https://github.com/Colin-b/httpx_auth) or `requests`, including custom schemes
 - Serialization/deserialization
   - [x] attrs
-  - [ ] dataclasses
-  - [ ] pydantic
+  - [x] dataclasses
+  - [x] pydantic
 - API support
   - [x] REST
   - [ ] GraphQL
-  - [ ] Maybe others?
+  - [ ] Others?
 - Response types supported
   - [x] JSON
   - [ ] XML
   - [ ] Others?
 
+## Goal
+
+Eventually, I would like for the API definition to end up looking more like this (though the current approach will still be supported):
+
+```python
+import quickapi
+
+
+@quickapi.define
+class MyApi:
+    url = "https://catfact.ninja/facts"
+    method = quickapi.BaseApiMethod.POST
+
+    class RequestBody:
+        required_input: str
+        optional_input: str | None = None
+
+    class ResponseBody:
+        current_page: int
+        data: list[Fact]
+```
+
+And also to be able to support multiple endpoints per API client.
+
 ## Installation
 
 You can easily install this using `pip`:
 
 ```console
 pip install quickapiclient
+# Or if you want to use `attrs` over `dataclasses`:
+pip install quickapiclient[attrs]
+# Or if you want to use `pydantic` over `dataclasses`:
+pip install quickapiclient[pydantic]
 # Or if you want to use `requests` over `httpx`:
 pip install quickapiclient[requests]
 ```
 
 Or if using `poetry`:
 
 ```console
 poetry add quickapiclient
+# Or if you want to use `attrs` over `dataclasses`:
+poetry add quickapiclient[attrs]
+# Or if you want to use `pydantic` over `dataclasses`:
+poetry add quickapiclient[pydantic]
 # Or if you want to use `requests` over `httpx`:
 poetry add quickapiclient[requests]
 ```
 
 ## More examples
 
 ### A GET request with query params
 
 An example of a GET request with query parameters with overridable default values.
 
 ```python
-import attrs
+from dataclasses import dataclass
 import quickapi
 
 
-@attrs.define
-class RequestParams(quickapi.BaseRequestParams):
+@dataclass
+class RequestParams:
     max_length: int = 100
     limit: int = 10
 
 
-@attrs.define
+@dataclass
 class Fact:
     fact: str
     length: int
 
 
-@attrs.define
-class ResponseBody(quickapi.BaseResponseBody):
+@dataclass
+class ResponseBody:
     current_page: int
     data: list[Fact]
 
 
 class MyApi(quickapi.BaseApi[ResponseBody]):
     url = "https://catfact.ninja/facts"
     request_params = RequestParams
@@ -174,32 +188,32 @@
 ```
 
 ### A POST request
 
 An example of a POST request with some optional and required data.
 
 ```python
-import attrs
+from dataclasses import dataclass
 import quickapi
 
 
-@attrs.define
-class RequestBody(quickapi.BaseRequestBody):
+@dataclass
+class RequestBody:
     required_input: str
     optional_input: str | None = None
 
 
-@attrs.define
+@dataclass
 class Fact:
     fact: str
     length: int
 
 
-@attrs.define
-class ResponseBody(quickapi.BaseResponseBody):
+@dataclass
+class ResponseBody:
     current_page: int
     data: list[Fact]
 
 
 class MyApi(quickapi.BaseApi[ResponseBody]):
     url = "https://catfact.ninja/facts"
     method = quickapi.BaseApiMethod.POST
@@ -216,33 +230,33 @@
 ```
 
 ### A POST request with authentication
 
 An example of a POST request with HTTP header API key.
 
 ```python
-import attrs
+from dataclasses import dataclass
 import httpx_auth
 import quickapi
 
 
-@attrs.define
-class RequestBody(quickapi.BaseRequestBody):
+@dataclass
+class RequestBody:
     required_input: str
     optional_input: str | None = None
 
 
-@attrs.define
+@dataclass
 class Fact:
     fact: str
     length: int
 
 
-@attrs.define
-class AuthResponseBody(quickapi.BaseResponseBody):
+@dataclass
+class AuthResponseBody:
     authenticated: bool
     user: str
 
 
 class MyApi(quickapi.BaseApi[AuthResponseBody]):
     url = "https://httpbin.org/bearer"
     method = quickapi.BaseApiMethod.POST
@@ -256,41 +270,41 @@
 ```python
 client = MyApi()
 request_body = RequestBody(required_input="dummy")
 auth = httpx_auth.HeaderApiKey(header_name="X-Api-Key", api_key="secret_api_key")
 response = client.execute(request_body=request_body, auth=auth)
 ```
 
-### A POST request with validation and conversion
+### A POST request with validation and conversion (Using `attrs`)
 
-An example of a POST request with custom validators and converters (from `attrs`).
+An example of a POST request with custom validators and converters (using `attrs` instead).
 
 ```python
 import attrs
 import quickapi
 import enum
 
 
 class State(enum.Enum):
     ON = "on"
     OFF = "off"
 
 
 @attrs.define
-class RequestBody(quickapi.BaseRequestBody):
+class RequestBody:
     state: State = attrs.field(validator=attrs.validators.in_(State))
     email: str = attrs.field(
         validator=attrs.validators.matches_re(
             r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)"
         )
     )
 
 
 @attrs.define
-class ResponseBody(quickapi.BaseResponseBody):
+class ResponseBody:
     success: bool = attrs.field(converter=attrs.converters.to_bool)
 
 
 class MyApi(quickapi.BaseApi[ResponseBody]):
     url = "https://example.com/"
     method = quickapi.BaseApiMethod.POST
     request_body = RequestBody
@@ -303,25 +317,66 @@
 client = MyApi()
 request_body = RequestBody(email="invalid_email", state="on") # Will raise an error
 response = client.execute(request_body=request_body)
 ```
 
 Check out [attrs](https://github.com/python-attrs/attrs) for full configuration.
 
+### A POST request with validation and conversion (Using `pydantic`)
+
+An example of a POST request with custom validators and converters (using `pydantic` instead).
+
+```python
+import enum
+import pydantic
+import quickapi
+
+
+class State(enum.Enum):
+    ON = "on"
+    OFF = "off"
+
+
+class RequestBody(pydantic.BaseModel):
+    state: State
+    email: pydantic.EmailStr
+
+
+class ResponseBody(pydantic.BaseModel):
+    success: bool
+
+
+class MyApi(quickapi.BaseApi[ResponseBody]):
+    url = "https://example.com/"
+    method = quickapi.BaseApiMethod.POST
+    request_body = RequestBody
+    response_body = ResponseBody
+```
+
+And to use it:
+
+```python
+client = MyApi()
+request_body = RequestBody(email="invalid_email", state="on") # Will raise an error
+response = client.execute(request_body=request_body)
+```
+
+Check out [pydantic](https://github.com/pydantic/pydantic) for full configuration.
+
 ### Using `requests` library
 
 An example of a GET request using the `requests` HTTP library instead of `HTTPx`.
 
 ```python
-import attrs
+from dataclasses import dataclass
 import quickapi
 
 
-@attrs.define
-class ResponseBody(quickapi.BaseResponseBody):
+@dataclass
+class ResponseBody:
     current_page: int
     data: list[Fact]
 
 
 class MyApi(quickapi.BaseApi[ResponseBody]):
     url = "https://catfact.ninja/facts"
     response_body = ResponseBody
@@ -335,10 +390,12 @@
 response = client.execute()
 ```
 
 ## Contributing
 
 Contributions are welcomed, and greatly appreciated!
 
-If you want to contribute, check out the
-[contributing guide](./CONTRIBUTING.md) to get started.
+The easiest way to contribute, if you found this useful or interesting,
+is by giving it a star! 🌟
 
+Otherwise, check out the
+[contributing guide](./CONTRIBUTING.md) for how else to help and get started.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

