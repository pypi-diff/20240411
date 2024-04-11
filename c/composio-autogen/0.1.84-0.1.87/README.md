# Comparing `tmp/composio_autogen-0.1.84.tar.gz` & `tmp/composio_autogen-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.84.tar", last modified: Sun Apr  7 19:53:11 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.87.tar", last modified: Thu Apr 11 12:40:44 2024, max compression
```

## Comparing `composio_autogen-0.1.84.tar` & `composio_autogen-0.1.87.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:53:11.096268 composio_autogen-0.1.84/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 19:53:11.096084 composio_autogen-0.1.84/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.84/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:53:11.094335 composio_autogen-0.1.84/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.84/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7468 2024-04-07 18:28:35.000000 composio_autogen-0.1.84/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:53:11.095856 composio_autogen-0.1.84/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-07 19:52:16.000000 composio_autogen-0.1.84/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 19:53:11.096319 composio_autogen-0.1.84/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-07 19:52:16.000000 composio_autogen-0.1.84/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:44.401886 composio_autogen-0.1.87/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 12:40:44.401695 composio_autogen-0.1.87/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.87/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:44.400518 composio_autogen-0.1.87/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.87/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     8397 2024-04-11 12:39:00.000000 composio_autogen-0.1.87/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:44.401485 composio_autogen-0.1.87/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 12:39:53.000000 composio_autogen-0.1.87/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 12:40:44.401931 composio_autogen-0.1.87/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-11 12:39:53.000000 composio_autogen-0.1.87/setup.py
```

### Comparing `composio_autogen-0.1.84/PKG-INFO` & `composio_autogen-0.1.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.84
+Version: 0.1.87
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.84
+Requires-Dist: composio_core===0.1.87
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.84/README.md` & `composio_autogen-0.1.87/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.84/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.87/composio_autogen/autogen_toolspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import types
 import logging
+import hashlib
 from inspect import Parameter, Signature
 from typing import Union, List, Annotated
 
 import autogen
 from composio import ComposioCore, App, Action, FrameworkEnum
 from pydantic import create_model, Field
 from autogen.agentchat.conversable_agent import ConversableAgent
@@ -50,54 +51,56 @@
                                                                              prop_title))
                                     ))
         else:
             optional_fields[prop_name] = (signature_prop_type, 
                                 Field(title=prop_title, 
                                     default=prop_default
                                     ))
+
     fieldModel = create_model(param_title, **required_fields, **optional_fields)
     return fieldModel
-        
-
     
 
-def get_signature_format_from_schema_params(
-        schema_params
-):
+def get_signature_format_from_schema_params(schema_params):
     required_parameters = []
     optional_parameters = []
-    required_params = schema_params.get('required', [])
 
+    required_params = schema_params.get('required', [])
     for param_name, param_schema in schema_params.get('properties', {}).items():
-        param_type = param_schema['type']
-        param_title = param_schema['title'].replace(" ", "")
+        try:
+            param_type = param_schema['type']
 
-        if param_type in schema_type_python_type_dict:
-            signature_param_type = schema_type_python_type_dict[param_type]
-        else:
-            signature_param_type = pydantic_model_from_param_schema(param_schema)
+            param_title = param_schema['title'].replace(" ", "")
 
-        param_default = param_schema.get('default', fallback_values[param_type])
-        param_annotation = Annotated[signature_param_type, param_schema.get('description', 
-                                                                            param_schema.get('desc',
-                                                                                             param_title))]
-        param = Parameter(
-            name=param_name,
-            kind=Parameter.POSITIONAL_OR_KEYWORD,
-            annotation=param_annotation,
-            default=Parameter.empty if param_name in required_params else param_default 
-        )
-
-        is_required = param_name in required_params
-        if is_required:
-            required_parameters.append(param)
-        else:
-            optional_parameters.append(param)
+            if param_type in schema_type_python_type_dict:
+                signature_param_type = schema_type_python_type_dict[param_type]
+            else:
+                signature_param_type = pydantic_model_from_param_schema(param_schema)
+
+            param_default = param_schema.get('default', fallback_values[param_type])
+            param_annotation = Annotated[signature_param_type, param_schema.get('description', 
+                                                                                param_schema.get('desc',
+                                                                                                param_title))]
+            is_required = param_name in required_params
+            param = Parameter(
+                name=param_name,
+                kind=Parameter.POSITIONAL_OR_KEYWORD,
+                annotation=param_annotation,
+                default=Parameter.empty if param_name in required_params else param_default 
+            )
+            if is_required:
+                required_parameters.append(param)
+            else :
+                optional_parameters.append(param)
+        except Exception as e:
+            logger.error(f"Error while processing param {param_name} with schema {param_schema}")
+            pass
     return required_parameters + optional_parameters
 
+
 class ComposioToolset:
     def __init__(self, caller = None, executor = None):
         self.caller = caller
         self.executor = executor
         self.client =  ComposioCore(framework=FrameworkEnum.AUTOGEN)
 
 
@@ -140,40 +143,52 @@
                                                 actions=actions)
         
         for schema in action_schemas:
             self._register_schema_to_autogen(action_schema=schema,
                                             caller = caller if caller else self.caller,
                                             executor = executor if executor else self.executor)
 
-
+    def process_function_name_for_registration(self, input_string, max_allowed_length = 64, num_hash_char = 10):
+        hash_obj = hashlib.sha256(input_string.encode())
+        hash_hex = hash_obj.hexdigest()
+        
+        num_input_str_char = max_allowed_length - (num_hash_char + 1)
+        hash_chars_to_attach = hash_hex[:10]
+        input_str_to_attach = input_string[-num_input_str_char:]
+        processed_name = input_str_to_attach + "_" + hash_chars_to_attach
+        
+        return processed_name
+    
     def _register_schema_to_autogen(self, 
                                     action_schema, 
                                     caller: ConversableAgent,
                                     executor: ConversableAgent):
 
         name = action_schema["name"]
+        processed_name = self.process_function_name_for_registration(name)
         appName = action_schema["appName"]
         description = action_schema["description"]
 
         parameters = get_signature_format_from_schema_params(
                                             action_schema["parameters"])
         action_signature = Signature(parameters=parameters)
         
-        placeholder_function = lambda **kwargs: self.client.execute_action(
-                                                    self.client.get_action_enum(name, appName), 
-                                                    kwargs)
+        def placeholder_function(**kwargs):
+            return self.client.execute_action(
+                        self.client.get_action_enum(name, appName), 
+                        kwargs)
         action_func = types.FunctionType(
                                     placeholder_function.__code__, 
                                     globals=globals(), 
-                                    name=name, 
+                                    name=processed_name, 
                                     closure=placeholder_function.__closure__
                           )
         action_func.__signature__ = action_signature
-        action_func.__doc__ = description
+        action_func.__doc__ = description if description else f"Action {name} from {appName}"
 
         autogen.agentchat.register_function(
             action_func,
             caller=caller,
             executor=executor,
-            name=name,
-            description=description
+            name=processed_name,
+            description=description if description else f"Action {name} from {appName}"
         )
```

### Comparing `composio_autogen-0.1.84/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.87/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.84
+Version: 0.1.87
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.84
+Requires-Dist: composio_core===0.1.87
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.84/setup.py` & `composio_autogen-0.1.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.84",
+    version="0.1.87",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

