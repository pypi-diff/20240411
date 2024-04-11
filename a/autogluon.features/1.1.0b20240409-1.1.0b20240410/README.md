# Comparing `tmp/autogluon.features-1.1.0b20240409.tar.gz` & `tmp/autogluon.features-1.1.0b20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.features-1.1.0b20240409.tar", last modified: Tue Apr  9 09:05:25 2024, max compression
+gzip compressed data, was "autogluon.features-1.1.0b20240410.tar", last modified: Wed Apr 10 09:06:00 2024, max compression
```

## Comparing `autogluon.features-1.1.0b20240409.tar` & `autogluon.features-1.1.0b20240410.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:25.165862 autogluon.features-1.1.0b20240409/
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-09 09:05:25.165862 autogluon.features-1.1.0b20240409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:05:25.165862 autogluon.features-1.1.0b20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:25.161862 autogluon.features-1.1.0b20240409/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:25.161862 autogluon.features-1.1.0b20240409/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:25.161862 autogluon.features-1.1.0b20240409/src/autogluon/features/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:25.165862 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44204 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/astype.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/auto_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/binned.py
--rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/drop_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/drop_unique.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/fillna.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/isnan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/memory_minimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/text_ngram.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/generators/text_special.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 09:04:42.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon/features/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:25.161862 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:05:25.000000 autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:00.867321 autogluon.features-1.1.0b20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-10 09:06:00.867321 autogluon.features-1.1.0b20240410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:06:00.867321 autogluon.features-1.1.0b20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:00.859321 autogluon.features-1.1.0b20240410/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:00.859321 autogluon.features-1.1.0b20240410/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:00.863321 autogluon.features-1.1.0b20240410/src/autogluon/features/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:00.867321 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44204 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/astype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/auto_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/binned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/drop_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/drop_unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/fillna.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/isnan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/memory_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/text_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/generators/text_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 09:05:21.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon/features/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:00.863321 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:00.000000 autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/zip-safe
```

### Comparing `autogluon.features-1.1.0b20240409/PKG-INFO` & `autogluon.features-1.1.0b20240410/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon.features
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

### Comparing `autogluon.features-1.1.0b20240409/setup.py` & `autogluon.features-1.1.0b20240410/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/binning.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/binning.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/__init__.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/abstract.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/astype.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/astype.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/auto_ml_pipeline.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/auto_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/binned.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/binned.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/bulk.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/bulk.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/category.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/category.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/datetime.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/drop_duplicates.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/drop_duplicates.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/drop_unique.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/drop_unique.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/dummy.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/dummy.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/fillna.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/identity.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/identity.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/isnan.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/isnan.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/label_encoder.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/memory_minimize.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/memory_minimize.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/one_hot_encoder.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/pipeline.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/rename.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/rename.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/text_ngram.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/text_ngram.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/generators/text_special.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/generators/text_special.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/utils.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon/features/vectorizers.py` & `autogluon.features-1.1.0b20240410/src/autogluon/features/vectorizers.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/PKG-INFO` & `autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon.features
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

### Comparing `autogluon.features-1.1.0b20240409/src/autogluon.features.egg-info/SOURCES.txt` & `autogluon.features-1.1.0b20240410/src/autogluon.features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

