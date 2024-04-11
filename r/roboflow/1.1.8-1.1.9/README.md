# Comparing `tmp/roboflow-1.1.8.tar.gz` & `tmp/roboflow-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.1.8.tar", last modified: Fri Nov  3 14:30:27 2023, max compression
+gzip compressed data, was "roboflow-1.1.9.tar", last modified: Fri Nov  3 19:35:05 2023, max compression
```

## Comparing `roboflow-1.1.8.tar` & `roboflow-1.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2023-11-03 14:29:55.000000 roboflow-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2023-11-03 14:30:26.998153 roboflow-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2023-11-03 14:29:55.000000 roboflow-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-03 14:29:55.000000 roboflow-1.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.994153 roboflow-1.1.8/roboflow/
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    30500 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    29203 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/gaze.py
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22548 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19835 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-11-03 14:29:55.000000 roboflow-1.1.8/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.994153 roboflow-1.1.8/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2023-11-03 14:30:26.000000 roboflow-1.1.8/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-11-03 14:30:26.000000 roboflow-1.1.8/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 14:30:26.000000 roboflow-1.1.8/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-03 14:30:26.000000 roboflow-1.1.8/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-03 14:30:26.000000 roboflow-1.1.8/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 14:30:26.998153 roboflow-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-03 14:29:55.000000 roboflow-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 14:30:26.998153 roboflow-1.1.8/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-03 14:29:55.000000 roboflow-1.1.8/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.978759 roboflow-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2023-11-03 19:34:44.000000 roboflow-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2023-11-03 19:35:05.978759 roboflow-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2023-11-03 19:34:44.000000 roboflow-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-03 19:34:44.000000 roboflow-1.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.970759 roboflow-1.1.9/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.974759 roboflow-1.1.9/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30500 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29203 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.974759 roboflow-1.1.9/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/gaze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22548 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.978759 roboflow-1.1.9/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19835 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-11-03 19:34:44.000000 roboflow-1.1.9/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.974759 roboflow-1.1.9/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2023-11-03 19:35:05.000000 roboflow-1.1.9/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-11-03 19:35:05.000000 roboflow-1.1.9/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 19:35:05.000000 roboflow-1.1.9/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-03 19:35:05.000000 roboflow-1.1.9/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-03 19:35:05.000000 roboflow-1.1.9/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 19:35:05.978759 roboflow-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-11-03 19:34:44.000000 roboflow-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.978759 roboflow-1.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.978759 roboflow-1.1.9/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.978759 roboflow-1.1.9/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 19:35:05.978759 roboflow-1.1.9/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-03 19:34:44.000000 roboflow-1.1.9/tests/util/test_versions.py
```

### Comparing `roboflow-1.1.8/LICENSE` & `roboflow-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/PKG-INFO` & `roboflow-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.1.8
+Version: 1.1.9
 Summary: Official Python package for working with the Roboflow API
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: support@roboflow.com
 License: UNKNOWN
 Description: <div align="center">
           <p>
```

### Comparing `roboflow-1.1.8/README.md` & `roboflow-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/__init__.py` & `roboflow-1.1.9/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.models import CLIPModel, GazeModel
 from roboflow.util.general import write_line
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.1.8/roboflow/config.py` & `roboflow-1.1.9/roboflow/config.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/core/project.py` & `roboflow-1.1.9/roboflow/core/project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/core/version.py` & `roboflow-1.1.9/roboflow/core/version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/core/workspace.py` & `roboflow-1.1.9/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/models/classification.py` & `roboflow-1.1.9/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/models/inference.py` & `roboflow-1.1.9/roboflow/models/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,14 @@
                 raise Exception(
                     f"There was an error uploading the video: {result.text}"
                 )
         else:
             signed_url = video_path
 
         url = urljoin(API_URL, "/videoinfer/?api_key=" + self.__api_key)
-
         if model_class in ("CLIPModel", "GazeModel"):
             if model_class == "CLIPModel":
                 model = "clip"
             else:
                 model = "gaze"
 
             models = [
@@ -253,14 +252,22 @@
                         "model_version"
                     ],
                     "inference_type": SUPPORTED_ADDITIONAL_MODELS[model][
                         "inference_type"
                     ],
                 }
             ]
+        else:
+            models = [
+                {
+                    "model_id": self.dataset_id,
+                    "model_version": self.version,
+                    "inference_type": self.type,
+                }
+            ]
 
         for model in additional_models:
             models.append(SUPPORTED_ADDITIONAL_MODELS[model])
 
         payload = json.dumps(
             {"input_url": signed_url, "infer_fps": 5, "models": models}
         )
@@ -304,36 +311,36 @@
 
         if job_id is None:
             job_id = self.job_id
 
         url = urljoin(
             API_URL, "/videoinfer/?api_key=" + self.__api_key + "&job_id=" + self.job_id
         )
-
         try:
             response = requests.get(url, headers={"Content-Type": "application/json"})
         except Exception as e:
             raise Exception(f"Error getting video inference results: {e}")
 
         if not response.ok:
             raise Exception(f"Error getting video inference results: {response.text}")
-
         data = response.json()
+        if "status" not in data:
+            return {}  # No status available
+        if data.get("status") > 1:
+            return data  # Error
+        elif data.get("status") == 1:
+            return {}  # Still running
+        else:  # done
+            output_signed_url = data["output_signed_url"]
+            inference_data = requests.get(
+                output_signed_url, headers={"Content-Type": "application/json"}
+            )
 
-        if data.get("status") != 0:
-            return {}
-
-        output_signed_url = data["output_signed_url"]
-
-        inference_data = requests.get(
-            output_signed_url, headers={"Content-Type": "application/json"}
-        )
-
-        # frame_offset and model name are top-level keys
-        return inference_data.json()
+            # frame_offset and model name are top-level keys
+            return inference_data.json()
 
     def poll_until_video_results(self, job_id) -> dict:
         """
         Polls the Roboflow API to check if video inference is complete.
 
         When inference is complete, the results are returned.
 
@@ -353,19 +360,16 @@
 
             >>> results = model.poll_until_results()
         """
         if job_id is None:
             job_id = self.job_id
 
         attempts = 0
-
+        print(f"Checking for video inference results for job {job_id} every 60s")
         while True:
+            time.sleep(60)
             print(f"({attempts * 60}s): Checking for inference results")
-
             response = self.poll_for_video_results()
-
-            time.sleep(60)
-
             attempts += 1
 
             if response != {}:
                 return response
```

### Comparing `roboflow-1.1.8/roboflow/models/instance_segmentation.py` & `roboflow-1.1.9/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/models/object_detection.py` & `roboflow-1.1.9/roboflow/models/object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/models/semantic_segmentation.py` & `roboflow-1.1.9/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/models/video.py` & `roboflow-1.1.9/roboflow/models/video.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/active_learning_utils.py` & `roboflow-1.1.9/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/clip_compare_utils.py` & `roboflow-1.1.9/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/general.py` & `roboflow-1.1.9/roboflow/util/general.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/image_utils.py` & `roboflow-1.1.9/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/prediction.py` & `roboflow-1.1.9/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/two_stage_utils.py` & `roboflow-1.1.9/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow/util/versions.py` & `roboflow-1.1.9/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/roboflow.egg-info/PKG-INFO` & `roboflow-1.1.9/roboflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.1.8
+Version: 1.1.9
 Summary: Official Python package for working with the Roboflow API
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: support@roboflow.com
 License: UNKNOWN
 Description: <div align="center">
           <p>
```

### Comparing `roboflow-1.1.8/roboflow.egg-info/SOURCES.txt` & `roboflow-1.1.9/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/setup.py` & `roboflow-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/models/test_instance_segmentation.py` & `roboflow-1.1.9/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/models/test_object_detection.py` & `roboflow-1.1.9/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/models/test_semantic_segmentation.py` & `roboflow-1.1.9/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/test_project.py` & `roboflow-1.1.9/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/test_queries.py` & `roboflow-1.1.9/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/test_version.py` & `roboflow-1.1.9/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/util/test_image_utils.py` & `roboflow-1.1.9/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.8/tests/util/test_versions.py` & `roboflow-1.1.9/tests/util/test_versions.py`

 * *Files identical despite different names*

