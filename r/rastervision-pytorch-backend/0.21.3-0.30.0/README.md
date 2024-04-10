# Comparing `tmp/rastervision_pytorch_backend-0.21.3.tar.gz` & `tmp/rastervision_pytorch_backend-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_pytorch_backend-0.21.3.tar", last modified: Tue Oct 17 19:14:42 2023, max compression
+gzip compressed data, was "rastervision_pytorch_backend-0.30.0.tar", last modified: Wed Apr 10 22:11:09 2024, max compression
```

## Comparing `rastervision_pytorch_backend-0.21.3.tar` & `rastervision_pytorch_backend-0.30.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      586 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/
--rw-rw-r--   0 root         (0) root         (0)      862 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/chip_classification/
--rw-rw-r--   0 root         (0) root         (0)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/chip_classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7174 2023-09-08 19:48:40.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/
--rw-rw-r--   0 root         (0) root         (0)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7894 2023-09-08 19:48:40.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      728 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py
--rw-rw-r--   0 root         (0) root         (0)     2631 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py
--rw-rw-r--   0 root         (0) root         (0)      804 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py
--rw-rw-r--   0 root         (0) root         (0)      978 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py
--rw-rw-r--   0 root         (0) root         (0)     4883 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/xview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/
--rw-rw-r--   0 root         (0) root         (0)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9051 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py
--rw-rw-r--   0 root         (0) root         (0)    10189 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py
--rw-rw-r--   0 root         (0) root         (0)     7907 2023-10-16 20:21:50.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py
--rw-rw-r--   0 root         (0) root         (0)     1472 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py
--rw-rw-r--   0 root         (0) root         (0)    23309 2023-10-16 20:22:08.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/test.py
--rw-rw-r--   0 root         (0) root         (0)     3762 2023-09-19 18:25:31.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/tiny_spacenet.py
--rw-rw-r--   0 root         (0) root         (0)     3668 2023-09-08 19:48:40.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/utils.py
--rw-rw-r--   0 root         (0) root         (0)     3064 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_chip_classification.py
--rw-rw-r--   0 root         (0) root         (0)     2362 2023-09-26 14:00:58.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_chip_classification_config.py
--rw-rw-r--   0 root         (0) root         (0)     5202 2023-09-26 14:00:58.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_learner_backend.py
--rw-rw-r--   0 root         (0) root         (0)     3933 2023-09-26 14:00:58.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_learner_backend_config.py
--rw-rw-r--   0 root         (0) root         (0)     4872 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_object_detection.py
--rw-rw-r--   0 root         (0) root         (0)     2324 2023-09-26 14:00:58.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_object_detection_config.py
--rw-rw-r--   0 root         (0) root         (0)     3796 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_semantic_segmentation.py
--rw-rw-r--   0 root         (0) root         (0)     2419 2023-09-26 14:00:58.000000 rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      586 2023-10-17 19:14:42.000000 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2300 2023-10-17 19:14:42.000000 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:42.000000 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:42.000000 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2023-10-17 19:14:42.000000 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:42.000000 rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      121 2023-10-17 13:37:07.000000 rastervision_pytorch_backend-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:42.623339 rastervision_pytorch_backend-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1165 2023-10-17 13:37:07.000000 rastervision_pytorch_backend-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      586 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.479691 rastervision_pytorch_backend-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      911 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/__init__.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/__init__.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7410 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8108 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      728 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2631 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      804 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      978 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4984 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/xview.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9562 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10068 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8255 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1480 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    21848 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/test.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3650 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/tiny_spacenet.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3788 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2990 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2344 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7949 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3575 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4908 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2349 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3417 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2401 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1363 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      586 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2338 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:49.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       89 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      121 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1753 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/setup.py
```

### Comparing `rastervision_pytorch_backend-0.21.3/PKG-INFO` & `rastervision_pytorch_backend-0.30.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_pytorch_backend
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds PyTorch backends for rastervision.core pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/__init__.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # flake8: noqa
 
 
 def register_plugin(registry):
-    registry.set_plugin_version('rastervision.pytorch_backend', 1)
+    registry.set_plugin_version('rastervision.pytorch_backend', 2)
 
 
 import rastervision.pipeline
 from rastervision.pytorch_backend.pytorch_chip_classification_config import *
 from rastervision.pytorch_backend.pytorch_chip_classification import *
 from rastervision.pytorch_backend.pytorch_semantic_segmentation_config import *
 from rastervision.pytorch_backend.pytorch_semantic_segmentation import *
 from rastervision.pytorch_backend.pytorch_object_detection_config import *
 from rastervision.pytorch_backend.pytorch_object_detection import *
+from rastervision.pytorch_backend.utils import *
 
 __all__ = [
     PyTorchChipClassification.__name__,
     PyTorchChipClassificationConfig.__name__,
     PyTorchSemanticSegmentation.__name__,
     PyTorchSemanticSegmentationConfig.__name__,
     PyTorchObjectDetection.__name__,
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# flake8: noqa
-
 import os
 from os.path import join
 
-import albumentations as A
-
-from rastervision.core.rv_pipeline import *
-from rastervision.core.backend import *
-from rastervision.core.data import *
-from rastervision.core.analyzer import *
-from rastervision.pytorch_backend import *
-from rastervision.pytorch_learner import *
+from rastervision.core.rv_pipeline import (
+    ChipClassificationConfig, ChipOptions, PredictOptions,
+    WindowSamplingConfig, WindowSamplingMethod)
+from rastervision.core.data import (
+    ChipClassificationLabelSourceConfig, ClassConfig,
+    ClassInferenceTransformerConfig, DatasetConfig, GeoJSONVectorSourceConfig,
+    RasterioSourceConfig, SceneConfig)
+from rastervision.pytorch_backend import PyTorchChipClassificationConfig
+from rastervision.pytorch_learner import (
+    Backbone, ClassificationGeoDataConfig, ClassificationImageDataConfig,
+    ClassificationModelConfig, ExternalModuleConfig, SolverConfig)
 from rastervision.pytorch_backend.examples.utils import (get_scene_info,
                                                          save_image_crop)
 
 aoi_path = 'AOIs/AOI_1_Rio/srcData/buildingLabels/Rio_OUTLINE_Public_AOI.geojson'
 
 CLASS_NAMES = ['no_building', 'building']
 
@@ -47,16 +48,15 @@
         nochip (bool, optional): If True, read directly from the TIFF during
             training instead of from pre-generated chips. The analyze and chip
             commands should not be run, if this is set to True. Defaults to
             True.
         test (bool, optional): If True, does the following simplifications:
             (1) Uses only the first 1 scene
             (2) Uses only a 600x600 crop of the scenes
-            (3) Enables test mode in the learner, which makes it use the
-                test_batch_sz and test_num_epochs, among other things.
+            (3) Trains for only 4 epochs.
             Defaults to False.
 
     Returns:
         ChipClassificationConfig: A pipeline config.
     """
     train_scene_info = get_scene_info(join(processed_uri, 'train-scenes.csv'))
     val_scene_info = get_scene_info(join(processed_uri, 'val-scenes.csv'))
@@ -96,15 +96,14 @@
 
         id = os.path.splitext(os.path.basename(raster_uri))[0]
         raster_source = RasterioSourceConfig(
             channel_order=[0, 1, 2], uris=[raster_uri])
         label_source = ChipClassificationLabelSourceConfig(
             vector_source=GeoJSONVectorSourceConfig(
                 uris=label_uri,
-                ignore_crs_field=True,
                 transformers=[
                     ClassInferenceTransformerConfig(default_class_id=1)
                 ]),
             ioa_thresh=0.5,
             use_intersection_over_cell=False,
             pick_min_class_id=False,
             background_class_id=0,
@@ -119,30 +118,32 @@
     train_scenes = [make_scene(info) for info in train_scene_info]
     val_scenes = [make_scene(info) for info in val_scene_info]
     scene_dataset = DatasetConfig(
         class_config=class_config,
         train_scenes=train_scenes,
         validation_scenes=val_scenes)
 
-    if nochip:
-        window_opts = {}
-        for s in train_scenes:
-            window_opts[s.id] = GeoDataWindowConfig(
-                method=GeoDataWindowMethod.sliding,
-                size=chip_sz,
-                stride=chip_sz // 2)
-        for s in val_scenes:
-            window_opts[s.id] = GeoDataWindowConfig(
-                method=GeoDataWindowMethod.sliding,
-                size=chip_sz,
-                stride=chip_sz // 2)
+    window_sampling_opts = {}
+    for s in train_scenes:
+        window_sampling_opts[s.id] = WindowSamplingConfig(
+            method=WindowSamplingMethod.sliding,
+            size=chip_sz,
+            stride=chip_sz // 2)
+    for s in val_scenes:
+        window_sampling_opts[s.id] = WindowSamplingConfig(
+            method=WindowSamplingMethod.sliding,
+            size=chip_sz,
+            stride=chip_sz // 2)
 
+    chip_options = ChipOptions(sampling=window_sampling_opts)
+
+    if nochip:
         data = ClassificationGeoDataConfig(
             scene_dataset=scene_dataset,
-            window_opts=window_opts,
+            sampling=window_sampling_opts,
             img_sz=img_sz,
             num_workers=4)
     else:
         data = ClassificationImageDataConfig(img_sz=img_sz, num_workers=4)
 
     if external_model:
         model = ClassificationModelConfig(
@@ -169,29 +170,27 @@
                 'gamma': 2
             })
     else:
         external_loss_def = None
 
     solver = SolverConfig(
         lr=1e-4,
-        num_epochs=20,
-        test_num_epochs=4,
+        num_epochs=20 if not test else 4,
         batch_sz=32,
         one_cycle=True,
         external_loss_def=external_loss_def)
 
     backend = PyTorchChipClassificationConfig(
         data=data,
         model=model,
         solver=solver,
-        test_mode=test,
         log_tensorboard=True,
         run_tensorboard=False)
 
     pipeline = ChipClassificationConfig(
         root_uri=root_uri,
         dataset=scene_dataset,
         backend=backend,
-        train_chip_sz=chip_sz,
-        predict_chip_sz=chip_sz)
+        chip_options=chip_options,
+        predict_options=PredictOptions(chip_sz=chip_sz))
 
     return pipeline
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-# flake8: noqa
-
 import os
 from os.path import join
 
-from rastervision.core.rv_pipeline import *
-from rastervision.core.backend import *
-from rastervision.core.data import *
-from rastervision.core.analyzer import *
-from rastervision.pytorch_backend import *
-from rastervision.pytorch_learner import *
+from rastervision.core.rv_pipeline import (
+    ObjectDetectionConfig, ObjectDetectionChipOptions,
+    ObjectDetectionPredictOptions, WindowSamplingMethod,
+    ObjectDetectionWindowSamplingConfig)
+from rastervision.core.data import (
+    ClassConfig, ClassInferenceTransformerConfig, DatasetConfig,
+    GeoJSONVectorSourceConfig, ObjectDetectionLabelSourceConfig,
+    RasterioSourceConfig, SceneConfig)
+from rastervision.pytorch_backend import PyTorchObjectDetectionConfig
+from rastervision.pytorch_learner import (
+    Backbone, ExternalModuleConfig, ObjectDetectionGeoDataConfig,
+    ObjectDetectionImageDataConfig, ObjectDetectionModelConfig, PlotOptions,
+    SolverConfig)
 from rastervision.pytorch_backend.examples.utils import save_image_crop
 
 TRAIN_IDS = [
     '2_10', '2_11', '2_12', '2_14', '3_11', '3_13', '4_10', '5_10', '6_7',
     '6_9'
 ]
 VAL_IDS = ['2_13', '6_8', '3_10']
@@ -43,27 +48,31 @@
             available in the raster source will be used. If False, only
             IR, R, G (in that order) will be used. Defaults to False.
         external_model (bool, optional): If True, use an external model defined
             by the ExternalModuleConfig. Defaults to True.
         test (bool, optional): If True, does the following simplifications:
             (1) Uses only the first 2 scenes
             (2) Uses only a 2000x2000 crop of the scenes
-            (3) Enables test mode in the learner, which makes it use the
-                test_batch_sz and test_num_epochs, among other things.
+            (3) Trains for only 2 epochs.
             Defaults to False.
 
     Returns:
         ObjectDetectionConfig: A pipeline config.
     """
     train_ids = TRAIN_IDS
     val_ids = VAL_IDS
 
+    chip_sz = 300
+    img_sz = chip_sz
+    chips_per_scene = 100
+
     if test:
         train_ids = train_ids[:2]
         val_ids = val_ids[:2]
+        chips_per_scene = 10
 
     if multiband:
         channel_order = [0, 1, 2, 3]
         channel_display_groups = {'RGB': [0, 1, 2], 'IR': [3]}
     else:
         channel_order = [0, 1, 2]
         channel_display_groups = None
@@ -87,47 +96,43 @@
             raster_uri = crop_uri
 
         raster_source = RasterioSourceConfig(
             uris=[raster_uri], channel_order=channel_order)
 
         vector_source = GeoJSONVectorSourceConfig(
             uris=label_uri,
-            ignore_crs_field=True,
             transformers=[ClassInferenceTransformerConfig(default_class_id=0)])
         label_source = ObjectDetectionLabelSourceConfig(
             vector_source=vector_source)
 
         return SceneConfig(
             id=id, raster_source=raster_source, label_source=label_source)
 
     class_config = ClassConfig(names=['vehicle'], colors=['red'])
     scene_dataset = DatasetConfig(
         class_config=class_config,
         train_scenes=[make_scene(id) for id in train_ids],
         validation_scenes=[make_scene(id) for id in val_ids])
 
-    chip_sz = 300
-    img_sz = chip_sz
+    window_sampling_opts = ObjectDetectionWindowSamplingConfig(
+        method=WindowSamplingMethod.random,
+        size=chip_sz,
+        size_lims=(chip_sz, chip_sz + 1),
+        max_windows=chips_per_scene,
+        max_sample_attempts=100,
+        clip=True,
+        neg_ratio=5.0,
+        ioa_thresh=0.9,
+        neg_ioa_thresh=0.2)
 
-    chip_options = ObjectDetectionChipOptions(neg_ratio=5.0, ioa_thresh=0.9)
+    chip_options = ObjectDetectionChipOptions(sampling=window_sampling_opts)
     if nochip:
-        window_opts = ObjectDetectionGeoDataWindowConfig(
-            method=GeoDataWindowMethod.random,
-            size=chip_sz,
-            size_lims=(chip_sz, chip_sz + 1),
-            max_windows=500,
-            max_sample_attempts=100,
-            clip=True,
-            neg_ratio=chip_options.neg_ratio,
-            ioa_thresh=chip_options.ioa_thresh,
-            neg_ioa_thresh=0.2)
-
         data = ObjectDetectionGeoDataConfig(
             scene_dataset=scene_dataset,
-            window_opts=window_opts,
+            sampling=window_sampling_opts,
             img_sz=img_sz,
             num_workers=4,
             plot_options=PlotOptions(
                 channel_display_groups=channel_display_groups))
     else:
         data = ObjectDetectionImageDataConfig(
             img_sz=img_sz,
@@ -177,28 +182,26 @@
         model = ObjectDetectionModelConfig(backbone=Backbone.resnet18)
 
     backend = PyTorchObjectDetectionConfig(
         data=data,
         model=model,
         solver=SolverConfig(
             lr=1e-4,
-            num_epochs=10,
-            test_num_epochs=2,
+            num_epochs=10 if not test else 2,
             batch_sz=16,
-            one_cycle=True),
+            one_cycle=True,
+        ),
         log_tensorboard=False,
         run_tensorboard=False,
-        test_mode=test)
+    )
 
     predict_options = ObjectDetectionPredictOptions(
-        merge_thresh=0.5, score_thresh=0.9)
+        chip_sz=chip_sz, merge_thresh=0.5, score_thresh=0.9)
 
     pipeline = ObjectDetectionConfig(
         root_uri=root_uri,
         dataset=scene_dataset,
         backend=backend,
-        train_chip_sz=chip_sz,
-        predict_chip_sz=chip_sz,
         chip_options=chip_options,
         predict_options=predict_options)
 
     return pipeline
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/object_detection/xview.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/xview.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# flake8: noqa
-
 import os
 from os.path import join
 
-from rastervision.core.rv_pipeline import *
-from rastervision.core.backend import *
-from rastervision.core.data import *
-from rastervision.core.analyzer import *
-from rastervision.pytorch_backend import *
-from rastervision.pytorch_learner import *
+from rastervision.core.rv_pipeline import (
+    ObjectDetectionConfig, ObjectDetectionChipOptions,
+    ObjectDetectionPredictOptions, ObjectDetectionWindowSamplingConfig,
+    WindowSamplingMethod)
+from rastervision.core.data import (
+    ClassConfig, ClassInferenceTransformerConfig, DatasetConfig,
+    GeoJSONVectorSourceConfig, ObjectDetectionLabelSourceConfig,
+    RasterioSourceConfig, SceneConfig)
+from rastervision.pytorch_backend import PyTorchObjectDetectionConfig
+from rastervision.pytorch_learner import (
+    Backbone, ObjectDetectionGeoDataConfig, ObjectDetectionImageDataConfig,
+    ObjectDetectionModelConfig, SolverConfig)
 from rastervision.pytorch_backend.examples.utils import (get_scene_info,
                                                          save_image_crop)
 
 
 def get_config(runner,
                raw_uri: str,
                processed_uri: str,
@@ -31,16 +35,15 @@
         nochip (bool, optional): If True, read directly from the TIFF during
             training instead of from pre-generated chips. The analyze and chip
             commands should not be run, if this is set to True. Defaults to
             False.
         test (bool, optional): If True, does the following simplifications:
             (1) Uses only the first 2 scenes.
             (2) Uses only a 2000x2000 crop of the scenes.
-            (3) Enables test mode in the learner, which makes it use the
-                test_batch_sz and test_num_epochs, among other things.
+            (3) Trains for only 2 epochs.
             Defaults to False.
 
     Returns:
         ObjectDetectionConfig: A pipeline config.
     """
     train_scene_info = get_scene_info(join(processed_uri, 'train-scenes.csv'))
     val_scene_info = get_scene_info(join(processed_uri, 'val-scenes.csv'))
@@ -63,15 +66,14 @@
 
         raster_source = RasterioSourceConfig(
             uris=[raster_uri], channel_order=[0, 1, 2])
 
         label_source = ObjectDetectionLabelSourceConfig(
             vector_source=GeoJSONVectorSourceConfig(
                 uris=label_uri,
-                ignore_crs_field=True,
                 transformers=[
                     ClassInferenceTransformerConfig(default_class_id=0)
                 ]))
 
         return SceneConfig(
             id=id, raster_source=raster_source, label_source=label_source)
 
@@ -82,51 +84,48 @@
         class_config=class_config,
         train_scenes=train_scenes,
         validation_scenes=val_scenes)
 
     chip_sz = 300
     img_sz = chip_sz
 
-    chip_options = ObjectDetectionChipOptions(neg_ratio=1.0, ioa_thresh=0.8)
-
-    if nochip:
-        window_opts = ObjectDetectionGeoDataWindowConfig(
-            method=GeoDataWindowMethod.random,
+    chip_options = ObjectDetectionChipOptions(
+        sampling=ObjectDetectionWindowSamplingConfig(
+            method=WindowSamplingMethod.random,
             size=chip_sz,
             size_lims=(chip_sz, chip_sz + 1),
             max_windows=200,
             clip=True,
-            neg_ratio=chip_options.neg_ratio,
-            ioa_thresh=chip_options.ioa_thresh)
+            neg_ratio=1.0,
+            ioa_thresh=0.8))
 
+    if nochip:
         data = ObjectDetectionGeoDataConfig(
             scene_dataset=scene_dataset,
-            window_opts=window_opts,
+            sampling=chip_options.sampling,
             img_sz=img_sz,
             augmentors=[])
     else:
         data = ObjectDetectionImageDataConfig(img_sz=img_sz, num_workers=4)
 
-    predict_options = ObjectDetectionPredictOptions(
-        merge_thresh=0.1, score_thresh=0.5)
-
     backend = PyTorchObjectDetectionConfig(
         data=data,
         model=ObjectDetectionModelConfig(backbone=Backbone.resnet50),
         solver=SolverConfig(
             lr=1e-4,
-            num_epochs=10,
-            test_num_epochs=2,
+            num_epochs=10 if not test else 2,
             batch_sz=16,
-            one_cycle=True),
+            one_cycle=True,
+        ),
         log_tensorboard=True,
         run_tensorboard=False,
-        test_mode=test)
+    )
+
+    predict_options = ObjectDetectionPredictOptions(
+        chip_sz=chip_sz, merge_thresh=0.1, score_thresh=0.5)
 
     return ObjectDetectionConfig(
         root_uri=root_uri,
         dataset=scene_dataset,
         backend=backend,
-        train_chip_sz=chip_sz,
-        predict_chip_sz=chip_sz,
         chip_options=chip_options,
         predict_options=predict_options)
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-# flake8: noqa
-
-import os
+from typing import Optional
 from os.path import join, basename
 
-from rastervision.core.rv_pipeline import *
-from rastervision.core.backend import *
-from rastervision.core.data import *
-from rastervision.core.analyzer import *
-from rastervision.pytorch_backend import *
-from rastervision.pytorch_learner import *
-from rastervision.pytorch_backend.examples.utils import (get_scene_info,
-                                                         save_image_crop)
+import albumentations as A
+
+from rastervision.core.rv_pipeline import (
+    SemanticSegmentationConfig, SemanticSegmentationChipOptions,
+    SemanticSegmentationPredictOptions, WindowSamplingConfig,
+    WindowSamplingMethod)
+from rastervision.core.data import (
+    ClassConfig, DatasetConfig, PolygonVectorOutputConfig,
+    RasterioSourceConfig, RGBClassTransformerConfig, SceneConfig,
+    SemanticSegmentationLabelSourceConfig,
+    SemanticSegmentationLabelStoreConfig)
+from rastervision.pytorch_backend import PyTorchSemanticSegmentationConfig
+from rastervision.pytorch_learner import (
+    Backbone, ExternalModuleConfig, PlotOptions, SolverConfig,
+    SemanticSegmentationGeoDataConfig, SemanticSegmentationImageDataConfig,
+    SemanticSegmentationModelConfig)
+from rastervision.pytorch_backend.examples.utils import save_image_crop
 from rastervision.pytorch_backend.examples.semantic_segmentation.utils import (
     example_multiband_transform, example_rgb_transform, imagenet_stats,
     Unnormalize)
 
 TRAIN_IDS = [
     '2_10', '2_11', '3_10', '3_11', '4_10', '4_11', '4_12', '5_10', '5_11',
     '5_12', '6_10', '6_11', '6_7', '6_9', '7_10', '7_11', '7_12', '7_7', '7_8',
@@ -28,59 +35,69 @@
 CLASS_COLORS = [
     '#ffff00', '#0000ff', '#00ffff', '#00ff00', '#ffffff', '#ff0000'
 ]
 
 
 def get_config(runner,
                raw_uri: str,
-               processed_uri: str,
                root_uri: str,
+               processed_uri: Optional[str] = None,
                multiband: bool = False,
                external_model: bool = True,
                augment: bool = False,
                nochip: bool = True,
-               test: bool = False):
+               num_epochs: int = 10,
+               batch_sz: int = 8,
+               test: bool = False) -> SemanticSegmentationConfig:
     """Generate the pipeline config for this task. This function will be called
     by RV, with arguments from the command line, when this example is run.
 
     Args:
         runner (Runner): Runner for the pipeline. Will be provided by RV.
         raw_uri (str): Directory where the raw data resides
-        processed_uri (str): Directory for storing processed data.
-                             E.g. crops for testing.
         root_uri (str): Directory where all the output will be written.
+        processed_uri (str): Directory for storing processed data.
+                             E.g. crops for testing. Defaults to None.
         multiband (bool, optional): If True, all 4 channels (R, G, B, & IR)
             available in the raster source will be used. If False, only
             IR, R, G (in that order) will be used. Defaults to False.
         external_model (bool, optional): If True, use an external model defined
             by the ExternalModuleConfig. Defaults to True.
         augment (bool, optional): If True, use custom data augmentation
             transforms. Some basic data augmentation is done even if this is
             False. To completely disable, specify augmentors=[] is the dat
             config. Defaults to False.
         nochip (bool, optional): If True, read directly from the TIFF during
             training instead of from pre-generated chips. The analyze and chip
             commands should not be run, if this is set to True. Defaults to
             True.
+        num_epochs (int): Number of epochs to train for.
+        batch_sz (int): Batch size.
         test (bool, optional): If True, does the following simplifications:
             (1) Uses only the first 2 scenes
             (2) Uses only a 600x600 crop of the scenes
-            (3) Enables test mode in the learner, which makes it use the
-                test_batch_sz and test_num_epochs, among other things.
+            (3) Trains for only 2 epochs and uses a batch size of 2.
             Defaults to False.
 
     Returns:
         SemanticSegmentationConfig: A pipeline config.
     """
     train_ids = TRAIN_IDS
     val_ids = VAL_IDS
 
+    chip_sz = 300
+    img_sz = chip_sz
+    num_epochs = int(num_epochs)
+    batch_sz = int(batch_sz)
+
     if test:
         train_ids = train_ids[:2]
         val_ids = val_ids[:2]
+        num_epochs = 2
+        batch_sz = 2
 
     if multiband:
         # use all 4 channels
         channel_order = [0, 1, 2, 3]
         channel_display_groups = {'RGB': (0, 1, 2), 'IR': (3, )}
         aug_transform = example_multiband_transform
     else:
@@ -104,16 +121,17 @@
         base_transform = None
         plot_transform = None
 
     class_config = ClassConfig(names=CLASS_NAMES, colors=CLASS_COLORS)
 
     def make_scene(id) -> SceneConfig:
         id = id.replace('-', '_')
-        raster_uri = f'{raw_uri}/4_Ortho_RGBIR/top_potsdam_{id}_RGBIR.tif'
-        label_uri = f'{raw_uri}/5_Labels_for_participants/top_potsdam_{id}_label.tif'
+        raster_uri = join(raw_uri, f'4_Ortho_RGBIR/top_potsdam_{id}_RGBIR.tif')
+        label_uri = join(
+            raw_uri, f'5_Labels_for_participants/top_potsdam_{id}_label.tif')
 
         if test:
             crop_uri = join(processed_uri, 'crops', basename(raster_uri))
             label_crop_uri = join(processed_uri, 'crops', basename(label_uri))
             save_image_crop(
                 raster_uri,
                 crop_uri,
@@ -151,93 +169,83 @@
         return scene
 
     scene_dataset = DatasetConfig(
         class_config=class_config,
         train_scenes=[make_scene(id) for id in train_ids],
         validation_scenes=[make_scene(id) for id in val_ids])
 
-    chip_sz = 300
-    img_sz = chip_sz
+    window_sampling_opts = {}
+    # set window configs for training scenes
+    for s in scene_dataset.train_scenes:
+        window_sampling_opts[s.id] = WindowSamplingConfig(
+            method=WindowSamplingMethod.sliding, size=chip_sz, stride=chip_sz)
+
+    # set window configs for validation scenes
+    for s in scene_dataset.validation_scenes:
+        window_sampling_opts[s.id] = WindowSamplingConfig(
+            method=WindowSamplingMethod.sliding, size=chip_sz, stride=chip_sz)
 
     chip_options = SemanticSegmentationChipOptions(
-        window_method=SemanticSegmentationWindowMethod.sliding, stride=chip_sz)
+        sampling=window_sampling_opts)
 
     if nochip:
-        window_opts = {}
-        # set window configs for training scenes
-        for s in scene_dataset.train_scenes:
-            window_opts[s.id] = GeoDataWindowConfig(
-                method=GeoDataWindowMethod.sliding,
-                size=chip_sz,
-                stride=chip_options.stride)
-
-        # set window configs for validation scenes
-        for s in scene_dataset.validation_scenes:
-            window_opts[s.id] = GeoDataWindowConfig(
-                method=GeoDataWindowMethod.sliding,
-                size=chip_sz,
-                stride=chip_options.stride)
-
         data = SemanticSegmentationGeoDataConfig(
             scene_dataset=scene_dataset,
-            window_opts=window_opts,
+            sampling=window_sampling_opts,
             img_sz=img_sz,
             img_channels=len(channel_order),
             num_workers=4,
             base_transform=base_transform,
             aug_transform=aug_transform,
             plot_options=PlotOptions(
                 transform=plot_transform,
                 channel_display_groups=channel_display_groups))
     else:
         data = SemanticSegmentationImageDataConfig(
             img_sz=img_sz,
             num_workers=4,
-            channel_display_groups=channel_display_groups,
             base_transform=base_transform,
             aug_transform=aug_transform,
             plot_options=PlotOptions(
                 transform=plot_transform,
                 channel_display_groups=channel_display_groups))
 
     if external_model:
         class_config.ensure_null_class()
         num_classes = len(class_config)
         model = SemanticSegmentationModelConfig(
             external_def=ExternalModuleConfig(
-                github_repo='AdeelH/pytorch-fpn:0.2',
+                github_repo='AdeelH/pytorch-fpn:0.3',
                 name='fpn',
                 entrypoint='make_fpn_resnet',
                 entrypoint_kwargs={
                     'name': 'resnet50',
                     'fpn_type': 'panoptic',
                     'num_classes': num_classes,
                     'fpn_channels': 256,
                     'in_channels': len(channel_order),
                     'out_size': (img_sz, img_sz)
                 }))
     else:
         model = SemanticSegmentationModelConfig(backbone=Backbone.resnet50)
 
+    solver = SolverConfig(
+        lr=1e-4, num_epochs=num_epochs, batch_sz=batch_sz, one_cycle=True)
+
     backend = PyTorchSemanticSegmentationConfig(
         data=data,
         model=model,
-        solver=SolverConfig(
-            lr=1e-4,
-            num_epochs=10,
-            test_num_epochs=2,
-            batch_sz=8,
-            test_batch_sz=2,
-            one_cycle=True),
+        solver=solver,
         log_tensorboard=True,
         run_tensorboard=False,
-        test_mode=test)
+    )
+
+    predict_options = SemanticSegmentationPredictOptions(chip_sz=chip_sz)
 
     pipeline = SemanticSegmentationConfig(
         root_uri=root_uri,
         dataset=scene_dataset,
         backend=backend,
-        train_chip_sz=chip_sz,
-        predict_chip_sz=chip_sz,
-        chip_options=chip_options)
+        chip_options=chip_options,
+        predict_options=predict_options)
 
     return pipeline
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from functools import partial
 from typing import Tuple, Union
 
 from rastervision.core.rv_pipeline import (
     SceneConfig, DatasetConfig, SemanticSegmentationChipOptions,
-    SemanticSegmentationWindowMethod, SemanticSegmentationConfig)
+    SemanticSegmentationConfig, SemanticSegmentationPredictOptions,
+    WindowSamplingConfig, WindowSamplingMethod)
 
 from rastervision.core.data import (
     ClassConfig, RasterioSourceConfig, MultiRasterSourceConfig,
     SemanticSegmentationLabelSourceConfig,
     SemanticSegmentationLabelStoreConfig, PolygonVectorOutputConfig,
     RGBClassTransformerConfig)
 
 from rastervision.pytorch_backend import (PyTorchSemanticSegmentationConfig,
                                           SemanticSegmentationModelConfig)
 from rastervision.pytorch_backend.examples.utils import (save_image_crop)
 from rastervision.pytorch_learner import (
     Backbone, SolverConfig, SemanticSegmentationImageDataConfig,
-    SemanticSegmentationGeoDataConfig, GeoDataWindowConfig,
-    GeoDataWindowMethod, PlotOptions)
+    SemanticSegmentationGeoDataConfig, PlotOptions)
 
 # -----------------------
 # Input files and paths
 # -----------------------
 RGBIR_DIR = '4_Ortho_RGBIR'
 ELEVATION_DIR = 'elevation'
 LABEL_DIR = '5_Labels_for_participants'
@@ -92,16 +92,15 @@
         nochip (bool, optional): If True, read directly from the TIFF during
             training instead of from pre-generated chips. The analyze and chip
             commands should not be run, if this is set to True. Defaults to
             True.
         test (bool, optional): If True, does the following simplifications:
             (1) Uses only the first 2 scenes
             (2) Uses only a 600x600 crop of the scenes
-            (3) Enables test mode in the learner, which makes it use the
-                test_batch_sz and test_num_epochs, among other things.
+            (3) Trains for only 2 epochs and uses a batch size of 2.
             Defaults to False.
 
     Returns:
         SemanticSegmentationConfig: A pipeline config.
     """
     if not test:
         train_ids, val_ids = TRAIN_IDS, VAL_IDS
@@ -121,26 +120,23 @@
 
     dataset_config = DatasetConfig(
         class_config=class_config,
         train_scenes=[_make_scene(scene_id) for scene_id in train_ids],
         validation_scenes=[_make_scene(scene_id) for scene_id in val_ids])
 
     chip_options = SemanticSegmentationChipOptions(
-        window_method=SemanticSegmentationWindowMethod.sliding,
-        stride=CHIP_SIZE)
-
-    if nochip:
-        window_opts = GeoDataWindowConfig(
-            method=GeoDataWindowMethod.sliding,
+        sampling=WindowSamplingConfig(
+            method=WindowSamplingMethod.sliding,
             size=CHIP_SIZE,
-            stride=chip_options.stride)
+            stride=CHIP_SIZE))
 
+    if nochip:
         data = SemanticSegmentationGeoDataConfig(
             scene_dataset=dataset_config,
-            window_opts=window_opts,
+            sampling=chip_options.sampling,
             img_sz=CHIP_SIZE,
             num_workers=4,
             plot_options=PlotOptions(
                 channel_display_groups=CHANNEL_DISPLAY_GROUPS))
     else:
         data = SemanticSegmentationImageDataConfig(
             img_sz=CHIP_SIZE,
@@ -149,40 +145,38 @@
                 channel_display_groups=CHANNEL_DISPLAY_GROUPS))
 
     # --------------------------------------------
     # Configure PyTorch backend and training
     # --------------------------------------------
     model_config = SemanticSegmentationModelConfig(backbone=Backbone.resnet50)
 
+    num_epochs = NUM_EPOCHS if not test else TEST_MODE_NUM_EPOCHS
+    batch_sz = BATCH_SIZE if not test else TEST_MODE_BATCH_SIZE
     solver_config = SolverConfig(
-        lr=LR,
-        num_epochs=NUM_EPOCHS,
-        batch_sz=BATCH_SIZE,
-        test_num_epochs=TEST_MODE_NUM_EPOCHS,
-        test_batch_sz=TEST_MODE_BATCH_SIZE,
-        one_cycle=ONE_CYCLE)
+        lr=LR, num_epochs=num_epochs, batch_sz=batch_sz, one_cycle=ONE_CYCLE)
 
     backend_config = PyTorchSemanticSegmentationConfig(
         data=data,
         model=model_config,
         solver=solver_config,
         log_tensorboard=LOG_TENSORBOARD,
         run_tensorboard=RUN_TENSORBOARD,
-        test_mode=test)
+    )
+
+    predict_options = SemanticSegmentationPredictOptions(chip_sz=CHIP_SIZE)
 
     # -----------------------------------------------
     # Pass configurations to the pipeline config
     # -----------------------------------------------
     pipeline_config = SemanticSegmentationConfig(
         root_uri=root_uri,
-        train_chip_sz=CHIP_SIZE,
-        predict_chip_sz=CHIP_SIZE,
-        chip_options=chip_options,
         dataset=dataset_config,
-        backend=backend_config)
+        backend=backend_config,
+        chip_options=chip_options,
+        predict_options=predict_options)
 
     return pipeline_config
 
 
 ####################
 # Utils
 ####################
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-# flake8: noqa
-
 from typing import Optional
 import re
 import random
 import os
 from abc import abstractmethod
 
-from rastervision.pipeline.file_system import list_paths
-from rastervision.core.rv_pipeline import *
-from rastervision.core.backend import *
-from rastervision.core.data import *
-from rastervision.pytorch_backend import *
-from rastervision.pytorch_learner import *
+from rastervision.pipeline.file_system.utils import list_paths
+from rastervision.core.rv_pipeline import (
+    SemanticSegmentationConfig, SemanticSegmentationChipOptions,
+    SemanticSegmentationPredictOptions, WindowSamplingConfig,
+    WindowSamplingMethod)
+from rastervision.core.data import (
+    BufferTransformerConfig, ClassConfig, ClassInferenceTransformerConfig,
+    DatasetConfig, GeoJSONVectorSourceConfig, PolygonVectorOutputConfig,
+    RasterioSourceConfig, RasterizedSourceConfig, RasterizerConfig,
+    SceneConfig, SemanticSegmentationLabelSourceConfig,
+    SemanticSegmentationLabelStoreConfig, StatsTransformerConfig)
+from rastervision.pytorch_backend import PyTorchSemanticSegmentationConfig
+from rastervision.pytorch_learner import (
+    Backbone, SolverConfig, SemanticSegmentationGeoDataConfig,
+    SemanticSegmentationImageDataConfig, SemanticSegmentationModelConfig)
 
 BUILDINGS = 'buildings'
 ROADS = 'roads'
 
 
 class SpacenetConfig(object):
     def __init__(self, raw_uri):
@@ -24,29 +31,30 @@
     @staticmethod
     def create(raw_uri, target):
         if target.lower() == BUILDINGS:
             return VegasBuildings(raw_uri)
         elif target.lower() == ROADS:
             return VegasRoads(raw_uri)
         else:
-            raise ValueError('{} is not a valid target.'.format(target))
+            raise ValueError(f'{target} is not a valid target.')
 
     def get_raster_source_uri(self, id):
+        filename = f'{self.raster_fn_prefix}{id}.tif'
         return os.path.join(self.raw_uri, self.base_dir, self.raster_dir,
-                            '{}{}.tif'.format(self.raster_fn_prefix, id))
+                            filename)
 
     def get_geojson_uri(self, id):
+        filename = f'{self.label_fn_prefix}{id}.geojson'
         return os.path.join(self.raw_uri, self.base_dir, self.label_dir,
-                            '{}{}.geojson'.format(self.label_fn_prefix, id))
+                            filename)
 
     def get_scene_ids(self):
         label_dir = os.path.join(self.raw_uri, self.base_dir, self.label_dir)
         label_paths = list_paths(label_dir, ext='.geojson')
-        label_re = re.compile(r'.*{}(\d+)\.geojson'.format(
-            self.label_fn_prefix))
+        label_re = re.compile(rf'.*{self.label_fn_prefix}(\d+)\.geojson')
         scene_ids = [
             label_re.match(label_path).group(1) for label_path in label_paths
         ]
         return scene_ids
 
     @abstractmethod
     def get_class_config(self):
@@ -101,15 +109,14 @@
         uris=[image_uri],
         channel_order=channel_order,
         transformers=[StatsTransformerConfig()])
 
     # Set a line buffer to convert line strings to polygons.
     vector_source = GeoJSONVectorSourceConfig(
         uris=label_uri,
-        ignore_crs_field=True,
         transformers=[
             ClassInferenceTransformerConfig(default_class_id=0),
             BufferTransformerConfig(
                 geom_type='LineString', class_bufs={0: 15}),
             BufferTransformerConfig(geom_type='Point'),
         ])
     label_source = SemanticSegmentationLabelSourceConfig(
@@ -143,16 +150,15 @@
         target (str): "buildings" | "roads". Defaults to "buildings".
         nochip (bool, optional): If True, read directly from the TIFF during
             training instead of from pre-generated chips. The analyze and chip
             commands should not be run, if this is set to True. Defaults to
             True.
         test (bool, optional): If True, does the following simplifications:
             (1) Uses only a small subset of training and validation scenes.
-            (2) Enables test mode in the learner, which makes it use the
-                test_batch_sz and test_num_epochs, among other things.
+            (2) Trains for only 2 epochs.
             Defaults to False.
 
     Returns:
         SemanticSegmentationConfig: An pipeline config.
     """
 
     spacenet_cfg = SpacenetConfig.create(raw_uri, target)
@@ -175,59 +181,52 @@
     val_ids = scene_ids[num_train_ids:]
 
     if test:
         train_ids = train_ids[:16]
         val_ids = val_ids[:4]
 
     channel_order = [0, 1, 2]
+    chip_sz = 325
+    img_sz = chip_sz
 
     class_config = spacenet_cfg.get_class_config()
     train_scenes = [
         build_scene(spacenet_cfg, id, channel_order) for id in train_ids
     ]
     val_scenes = [
         build_scene(spacenet_cfg, id, channel_order) for id in val_ids
     ]
     scene_dataset = DatasetConfig(
         class_config=class_config,
         train_scenes=train_scenes,
         validation_scenes=val_scenes)
 
-    chip_sz = 325
-    img_sz = chip_sz
-
     chip_options = SemanticSegmentationChipOptions(
-        window_method=SemanticSegmentationWindowMethod.sliding, stride=chip_sz)
+        sampling=WindowSamplingConfig(
+            method=WindowSamplingMethod.sliding, size=chip_sz, stride=chip_sz))
 
     if nochip:
         data = SemanticSegmentationGeoDataConfig(
             scene_dataset=scene_dataset,
-            window_opts=GeoDataWindowConfig(
-                method=GeoDataWindowMethod.sliding,
-                size=chip_sz,
-                stride=chip_options.stride),
+            sampling=chip_options.sampling,
             img_sz=img_sz,
             num_workers=4)
     else:
         data = SemanticSegmentationImageDataConfig(
             img_sz=img_sz, num_workers=4)
 
     backend = PyTorchSemanticSegmentationConfig(
         data=data,
         model=SemanticSegmentationModelConfig(backbone=Backbone.resnet50),
-        solver=SolverConfig(
-            lr=1e-4,
-            num_epochs=5,
-            test_num_epochs=2,
-            batch_sz=8,
-            one_cycle=True),
+        solver=SolverConfig(lr=1e-4, num_epochs=5, batch_sz=8, one_cycle=True),
         log_tensorboard=True,
         run_tensorboard=False,
-        test_mode=test)
+    )
+
+    predict_options = SemanticSegmentationPredictOptions(chip_sz=chip_sz)
 
     return SemanticSegmentationConfig(
         root_uri=root_uri,
         dataset=scene_dataset,
         backend=backend,
-        train_chip_sz=chip_sz,
-        predict_chip_sz=chip_sz,
-        chip_options=chip_options)
+        chip_options=chip_options,
+        predict_options=predict_options)
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         A.FancyPCA(),
         A.HueSaturationValue(hue_shift_limit=10),
         A.RGBShift(),
         A.ToGray(),
         A.ToSepia(),
     ]),
     A.OneOf([
-        A.RandomBrightness(),
+        A.RandomBrightnessContrast(),
         A.RandomGamma(),
     ]),
     A.OneOf([
         A.GaussNoise(),
         A.ISONoise(),
         A.RandomFog(),
     ]),
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/test.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any
 from genericpath import exists
 from pprint import pformat
 import subprocess
-from os.path import (basename, isdir, isfile, join, relpath, split)
+from os.path import basename, join, relpath, split
 from tempfile import TemporaryDirectory
 
 import click
 
 from rastervision.pipeline.file_system import (
-    file_to_json, sync_from_dir, upload_or_copy, download_or_copy, file_exists,
-    sync_to_dir, NotReadableError, download_if_needed)
+    file_to_json, sync_from_dir, download_or_copy, file_exists, sync_to_dir,
+    NotReadableError, download_if_needed)
 
-NEW_VERSION_FULL = '0.21.2'
-NEW_VERSION_MAJOR_MINOR = '0.21'
+NEW_VERSION_FULL = '0.30.0'  # x.y.z
+NEW_VERSION_MAJOR_MINOR = '0.30'  # x.y
 
 EXAMPLES_MODULE_ROOT = 'rastervision.pytorch_backend.examples'
 EXAMPLES_PATH_ROOT = '/opt/src/rastervision_pytorch_backend/rastervision/pytorch_backend/examples'  # noqa
 REMOTE_PROCESSED_ROOT = f's3://raster-vision/examples/{NEW_VERSION_FULL}/processed-data'
 REMOTE_OUTPUT_ROOT = f's3://raster-vision/examples/{NEW_VERSION_FULL}/output'
 LOCAL_RAW_ROOT = '/opt/data/raw-data'
 LOCAL_PROCESSED_ROOT = '/opt/data/examples/processed-data'
@@ -143,15 +143,15 @@
 # --------------------
 @test.command()
 @click.argument('keys', nargs=-1)
 @click.option('--test', is_flag=True, help='Do short test run')
 @click.option('--remote', is_flag=True, default=False)
 @click.option(
     '--commands',
-    help='Space-separated string with RV commansd to run.',
+    help='Space-separated string with RV command to run.',
     default=None)
 @click.option(
     '--overrides',
     '-o',
     type=(str, str),
     multiple=True,
     metavar='KEY VALUE',
@@ -201,14 +201,15 @@
     """Download outputs of paths for each example.
 
     By default, only downloads eval and bundle.
     """
     overrides = dict(overrides)
     if paths is None:
         paths = [
+            'analyze',
             'train/model-bundle.zip',
             'train/last-model.pth',
             'eval',
             'bundle',
         ]
     else:
         paths = paths.split(' ')
@@ -224,19 +225,20 @@
                 override_cfg(exp_cfg, overrides)
             dirs[key] = {}
             uris = exp_cfg['remote'] if remote else exp_cfg['local']
             root_uri = uris['root_uri']
             for path in paths:
                 src_uri = join(root_uri, path)
                 console_info(f'{key}: Fetching {path}')
+                dst_dir = None
                 if file_exists(src_uri, include_dir=False):
                     # is a single file
                     dst_dir = join(collect_dir, key, split(path)[0])
                     dst_dir = split(to_local_uri(src_uri, dst_dir))[0]
-                    download_or_copy(src_uri, dst_dir)
+                    download_or_copy(src_uri, dst_dir, delete_tmp=True)
                 elif file_exists(src_uri, include_dir=True):
                     # is a directory
                     dst_dir = join(collect_dir, key, path)
                     sync_from_dir(src_uri, dst_dir)
                 else:
                     # does not exist
                     console_failure(f'File or dir not found: {src_uri}.')
@@ -284,35 +286,35 @@
 # --------------------
 @test.command()
 @click.option('--root_uri_old', default=None)
 @click.option('--root_uri_new', default=None)
 @click.option('--examples_root_old', default=None)
 @click.option('--examples_root_new', default=None)
 @click.option('--download_dir', '-d', default=LOCAL_COLLECT_ROOT)
-def compare(root_uri_old: Optional[str],
-            root_uri_new: Optional[str],
-            examples_root_old: Optional[str] = None,
-            examples_root_new: Optional[str] = None,
-            download_dir: Optional[str] = LOCAL_COLLECT_ROOT) -> None:
+def compare(root_uri_old: str | None,
+            root_uri_new: str | None,
+            examples_root_old: str | None = None,
+            examples_root_new: str | None = None,
+            download_dir: str | None = LOCAL_COLLECT_ROOT) -> None:
     """Compare different runs of the same example."""
     if root_uri_old is None and root_uri_new is None:
         assert examples_root_old is not None and examples_root_new is not None
         for exp_cfg in cfg:
             key = exp_cfg['key']
             root_uri_old = join(examples_root_old, key)
             root_uri_new = join(examples_root_new, key)
             console_info(f'Comparing\n- {root_uri_old}\n- {root_uri_new}')
             _compare(root_uri_old, root_uri_new, download_dir)
         return
     return _compare(root_uri_old, root_uri_new, download_dir)
 
 
-def _compare(root_uri_old: Optional[str],
-             root_uri_new: Optional[str],
-             download_dir: Optional[str] = None) -> None:
+def _compare(root_uri_old: str | None,
+             root_uri_new: str | None,
+             download_dir: str | None = None) -> None:
     """Compare different runs of the same example."""
     if root_uri_old != '/':
         root_uri_old = root_uri_old.rstrip('/')
     if root_uri_new != '/':
         root_uri_new = root_uri_new.rstrip('/')
     if download_dir is not None:
         return _compare_runs(root_uri_old, root_uri_new, download_dir)
@@ -346,24 +348,24 @@
     for exp_cfg in cfg:
         key = exp_cfg['key']
         if run_all or key in keys:
             if len(keys) == 1:
                 override_cfg(exp_cfg, overrides)
             _collect_dir = join(collect_dir, key)
             _upload_dir = join(upload_dir, key)
-            _upload_to_zoo(exp_cfg, _collect_dir, _upload_dir)
+            sync_to_dir(_collect_dir, _upload_dir)
 
 
 ######################
 # utils
 ######################
 def _run(exp_cfg: dict,
          test: bool = False,
          remote: bool = False,
-         commands: List[str] = None) -> None:
+         commands: list[str] = None) -> None:
     """Builds a command from the params in exp_cfg and other arguments and
     then executes it.
     """
     uris = exp_cfg['remote'] if remote else exp_cfg['local']
     cmd = ['rastervision']
     rv_profile = exp_cfg.get('rv_profile')
     if rv_profile is not None:
@@ -408,51 +410,17 @@
     out_uri = join(pred_dir, f'sample-pred-{key}{pred_ext}')
     cmd = [
         'rastervision', 'predict', model_bundle_uri, sample_uri_dst, out_uri
     ]
     run_command(cmd)
 
 
-def _upload_to_zoo(exp_cfg: dict, collect_dir: str, upload_dir: str) -> None:
-    src_uris = {}
-    dst_uris = {}
-
-    src_uris['eval'] = join(collect_dir, 'eval', 'validation_scenes',
-                            'eval.json')
-    src_uris['bundle'] = join(collect_dir, 'bundle', 'model-bundle.zip')
-    src_uris['sample_predictions'] = join(collect_dir, 'sample-predictions')
-    src_uris['learner_bundle'] = join(collect_dir, 'train', 'model-bundle.zip')
-    src_uris['learner_model'] = join(collect_dir, 'train', 'last-model.pth')
-
-    dst_uris['eval'] = join(upload_dir, 'validation_scenes', 'eval.json')
-    dst_uris['bundle'] = join(upload_dir, 'model-bundle.zip')
-    dst_uris['sample_predictions'] = join(upload_dir, 'sample-predictions')
-    dst_uris['learner_bundle'] = join(upload_dir, 'train', 'model-bundle.zip')
-    dst_uris['learner_model'] = join(upload_dir, 'model.pth')
-
-    assert len(src_uris) == len(dst_uris)
-
-    for k, src in src_uris.items():
-        dst = dst_uris[k]
-        if not exists(src):
-            console_failure(f'{k}: {src} not found.')
-            exit(1)
-        if isfile(src):
-            console_info(f'Uploading {k} file: {src} to {dst}.')
-            upload_or_copy(src, dst)
-        elif isdir(src):
-            console_info(f'Syncing {k} dir: {src} to {dst}.')
-            sync_to_dir(src, dst)
-        else:
-            raise ValueError(src)
-
-
 def _compare_runs(root_uri_old: str,
                   root_uri_new: str,
-                  download_dir: Optional[str],
+                  download_dir: str | None,
                   commands=['eval']) -> None:
     """Compare outputs of commands for two runs of an example.
     Currently only supports eval, but can be extended to include others.
     """
     for cmd in commands:
         key_old = basename(root_uri_old)
         key_new = basename(root_uri_new)
@@ -479,15 +447,15 @@
         eval_old = file_to_json(download_if_needed(eval_json_old))
     eval_json_new = join(root_uri_new, 'validation_scenes', 'eval.json')
     eval_new = file_to_json(download_if_needed(eval_json_new))
     _compare_dicts(
         eval_old, eval_new, float_tol=float_tol, exclude_keys=exclude_keys)
 
 
-def validate_keys(keys: List[str]) -> None:
+def validate_keys(keys: list[str]) -> None:
     exp_keys = [exp_cfg['key'] for exp_cfg in cfg]
     invalid_keys = set(keys).difference(exp_keys)
     if invalid_keys:
         raise ValueError('{} are invalid keys'.format(', '.join(invalid_keys)))
 
 
 def run_command(cmd: str) -> None:
@@ -533,24 +501,23 @@
     console_info(f'Fetching {cmd} directory: {cmd_root_uri}')
     cmd_root_uri_local = to_local_uri(
         cmd_root_uri, download_dir, full_path=False)
     sync_from_dir(cmd_root_uri, cmd_root_uri_local)
     return cmd_root_uri_local
 
 
-def flatten_dict(d: Union[dict, list], sep: str = '.') -> dict:
+def flatten_dict(d: dict | list, sep: str = '.') -> dict:
     """Flatten a dict so that it does not have any nested dicts or lists.
     Nested keys will be concatenated using the separator, sep. For example,
     {'a': {'b': ['x', 10]}} becomes {'a.b.0': 'x', 'a.b.1': 10}.
     This makes it simpler to compare dicts.
 
     Args:
-        d (Union[dict, list]): A dict or list.
-        sep (str, optional): Separator to use for concatenating nested keys.
-            Defaults to '.'.
+        d: A dict or list.
+        sep: Separator to use for concatenating nested keys. Defaults to '.'.
 
     Returns:
         dict: The flattened dict.
     """
     if not isinstance(d, (dict, list)):
         return d
 
@@ -586,15 +553,15 @@
         dict_new (dict): A dict.
         float_tol (float, optional): Count float values as different if the
             abs difference exceeds this threshold. Defaults to 1e-3.
         exclude_keys (list, optional): Ignore the following keys when
             comparing values. Defaults to [].
     """
     dict_old = flatten_dict(dict_old)
-    dict_new: Dict[str, Any] = flatten_dict(dict_new)
+    dict_new: dict[str, Any] = flatten_dict(dict_new)
     keys_old, keys_new = set(dict_old.keys()), set(dict_new.keys())
     diff1, diff2 = keys_new - keys_old, keys_old - keys_new
     if len(diff1) > 0:
         console_failure(f'Missing keys in old: {keys_new - keys_old}')
     if len(diff2) > 0:
         console_failure(f'Missing keys in new: {keys_old - keys_new}')
     if len(diff1) + len(diff2) == 0:
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/tiny_spacenet.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/tiny_spacenet.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rastervision.core.backend import *
 from rastervision.core.data import *
 from rastervision.pytorch_backend import *
 from rastervision.pytorch_learner import *
 
 
 def get_config(runner) -> SemanticSegmentationConfig:
-    output_root_uri = '/opt/data/output/'
+    output_root_uri = '/opt/data/output/tiny_spacenet'
     class_config = ClassConfig(
         names=['building', 'background'], colors=['red', 'black'])
 
     base_uri = ('https://s3.amazonaws.com/azavea-research-public-data/'
                 'raster-vision/examples/spacenet')
     train_image_uri = join(base_uri, 'RGB-PanSharpen_AOI_2_Vegas_img205.tif')
     train_label_uri = join(base_uri, 'buildings_AOI_2_Vegas_img205.geojson')
@@ -31,30 +31,29 @@
 
     # Use the PyTorch backend for the SemanticSegmentation pipeline.
     chip_sz = 300
 
     backend = PyTorchSemanticSegmentationConfig(
         data=SemanticSegmentationGeoDataConfig(
             scene_dataset=scene_dataset,
-            window_opts=GeoDataWindowConfig(
+            sampling=WindowSamplingConfig(
                 # randomly sample training chips from scene
-                method=GeoDataWindowMethod.random,
+                method=WindowSamplingMethod.random,
                 # ... of size chip_sz x chip_sz
                 size=chip_sz,
                 # ... and at most 10 chips per scene
                 max_windows=10)),
         model=SemanticSegmentationModelConfig(backbone=Backbone.resnet50),
         solver=SolverConfig(lr=1e-4, num_epochs=1, batch_sz=2))
 
     return SemanticSegmentationConfig(
         root_uri=output_root_uri,
         dataset=scene_dataset,
         backend=backend,
-        train_chip_sz=chip_sz,
-        predict_chip_sz=chip_sz)
+        predict_options=SemanticSegmentationPredictOptions(chip_sz=chip_sz))
 
 
 def make_scene(scene_id: str, image_uri: str, label_uri: str,
                class_config: ClassConfig) -> SceneConfig:
     """Define a Scene with image and labels from the given URIs."""
 
     raster_source = RasterioSourceConfig(
@@ -62,20 +61,17 @@
         # use only the first 3 bands
         channel_order=[0, 1, 2],
     )
 
     # configure GeoJSON reading
     vector_source = GeoJSONVectorSourceConfig(
         uris=label_uri,
-        # This assumes the CRS is WGS-84 and ignores whatever the CRS specified
-        # in the file is.
-        ignore_crs_field=True,
         # The geoms in the label GeoJSON do not have a "class_id" property, so
         # classes must be inferred. Since all geoms are for the building class,
-        # this is easy to do: we just assing the building class ID to all of
+        # this is easy to do: we just assign the building class ID to all of
         # them.
         transformers=[
             ClassInferenceTransformerConfig(
                 default_class_id=class_config.get_class_id('building'))
         ])
     # configure transformation of vector data into semantic segmentation labels
     label_source = SemanticSegmentationLabelSourceConfig(
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/examples/utils.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TYPE_CHECKING, Optional
 import os
 import csv
 from io import StringIO
 
+from rastervision.pipeline.file_system.utils import file_exists
 from rastervision.core.data import (RasterioSource, GeoJSONVectorSource,
                                     ClassInferenceTransformer)
 from rastervision.core.data.utils import geoms_to_geojson, crop_geotiff
 from rastervision.pipeline.file_system import (file_to_str, json_to_file)
 from rastervision.aws_s3 import S3FileSystem
 
 if TYPE_CHECKING:
@@ -44,26 +45,28 @@
         default_class_id: default class ID to use to infer labels
         class_config: ClassConfig to use to infer labels
 
     Raises:
         ValueError if cannot find a crop satisfying min_features constraint.
     """
     print(f'Saving test crop to {image_crop_uri}...')
+    if file_exists(image_crop_uri):
+        print(f'Already exists. Skipping.')
+        return
     old_environ = os.environ.copy()
     try:
         request_payer = S3FileSystem.get_request_payer()
         if request_payer == 'requester':
             os.environ['AWS_REQUEST_PAYER'] = request_payer
         rs = RasterioSource(image_uri, allow_streaming=True)
         if label_uri and vector_labels:
             crs_tf = rs.crs_transformer
             vs = GeoJSONVectorSource(
                 uris=label_uri,
                 crs_transformer=crs_tf,
-                ignore_crs_field=True,
                 vector_transformers=[
                     ClassInferenceTransformer(
                         default_class_id=default_class_id,
                         class_config=class_config)
                 ])
             labels_df = vs.get_dataframe()
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_chip_classification_config.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rastervision.pytorch_learner.classification_learner_config import (
     ClassificationModelConfig, ClassificationLearnerConfig,
     ClassificationImageDataConfig)
 from rastervision.pytorch_backend.pytorch_chip_classification import (
     PyTorchChipClassification)
 
 
-def clf_learner_backend_config_upgrader(cfg_dict, version):
+def clf_learner_backend_config_upgrader(cfg_dict, version):  # pragma: no cover
     if version == 0:
         fields = {
             'augmentors': default_augmentors,
             'group_uris': None,
             'group_train_sz': None,
             'group_train_sz_rel': None,
             'num_workers': 4,
@@ -46,15 +46,14 @@
     model: ClassificationModelConfig
 
     def get_learner_config(self, pipeline):
         learner = ClassificationLearnerConfig(
             data=self.data,
             model=self.model,
             solver=self.solver,
-            test_mode=self.test_mode,
             output_uri=pipeline.train_uri,
             log_tensorboard=self.log_tensorboard,
             run_tensorboard=self.run_tensorboard,
             save_all_checkpoints=self.save_all_checkpoints)
         learner.update()
         learner.validate_config()
         return learner
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_learner_backend_config.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,32 +7,36 @@
 from rastervision.core.rv_pipeline import RVPipelineConfig
 from rastervision.pytorch_learner.learner_config import (
     SolverConfig, ModelConfig, DataConfig, ImageDataConfig, GeoDataConfig)
 
 log = logging.getLogger(__name__)
 
 
-@register_config('pytorch_learner_backend')
+def pytorch_learner_backend_config_upgrader(cfg_dict: dict,
+                                            version: int) -> dict:
+    if version == 1:
+        # removed in version 2
+        cfg_dict.pop('test_mode', None)
+    return cfg_dict
+
+
+@register_config(
+    'pytorch_learner_backend',
+    upgrader=pytorch_learner_backend_config_upgrader)
 class PyTorchLearnerBackendConfig(BackendConfig):
     """Configure a :class:`.PyTorchLearnerBackend`."""
 
     model: ModelConfig
     solver: SolverConfig
     data: DataConfig
     log_tensorboard: bool = Field(
         True, description='If True, log events to Tensorboard log files.')
     run_tensorboard: bool = Field(
         False,
         description='If True, run Tensorboard server pointing at log files.')
-    test_mode: bool = Field(
-        False,
-        description=
-        ('This field is passed along to the LearnerConfig which is returned by '
-         'get_learner_config(). For more info, see the docs for'
-         'pytorch_learner.learner_config.LearnerConfig.test_mode.'))
     save_all_checkpoints: bool = Field(
         False,
         description=(
             'If True, all checkpoints would be saved. The latest checkpoint '
             'would be saved as `last-model.pth`. The checkpoints prior to '
             'last epoch are stored as `model-ckpt-epoch-{N}.pth` where `N` '
             'is the epoch number.'))
@@ -43,22 +47,16 @@
     def update(self, pipeline: Optional[RVPipelineConfig] = None):
         super().update(pipeline=pipeline)
 
         if isinstance(self.data, ImageDataConfig):
             if self.data.uri is None and self.data.group_uris is None:
                 self.data.uri = pipeline.chip_uri
 
-        if not self.data.class_names:
-            # We want to defer validating class_names against class_colors
-            # until we have updated both. Hence, we use Config.copy(update=)
-            # here because it does not trigger pydantic validators.
-            self.data = self.data.copy(
-                update={'class_names': pipeline.dataset.class_config.names})
-        if not self.data.class_colors:
-            self.data.class_colors = pipeline.dataset.class_config.colors
+        if self.data.class_config is None:
+            self.data.class_config = pipeline.dataset.class_config
 
         if not self.data.img_channels:
             self.data.img_channels = self.get_img_channels(pipeline)
 
     def get_learner_config(self, pipeline: Optional[RVPipelineConfig]):
         raise NotImplementedError()
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_object_detection_config.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from rastervision.pytorch_learner.object_detection_learner_config import (
     ObjectDetectionModelConfig, ObjectDetectionLearnerConfig,
     ObjectDetectionImageDataConfig)
 from rastervision.pytorch_backend.pytorch_object_detection import (
     PyTorchObjectDetection)
 
 
-def objdet_learner_backend_config_upgrader(cfg_dict, version):
+def objdet_learner_backend_config_upgrader(cfg_dict,
+                                           version):  # pragma: no cover
     if version == 0:
         fields = {
             'augmentors': default_augmentors,
             'group_uris': None,
             'group_train_sz': None,
             'group_train_sz_rel': None,
             'num_workers': 4,
@@ -46,15 +47,14 @@
     model: ObjectDetectionModelConfig
 
     def get_learner_config(self, pipeline):
         learner = ObjectDetectionLearnerConfig(
             data=self.data,
             model=self.model,
             solver=self.solver,
-            test_mode=self.test_mode,
             output_uri=pipeline.train_uri,
             log_tensorboard=self.log_tensorboard,
             run_tensorboard=self.run_tensorboard,
             save_all_checkpoints=self.save_all_checkpoints)
         learner.update()
         return learner
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py` & `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rastervision.pytorch_learner.semantic_segmentation_learner_config import (
     SemanticSegmentationModelConfig, SemanticSegmentationLearnerConfig,
     SemanticSegmentationImageDataConfig)
 from rastervision.pytorch_backend.pytorch_semantic_segmentation import (
     PyTorchSemanticSegmentation)
 
 
-def ss_learner_backend_config_upgrader(cfg_dict, version):
+def ss_learner_backend_config_upgrader(cfg_dict, version):  # pragma: no cover
     if version == 0:
         fields = {
             'augmentors': default_augmentors,
             'group_uris': None,
             'group_train_sz': None,
             'group_train_sz_rel': None,
             'num_workers': 4,
@@ -46,15 +46,14 @@
     model: SemanticSegmentationModelConfig
 
     def get_learner_config(self, pipeline):
         learner = SemanticSegmentationLearnerConfig(
             data=self.data,
             model=self.model,
             solver=self.solver,
-            test_mode=self.test_mode,
             output_uri=pipeline.train_uri,
             log_tensorboard=self.log_tensorboard,
             run_tensorboard=self.run_tensorboard,
             save_all_checkpoints=self.save_all_checkpoints)
         learner.update()
         learner.validate_config()
         return learner
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/PKG-INFO` & `rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-pytorch-backend
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds PyTorch backends for rastervision.core pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_backend-0.21.3/rastervision_pytorch_backend.egg-info/SOURCES.txt` & `rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 rastervision/pytorch_backend/pytorch_chip_classification_config.py
 rastervision/pytorch_backend/pytorch_learner_backend.py
 rastervision/pytorch_backend/pytorch_learner_backend_config.py
 rastervision/pytorch_backend/pytorch_object_detection.py
 rastervision/pytorch_backend/pytorch_object_detection_config.py
 rastervision/pytorch_backend/pytorch_semantic_segmentation.py
 rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py
+rastervision/pytorch_backend/utils.py
 rastervision/pytorch_backend/examples/__init__.py
 rastervision/pytorch_backend/examples/test.py
 rastervision/pytorch_backend/examples/tiny_spacenet.py
 rastervision/pytorch_backend/examples/utils.py
 rastervision/pytorch_backend/examples/chip_classification/__init__.py
 rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py
 rastervision/pytorch_backend/examples/object_detection/__init__.py
```

### Comparing `rastervision_pytorch_backend-0.21.3/setup.py` & `rastervision_pytorch_backend-0.30.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 # flake8: noqa
 
-from os import path as op
-import io
-from setuptools import (setup, find_namespace_packages)
-
-here = op.abspath(op.dirname(__file__))
-with io.open(op.join(here, 'requirements.txt'), encoding='utf-8') as f:
-    all_reqs = f.read().split('\n')
-install_requires = [x.strip() for x in all_reqs if 'git+' not in x]
+from os.path import abspath, dirname, join
+from setuptools import setup, find_namespace_packages
+import re
 
 name = 'rastervision_pytorch_backend'
-version = '0.21.3'
+version = '0.30.0'
 description = 'A rastervision plugin that adds PyTorch backends for rastervision.core pipelines'
+requirement_constraints = {}
+
+here = abspath(dirname(__file__))
+
+
+def parse_requirements(requirements_path: str) -> list[str]:
+    requirements = []
+    with open(requirements_path, 'r', encoding='utf-8') as f:
+        for line in f:
+            if 'git+' in line:
+                continue
+            # match package name, ignoring version constraints
+            match = re.match(r'^\s*([^\s<=>]+)', line)
+            if not match:
+                continue
+            package_name = match.group(1)
+            if package_name in requirement_constraints:
+                constraint = requirement_constraints[package_name]
+                package_name = f'{package_name}{constraint}'
+            requirements.append(package_name)
+    return requirements
+
 
 setup(
     name=name,
     version=version,
     description=description,
     url='https://github.com/azavea/raster-vision',
     author='Azavea',
@@ -26,9 +43,9 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     keywords=
     'raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing',
     packages=find_namespace_packages(exclude=['integration_tests*', 'tests*']),
-    install_requires=install_requires,
+    install_requires=parse_requirements(join(here, 'requirements.txt')),
     zip_safe=False)
```

