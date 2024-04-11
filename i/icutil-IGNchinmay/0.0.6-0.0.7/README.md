# Comparing `tmp/icutil_IGNchinmay-0.0.6.tar.gz` & `tmp/icutil_IGNchinmay-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icutil_IGNchinmay-0.0.6.tar", last modified: Fri Apr  5 08:16:14 2024, max compression
+gzip compressed data, was "icutil_IGNchinmay-0.0.7.tar", last modified: Thu Apr 11 05:15:53 2024, max compression
```

## Comparing `icutil_IGNchinmay-0.0.6.tar` & `icutil_IGNchinmay-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:16:14.495269 icutil_IGNchinmay-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 08:16:14.495269 icutil_IGNchinmay-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:16:14.491269 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9800 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/draw_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/typehint_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:16:14.495269 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 08:16:14.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 08:16:14.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:16:14.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 08:16:14.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 08:16:14.000000 icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:16:14.495269 icutil_IGNchinmay-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:16:14.495269 icutil_IGNchinmay-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 08:16:07.000000 icutil_IGNchinmay-0.0.6/test/test_json.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-11 05:15:53.269768 icutil_IGNchinmay-0.0.7/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    11357 2024-04-03 11:56:29.000000 icutil_IGNchinmay-0.0.7/LICENSE.txt
+-rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1124 2024-04-11 05:15:53.269768 icutil_IGNchinmay-0.0.7/PKG-INFO
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      205 2024-04-05 12:19:49.000000 icutil_IGNchinmay-0.0.7/README.md
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-11 05:15:53.269768 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      132 2024-04-04 10:12:43.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/__init__.py
+-rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)     9800 2024-04-04 10:08:46.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/draw_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3061 2024-04-03 11:56:29.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/json_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1756 2024-04-01 09:49:27.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/typehint_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-11 05:15:53.269768 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/
+-rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1124 2024-04-11 05:15:53.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/PKG-INFO
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      405 2024-04-11 05:15:53.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)        1 2024-04-11 05:15:53.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      147 2024-04-11 05:15:53.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/requires.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       18 2024-04-11 05:15:53.000000 icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/top_level.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      740 2024-04-11 05:15:40.000000 icutil_IGNchinmay-0.0.7/pyproject.toml
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      146 2024-04-05 06:49:19.000000 icutil_IGNchinmay-0.0.7/requirements.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       38 2024-04-11 05:15:53.269768 icutil_IGNchinmay-0.0.7/setup.cfg
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-11 05:15:53.269768 icutil_IGNchinmay-0.0.7/test/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       94 2024-04-04 10:08:00.000000 icutil_IGNchinmay-0.0.7/test/test_json.py
```

### Comparing `icutil_IGNchinmay-0.0.6/LICENSE.txt` & `icutil_IGNchinmay-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.6/PKG-INFO` & `icutil_IGNchinmay-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icutil_IGNchinmay
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://github.com/IGNchinmay/PypiPublishTest
 Project-URL: Issues, https://github.com/IGNchinmay/PypiPublishTest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,9 +25,14 @@
 Requires-Dist: pynput
 Requires-Dist: scikit-image
 Requires-Dist: shapely
 Requires-Dist: sympy
 Requires-Dist: termcolor
 
 # icutils
+<div align="center">
+  <img src="ignitarium-logo.png">
+</div>
+
+[![PyPI version](https://badge.fury.io/py/icutil-IGNchinmay.svg)](https://badge.fury.io/py/icutil-IGNchinmay)
 
 A sample test package
```

### Comparing `icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/draw_utils.py` & `icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/draw_utils.py`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/json_utils.py` & `icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/json_utils.py`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.6/icutil_IGNchinmay/typehint_utils.py` & `icutil_IGNchinmay-0.0.7/icutil_IGNchinmay/typehint_utils.py`

 * *Files identical despite different names*

### Comparing `icutil_IGNchinmay-0.0.6/icutil_IGNchinmay.egg-info/PKG-INFO` & `icutil_IGNchinmay-0.0.7/icutil_IGNchinmay.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icutil_IGNchinmay
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://github.com/IGNchinmay/PypiPublishTest
 Project-URL: Issues, https://github.com/IGNchinmay/PypiPublishTest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,9 +25,14 @@
 Requires-Dist: pynput
 Requires-Dist: scikit-image
 Requires-Dist: shapely
 Requires-Dist: sympy
 Requires-Dist: termcolor
 
 # icutils
+<div align="center">
+  <img src="ignitarium-logo.png">
+</div>
+
+[![PyPI version](https://badge.fury.io/py/icutil-IGNchinmay.svg)](https://badge.fury.io/py/icutil-IGNchinmay)
 
 A sample test package
```

### Comparing `icutil_IGNchinmay-0.0.6/pyproject.toml` & `icutil_IGNchinmay-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icutil_IGNchinmay"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

