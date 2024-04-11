# Comparing `tmp/apoplast-2.0.1.tar.gz` & `tmp/apoplast-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apoplast-2.0.1.tar", max compression
+gzip compressed data, was "apoplast-2.0.2.tar", max compression
```

## Comparing `apoplast-2.0.1.tar` & `apoplast-2.0.2.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0      640 2024-04-11 20:20:04.967018 apoplast-2.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.1/readme.md
--rw-r--r--   0        0        0       21 2024-04-11 20:17:16.500712 apoplast-2.0.1/venues/stages/apoplast/__init__.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 apoplast-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      676 2024-04-11 20:22:11.425870 apoplast-2.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.2/readme.md
+-rw-r--r--   0        0        0       21 2024-04-11 20:17:16.500712 apoplast-2.0.2/venues/stages/apoplast/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-11 20:20:40.718700 apoplast-2.0.2/venues/stages/apoplast/apoplast.S.HTML
+-rw-r--r--   0        0        0       24 2024-04-11 20:21:27.086280 apoplast-2.0.2/venues/stages/apoplast/exclude_this/__init__.py
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 apoplast-2.0.2/PKG-INFO
```

### Comparing `apoplast-2.0.1/pyproject.toml` & `apoplast-2.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 
 
 
 
 
 [tool.poetry]
 name = "apoplast"
-version = "2.0.1"
+version = "2.0.2"
 description = ""
 authors = []
 readme = "readme.md"
 #packages = [
 #    { include = "apoplast", from = "venues/stages" }
 #]
 
 packages = [
     { include = "apoplast", from = "venues/stages" }
 ]
+exclude = ["apoplast/exclude_this"]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 #volts = "^1.0.9"
 #click = "^8.1.7"
 #somatic = "^3.0.1"
```

### Comparing `apoplast-2.0.1/readme.md` & `apoplast-2.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.1/PKG-INFO` & `apoplast-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apoplast
-Version: 2.0.1
+Version: 2.0.2
 Summary: 
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

