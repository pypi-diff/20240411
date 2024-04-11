# Comparing `tmp/autogluon-1.1.0b20240409.tar.gz` & `tmp/autogluon-1.1.0b20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.0b20240409.tar", last modified: Tue Apr  9 09:06:18 2024, max compression
+gzip compressed data, was "autogluon-1.1.0b20240410.tar", last modified: Wed Apr 10 09:06:55 2024, max compression
```

## Comparing `autogluon-1.1.0b20240409.tar` & `autogluon-1.1.0b20240410.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-09 09:04:42.000000 autogluon-1.1.0b20240409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.897552 autogluon-1.1.0b20240409/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.897552 autogluon-1.1.0b20240409/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:04:42.000000 autogluon-1.1.0b20240409/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:18.901552 autogluon-1.1.0b20240409/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:18.000000 autogluon-1.1.0b20240409/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-10 09:05:21.000000 autogluon-1.1.0b20240410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:05:21.000000 autogluon-1.1.0b20240410/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:55.195539 autogluon-1.1.0b20240410/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:55.000000 autogluon-1.1.0b20240410/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.0b20240409/PKG-INFO` & `autogluon-1.1.0b20240410/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.0b20240409
-Summary: AutoML for Image, Text, and Tabular Data
+Version: 1.1.0b20240410
+Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
 Project-URL: Contribute!, https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md
 Description: 
         
         <div align="center">
         <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         
-        ## AutoML for Image, Text, Time Series, and Tabular Data
+        ## Fast and Accurate ML in 3 Lines of Code
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Conda Forge](https://img.shields.io/conda/vn/conda-forge/autogluon.svg)](https://anaconda.org/conda-forge/autogluon)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/autogluon/)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Discord](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
```

### Comparing `autogluon-1.1.0b20240409/setup.py` & `autogluon-1.1.0b20240410/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.0b20240409/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.0b20240410/src/autogluon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.0b20240409
-Summary: AutoML for Image, Text, and Tabular Data
+Version: 1.1.0b20240410
+Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
 Project-URL: Contribute!, https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md
 Description: 
         
         <div align="center">
         <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         
-        ## AutoML for Image, Text, Time Series, and Tabular Data
+        ## Fast and Accurate ML in 3 Lines of Code
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Conda Forge](https://img.shields.io/conda/vn/conda-forge/autogluon.svg)](https://anaconda.org/conda-forge/autogluon)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/autogluon/)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Discord](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
```

