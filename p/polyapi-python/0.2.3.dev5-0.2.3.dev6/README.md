# Comparing `tmp/polyapi-python-0.2.3.dev5.tar.gz` & `tmp/polyapi-python-0.2.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi-python-0.2.3.dev5.tar", last modified: Tue Apr  9 19:29:34 2024, max compression
+gzip compressed data, was "polyapi-python-0.2.3.dev6.tar", last modified: Thu Apr 11 15:28:35 2024, max compression
```

## Comparing `polyapi-python-0.2.3.dev5.tar` & `polyapi-python-0.2.3.dev6.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.820026 polyapi-python-0.2.3.dev5/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 19:29:34.000000 polyapi-python-0.2.3.dev5/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:29:34.824026 polyapi-python-0.2.3.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:29:34.820026 polyapi-python-0.2.3.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 19:29:27.000000 polyapi-python-0.2.3.dev5/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:28:35.194869 polyapi-python-0.2.3.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-11 15:28:35.194869 polyapi-python-0.2.3.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:28:35.194869 polyapi-python-0.2.3.dev6/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:28:35.194869 polyapi-python-0.2.3.dev6/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-11 15:28:35.000000 polyapi-python-0.2.3.dev6/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-11 15:28:35.000000 polyapi-python-0.2.3.dev6/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:28:35.000000 polyapi-python-0.2.3.dev6/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 15:28:35.000000 polyapi-python-0.2.3.dev6/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 15:28:35.000000 polyapi-python-0.2.3.dev6/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:28:35.194869 polyapi-python-0.2.3.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:28:35.194869 polyapi-python-0.2.3.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-11 15:28:31.000000 polyapi-python-0.2.3.dev6/tests/test_variables.py
```

### Comparing `polyapi-python-0.2.3.dev5/LICENSE` & `polyapi-python-0.2.3.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/PKG-INFO` & `polyapi-python-0.2.3.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev5
+Version: 0.2.3.dev6
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi-python-0.2.3.dev5/README.md` & `polyapi-python-0.2.3.dev6/README.md`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/api.py` & `polyapi-python-0.2.3.dev6/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/auth.py` & `polyapi-python-0.2.3.dev6/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/cli.py` & `polyapi-python-0.2.3.dev6/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/config.py` & `polyapi-python-0.2.3.dev6/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/error_handler.py` & `polyapi-python-0.2.3.dev6/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/execute.py` & `polyapi-python-0.2.3.dev6/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/function_cli.py` & `polyapi-python-0.2.3.dev6/polyapi/function_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,16 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("subcommand", choices=["add"])
     parser.add_argument("function_name")
     parser.add_argument("filename")
     args = parser.parse_args(subcommands)
 
     verb = "Updating" if _func_already_exists(context, args.function_name) else "Adding"
-    print(f"{verb} custom server side function...", end="")
+    ftype = "server" if server else "client"
+    print(f"{verb} custom {ftype} function...", end="")
 
     with open(args.filename, "r") as f:
         code = f.read()
 
     # OK! let's parse the code and generate the arguments
     (
         arguments,
@@ -198,37 +199,36 @@
     ) = _parse_code(code, args.function_name)
 
     if not return_type:
         print_red("ERROR")
         print(f"Function {args.function_name} not found as top-level function in {args.filename}")
         sys.exit(1)
 
-    if requirements:
-        print_yellow('\nPlease note that deploying your functions will take a few minutes because it makes use of libraries other than polyapi.')
-
     data = {
         "context": context,
         "name": args.function_name,
         "description": description,
         "code": code,
         "language": "python",
         "returnType": return_type,
         "returnTypeSchema": return_type_schema,
-        "requirements": requirements,
         "arguments": arguments,
         "logsEnabled": logs_enabled,
     }
 
+    if server and requirements:
+        print_yellow('\nPlease note that deploying your functions will take a few minutes because it makes use of libraries other than polyapi.')
+        data["requirements"] = requirements
+
     api_key, api_url = get_api_key_and_url()
     assert api_key
     if server:
         url = f"{api_url}/functions/server"
     else:
-        raise NotImplementedError("Client functions not yet implemented.")
-        # url = f"{base_url}/functions/client"
+        url = f"{api_url}/functions/client"
 
     headers = get_auth_headers(api_key)
     resp = requests.post(url, headers=headers, json=data)
     if resp.status_code == 201:
         print_green("DEPLOYED")
         function_id = resp.json()["id"]
         print(f"Function ID: {function_id}")
```

### Comparing `polyapi-python-0.2.3.dev5/polyapi/generate.py` & `polyapi-python-0.2.3.dev6/polyapi/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import json
 import requests
 import os
 import shutil
-from typing import Any, Dict, List, Tuple
+from typing import List
 
 from polyapi.auth import render_auth_function
+from polyapi.client import render_client_function
 from polyapi.execute import execute_post
 from polyapi.webhook import render_webhook_handle
 
 from .typedefs import PropertySpecification, SpecificationDto, VariableSpecDto
 from .api import render_api_function
 from .server import render_server_function
 from .utils import add_import_to_init, get_auth_headers, init_the_init
 from .variables import generate_variables
 from .config import get_api_key_and_url, initialize_config
 
 SUPPORTED_FUNCTION_TYPES = {
     "apiFunction",
     "authFunction",
+    "customFunction",
     "serverFunction",
     "webhookHandle",
 }
 
 SUPPORTED_TYPES = SUPPORTED_FUNCTION_TYPES | {"serverVariable"}
 
 
@@ -34,40 +36,37 @@
     if resp.status_code == 200:
         return resp.json()
     else:
         raise NotImplementedError(resp.content)
 
 
 def parse_function_specs(
-    specs: List, limit_ids: List[str] | None  # optional list of ids to limit to
-) -> List[Tuple[str, str, str, str, List[PropertySpecification], Dict[str, Any]]]:
+    specs: List[SpecificationDto],
+    limit_ids: List[str] | None,  # optional list of ids to limit to
+) -> List[SpecificationDto]:
     functions = []
     for spec in specs:
+        if not spec or "function" not in spec:
+            continue
+
+        if not spec["function"]:
+            continue
+
         if limit_ids and spec["id"] not in limit_ids:
             continue
 
         if spec["type"] not in SUPPORTED_FUNCTION_TYPES:
             continue
 
-        function_type = spec["type"]
-        function_name = f"poly.{spec['context']}.{spec['name']}"
-        function_id = spec["id"]
-        arguments: List[PropertySpecification] = [
-            arg for arg in spec["function"]["arguments"]
-        ]
-        functions.append(
-            (
-                function_type,
-                function_name,
-                function_id,
-                spec["description"],
-                arguments,
-                spec["function"]["returnType"],
-            )
-        )
+        if spec["type"] == "customFunction" and spec["language"] != "python":
+            # poly libraries only support client functions of same language
+            continue
+
+        functions.append(spec)
+
     return functions
 
 
 def cache_specs(specs: List[SpecificationDto]):
     supported = []
     for spec in specs:
         # this needs to stay in sync with logic in parse_specs
@@ -86,19 +85,18 @@
 def read_cached_specs() -> List[SpecificationDto]:
     full_path = os.path.dirname(os.path.abspath(__file__))
     full_path = os.path.join(full_path, "poly")
     with open(os.path.join(full_path, "specs.json"), "r") as f:
         return json.loads(f.read())
 
 
-def get_functions_and_parse(limit_ids: List[str] | None = None):
+def get_functions_and_parse(limit_ids: List[str] | None = None) -> List[SpecificationDto]:
     specs = get_specs()
     cache_specs(specs)
-    functions = parse_function_specs(specs, limit_ids=limit_ids)
-    return functions
+    return parse_function_specs(specs, limit_ids=limit_ids)
 
 
 def get_variables() -> List[VariableSpecDto]:
     api_key, api_url = get_api_key_and_url()
     headers = {"Authorization": f"Bearer {api_key}"}
     # TODO do some caching so this and get_functions just do 1 function call
     url = f"{api_url}/specs"
@@ -158,50 +156,56 @@
 
 def save_rendered_specs() -> None:
     specs = read_cached_specs()
     # right now we just support rendered apiFunctions
     api_specs = [spec for spec in specs if spec["type"] == "apiFunction"]
     for spec in api_specs:
         assert spec["function"]
-        func_str, type_defs = render_spec(
-            spec["type"],
-            spec["name"],
-            spec["id"],
-            spec["description"],
-            spec["function"]["arguments"],
-            spec["function"]["returnType"],
-        )
+        func_str, type_defs = render_spec(spec)
         data = {
             "language": "python",
             "apiFunctionId": spec["id"],
             "signature": func_str,
             "typedefs": type_defs,
         }
         resp = execute_post("/functions/rendered-specs", data)
         print("adding", spec["context"], spec["name"])
         assert resp.status_code == 201, (resp.text, resp.status_code)
 
 
-def render_spec(
-    function_type: str,
-    function_name: str,
-    function_id: str,
-    function_description: str,
-    arguments: List[PropertySpecification],
-    return_type: Dict[str, Any],
-):
+def render_spec(spec: SpecificationDto):
+    function_type = spec["type"]
+    function_description = spec["description"]
+    function_name = spec["name"]
+    function_id = spec["id"]
+
+    arguments: List[PropertySpecification] = []
+    return_type = {}
+    if spec["function"]:
+        arguments = [
+            arg for arg in spec["function"]["arguments"]
+        ]
+        return_type = spec["function"]["returnType"]
+
     if function_type == "apiFunction":
         func_str, func_type_defs = render_api_function(
             function_type,
             function_name,
             function_id,
             function_description,
             arguments,
             return_type,
         )
+    elif function_type == "customFunction":
+        func_str, func_type_defs = render_client_function(
+            function_name,
+            spec["code"],
+            arguments,
+            return_type,
+        )
     elif function_type == "serverFunction":
         func_str, func_type_defs = render_server_function(
             function_type,
             function_name,
             function_id,
             function_description,
             arguments,
@@ -225,80 +229,56 @@
             arguments,
             return_type,
         )
     return func_str, func_type_defs
 
 
 def add_function_file(
-    function_type: str,
     full_path: str,
     function_name: str,
-    function_id: str,
-    function_description: str,
-    arguments: List[PropertySpecification],
-    return_type: Dict[str, Any],
+    spec: SpecificationDto,
 ):
     # first lets add the import to the __init__
     init_the_init(full_path)
 
-    func_str, func_type_defs = render_spec(
-        function_type,
-        function_name,
-        function_id,
-        function_description,
-        arguments,
-        return_type,
-    )
+    func_str, func_type_defs = render_spec(spec)
 
     if func_str:
         # add function to init
         init_path = os.path.join(full_path, "__init__.py")
         with open(init_path, "a") as f:
             f.write(f"\n\nfrom . import _{function_name}\n\n{func_str}")
 
         # add type_defs to underscore file
         file_path = os.path.join(full_path, f"_{function_name}.py")
         with open(file_path, "w") as f:
             f.write(func_type_defs)
 
 
 def create_function(
-    function_type: str,
-    path: str,
-    function_id: str,
-    function_description: str,
-    arguments: List[PropertySpecification],
-    return_type: Dict[str, Any],
+    spec: SpecificationDto
 ) -> None:
     full_path = os.path.dirname(os.path.abspath(__file__))
-
-    folders = path.split(".")
+    folders = f"poly.{spec['context']}.{spec['name']}".split(".")
     for idx, folder in enumerate(folders):
         if idx + 1 == len(folders):
             # special handling for final level
             add_function_file(
-                function_type,
                 full_path,
                 folder,
-                function_id,
-                function_description,
-                arguments,
-                return_type,
+                spec,
             )
         else:
             full_path = os.path.join(full_path, folder)
             if not os.path.exists(full_path):
                 os.makedirs(full_path)
 
             # append to __init__.py file if nested folders
             next = folders[idx + 1] if idx + 2 < len(folders) else ""
             if next:
                 init_the_init(full_path)
                 add_import_to_init(full_path, next)
 
 
-# TODO create the socket and pass to create_function?
-
-
-def generate_functions(functions: List) -> None:
+def generate_functions(functions: List[SpecificationDto]) -> None:
     for func in functions:
-        create_function(*func)
+        create_function(func)
```

### Comparing `polyapi-python-0.2.3.dev5/polyapi/schema.py` & `polyapi-python-0.2.3.dev6/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/server.py` & `polyapi-python-0.2.3.dev6/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/typedefs.py` & `polyapi-python-0.2.3.dev6/polyapi/typedefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 
 
 class SpecificationDto(TypedDict):
     id: str
     context: str
     name: str
     description: str
-    # function is none if this is actually VariableSpecDto
-    function: FunctionSpecification | None
+    # function is none (or function key not present) if this is actually VariableSpecDto
+    function: NotRequired[FunctionSpecification | None]
     type: Literal['apiFunction', 'customFunction', 'serverFunction', 'authFunction', 'webhookHandle', 'serverVariable']
+    code: NotRequired[str]
+    language: str
 
 
 class VariableSpecification(TypedDict):
     environmentId: str
     value: Any
     valueType: PropertyType
     secret: bool
```

### Comparing `polyapi-python-0.2.3.dev5/polyapi/utils.py` & `polyapi-python-0.2.3.dev6/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/variables.py` & `polyapi-python-0.2.3.dev6/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi/webhook.py` & `polyapi-python-0.2.3.dev6/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/polyapi_python.egg-info/PKG-INFO` & `polyapi-python-0.2.3.dev6/polyapi_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.3.dev5
+Version: 0.2.3.dev6
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi-python-0.2.3.dev5/polyapi_python.egg-info/SOURCES.txt` & `polyapi-python-0.2.3.dev6/polyapi_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 polyapi/__init__.py
 polyapi/__main__.py
 polyapi/api.py
 polyapi/auth.py
 polyapi/cli.py
+polyapi/client.py
 polyapi/config.py
 polyapi/constants.py
 polyapi/error_handler.py
 polyapi/exceptions.py
 polyapi/execute.py
 polyapi/function_cli.py
 polyapi/generate.py
```

### Comparing `polyapi-python-0.2.3.dev5/pyproject.toml` & `polyapi-python-0.2.3.dev6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.3.dev5"
+version = "0.2.3.dev6"
 description = "The PolyAPI Python Client"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi-python-0.2.3.dev5/tests/test_api.py` & `polyapi-python-0.2.3.dev6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/tests/test_auth.py` & `polyapi-python-0.2.3.dev6/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/tests/test_function_cli.py` & `polyapi-python-0.2.3.dev6/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/tests/test_server.py` & `polyapi-python-0.2.3.dev6/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/tests/test_utils.py` & `polyapi-python-0.2.3.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi-python-0.2.3.dev5/tests/test_variables.py` & `polyapi-python-0.2.3.dev6/tests/test_variables.py`

 * *Files identical despite different names*

