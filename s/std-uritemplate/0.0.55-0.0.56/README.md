# Comparing `tmp/std_uritemplate-0.0.55.tar.gz` & `tmp/std_uritemplate-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_uritemplate-0.0.55.tar", max compression
+gzip compressed data, was "std_uritemplate-0.0.56.tar", max compression
```

## Comparing `std_uritemplate-0.0.55.tar` & `std_uritemplate-0.0.56.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7597 2024-03-18 11:24:54.203862 std_uritemplate-0.0.55/Readme.md
--rw-r--r--   0        0        0      748 2024-03-18 11:24:54.491862 std_uritemplate-0.0.55/pyproject.toml
--rw-r--r--   0        0        0    15222 2024-03-18 11:24:41.507821 std_uritemplate-0.0.55/stduritemplate/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 11:24:41.507821 std_uritemplate-0.0.55/stduritemplate/py.typed
--rw-r--r--   0        0        0     8418 1970-01-01 00:00:00.000000 std_uritemplate-0.0.55/PKG-INFO
+-rw-r--r--   0        0        0     7597 2024-04-11 09:18:19.242291 std_uritemplate-0.0.56/Readme.md
+-rw-r--r--   0        0        0      748 2024-04-11 09:18:19.550290 std_uritemplate-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0    15222 2024-04-11 09:18:05.254332 std_uritemplate-0.0.56/stduritemplate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:18:05.254332 std_uritemplate-0.0.56/stduritemplate/py.typed
+-rw-r--r--   0        0        0     8418 1970-01-01 00:00:00.000000 std_uritemplate-0.0.56/PKG-INFO
```

### Comparing `std_uritemplate-0.0.55/Readme.md` & `std_uritemplate-0.0.56/Readme.md`

 * *Files identical despite different names*

### Comparing `std_uritemplate-0.0.55/pyproject.toml` & `std_uritemplate-0.0.56/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "std-uritemplate"
-version = "0.0.55"
+version = "0.0.56"
 description = "std-uritemplate implementation for Python"
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "Readme.md"
 packages = [{include = "stduritemplate"}]
 exclude = [
     { path = "stduritemplate/__pycache__", format=["sdist", "wheel"] },
 ]
```

### Comparing `std_uritemplate-0.0.55/stduritemplate/__init__.py` & `std_uritemplate-0.0.56/stduritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `std_uritemplate-0.0.55/PKG-INFO` & `std_uritemplate-0.0.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std-uritemplate
-Version: 0.0.55
+Version: 0.0.56
 Summary: std-uritemplate implementation for Python
 Home-page: https://github.com/std-uritemplate/std-uritemplate
 License: Apache 2.0
 Keywords: std-uritemplate,uritemplate,uritemplates,stduritemplate
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.8,<4.0
```

