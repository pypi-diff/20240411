# Comparing `tmp/jsonschema_markdown-0.3.4.tar.gz` & `tmp/jsonschema_markdown-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_markdown-0.3.4.tar", max compression
+gzip compressed data, was "jsonschema_markdown-0.3.5.tar", max compression
```

## Comparing `jsonschema_markdown-0.3.4.tar` & `jsonschema_markdown-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-04-04 23:32:25.139091 jsonschema_markdown-0.3.4/LICENSE
--rw-r--r--   0        0        0     2846 2024-04-04 23:32:25.139091 jsonschema_markdown-0.3.4/README.md
--rw-r--r--   0        0        0       81 2024-04-04 23:32:25.139091 jsonschema_markdown-0.3.4/jsonschema_markdown/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 23:32:25.139091 jsonschema_markdown-0.3.4/jsonschema_markdown/converter/__init__.py
--rw-r--r--   0        0        0    13790 2024-04-04 23:32:25.139091 jsonschema_markdown-0.3.4/jsonschema_markdown/converter/markdown.py
--rw-r--r--   0        0        0     1321 2024-04-04 23:32:25.143091 jsonschema_markdown-0.3.4/jsonschema_markdown/main.py
--rw-r--r--   0        0        0     1103 2024-04-04 23:32:25.143091 jsonschema_markdown-0.3.4/jsonschema_markdown/utils.py
--rw-r--r--   0        0        0     1340 2024-04-04 23:32:25.143091 jsonschema_markdown-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2846 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/README.md
+-rw-r--r--   0        0        0       81 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/converter/__init__.py
+-rw-r--r--   0        0        0    13815 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/converter/markdown.py
+-rw-r--r--   0        0        0     1321 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/main.py
+-rw-r--r--   0        0        0     1103 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/jsonschema_markdown/utils.py
+-rw-r--r--   0        0        0     1340 2024-04-11 15:45:33.615499 jsonschema_markdown-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.5/PKG-INFO
```

### Comparing `jsonschema_markdown-0.3.4/LICENSE` & `jsonschema_markdown-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.4/README.md` & `jsonschema_markdown-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.4/jsonschema_markdown/converter/markdown.py` & `jsonschema_markdown-0.3.5/jsonschema_markdown/converter/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,23 +115,25 @@
         logger.debug("Creating enum markdown")
         return create_enum_markdown(schema)
 
     if schema.get("const"):
         logger.debug("Creating const markdown")
         return create_const_markdown(schema)
 
-    if schema.get("properties"):
-        schema["properties"] = sort_properties(schema)
-
     markdown = ""
 
     # Add a warning before the table to indicate if additional properties are allowed
     if not schema.get("additionalProperties", True):
         markdown += "> ⚠️ Additional properties are not allowed.\n\n"
 
+    if not schema.get("properties"):
+        return markdown
+
+    schema["properties"] = sort_properties(schema)
+
     markdown += "| Property | Type | Required | Possible Values | Deprecated | Default | Description | Examples\n"
     markdown += "| -------- | ---- | -------- | --------------- | ---------- | ------- | ----------- | --------\n"
 
     for property_name, property_details in schema["properties"].items():
         property_type = property_details.get("type")
 
         logger.debug(f"Processing {property_name} of type {property_type}")
```

### Comparing `jsonschema_markdown-0.3.4/jsonschema_markdown/main.py` & `jsonschema_markdown-0.3.5/jsonschema_markdown/main.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.4/jsonschema_markdown/utils.py` & `jsonschema_markdown-0.3.5/jsonschema_markdown/utils.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.4/pyproject.toml` & `jsonschema_markdown-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "jsonschema-markdown"
 license = "MIT"
-version = "0.3.4"
+version = "0.3.5"
 description = "Export a JSON Schema document to Markdown documentation."
 authors = ["Elisiário Couto <elisiario@couto.io>"]
 repository = "https://github.com/elisiariocouto/jsonschema-markdown"
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
```

### Comparing `jsonschema_markdown-0.3.4/PKG-INFO` & `jsonschema_markdown-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.3.4
+Version: 0.3.5
 Summary: Export a JSON Schema document to Markdown documentation.
 Home-page: https://github.com/elisiariocouto/jsonschema-markdown
 License: MIT
 Keywords: jsonschema,markdown,documentation,docs,json
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.9,<4.0
```

