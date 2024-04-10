# Comparing `tmp/sdkgen-client-0.2.0.tar.gz` & `tmp/sdkgen-client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkgen-client-0.2.0.tar", last modified: Wed Apr 10 17:33:11 2024, max compression
+gzip compressed data, was "sdkgen-client-0.2.1.tar", last modified: Wed Apr 10 20:24:40 2024, max compression
```

## Comparing `sdkgen-client-0.2.0.tar` & `sdkgen-client-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:33:11.519335 sdkgen-client-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/src/sdkgen/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/client_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/src/sdkgen/token_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 17:33:11.000000 sdkgen-client-0.2.0/src/sdkgen_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:33:11.515335 sdkgen-client-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-10 17:33:07.000000 sdkgen-client-0.2.0/tests/test_serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:40.868723 sdkgen-client-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 20:24:40.868723 sdkgen-client-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:24:40.868723 sdkgen-client-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:40.864723 sdkgen-client-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:40.864723 sdkgen-client-0.2.1/src/sdkgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/client_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/src/sdkgen/token_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:40.868723 sdkgen-client-0.2.1/src/sdkgen_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 20:24:40.000000 sdkgen-client-0.2.1/src/sdkgen_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-10 20:24:40.000000 sdkgen-client-0.2.1/src/sdkgen_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:24:40.000000 sdkgen-client-0.2.1/src/sdkgen_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 20:24:40.000000 sdkgen-client-0.2.1/src/sdkgen_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 20:24:40.000000 sdkgen-client-0.2.1/src/sdkgen_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:24:40.868723 sdkgen-client-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 20:24:33.000000 sdkgen-client-0.2.1/tests/test_serialize.py
```

### Comparing `sdkgen-client-0.2.0/LICENSE` & `sdkgen-client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.2.0/PKG-INFO` & `sdkgen-client-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkgen-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDKgen is a powerful code generator to automatically build client SDKs for your REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/sdkgen-python
 Project-URL: Issues, https://github.com/apioo/sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkgen-client-0.2.0/pyproject.toml` & `sdkgen-client-0.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkgen-client"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDKgen is a powerful code generator to automatically build client SDKs for your REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkgen-client-0.2.0/src/sdkgen/__init__.py` & `sdkgen-client-0.2.1/src/sdkgen/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.2.0/src/sdkgen/access_token.py` & `sdkgen-client-0.2.1/src/sdkgen/access_token.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import time
-from dataclasses import dataclass
-from dataclasses import field as data_field
 from typing import Optional
 
-from dataclasses_json import config as json_config
-from dataclasses_json import dataclass_json
+from pydantic import BaseModel, Field
 
 
-@dataclass_json
-@dataclass
-class AccessToken:
-    access_token: Optional[str] = data_field(default=None, metadata=json_config(field_name="access_token"))
-    token_type: Optional[str] = data_field(default=None, metadata=json_config(field_name="token_type"))
-    expires_in: Optional[int] = data_field(default=None, metadata=json_config(field_name="expires_in"))
-    refresh_token: Optional[str] = data_field(default=None, metadata=json_config(field_name="refresh_token"))
-    scope: Optional[str] = data_field(default=None, metadata=json_config(field_name="scope"))
+class AccessToken(BaseModel):
+    access_token: Optional[str] = Field(default=None, alias="access_token")
+    token_type: Optional[str] = Field(default=None, alias="token_type")
+    expires_in: Optional[int] = Field(default=None, alias="expires_in")
+    refresh_token: Optional[str] = Field(default=None, alias="refresh_token")
+    scope: Optional[str] = Field(default=None, alias="scope")
 
     @classmethod
     def get_expires_in_timestamp(cls):
         now = time.time()
 
         expires_in = cls.expires_in
         if cls.expires_in < 529196400:
```

### Comparing `sdkgen-client-0.2.0/src/sdkgen/authenticator.py` & `sdkgen-client-0.2.1/src/sdkgen/authenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
     @classmethod
     def parse_token_response(cls, response: Response) -> AccessToken:
         if response.status_code != 200:
             raise InvalidAccessTokenException(
                 "Could not obtain access token, received a non successful status code: " + str(response.status_code))
 
-        token = AccessToken.from_json(response.content)
+        token = AccessToken.model_validate_json(json_data=response.content)
 
         cls.token_store.persist(token)
 
         return token
 
     @classmethod
     def new_http_client(cls, credentials: CredentialsInterface) -> Session:
```

### Comparing `sdkgen-client-0.2.0/src/sdkgen/client_abstract.py` & `sdkgen-client-0.2.1/src/sdkgen/client_abstract.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.2.0/src/sdkgen/credentials.py` & `sdkgen-client-0.2.1/src/sdkgen/credentials.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.2.0/src/sdkgen/parser.py` & `sdkgen-client-0.2.1/src/sdkgen/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def query(cls, parameters: dict[str, any], struct_names: list[str] = None) -> dict[str, any]:
         result: dict[str, any] = {}
         for name, value in parameters.items():
             if value is None:
                 continue
 
             if struct_names and name in struct_names:
-                result = result | cls.query(value.to_dict())
+                result = result | cls.query(value.model_dump())
             else:
                 result[name] = cls.to_string(value)
 
         return result
 
     @classmethod
     def to_string(cls, value: any) -> string:
```

### Comparing `sdkgen-client-0.2.0/src/sdkgen/token_store.py` & `sdkgen-client-0.2.1/src/sdkgen/token_store.py`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.2.0/src/sdkgen_client.egg-info/PKG-INFO` & `sdkgen-client-0.2.1/src/sdkgen_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkgen-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDKgen is a powerful code generator to automatically build client SDKs for your REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/sdkgen-python
 Project-URL: Issues, https://github.com/apioo/sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkgen-client-0.2.0/src/sdkgen_client.egg-info/SOURCES.txt` & `sdkgen-client-0.2.1/src/sdkgen_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdkgen-client-0.2.0/tests/test_integration.py` & `sdkgen-client-0.2.1/tests/test_integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,62 +25,73 @@
         payload = self.new_payload()
         response = client.product().create(payload)
 
         self.assertEqual(response.headers["Authorization"], "Bearer my_token")
         self.assertEqual(response.headers["Accept"], "application/json")
         self.assertEqual(response.headers["User-Agent"], "SDKgen Client v1.0")
         self.assertEqual(response.method, "POST")
-        self.assertEqual(response.json.to_json(),
-                         '{"int": 1337, "float": 13.37, "string": "foobar", "bool": true, "array_scalar": ["foo", "bar"], "array_object": [{"id": 1, "name": "foo"}, {"id": 1, "name": "bar"}], "map_scalar": {"bar": "foo", "foo": "bar"}, "map_object": {"bar": {"id": 1, "name": "bar"}, "foo": {"id": 1, "name": "foo"}}, "object": {"id": 1, "name": "foo"}}')
+        self.assertEqual(response.json.model_dump_json(by_alias=True), '{"int":1337,"float":13.37,"string":"foobar","bool":true,"arrayScalar":["foo","bar"],"arrayObject":[{"id":1,"name":"foo"},{"id":1,"name":"bar"}],"mapScalar":{"bar":"foo","foo":"bar"},"mapObject":{"bar":{"id":1,"name":"bar"},"foo":{"id":1,"name":"foo"}},"object":{"id":1,"name":"foo"}}')
 
     def test_client_update(self):
         client = Client.build("my_token")
 
         payload = self.new_payload()
         response = client.product().update(1, payload)
 
         self.assertEqual(response.headers["Authorization"], "Bearer my_token")
         self.assertEqual(response.headers["Accept"], "application/json")
         self.assertEqual(response.headers["User-Agent"], "SDKgen Client v1.0")
         self.assertEqual(response.method, "PUT")
-        self.assertEqual(response.json.to_json(),
-                         '{"int": 1337, "float": 13.37, "string": "foobar", "bool": true, "array_scalar": ["foo", "bar"], "array_object": [{"id": 1, "name": "foo"}, {"id": 1, "name": "bar"}], "map_scalar": {"bar": "foo", "foo": "bar"}, "map_object": {"bar": {"id": 1, "name": "bar"}, "foo": {"id": 1, "name": "foo"}}, "object": {"id": 1, "name": "foo"}}')
+        self.assertEqual(response.json.model_dump_json(by_alias=True), '{"int":1337,"float":13.37,"string":"foobar","bool":true,"arrayScalar":["foo","bar"],"arrayObject":[{"id":1,"name":"foo"},{"id":1,"name":"bar"}],"mapScalar":{"bar":"foo","foo":"bar"},"mapObject":{"bar":{"id":1,"name":"bar"},"foo":{"id":1,"name":"foo"}},"object":{"id":1,"name":"foo"}}')
 
     def test_client_patch(self):
         client = Client.build("my_token")
 
         payload = self.new_payload()
         response = client.product().patch(1, payload)
 
         self.assertEqual(response.headers["Authorization"], "Bearer my_token")
         self.assertEqual(response.headers["Accept"], "application/json")
         self.assertEqual(response.headers["User-Agent"], "SDKgen Client v1.0")
         self.assertEqual(response.method, "PATCH")
-        self.assertEqual(response.json.to_json(),
-                         '{"int": 1337, "float": 13.37, "string": "foobar", "bool": true, "array_scalar": ["foo", "bar"], "array_object": [{"id": 1, "name": "foo"}, {"id": 1, "name": "bar"}], "map_scalar": {"bar": "foo", "foo": "bar"}, "map_object": {"bar": {"id": 1, "name": "bar"}, "foo": {"id": 1, "name": "foo"}}, "object": {"id": 1, "name": "foo"}}')
+        self.assertEqual(response.json.model_dump_json(by_alias=True), '{"int":1337,"float":13.37,"string":"foobar","bool":true,"arrayScalar":["foo","bar"],"arrayObject":[{"id":1,"name":"foo"},{"id":1,"name":"bar"}],"mapScalar":{"bar":"foo","foo":"bar"},"mapObject":{"bar":{"id":1,"name":"bar"},"foo":{"id":1,"name":"foo"}},"object":{"id":1,"name":"foo"}}')
 
     def test_client_delete(self):
         client = Client.build("my_token")
 
         response = client.product().delete(1)
 
         self.assertEqual(response.headers["Authorization"], "Bearer my_token")
         self.assertEqual(response.headers["Accept"], "application/json")
         self.assertEqual(response.headers["User-Agent"], "SDKgen Client v1.0")
         self.assertEqual(response.method, "DELETE")
         self.assertEqual(response.json, None)
 
     def new_payload(self) -> TestRequest:
-        object_foo = TestObject(1, "foo")
-        object_bar = TestObject(1, "bar")
+        object_foo = TestObject()
+        object_foo.id = 1
+        object_foo.name = "foo"
+        object_bar = TestObject()
+        object_bar.id = 1
+        object_bar.name = "bar"
 
         array_scalar = ["foo", "bar"]
         array_object = [object_foo, object_bar]
 
         map_scalar = {"foo": "bar", "bar": "foo"}
         map_object = {"foo": object_foo, "bar": object_bar}
 
-        return TestRequest(1337, 13.37, "foobar", True, array_scalar, array_object, map_scalar, map_object, object_foo)
+        request = TestRequest()
+        request.int_ = 1337
+        request.float_ = 13.37
+        request.string = "foobar"
+        request.bool_ = True
+        request.array_scalar = array_scalar
+        request.array_object = array_object
+        request.map_scalar = map_scalar
+        request.map_object = map_object
+        request.object = object_foo
+        return request
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sdkgen-client-0.2.0/tests/test_parser.py` & `sdkgen-client-0.2.1/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         self.assertEqual(parser.url("/foo/:bar", {"bar": True}), "https://api.acme.com/foo/1")
         self.assertEqual(parser.url("/foo/:bar", {"bar": False}), "https://api.acme.com/foo/0")
         self.assertEqual(parser.url("/foo/:bar", {"bar": "foo"}), "https://api.acme.com/foo/foo")
 
     def test_query(self):
         parser = Parser("https://api.acme.com/")
 
-        test = TestObject(None, "foo")
+        test = TestObject()
+        test.name = "foo"
 
         parameters = {
             "null": None,
             "int": 1337,
             "float": 13.37,
             "true": True,
             "false": False,
```

