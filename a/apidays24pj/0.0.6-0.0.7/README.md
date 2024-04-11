# Comparing `tmp/apidays24pj-0.0.6.tar.gz` & `tmp/apidays24pj-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidays24pj-0.0.6.tar", last modified: Thu Apr 11 13:52:55 2024, max compression
+gzip compressed data, was "apidays24pj-0.0.7.tar", last modified: Thu Apr 11 14:12:50 2024, max compression
```

## Comparing `apidays24pj-0.0.6.tar` & `apidays24pj-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:55.544982 apidays24pj-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 13:52:55.544982 apidays24pj-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:52:55.544982 apidays24pj-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:55.540982 apidays24pj-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:55.544982 apidays24pj-0.0.6/src/apidays24pj/
--rw-r--r--   0 runner    (1001) docker     (127)   741362 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/src/apidays24pj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:55.544982 apidays24pj-0.0.6/src/apidays24pj/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/src/apidays24pj/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100937 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/src/apidays24pj/_jsii/apidays24pj@0.0.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:52:43.000000 apidays24pj-0.0.6/src/apidays24pj/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:52:55.544982 apidays24pj-0.0.6/src/apidays24pj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 13:52:55.000000 apidays24pj-0.0.6/src/apidays24pj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 13:52:55.000000 apidays24pj-0.0.6/src/apidays24pj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:52:55.000000 apidays24pj-0.0.6/src/apidays24pj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 13:52:55.000000 apidays24pj-0.0.6/src/apidays24pj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:52:55.000000 apidays24pj-0.0.6/src/apidays24pj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:12:50.858835 apidays24pj-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 14:12:50.858835 apidays24pj-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:12:50.858835 apidays24pj-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:12:50.854835 apidays24pj-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:12:50.854835 apidays24pj-0.0.7/src/apidays24pj/
+-rw-r--r--   0 runner    (1001) docker     (127)   741362 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/src/apidays24pj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:12:50.858835 apidays24pj-0.0.7/src/apidays24pj/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/src/apidays24pj/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100937 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/src/apidays24pj/_jsii/apidays24pj@0.0.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:12:31.000000 apidays24pj-0.0.7/src/apidays24pj/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:12:50.858835 apidays24pj-0.0.7/src/apidays24pj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 14:12:50.000000 apidays24pj-0.0.7/src/apidays24pj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 14:12:50.000000 apidays24pj-0.0.7/src/apidays24pj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:12:50.000000 apidays24pj-0.0.7/src/apidays24pj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 14:12:50.000000 apidays24pj-0.0.7/src/apidays24pj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 14:12:50.000000 apidays24pj-0.0.7/src/apidays24pj.egg-info/top_level.txt
```

### Comparing `apidays24pj-0.0.6/LICENSE` & `apidays24pj-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apidays24pj-0.0.6/PKG-INFO` & `apidays24pj-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidays24pj
-Version: 0.0.6
+Version: 0.0.7
 Summary: apidays24pj
 Home-page: https://github.com/vianho/projen-projects
 Author: Silviana<email@example.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vianho/projen-projects
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `apidays24pj-0.0.6/setup.py` & `apidays24pj-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "apidays24pj",
-    "version": "0.0.6",
+    "version": "0.0.7",
     "description": "apidays24pj",
     "license": "Apache-2.0",
     "url": "https://github.com/vianho/projen-projects",
     "long_description_content_type": "text/markdown",
     "author": "Silviana<email@example.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "apidays24pj",
         "apidays24pj._jsii"
     ],
     "package_data": {
         "apidays24pj._jsii": [
-            "apidays24pj@0.0.6.jsii.tgz"
+            "apidays24pj@0.0.7.jsii.tgz"
         ],
         "apidays24pj": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `apidays24pj-0.0.6/src/apidays24pj/__init__.py` & `apidays24pj-0.0.7/src/apidays24pj/__init__.py`

 * *Files identical despite different names*

### Comparing `apidays24pj-0.0.6/src/apidays24pj.egg-info/PKG-INFO` & `apidays24pj-0.0.7/src/apidays24pj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidays24pj
-Version: 0.0.6
+Version: 0.0.7
 Summary: apidays24pj
 Home-page: https://github.com/vianho/projen-projects
 Author: Silviana<email@example.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vianho/projen-projects
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

