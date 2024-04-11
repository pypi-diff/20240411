# Comparing `tmp/badb-0.0.4.tar.gz` & `tmp/badb-0.0.5.tar.gz`

## Comparing `badb-0.0.4.tar` & `badb-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.4/badb.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.4/src/badb/__init__.py
--rw-r--r--   0        0        0    12373 2020-02-02 00:00:00.000000 badb-0.0.4/src/badb/__main__.py
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.4/src/badb/questionnaire.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.4/LICENSE
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.4/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 badb-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 badb-0.0.5/badb.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 badb-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 badb-0.0.5/src/badb/__init__.py
+-rw-r--r--   0        0        0    12373 2020-02-02 00:00:00.000000 badb-0.0.5/src/badb/__main__.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 badb-0.0.5/src/badb/questionnaire.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 badb-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 badb-0.0.5/LICENSE
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 badb-0.0.5/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 badb-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 badb-0.0.5/PKG-INFO
```

### Comparing `badb-0.0.4/badb.json` & `badb-0.0.5/badb.json`

 * *Files identical despite different names*

### Comparing `badb-0.0.4/src/badb/__main__.py` & `badb-0.0.5/src/badb/__main__.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.4/src/badb/questionnaire.py` & `badb-0.0.5/src/badb/questionnaire.py`

 * *Files identical despite different names*

### Comparing `badb-0.0.4/.gitignore` & `badb-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `badb-0.0.4/LICENSE` & `badb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `badb-0.0.4/pyproject.toml` & `badb-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "badB"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Akash Srivastava", email="sriakash.dev@gmail.com" },
 ]
 description = "A pip package to create Flask RESTful-api seamlessly with customizations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Dev-Akash/badb"
-Issues = "https://github.com/Dev-Akash/badb/issues"
+Issues = "https://github.com/Dev-Akash/badb/issues"
+
+[project.scripts]
+badB = "badb"
```

### Comparing `badb-0.0.4/PKG-INFO` & `badb-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: badB
-Version: 0.0.4
+Version: 0.0.5
 Summary: A pip package to create Flask RESTful-api seamlessly with customizations
 Project-URL: Homepage, https://github.com/Dev-Akash/badb
 Project-URL: Issues, https://github.com/Dev-Akash/badb/issues
 Author-email: Akash Srivastava <sriakash.dev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

