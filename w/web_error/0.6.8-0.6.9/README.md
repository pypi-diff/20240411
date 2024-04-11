# Comparing `tmp/web_error-0.6.8.tar.gz` & `tmp/web_error-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_error-0.6.8.tar", max compression
+gzip compressed data, was "web_error-0.6.9.tar", max compression
```

## Comparing `web_error-0.6.8.tar` & `web_error-0.6.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11307 2024-03-12 13:44:17.481603 web_error-0.6.8/LICENSE
--rw-r--r--   0        0        0     5090 2024-03-12 13:44:17.481603 web_error-0.6.8/README.md
--rw-r--r--   0        0        0     2128 2024-03-12 13:44:17.481603 web_error-0.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/__init__.py
--rw-r--r--   0        0        0      220 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/cors.py
--rw-r--r--   0        0        0     4204 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/error.py
--rw-r--r--   0        0        0        0 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/handler/__init__.py
--rw-r--r--   0        0        0     4546 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/handler/fastapi.py
--rw-r--r--   0        0        0     6121 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/handler/starlette.py
--rw-r--r--   0        0        0      297 2024-03-12 13:44:17.481603 web_error-0.6.8/web_error/handler/util.py
--rw-r--r--   0        0        0     5763 1970-01-01 00:00:00.000000 web_error-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-03-12 14:03:46.518997 web_error-0.6.9/LICENSE
+-rw-r--r--   0        0        0     5090 2024-03-12 14:03:46.518997 web_error-0.6.9/README.md
+-rw-r--r--   0        0        0     2128 2024-03-12 14:03:46.522997 web_error-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/__init__.py
+-rw-r--r--   0        0        0      220 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/cors.py
+-rw-r--r--   0        0        0     4202 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/error.py
+-rw-r--r--   0        0        0        0 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/handler/__init__.py
+-rw-r--r--   0        0        0     4546 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/handler/fastapi.py
+-rw-r--r--   0        0        0     6121 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/handler/starlette.py
+-rw-r--r--   0        0        0      297 2024-03-12 14:03:46.522997 web_error-0.6.9/web_error/handler/util.py
+-rw-r--r--   0        0        0     5763 1970-01-01 00:00:00.000000 web_error-0.6.9/PKG-INFO
```

### Comparing `web_error-0.6.8/LICENSE` & `web_error-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web_error-0.6.8/README.md` & `web_error-0.6.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Web Errors v0.6.8
+# Web Errors v0.6.9
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/NRWLDev/web-error/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/web-error/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/web-error/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/web-error)
```

### Comparing `web_error-0.6.8/pyproject.toml` & `web_error-0.6.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web_error"
-version = "0.6.8"
+version = "0.6.9"
 description = "Web based error utils"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/web-error/"
 homepage="https://github.com/EdgyEdgemond/web-error/"
 readme = "README.md"
 
@@ -23,15 +23,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.6.8"
+current_version = "0.6.9"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "README.md"
 
 [[tool.bumpversion.files]]
```

### Comparing `web_error-0.6.8/web_error/error.py` & `web_error-0.6.9/web_error/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             DeprecationWarning,
             stacklevel=2,
         )
         return self.details
 
     @property
     def type(self: t.Self) -> str:
-        type_ = "".join(self.__class__.__name__.rreplace("Error", 1))
+        type_ = "".join(self.__class__.__name__.rsplit("Error", 1))
         type_ = CONVERT_RE.sub("-", type_).lower()
         return self._code if self._code else type_
 
     def marshal(self: t.Self, *, strip_debug: bool = False, legacy: bool = False) -> dict[str, t.Any]:
         """Generate a JSON compatible representation.
 
         Args:
```

### Comparing `web_error-0.6.8/web_error/handler/fastapi.py` & `web_error-0.6.9/web_error/handler/fastapi.py`

 * *Files identical despite different names*

### Comparing `web_error-0.6.8/web_error/handler/starlette.py` & `web_error-0.6.9/web_error/handler/starlette.py`

 * *Files identical despite different names*

### Comparing `web_error-0.6.8/PKG-INFO` & `web_error-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web_error
-Version: 0.6.8
+Version: 0.6.9
 Summary: Web based error utils
 Home-page: https://github.com/EdgyEdgemond/web-error/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/EdgyEdgemond/web-error/
 Description-Content-Type: text/markdown
 
-# Web Errors v0.6.8
+# Web Errors v0.6.9
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/NRWLDev/web-error/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/web-error/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/web-error/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/web-error)
```

