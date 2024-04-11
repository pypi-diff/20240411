# Comparing `tmp/apoplast-2.0.3.tar.gz` & `tmp/apoplast-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apoplast-2.0.3.tar", max compression
+gzip compressed data, was "apoplast-2.0.4.tar", max compression
```

## Comparing `apoplast-2.0.3.tar` & `apoplast-2.0.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      676 2024-04-11 20:24:01.096825 apoplast-2.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.3/readme.md
--rw-r--r--   0        0        0       29 2024-04-11 20:23:18.373237 apoplast-2.0.3/venues/stages/apoplast/__init__.py
--rw-r--r--   0        0        0       19 2024-04-11 20:20:40.718700 apoplast-2.0.3/venues/stages/apoplast/apoplast.S.HTML
--rw-r--r--   0        0        0       24 2024-04-11 20:21:27.086280 apoplast-2.0.3/venues/stages/apoplast/exclude_this/__init__.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 apoplast-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      690 2024-04-11 20:24:56.240284 apoplast-2.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.4/readme.md
+-rw-r--r--   0        0        0       29 2024-04-11 20:23:18.373237 apoplast-2.0.4/venues/stages/apoplast/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-11 20:20:40.718700 apoplast-2.0.4/venues/stages/apoplast/apoplast.S.HTML
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 apoplast-2.0.4/PKG-INFO
```

### Comparing `apoplast-2.0.3/pyproject.toml` & `apoplast-2.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 
 
 
 
 [tool.poetry]
 name = "apoplast"
-version = "2.0.3"
+version = "2.0.4"
 description = ""
 authors = []
 readme = "readme.md"
 #packages = [
 #    { include = "apoplast", from = "venues/stages" }
 #]
 
 packages = [
     { include = "apoplast", from = "venues/stages" }
 ]
-exclude = ["apoplast/exclude_this"]
+exclude = ["venues/stages/apoplast/exclude_this"]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 #volts = "^1.0.9"
 #click = "^8.1.7"
 #somatic = "^3.0.1"
```

### Comparing `apoplast-2.0.3/readme.md` & `apoplast-2.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.3/PKG-INFO` & `apoplast-2.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apoplast
-Version: 2.0.3
+Version: 2.0.4
 Summary: 
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

