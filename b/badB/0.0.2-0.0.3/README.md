# Comparing `tmp/badb-0.0.2.tar.gz` & `tmp/badb-0.0.3.tar.gz`

## Comparing `badb-0.0.2.tar` & `badb-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.2/badb.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.2/requirements.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 badb-0.0.2/src/badb/__init__.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 badb-0.0.2/src/badb/__main__.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.2/src/badb/questionnaire.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.2/LICENSE
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.2/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 badb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.3/badb.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.3/src/badb/__init__.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 badb-0.0.3/src/badb/__main__.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.3/src/badb/questionnaire.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.3/LICENSE
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.3/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 badb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.3/PKG-INFO
```

### Comparing `badb-0.0.2/badb.json` & `badb-0.0.3/badb.json`

 * *Files identical despite different names*

### Comparing `badb-0.0.2/src/badb/__main__.py` & `badb-0.0.3/src/badb/__main__.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.2/src/badb/questionnaire.py` & `badb-0.0.3/src/badb/questionnaire.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.2/.gitignore` & `badb-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `badb-0.0.2/LICENSE` & `badb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `badb-0.0.2/pyproject.toml` & `badb-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "badB"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Akash Srivastava", email="sriakash.dev@gmail.com" },
 ]
 description = "A pip package to create Flask RESTful-api seamlessly with customizations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `badb-0.0.2/PKG-INFO` & `badb-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: badB
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pip package to create Flask RESTful-api seamlessly with customizations
 Project-URL: Homepage, https://github.com/Dev-Akash/badb
 Project-URL: Issues, https://github.com/Dev-Akash/badb/issues
 Author-email: Akash Srivastava <sriakash.dev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

