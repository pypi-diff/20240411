# Comparing `tmp/vtjson-1.6.7.tar.gz` & `tmp/vtjson-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.6.7.tar", last modified: Wed Apr 10 11:50:07 2024, max compression
+gzip compressed data, was "vtjson-1.6.8.tar", last modified: Wed Apr 10 21:46:58 2024, max compression
```

## Comparing `vtjson-1.6.7.tar` & `vtjson-1.6.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:50:07.681743 vtjson-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 11:50:01.000000 vtjson-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17264 2024-04-10 11:50:07.681743 vtjson-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-10 11:50:01.000000 vtjson-1.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-10 11:50:01.000000 vtjson-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:50:07.681743 vtjson-1.6.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:50:07.681743 vtjson-1.6.7/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17264 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24065 2024-04-10 11:50:01.000000 vtjson-1.6.7/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:46:58.600574 vtjson-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 21:46:54.000000 vtjson-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17961 2024-04-10 21:46:58.600574 vtjson-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-10 21:46:54.000000 vtjson-1.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-10 21:46:54.000000 vtjson-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:46:58.600574 vtjson-1.6.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:46:58.600574 vtjson-1.6.8/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17961 2024-04-10 21:46:58.000000 vtjson-1.6.8/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 21:46:58.000000 vtjson-1.6.8/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:46:58.000000 vtjson-1.6.8/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 21:46:58.000000 vtjson-1.6.8/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 21:46:58.000000 vtjson-1.6.8/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25215 2024-04-10 21:46:54.000000 vtjson-1.6.8/vtjson.py
```

### Comparing `vtjson-1.6.7/LICENSE` & `vtjson-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.7/PKG-INFO` & `vtjson-1.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.7
+Version: 1.6.8
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -315,14 +315,18 @@
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
+Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
+
+A: They did not seem to essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
 More generally one may use the pattern `intersect(schema, more_validations)` where the first argument makes sure that the object to be validated has the required layout to be an acceptable input for the later arguments. For example an ordered pair of integers can be validated using the schema
```

### Comparing `vtjson-1.6.7/README.md` & `vtjson-1.6.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,18 @@
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
+Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
+
+A: They did not seem to essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
 More generally one may use the pattern `intersect(schema, more_validations)` where the first argument makes sure that the object to be validated has the required layout to be an acceptable input for the later arguments. For example an ordered pair of integers can be validated using the schema
```

### Comparing `vtjson-1.6.7/pyproject.toml` & `vtjson-1.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.7/vtjson.egg-info/PKG-INFO` & `vtjson-1.6.8/vtjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.7
+Version: 1.6.8
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -315,14 +315,18 @@
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario. 
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
+Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
+
+A: They did not seem to essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
 More generally one may use the pattern `intersect(schema, more_validations)` where the first argument makes sure that the object to be validated has the required layout to be an acceptable input for the later arguments. For example an ordered pair of integers can be validated using the schema
```

### Comparing `vtjson-1.6.7/vtjson.py` & `vtjson-1.6.8/vtjson.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.6.7"
+__version__ = "1.6.8"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -369,36 +369,60 @@
         try:
             L = len(object)
         except Exception:
             return f"{name} (value:{_c(object)}) has no len()"
         return self.interval.__validate__(L, f"len({name})", strict)
 
 
-def compile(schema):
+class _deferred:
+    def __init__(self, collection, key):
+        if not isinstance(collection, dict):
+            raise SchemaError(f"{repr(collection)} is not a dictionary")
+        self.collection = collection
+        self.key = key
+
+    def __validate__(self, object, name, strict):
+        if self.key not in self.collection:
+            raise ValidationError(f"{name}: key {self.key} is unknown")
+        return self.collection[self.key].__validate__(object, name, strict)
+
+
+def compile(schema, _compiled_schemas={}):
+    id_ = id(schema)
+    # avoid infinite loop in case of a recursive schema
+    if id_ in _compiled_schemas:
+        compiled_schema = _compiled_schemas[id_]
+        if isinstance(compiled_schema, _deferred):
+            return compiled_schema
+    _compiled_schemas[id_] = _deferred(_compiled_schemas, id_)
     if isinstance(schema, type) and hasattr(schema, "__validate__"):
         try:
-            return schema()
+            ret = schema()
         except Exception:
             raise SchemaError(
                 f"{repr(schema.__name__)} does " f"not have a no-argument constructor"
             ) from None
     elif hasattr(schema, "__validate__"):
-        return schema
+        ret = schema
     elif isinstance(schema, type) or isinstance(schema, _GenericAlias):
-        return _type(schema)
+        ret = _type(schema)
     elif callable(schema):
-        return _callable(schema)
+        ret = _callable(schema)
     elif isinstance(schema, tuple) or isinstance(schema, list):
-        return _sequence(schema)
+        ret = _sequence(schema, _compiled_schemas=_compiled_schemas)
     elif isinstance(schema, dict):
-        return _dict(schema)
+        ret = _dict(schema, _compiled_schemas=_compiled_schemas)
     elif isinstance(schema, set):
-        return union(*schema)
+        ret = union(*schema)
     else:
-        return _object(schema)
+        if object is None:
+            raise Exception("object is None")
+        ret = _object(schema)
+    _compiled_schemas[id_] = ret
+    return ret
 
 
 def _validate(schema, object, name="object", strict=True):
     schema = compile(schema)
     return schema.__validate__(object, name=name, strict=strict)
 
 
@@ -626,18 +650,18 @@
         for c in self.conditions:
             if c[0].__validate__(object, name, strict) == "":
                 return c[1].__validate__(object, name, strict)
         return ""
 
 
 class _dict:
-    def __init__(self, schema):
+    def __init__(self, schema, _compiled_schemas={}):
         self.schema = collections.OrderedDict()
         for k, v in schema.items():
-            self.schema[k] = compile(v)
+            self.schema[k] = compile(v, _compiled_schemas=_compiled_schemas)
         self.keys = _keys(self.schema)
         self.keys2 = _keys2(self.schema)
 
     def __validate__(self, object, name, strict):
         if type(object) is not dict:
             return _wrong_type_message(object, name, type(self.schema).__name__)
         for k_, k, o in self.keys2:
@@ -678,17 +702,20 @@
             return f"{self.schema} is not a valid type: {str(e)}"
 
     def __str__(self):
         return self.schema.__name__
 
 
 class _sequence:
-    def __init__(self, schema):
+    def __init__(self, schema, _compiled_schemas={}):
         self.type_schema = type(schema)
-        self.schema = [compile(o) if o is not ... else ... for o in schema]
+        self.schema = [
+            compile(o, _compiled_schemas=_compiled_schemas) if o is not ... else ...
+            for o in schema
+        ]
         if len(schema) > 0 and schema[-1] is ...:
             if len(schema) >= 2:
                 self.fill = self.schema[-2]
                 self.schema = self.schema[:-2]
             else:
                 self.fill = _type(object)
                 self.schema = []
```

