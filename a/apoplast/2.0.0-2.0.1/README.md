# Comparing `tmp/apoplast-2.0.0.tar.gz` & `tmp/apoplast-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apoplast-2.0.0.tar", max compression
+gzip compressed data, was "apoplast-2.0.1.tar", max compression
```

## Comparing `apoplast-2.0.0.tar` & `apoplast-2.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      619 2024-04-11 20:18:02.088181 apoplast-2.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.0/readme.md
--rw-r--r--   0        0        0       21 2024-04-11 20:17:16.500712 apoplast-2.0.0/venues/stages/apoplast/__init__.py
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 apoplast-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      640 2024-04-11 20:20:04.967018 apoplast-2.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.1/readme.md
+-rw-r--r--   0        0        0       21 2024-04-11 20:17:16.500712 apoplast-2.0.1/venues/stages/apoplast/__init__.py
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 apoplast-2.0.1/PKG-INFO
```

### Comparing `apoplast-2.0.0/pyproject.toml` & `apoplast-2.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 
 
 
 
 
 [tool.poetry]
 name = "apoplast"
-version = "2.0.0"
+version = "2.0.1"
 description = ""
 authors = []
 readme = "readme.md"
 #packages = [
 #    { include = "apoplast", from = "venues/stages" }
 #]
 
 packages = [
-    { include = "venues/stages/apoplast" }
+    { include = "apoplast", from = "venues/stages" }
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-volts = "^1.0.9"
-click = "^8.1.7"
-somatic = "^3.0.1"
-ships = "^1.2.6"
-sphene = "^1.0.7"
-sanic = "^23.12.1"
-pymongo = "^4.6.3"
-pydash = "^8.0.0"
-rich = "^13.7.1"
-tinydb = "^4.8.0"
-numpy = "^1.26.4"
+#volts = "^1.0.9"
+#click = "^8.1.7"
+#somatic = "^3.0.1"
+#ships = "^1.2.6"
+#sphene = "^1.0.7"
+#sanic = "^23.12.1"
+#pymongo = "^4.6.3"
+#pydash = "^8.0.0"
+#rich = "^13.7.1"
+#tinydb = "^4.8.0"
+#numpy = "^1.26.4"
 
 #[tool.poetry.scripts]
 #apoplast = 'apoplast:clique'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `apoplast-2.0.0/readme.md` & `apoplast-2.0.1/readme.md`

 * *Files identical despite different names*

