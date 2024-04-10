# Comparing `tmp/multion-1.0.0.tar.gz` & `tmp/multion-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-1.0.0.tar", max compression
+gzip compressed data, was "multion-1.0.1.tar", max compression
```

## Comparing `multion-1.0.0.tar` & `multion-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     3937 2024-04-06 20:26:20.192376 multion-1.0.0/README.md
--rw-r--r--   0        0        0      592 2024-04-06 20:26:20.192376 multion-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1417 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/__init__.py
--rw-r--r--   0        0        0    15767 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/client.py
--rw-r--r--   0        0        0      853 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/api_error.py
--rw-r--r--   0        0        0     1490 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/request_options.py
--rw-r--r--   0        0        0      162 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/environment.py
--rw-r--r--   0        0        0      385 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/__init__.py
--rw-r--r--   0        0        0      301 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/bad_request_error.py
--rw-r--r--   0        0        0      333 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/internal_server_error.py
--rw-r--r--   0        0        0      308 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/py.typed
--rw-r--r--   0        0        0      427 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/__init__.py
--rw-r--r--   0        0        0    28787 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/client.py
--rw-r--r--   0        0        0      590 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/create_session_input_browser_params.py
--rw-r--r--   0        0        0     1048 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/sessions_close_response.py
--rw-r--r--   0        0        0      953 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/sessions_list_response.py
--rw-r--r--   0        0        0      967 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/sessions_screenshot_response.py
--rw-r--r--   0        0        0     1022 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/step_session_input_browser_params.py
--rw-r--r--   0        0        0     1015 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/bad_request_response.py
--rw-r--r--   0        0        0     1355 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/browse_output.py
--rw-r--r--   0        0        0      953 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/http_validation_error.py
--rw-r--r--   0        0        0     1100 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/internal_server_error_response.py
--rw-r--r--   0        0        0     1096 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/payment_required_response.py
--rw-r--r--   0        0        0      850 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/remote_value.py
--rw-r--r--   0        0        0     1312 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/retrieve_output.py
--rw-r--r--   0        0        0     1361 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/session_created.py
--rw-r--r--   0        0        0     1365 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/session_step_success.py
--rw-r--r--   0        0        0     1093 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/unauthorized_response.py
--rw-r--r--   0        0        0      972 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       75 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/version.py
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3937 2024-04-10 23:22:32.678930 multion-1.0.1/README.md
+-rw-r--r--   0        0        0      592 2024-04-10 23:22:32.678930 multion-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1447 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/__init__.py
+-rw-r--r--   0        0        0    16274 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/client.py
+-rw-r--r--   0        0        0     1006 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/api_error.py
+-rw-r--r--   0        0        0     1490 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      162 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/environment.py
+-rw-r--r--   0        0        0      385 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/__init__.py
+-rw-r--r--   0        0        0      301 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/bad_request_error.py
+-rw-r--r--   0        0        0      333 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/internal_server_error.py
+-rw-r--r--   0        0        0      308 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/py.typed
+-rw-r--r--   0        0        0      427 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/__init__.py
+-rw-r--r--   0        0        0    29484 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/client.py
+-rw-r--r--   0        0        0      590 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/create_session_input_browser_params.py
+-rw-r--r--   0        0        0     1105 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/sessions_close_response.py
+-rw-r--r--   0        0        0     1010 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/sessions_list_response.py
+-rw-r--r--   0        0        0     1024 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/sessions_screenshot_response.py
+-rw-r--r--   0        0        0     1079 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/sessions/types/step_session_input_browser_params.py
+-rw-r--r--   0        0        0     1062 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/bad_request_response.py
+-rw-r--r--   0        0        0     1573 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/browse_output.py
+-rw-r--r--   0        0        0     1009 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/http_validation_error.py
+-rw-r--r--   0        0        0     1156 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/internal_server_error_response.py
+-rw-r--r--   0        0        0     1231 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/metadata.py
+-rw-r--r--   0        0        0     1152 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/payment_required_response.py
+-rw-r--r--   0        0        0      906 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/remote_value.py
+-rw-r--r--   0        0        0     1368 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/retrieve_output.py
+-rw-r--r--   0        0        0     1417 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/session_created.py
+-rw-r--r--   0        0        0     1421 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/session_step_success.py
+-rw-r--r--   0        0        0     1149 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/unauthorized_response.py
+-rw-r--r--   0        0        0     1028 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       75 2024-04-10 23:22:32.678930 multion-1.0.1/src/multion/version.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-1.0.1/PKG-INFO
```

### Comparing `multion-1.0.0/README.md` & `multion-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/pyproject.toml` & `multion-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multion"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "multion", from = "src"}
 ]
```

### Comparing `multion-1.0.0/src/multion/__init__.py` & `multion-1.0.1/src/multion/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     BadRequestResponse,
     BrowseOutput,
     HttpValidationError,
     InternalServerErrorResponse,
+    Metadata,
     PaymentRequiredResponse,
     RemoteValue,
     RetrieveOutput,
     SessionCreated,
     SessionStepSuccess,
     UnauthorizedResponse,
     ValidationError,
@@ -30,14 +31,15 @@
     "BadRequestError",
     "BadRequestResponse",
     "BrowseOutput",
     "CreateSessionInputBrowserParams",
     "HttpValidationError",
     "InternalServerError",
     "InternalServerErrorResponse",
+    "Metadata",
     "MultiOnEnvironment",
     "PaymentRequiredResponse",
     "RemoteValue",
     "RetrieveOutput",
     "SessionCreated",
     "SessionStepSuccess",
     "SessionsCloseResponse",
```

### Comparing `multion-1.0.0/src/multion/client.py` & `multion-1.0.1/src/multion/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 
 from .core.api_error import ApiError
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .core.jsonable_encoder import jsonable_encoder
-from .core.pydantic_utilities import pydantic_v1
 from .core.remove_none_from_dict import remove_none_from_dict
 from .core.request_options import RequestOptions
+from .core.unchecked_base_model import construct_type
 from .environment import MultiOnEnvironment
 from .errors.bad_request_error import BadRequestError
 from .errors.internal_server_error import InternalServerError
 from .errors.unauthorized_error import UnauthorizedError
 from .errors.unprocessable_entity_error import UnprocessableEntityError
 from .sessions.client import AsyncSessionsClient, SessionsClient
 from .types.bad_request_response import BadRequestResponse
@@ -155,26 +155,30 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BrowseOutput, _response.json())  # type: ignore
+            return typing.cast(BrowseOutput, construct_type(type_=BrowseOutput, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequestResponse, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequestResponse, construct_type(type_=BadRequestResponse, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic_v1.parse_obj_as(UnauthorizedResponse, _response.json()))  # type: ignore
+            raise UnauthorizedError(
+                typing.cast(UnauthorizedResponse, construct_type(type_=UnauthorizedResponse, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
-                pydantic_v1.parse_obj_as(InternalServerErrorResponse, _response.json())  # type: ignore
+                typing.cast(InternalServerErrorResponse, construct_type(type_=InternalServerErrorResponse, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -305,26 +309,30 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BrowseOutput, _response.json())  # type: ignore
+            return typing.cast(BrowseOutput, construct_type(type_=BrowseOutput, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequestResponse, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequestResponse, construct_type(type_=BadRequestResponse, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic_v1.parse_obj_as(UnauthorizedResponse, _response.json()))  # type: ignore
+            raise UnauthorizedError(
+                typing.cast(UnauthorizedResponse, construct_type(type_=UnauthorizedResponse, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 500:
             raise InternalServerError(
-                pydantic_v1.parse_obj_as(InternalServerErrorResponse, _response.json())  # type: ignore
+                typing.cast(InternalServerErrorResponse, construct_type(type_=InternalServerErrorResponse, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `multion-1.0.0/src/multion/core/__init__.py` & `multion-1.0.1/src/multion/core/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
 from .pydantic_utilities import pydantic_v1
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
+from .unchecked_base_model import UncheckedBaseModel, UnionMetadata, construct_type
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
     "AsyncHttpClient",
     "BaseClientWrapper",
     "File",
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
+    "UncheckedBaseModel",
+    "UnionMetadata",
+    "construct_type",
     "convert_file_dict_to_httpx_tuples",
     "jsonable_encoder",
     "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `multion-1.0.0/src/multion/core/client_wrapper.py` & `multion-1.0.1/src/multion/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "multion",
-            "X-Fern-SDK-Version": "1.0.0",
+            "X-Fern-SDK-Version": "1.0.1",
         }
         headers["X_MULTION_API_KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `multion-1.0.0/src/multion/core/datetime_utils.py` & `multion-1.0.1/src/multion/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/src/multion/core/file.py` & `multion-1.0.1/src/multion/core/file.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/src/multion/core/http_client.py` & `multion-1.0.1/src/multion/core/http_client.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/src/multion/core/jsonable_encoder.py` & `multion-1.0.1/src/multion/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/src/multion/core/request_options.py` & `multion-1.0.1/src/multion/core/request_options.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/src/multion/sessions/client.py` & `multion-1.0.1/src/multion/sessions/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.session_created import SessionCreated
 from ..types.session_step_success import SessionStepSuccess
 from .types.create_session_input_browser_params import CreateSessionInputBrowserParams
 from .types.sessions_close_response import SessionsCloseResponse
 from .types.sessions_list_response import SessionsListResponse
@@ -90,18 +90,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionCreated, _response.json())  # type: ignore
+            return typing.cast(SessionCreated, construct_type(type_=SessionCreated, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -176,18 +176,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionStepSuccess, _response.json())  # type: ignore
+            return typing.cast(SessionStepSuccess, construct_type(type_=SessionStepSuccess, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -228,18 +228,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionsCloseResponse, _response.json())  # type: ignore
+            return typing.cast(SessionsCloseResponse, construct_type(type_=SessionsCloseResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -282,18 +282,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionsScreenshotResponse, _response.json())  # type: ignore
+            return typing.cast(SessionsScreenshotResponse, construct_type(type_=SessionsScreenshotResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -328,15 +328,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionsListResponse, _response.json())  # type: ignore
+            return typing.cast(SessionsListResponse, construct_type(type_=SessionsListResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -406,18 +406,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionCreated, _response.json())  # type: ignore
+            return typing.cast(SessionCreated, construct_type(type_=SessionCreated, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -492,18 +492,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionStepSuccess, _response.json())  # type: ignore
+            return typing.cast(SessionStepSuccess, construct_type(type_=SessionStepSuccess, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -544,18 +544,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionsCloseResponse, _response.json())  # type: ignore
+            return typing.cast(SessionsCloseResponse, construct_type(type_=SessionsCloseResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -598,18 +598,18 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionsScreenshotResponse, _response.json())  # type: ignore
+            return typing.cast(SessionsScreenshotResponse, construct_type(type_=SessionsScreenshotResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
-                pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
@@ -644,13 +644,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SessionsListResponse, _response.json())  # type: ignore
+            return typing.cast(SessionsListResponse, construct_type(type_=SessionsListResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `multion-1.0.0/src/multion/sessions/types/__init__.py` & `multion-1.0.1/src/multion/sessions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-1.0.0/src/multion/sessions/types/create_session_input_browser_params.py` & `multion-1.0.1/src/multion/sessions/types/create_session_input_browser_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class CreateSessionInputBrowserParams(pydantic_v1.BaseModel):
+class CreateSessionInputBrowserParams(UncheckedBaseModel):
     """
     Object containing height and width for the browser screen size.
     """
 
     height: typing.Optional[float] = None
     width: typing.Optional[float] = None
```

### Comparing `multion-1.0.0/src/multion/sessions/types/sessions_close_response.py` & `multion-1.0.1/src/multion/sessions/types/sessions_close_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SessionsCloseResponse(pydantic_v1.BaseModel):
+class SessionsCloseResponse(UncheckedBaseModel):
     status: str = pydantic_v1.Field()
     """
     response data
     """
 
     session_id: str = pydantic_v1.Field()
     """
```

### Comparing `multion-1.0.0/src/multion/sessions/types/sessions_list_response.py` & `multion-1.0.1/src/multion/types/remote_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SessionsListResponse(pydantic_v1.BaseModel):
-    session_ids: typing.List[str] = pydantic_v1.Field()
-    """
-    The list of active session IDs.
-    """
+class RemoteValue(UncheckedBaseModel):
+    value: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `multion-1.0.0/src/multion/sessions/types/sessions_screenshot_response.py` & `multion-1.0.1/src/multion/sessions/types/sessions_screenshot_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SessionsScreenshotResponse(pydantic_v1.BaseModel):
+class SessionsScreenshotResponse(UncheckedBaseModel):
     screenshot: str = pydantic_v1.Field()
     """
     Image url of the screenshot taken during the session.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `multion-1.0.0/src/multion/sessions/types/step_session_input_browser_params.py` & `multion-1.0.1/src/multion/sessions/types/step_session_input_browser_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class StepSessionInputBrowserParams(pydantic_v1.BaseModel):
+class StepSessionInputBrowserParams(UncheckedBaseModel):
     """
     Object containing height and width for the browser screen size.
     """
 
     height: typing.Optional[float] = None
     width: typing.Optional[float] = None
```

### Comparing `multion-1.0.0/src/multion/types/__init__.py` & `multion-1.0.1/src/multion/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .bad_request_response import BadRequestResponse
 from .browse_output import BrowseOutput
 from .http_validation_error import HttpValidationError
 from .internal_server_error_response import InternalServerErrorResponse
+from .metadata import Metadata
 from .payment_required_response import PaymentRequiredResponse
 from .remote_value import RemoteValue
 from .retrieve_output import RetrieveOutput
 from .session_created import SessionCreated
 from .session_step_success import SessionStepSuccess
 from .unauthorized_response import UnauthorizedResponse
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
 
 __all__ = [
     "BadRequestResponse",
     "BrowseOutput",
     "HttpValidationError",
     "InternalServerErrorResponse",
+    "Metadata",
     "PaymentRequiredResponse",
     "RemoteValue",
     "RetrieveOutput",
     "SessionCreated",
     "SessionStepSuccess",
     "UnauthorizedResponse",
     "ValidationError",
```

### Comparing `multion-1.0.0/src/multion/types/bad_request_response.py` & `multion-1.0.1/src/multion/sessions/types/sessions_list_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BadRequestResponse(pydantic_v1.BaseModel):
-    status_code: typing.Optional[int] = pydantic_v1.Field(alias="statusCode", default=None)
-    error: typing.Optional[str] = None
-    message: typing.Optional[str] = None
+class SessionsListResponse(UncheckedBaseModel):
+    session_ids: typing.List[str] = pydantic_v1.Field()
+    """
+    The list of active session IDs.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `multion-1.0.0/src/multion/types/browse_output.py` & `multion-1.0.1/src/multion/types/browse_output.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .metadata import Metadata
 
 
-class BrowseOutput(pydantic_v1.BaseModel):
+class BrowseOutput(UncheckedBaseModel):
     message: str = pydantic_v1.Field()
     """
     The final message or result of the browsing session.
     """
 
     status: str = pydantic_v1.Field()
     """
@@ -29,14 +31,19 @@
     """
 
     session_id: str = pydantic_v1.Field()
     """
     The unique identifier for the session.
     """
 
+    metadata: typing.Optional[Metadata] = pydantic_v1.Field(default=None)
+    """
+    Additional metadata for the session
+    """
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `multion-1.0.0/src/multion/types/http_validation_error.py` & `multion-1.0.1/src/multion/types/validation_error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .validation_error import ValidationError
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class HttpValidationError(pydantic_v1.BaseModel):
-    detail: typing.Optional[typing.List[ValidationError]] = None
+class ValidationError(UncheckedBaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `multion-1.0.0/src/multion/types/internal_server_error_response.py` & `multion-1.0.1/src/multion/types/internal_server_error_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class InternalServerErrorResponse(pydantic_v1.BaseModel):
+class InternalServerErrorResponse(UncheckedBaseModel):
     status_code: typing.Optional[int] = pydantic_v1.Field(alias="statusCode", default=None)
     error: typing.Optional[str] = None
     message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `multion-1.0.0/src/multion/types/payment_required_response.py` & `multion-1.0.1/src/multion/types/payment_required_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class PaymentRequiredResponse(pydantic_v1.BaseModel):
+class PaymentRequiredResponse(UncheckedBaseModel):
     status_code: typing.Optional[int] = pydantic_v1.Field(alias="statusCode", default=None)
     error: typing.Optional[str] = None
     message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `multion-1.0.0/src/multion/types/retrieve_output.py` & `multion-1.0.1/src/multion/types/retrieve_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class RetrieveOutput(pydantic_v1.BaseModel):
+class RetrieveOutput(UncheckedBaseModel):
     message: str = pydantic_v1.Field()
     """
     information on a webpage based on a user query
     """
 
     url: str = pydantic_v1.Field()
     """
```

### Comparing `multion-1.0.0/src/multion/types/session_created.py` & `multion-1.0.1/src/multion/types/session_created.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SessionCreated(pydantic_v1.BaseModel):
+class SessionCreated(UncheckedBaseModel):
     status: str = pydantic_v1.Field()
     """
     The current status of the session.
     """
 
     message: str = pydantic_v1.Field()
     """
```

### Comparing `multion-1.0.0/src/multion/types/session_step_success.py` & `multion-1.0.1/src/multion/types/session_step_success.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SessionStepSuccess(pydantic_v1.BaseModel):
+class SessionStepSuccess(UncheckedBaseModel):
     status: str = pydantic_v1.Field()
     """
     The current status of the session.
     """
 
     message: str = pydantic_v1.Field()
     """
```

### Comparing `multion-1.0.0/src/multion/types/unauthorized_response.py` & `multion-1.0.1/src/multion/types/unauthorized_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class UnauthorizedResponse(pydantic_v1.BaseModel):
+class UnauthorizedResponse(UncheckedBaseModel):
     status_code: typing.Optional[int] = pydantic_v1.Field(alias="statusCode", default=None)
     error: typing.Optional[str] = None
     message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `multion-1.0.0/PKG-INFO` & `multion-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multion
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

