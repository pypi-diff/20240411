# Comparing `tmp/five_strips_of_bacon-0.1.0.tar.gz` & `tmp/five_strips_of_bacon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_strips_of_bacon-0.1.0.tar", max compression
+gzip compressed data, was "five_strips_of_bacon-0.1.1.tar", max compression
```

## Comparing `five_strips_of_bacon-0.1.0.tar` & `five_strips_of_bacon-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1118 2024-04-09 18:02:12.474693 five_strips_of_bacon-0.1.0/README.md
--rw-r--r--   0        0        0     2256 2023-10-20 03:40:16.732000 five_strips_of_bacon-0.1.0/five_strips_of_bacon/bacon.py
--rw-r--r--   0        0        0     2866 2024-04-09 18:08:34.450000 five_strips_of_bacon-0.1.0/five_strips_of_bacon/decode_five_strips_of_bacon.py
--rw-r--r--   0        0        0      536 2024-04-10 16:50:42.345827 five_strips_of_bacon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 five_strips_of_bacon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1118 2024-04-09 18:02:12.474693 five_strips_of_bacon-0.1.1/README.md
+-rw-r--r--   0        0        0      553 2024-04-11 01:38:58.610437 five_strips_of_bacon-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2256 2023-10-20 03:40:16.732000 five_strips_of_bacon-0.1.1/src/bacon.py
+-rw-r--r--   0        0        0     2866 2024-04-09 18:08:34.450000 five_strips_of_bacon-0.1.1/src/decode_five_strips_of_bacon.py
+-rw-r--r--   0        0        0     7878 2024-04-11 01:35:20.243192 five_strips_of_bacon-0.1.1/src/main.py
+-rw-r--r--   0        0        0    29094 2024-03-08 05:34:01.619000 five_strips_of_bacon-0.1.1/src/resources/bacon_five.png
+-rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 five_strips_of_bacon-0.1.1/PKG-INFO
```

### Comparing `five_strips_of_bacon-0.1.0/README.md` & `five_strips_of_bacon-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.0/five_strips_of_bacon/bacon.py` & `five_strips_of_bacon-0.1.1/src/bacon.py`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.0/five_strips_of_bacon/decode_five_strips_of_bacon.py` & `five_strips_of_bacon-0.1.1/src/decode_five_strips_of_bacon.py`

 * *Files identical despite different names*

### Comparing `five_strips_of_bacon-0.1.0/pyproject.toml` & `five_strips_of_bacon-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "five-strips-of-bacon"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Odyhibit <josh.2990@gmail.com>"]
 readme = "README.md"
 packages = [
-    { include = "five_strips_of_bacon/decode_five_strips_of_bacon.py"},
-    { include = "five_strips_of_bacon/bacon.py"},
+    { include = "src/main.py"},
+    { include = "src/bacon.py"},
+    { include = "src/decode_five_strips_of_bacon.py"},
+    { include = "src/resources/*"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 customtkinter = "^5.2.2"
 pillow = "^10.3.0"
 
 [tool.poetry.scripts]
-five-strips-of-bacon = "five_strips_of_bacon.main:main"
+five-strips-of-bacon = "src.main:main"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `five_strips_of_bacon-0.1.0/PKG-INFO` & `five_strips_of_bacon-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five-strips-of-bacon
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Odyhibit
 Author-email: josh.2990@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: customtkinter (>=5.2.2,<6.0.0)
```

