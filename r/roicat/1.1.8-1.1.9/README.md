# Comparing `tmp/roicat-1.1.8.tar.gz` & `tmp/roicat-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roicat-1.1.8.tar", last modified: Sat Sep 30 19:38:13 2023, max compression
+gzip compressed data, was "roicat-1.1.9.tar", last modified: Sat Sep 30 19:41:34 2023, max compression
```

## Comparing `roicat-1.1.8.tar` & `roicat-1.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.307802 roicat-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34655 2023-09-30 19:37:58.000000 roicat-1.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-30 19:37:58.000000 roicat-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2023-09-30 19:38:13.307802 roicat-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2023-09-30 19:37:58.000000 roicat-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-09-30 19:37:58.000000 roicat-1.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.291801 roicat-1.1.8/roicat/
--rw-r--r--   0 runner    (1001) docker     (127)    66589 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/ROInet.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.291801 roicat-1.1.8/roicat/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30550 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/classification/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    82976 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/data_importing.py
--rw-r--r--   0 runner    (1001) docker     (127)   177786 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.291801 roicat-1.1.8/roicat/model_training/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/model_training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17009 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/model_training/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11717 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/model_training/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.291801 roicat-1.1.8/roicat/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45626 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/tracking/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/tracking/blurring.py
--rw-r--r--   0 runner    (1001) docker     (127)    65719 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/tracking/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/tracking/scatteringWaveletTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29549 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/tracking/similarity_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    48702 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29636 2023-09-30 19:37:58.000000 roicat-1.1.8/roicat/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.291801 roicat-1.1.8/roicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2023-09-30 19:38:13.000000 roicat-1.1.8/roicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-09-30 19:38:13.000000 roicat-1.1.8/roicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 19:38:13.000000 roicat-1.1.8/roicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-09-30 19:38:13.000000 roicat-1.1.8/roicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-30 19:38:13.000000 roicat-1.1.8/roicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-30 19:38:13.307802 roicat-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2023-09-30 19:37:58.000000 roicat-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:38:13.291801 roicat-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-09-30 19:37:58.000000 roicat-1.1.8/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2023-09-30 19:37:58.000000 roicat-1.1.8/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-09-30 19:37:58.000000 roicat-1.1.8/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2023-09-30 19:37:58.000000 roicat-1.1.8/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.921299 roicat-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34655 2023-09-30 19:41:26.000000 roicat-1.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-30 19:41:26.000000 roicat-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2023-09-30 19:41:34.921299 roicat-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2023-09-30 19:41:26.000000 roicat-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-09-30 19:41:26.000000 roicat-1.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.905299 roicat-1.1.9/roicat/
+-rw-r--r--   0 runner    (1001) docker     (127)    66589 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/ROInet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.905299 roicat-1.1.9/roicat/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30550 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/classification/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82976 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/data_importing.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177786 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.905299 roicat-1.1.9/roicat/model_training/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/model_training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17009 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/model_training/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11717 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/model_training/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.905299 roicat-1.1.9/roicat/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45626 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/tracking/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/tracking/blurring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65719 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/tracking/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/tracking/scatteringWaveletTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29549 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/tracking/similarity_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48702 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29636 2023-09-30 19:41:26.000000 roicat-1.1.9/roicat/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.905299 roicat-1.1.9/roicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2023-09-30 19:41:34.000000 roicat-1.1.9/roicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2023-09-30 19:41:34.000000 roicat-1.1.9/roicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 19:41:34.000000 roicat-1.1.9/roicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-09-30 19:41:34.000000 roicat-1.1.9/roicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-30 19:41:34.000000 roicat-1.1.9/roicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-30 19:41:34.921299 roicat-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2023-09-30 19:41:26.000000 roicat-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 19:41:34.905299 roicat-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-09-30 19:41:26.000000 roicat-1.1.9/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2023-09-30 19:41:26.000000 roicat-1.1.9/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-09-30 19:41:26.000000 roicat-1.1.9/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2023-09-30 19:41:26.000000 roicat-1.1.9/tests/test_unit.py
```

### Comparing `roicat-1.1.8/LICENSE.md` & `roicat-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/PKG-INFO` & `roicat-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roicat
-Version: 1.1.8
+Version: 1.1.9
 Summary: A library for classifying and tracking ROIs.
 Home-page: https://github.com/RichieHakim/ROICaT
 Author: Richard Hakim
 License: LICENSE
 Keywords: neuroscience,neuroimaging,machine learning,deep learning
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `roicat-1.1.8/README.md` & `roicat-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/ROInet.py` & `roicat-1.1.9/roicat/ROInet.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/classification/classifier.py` & `roicat-1.1.9/roicat/classification/classifier.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/data_importing.py` & `roicat-1.1.9/roicat/data_importing.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/helpers.py` & `roicat-1.1.9/roicat/helpers.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/model_training/augmentation.py` & `roicat-1.1.9/roicat/model_training/augmentation.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/model_training/model.py` & `roicat-1.1.9/roicat/model_training/model.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/pipelines.py` & `roicat-1.1.9/roicat/pipelines.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/tracking/alignment.py` & `roicat-1.1.9/roicat/tracking/alignment.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/tracking/blurring.py` & `roicat-1.1.9/roicat/tracking/blurring.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/tracking/clustering.py` & `roicat-1.1.9/roicat/tracking/clustering.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/tracking/scatteringWaveletTransformer.py` & `roicat-1.1.9/roicat/tracking/scatteringWaveletTransformer.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/tracking/similarity_graph.py` & `roicat-1.1.9/roicat/tracking/similarity_graph.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/util.py` & `roicat-1.1.9/roicat/util.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat/visualization.py` & `roicat-1.1.9/roicat/visualization.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat.egg-info/PKG-INFO` & `roicat-1.1.9/roicat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roicat
-Version: 1.1.8
+Version: 1.1.9
 Summary: A library for classifying and tracking ROIs.
 Home-page: https://github.com/RichieHakim/ROICaT
 Author: Richard Hakim
 License: LICENSE
 Keywords: neuroscience,neuroimaging,machine learning,deep learning
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `roicat-1.1.8/roicat.egg-info/SOURCES.txt` & `roicat-1.1.9/roicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/roicat.egg-info/requires.txt` & `roicat-1.1.9/roicat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/setup.py` & `roicat-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/tests/test_environment.py` & `roicat-1.1.9/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/tests/test_integration.py` & `roicat-1.1.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/tests/test_packages.py` & `roicat-1.1.9/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `roicat-1.1.8/tests/test_unit.py` & `roicat-1.1.9/tests/test_unit.py`

 * *Files identical despite different names*

