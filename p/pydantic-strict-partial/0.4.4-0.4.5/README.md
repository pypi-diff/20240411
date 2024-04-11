# Comparing `tmp/pydantic_strict_partial-0.4.4.tar.gz` & `tmp/pydantic_strict_partial-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_strict_partial-0.4.4.tar", max compression
+gzip compressed data, was "pydantic_strict_partial-0.4.5.tar", max compression
```

## Comparing `pydantic_strict_partial-0.4.4.tar` & `pydantic_strict_partial-0.4.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/LICENSE
--rw-r--r--   0        0        0     2073 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/README.md
--rw-r--r--   0        0        0     1182 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/pydantic_strict_partial/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 23:48:47.596517 pydantic_strict_partial-0.4.4/pydantic_strict_partial/py.typed
--rw-r--r--   0        0        0     5163 2024-04-10 23:48:48.584518 pydantic_strict_partial-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 pydantic_strict_partial-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-11 00:14:31.162708 pydantic_strict_partial-0.4.5/LICENSE
+-rw-r--r--   0        0        0     2423 2024-04-11 00:14:31.162708 pydantic_strict_partial-0.4.5/README.md
+-rw-r--r--   0        0        0     1182 2024-04-11 00:14:31.162708 pydantic_strict_partial-0.4.5/pydantic_strict_partial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:14:31.162708 pydantic_strict_partial-0.4.5/pydantic_strict_partial/py.typed
+-rw-r--r--   0        0        0     5163 2024-04-11 00:14:32.290692 pydantic_strict_partial-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3209 1970-01-01 00:00:00.000000 pydantic_strict_partial-0.4.5/PKG-INFO
```

### Comparing `pydantic_strict_partial-0.4.4/LICENSE` & `pydantic_strict_partial-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_strict_partial-0.4.4/README.md` & `pydantic_strict_partial-0.4.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -54,10 +54,22 @@
 }
 
 UserPartialUpdateSchema(name=None)  # raises ValidationError
 UserPartialUpdateSchema(age=17)  # raises ValidationError
 
 ```
 
+## Known limitations
+
+#### MyPy: "is not valid as a type" error
+
+You may be faced with `Variable "UserPartialUpdateSchema" is not valid as a type` error.
+There is no good solution for that. But the next approach can be used as a workaround: 
+
+```py
+class UserPartialUpdateSchema(create_partial_model(UserSchema)):  # type: ignore[misc]
+    pass
+```
+
 ## Alternatives
 
 [pydantic-partial](https://github.com/team23/pydantic-partial) - it makes all fields nullable and disables all validators, which is not suitable for payload validation on `PATCH` endpoints.
```

### Comparing `pydantic_strict_partial-0.4.4/pydantic_strict_partial/__init__.py` & `pydantic_strict_partial-0.4.5/pydantic_strict_partial/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_strict_partial-0.4.4/pyproject.toml` & `pydantic_strict_partial-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-strict-partial"
-version = "0.4.4"
+version = "0.4.5"
 description = "Makes partial Pydantic models without making fields nullable."
 authors = ["Adrian Dankiv <adr-007@ukr.net>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "partial", "fastapi"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pydantic_strict_partial-0.4.4/PKG-INFO` & `pydantic_strict_partial-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-strict-partial
-Version: 0.4.4
+Version: 0.4.5
 Summary: Makes partial Pydantic models without making fields nullable.
 Home-page: https://github.com/ADR-007/pydantic-strict-partial
 License: MIT
 Keywords: pydantic,partial,fastapi
 Author: Adrian Dankiv
 Author-email: adr-007@ukr.net
 Requires-Python: >=3.10,<4.0
@@ -75,11 +75,23 @@
 }
 
 UserPartialUpdateSchema(name=None)  # raises ValidationError
 UserPartialUpdateSchema(age=17)  # raises ValidationError
 
 ```
 
+## Known limitations
+
+#### MyPy: "is not valid as a type" error
+
+You may be faced with `Variable "UserPartialUpdateSchema" is not valid as a type` error.
+There is no good solution for that. But the next approach can be used as a workaround: 
+
+```py
+class UserPartialUpdateSchema(create_partial_model(UserSchema)):  # type: ignore[misc]
+    pass
+```
+
 ## Alternatives
 
 [pydantic-partial](https://github.com/team23/pydantic-partial) - it makes all fields nullable and disables all validators, which is not suitable for payload validation on `PATCH` endpoints.
```

