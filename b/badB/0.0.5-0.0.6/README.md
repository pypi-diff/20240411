# Comparing `tmp/badb-0.0.5.tar.gz` & `tmp/badb-0.0.6.tar.gz`

## Comparing `badb-0.0.5.tar` & `badb-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.5/badb.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.5/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.5/src/badb/__init__.py
--rw-r--r--   0        0        0    12373 2020-02-02 00:00:00.000000 badb-0.0.5/src/badb/__main__.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.5/src/badb/questionnaire.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.5/LICENSE
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.5/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 badb-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.6/badb.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.6/src/badb/__init__.py
+-rw-r--r--   0        0        0    12373 2020-02-02 00:00:00.000000 badb-0.0.6/src/badb/__main__.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.6/src/badb/questionnaire.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.6/LICENSE
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.6/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 badb-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.6/PKG-INFO
```

### Comparing `badb-0.0.5/badb.json` & `badb-0.0.6/badb.json`

 * *Files identical despite different names*

### Comparing `badb-0.0.5/src/badb/__main__.py` & `badb-0.0.6/src/badb/__main__.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.5/src/badb/questionnaire.py` & `badb-0.0.6/src/badb/questionnaire.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.5/.gitignore` & `badb-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `badb-0.0.5/LICENSE` & `badb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `badb-0.0.5/pyproject.toml` & `badb-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "badB"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Akash Srivastava", email="sriakash.dev@gmail.com" },
 ]
 description = "A pip package to create Flask RESTful-api seamlessly with customizations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,8 +18,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/Dev-Akash/badb"
 Issues = "https://github.com/Dev-Akash/badb/issues"
 
 [project.scripts]
-badB = "badb"
+badB = "badb.__main__:init"
```

### Comparing `badb-0.0.5/PKG-INFO` & `badb-0.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: badB
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pip package to create Flask RESTful-api seamlessly with customizations
 Project-URL: Homepage, https://github.com/Dev-Akash/badb
 Project-URL: Issues, https://github.com/Dev-Akash/badb/issues
 Author-email: Akash Srivastava <sriakash.dev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

