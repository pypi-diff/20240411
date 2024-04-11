# Comparing `tmp/toml_to_requirements-0.2.1.tar.gz` & `tmp/toml_to_requirements-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_to_requirements-0.2.1.tar", max compression
+gzip compressed data, was "toml_to_requirements-0.2.2.tar", max compression
```

## Comparing `toml_to_requirements-0.2.1.tar` & `toml_to_requirements-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      735 2024-04-09 03:26:20.190502 toml_to_requirements-0.2.1/README.md
--rw-r--r--   0        0        0      873 2024-04-11 03:07:16.943823 toml_to_requirements-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-09 03:26:20.190954 toml_to_requirements-0.2.1/toml_to_requirements/__init__.py
--rw-r--r--   0        0        0     1355 2024-04-09 04:24:50.339822 toml_to_requirements-0.2.1/toml_to_requirements/cli.py
--rw-r--r--   0        0        0     1862 2024-04-09 04:05:02.834415 toml_to_requirements-0.2.1/toml_to_requirements/convert_toml_to_requirements.py
--rw-r--r--   0        0        0      817 2024-04-11 02:57:53.493379 toml_to_requirements-0.2.1/toml_to_requirements/main.py
--rw-r--r--   0        0        0        0 2024-04-09 04:09:07.409513 toml_to_requirements-0.2.1/toml_to_requirements/py.typed
--rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 toml_to_requirements-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      590 2024-04-11 03:12:07.855595 toml_to_requirements-0.2.2/README.md
+-rw-r--r--   0        0        0      873 2024-04-11 03:12:44.013387 toml_to_requirements-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-09 03:26:20.190954 toml_to_requirements-0.2.2/toml_to_requirements/__init__.py
+-rw-r--r--   0        0        0     1355 2024-04-11 03:12:07.857358 toml_to_requirements-0.2.2/toml_to_requirements/cli.py
+-rw-r--r--   0        0        0     1862 2024-04-11 03:12:07.857514 toml_to_requirements-0.2.2/toml_to_requirements/convert_toml_to_requirements.py
+-rw-r--r--   0        0        0      817 2024-04-11 03:12:07.857753 toml_to_requirements-0.2.2/toml_to_requirements/main.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:12:07.857816 toml_to_requirements-0.2.2/toml_to_requirements/py.typed
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 toml_to_requirements-0.2.2/PKG-INFO
```

### Comparing `toml_to_requirements-0.2.1/README.md` & `toml_to_requirements-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,12 @@
 
 Run the following command to generate a requirements.txt file without including optional dependencies:
 
 ```bash
 toml-to-req --toml-file pyproject.toml
 ```
 
-To include optional dependencies, include the `--include-optional` flag in the above command:
+To include optional dependencies, include the `--optional-lists` flag in the above command:
 
 ```bash
-toml-to-req --toml-file pyproject.toml --include-optional
-```
-
-The optional lists to include can also be specified
-
-```bash
-toml-to-req --toml-file pyproject.toml --include-optional --optional-lists dev,test
+toml-to-req --toml-file pyproject.toml --optional-lists dev,test
 ```
```

### Comparing `toml_to_requirements-0.2.1/pyproject.toml` & `toml_to_requirements-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toml_to_requirements"
-version = "0.2.1"
+version = "0.2.2"
 description = "Convert a pyproject.toml file to a requirements.txt file"
 authors = ["Jake Cyr <cyrjake@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["toml", "requirements", "converter", "parser"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `toml_to_requirements-0.2.1/toml_to_requirements/cli.py` & `toml_to_requirements-0.2.2/toml_to_requirements/cli.py`

 * *Files identical despite different names*

### Comparing `toml_to_requirements-0.2.1/toml_to_requirements/convert_toml_to_requirements.py` & `toml_to_requirements-0.2.2/toml_to_requirements/convert_toml_to_requirements.py`

 * *Files identical despite different names*

### Comparing `toml_to_requirements-0.2.1/toml_to_requirements/main.py` & `toml_to_requirements-0.2.2/toml_to_requirements/main.py`

 * *Files identical despite different names*

### Comparing `toml_to_requirements-0.2.1/PKG-INFO` & `toml_to_requirements-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toml_to_requirements
-Version: 0.2.1
+Version: 0.2.2
 Summary: Convert a pyproject.toml file to a requirements.txt file
 License: MIT
 Keywords: toml,requirements,converter,parser
 Author: Jake Cyr
 Author-email: cyrjake@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
@@ -35,19 +35,13 @@
 
 Run the following command to generate a requirements.txt file without including optional dependencies:
 
 ```bash
 toml-to-req --toml-file pyproject.toml
 ```
 
-To include optional dependencies, include the `--include-optional` flag in the above command:
+To include optional dependencies, include the `--optional-lists` flag in the above command:
 
 ```bash
-toml-to-req --toml-file pyproject.toml --include-optional
-```
-
-The optional lists to include can also be specified
-
-```bash
-toml-to-req --toml-file pyproject.toml --include-optional --optional-lists dev,test
+toml-to-req --toml-file pyproject.toml --optional-lists dev,test
 ```
```

