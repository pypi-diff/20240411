# Comparing `tmp/rastervision_pytorch_learner-0.21.3.tar.gz` & `tmp/rastervision_pytorch_learner-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_pytorch_learner-0.21.3.tar", last modified: Tue Oct 17 19:14:42 2023, max compression
+gzip compressed data, was "rastervision_pytorch_learner-0.30.0.tar", last modified: Wed Apr 10 22:11:09 2024, max compression
```

## Comparing `rastervision_pytorch_learner-0.21.3.tar` & `rastervision_pytorch_learner-0.30.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.347330 rastervision_pytorch_learner-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      564 2023-10-17 19:14:42.347330 rastervision_pytorch_learner-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.343330 rastervision_pytorch_learner-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.343330 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/
--rw-rw-r--   0 root         (0) root         (0)     3955 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1437 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/classification_learner.py
--rw-rw-r--   0 root         (0) root         (0)     6076 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/classification_learner_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.343330 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/
--rw-rw-r--   0 root         (0) root         (0)     1542 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5359 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/classification_dataset.py
--rw-rw-r--   0 root         (0) root         (0)    20177 2023-09-08 19:48:40.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/dataset.py
--rw-rw-r--   0 root         (0) root         (0)    12974 2023-09-08 19:48:40.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/object_detection_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     1979 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/regression_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     7109 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     8249 2023-10-16 20:22:55.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.343330 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/utils/
--rw-r--r--   0 root         (0) root         (0)      372 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-09-26 14:00:58.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/utils/aoi_sampler.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-10-16 20:21:57.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.343330 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/
--rw-r--r--   0 root         (0) root         (0)      645 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-09-08 19:48:40.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py
--rw-r--r--   0 root         (0) root         (0)     9600 2023-10-16 20:22:58.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/visualizer.py
--rw-rw-r--   0 root         (0) root         (0)    54038 2023-09-26 14:00:58.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/learner.py
--rw-rw-r--   0 root         (0) root         (0)    59591 2023-09-26 14:00:58.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/learner_config.py
--rw-rw-r--   0 root         (0) root         (0)      601 2023-08-22 15:58:07.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/learner_pipeline.py
--rw-rw-r--   0 root         (0) root         (0)      673 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/learner_pipeline_config.py
--rw-rw-r--   0 root         (0) root         (0)     6343 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/object_detection_learner.py
--rw-rw-r--   0 root         (0) root         (0)    10364 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/object_detection_learner_config.py
--rw-rw-r--   0 root         (0) root         (0)    14607 2023-09-26 14:00:58.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/object_detection_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4404 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/regression_learner.py
--rw-rw-r--   0 root         (0) root         (0)     8383 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/regression_learner_config.py
--rw-rw-r--   0 root         (0) root         (0)     4006 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/semantic_segmentation_learner.py
--rw-rw-r--   0 root         (0) root         (0)     8134 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/semantic_segmentation_learner_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.347330 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/utils/
--rw-rw-r--   0 root         (0) root         (0)      743 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5128 2023-09-08 19:48:40.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/utils/torch_hub.py
--rw-rw-r--   0 root         (0) root         (0)    17205 2023-09-08 19:48:40.000000 rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.347330 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/
--rw-r--r--   0 root         (0) root         (0)      564 2023-10-17 19:14:42.000000 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2256 2023-10-17 19:14:42.000000 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:42.000000 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:42.000000 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      329 2023-10-17 19:14:42.000000 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:42.000000 rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      329 2023-10-17 13:37:07.000000 rastervision_pytorch_learner-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:42.347330 rastervision_pytorch_learner-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1143 2023-10-17 13:37:07.000000 rastervision_pytorch_learner-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.247691 rastervision_pytorch_learner-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.247691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3813 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1888 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6605 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.247691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1542 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5360 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/classification_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    22638 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    12981 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/object_detection_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1979 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/regression_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7110 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8253 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/transform.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      278 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2574 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      645 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3345 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1259 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3590 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3284 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9916 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    70836 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    57769 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7031 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9205 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    14607 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4381 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8727 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4456 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8409 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1008 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3593 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/distributed.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4655 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/prediction.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5394 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/torch_hub.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    19003 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2192 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:49.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      168 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      285 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1731 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/setup.py
```

### Comparing `rastervision_pytorch_learner-0.21.3/PKG-INFO` & `rastervision_pytorch_learner-0.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_pytorch_learner
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds PyTorch training pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/__init__.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # flake8: noqa
+from typing import TYPE_CHECKING
 
+if TYPE_CHECKING:
+    from rastervision.pipeline import Registry
 
-def register_plugin(registry):
-    registry.set_plugin_version('rastervision.pytorch_learner', 4)
+
+def register_plugin(registry: 'Registry'):
+    registry.set_plugin_version('rastervision.pytorch_learner', 7)
+    registry.register_renamed_type_hints('geo_data_window', 'window_sampling')
 
 
 import rastervision.pipeline
 from rastervision.pytorch_learner.learner_config import *
 from rastervision.pytorch_learner.learner import *
-from rastervision.pytorch_learner.learner_pipeline_config import *
-from rastervision.pytorch_learner.learner_pipeline import *
 from rastervision.pytorch_learner.classification_learner_config import *
 from rastervision.pytorch_learner.classification_learner import *
 from rastervision.pytorch_learner.regression_learner_config import *
 from rastervision.pytorch_learner.regression_learner import *
 from rastervision.pytorch_learner.semantic_segmentation_learner_config import *
 from rastervision.pytorch_learner.semantic_segmentation_learner import *
 from rastervision.pytorch_learner.object_detection_learner_config import *
 from rastervision.pytorch_learner.object_detection_learner import *
 from rastervision.pytorch_learner.dataset import *
 
 __all__ = [
-    # LearnerPipeline
-    LearnerPipeline.__name__,
-    LearnerPipelineConfig.__name__,
     # Learner
     Learner.__name__,
     SemanticSegmentationLearner.__name__,
     ClassificationLearner.__name__,
     ObjectDetectionLearner.__name__,
     RegressionLearner.__name__,
     # LearnerConfig
@@ -35,28 +35,25 @@
     SemanticSegmentationLearnerConfig.__name__,
     ClassificationLearnerConfig.__name__,
     ObjectDetectionLearnerConfig.__name__,
     RegressionLearnerConfig.__name__,
     # DataConfig
     DataConfig.__name__,
     GeoDataConfig.__name__,
-    GeoDataWindowConfig.__name__,
-    GeoDataWindowMethod.__name__,
     PlotOptions.__name__,
     ImageDataConfig.__name__,
     SemanticSegmentationDataConfig.__name__,
     SemanticSegmentationGeoDataConfig.__name__,
     SemanticSegmentationImageDataConfig.__name__,
     ClassificationDataConfig.__name__,
     ClassificationGeoDataConfig.__name__,
     ClassificationImageDataConfig.__name__,
     ObjectDetectionDataConfig.__name__,
     ObjectDetectionGeoDataConfig.__name__,
     ObjectDetectionImageDataConfig.__name__,
-    ObjectDetectionGeoDataWindowConfig.__name__,
     RegressionDataConfig.__name__,
     RegressionGeoDataConfig.__name__,
     RegressionImageDataConfig.__name__,
     PlotOptions.__name__,
     # DataFormat
     SemanticSegmentationDataFormat.__name__,
     ClassificationDataFormat.__name__,
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/classification_learner.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import warnings
 import logging
 
+import torch.distributed as dist
+
 from rastervision.pytorch_learner.learner import Learner
 from rastervision.pytorch_learner.utils import (
     compute_conf_mat_metrics, compute_conf_mat, aggregate_metrics)
 from rastervision.pytorch_learner.dataset.visualizer import (
     ClassificationVisualizer)
 
 warnings.filterwarnings('ignore')
@@ -31,14 +33,27 @@
         conf_mat = compute_conf_mat(out, y, num_labels)
 
         return {'val_loss': val_loss, 'conf_mat': conf_mat}
 
     def validate_end(self, outputs):
         metrics = aggregate_metrics(outputs, exclude_keys={'conf_mat'})
         conf_mat = sum([o['conf_mat'] for o in outputs])
-        conf_mat_metrics = compute_conf_mat_metrics(conf_mat,
-                                                    self.cfg.data.class_names)
+
+        if self.is_ddp_process:
+            metrics = self.reduce_distributed_metrics(metrics)
+            dist.reduce(conf_mat, dst=0, op=dist.ReduceOp.SUM)
+            if not self.is_ddp_master:
+                return metrics
+
+        ignored_idx = self.cfg.solver.ignore_class_index
+        if ignored_idx is not None and ignored_idx < 0:
+            ignored_idx += self.cfg.data.num_classes
+
+        class_names = self.cfg.data.class_names
+        conf_mat_metrics = compute_conf_mat_metrics(
+            conf_mat, class_names, ignore_idx=ignored_idx)
+
         metrics.update(conf_mat_metrics)
         return metrics
 
     def prob_to_pred(self, x):
         return x.argmax(-1)
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/classification_learner_config.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import Callable, Optional, Union
+from typing import TYPE_CHECKING, Callable, Iterable, Optional, Union
 from enum import Enum
 import logging
 
 import albumentations as A
 from torch import nn
 
 from rastervision.core.data import Scene
+from rastervision.core.rv_pipeline import WindowSamplingMethod
 from rastervision.pipeline.config import (Config, register_config, ConfigError)
 from rastervision.pytorch_learner.learner_config import (
-    LearnerConfig, ModelConfig, ImageDataConfig, GeoDataConfig,
-    GeoDataWindowMethod)
+    LearnerConfig, ModelConfig, ImageDataConfig, GeoDataConfig)
 from rastervision.pytorch_learner.dataset import (
     ClassificationImageDataset, ClassificationSlidingWindowGeoDataset,
     ClassificationRandomWindowGeoDataset)
 from rastervision.pytorch_learner.utils import adjust_conv_channels
 
+if TYPE_CHECKING:
+    from rastervision.core.data import SceneConfig
+
 log = logging.getLogger(__name__)
 
 
 class ClassificationDataFormat(Enum):
     image_folder = 'image_folder'
 
 
@@ -49,50 +52,64 @@
 @register_config('classification_geo_data')
 class ClassificationGeoDataConfig(ClassificationDataConfig, GeoDataConfig):
     """Configure classification :class:`GeoDatasets <.GeoDataset>`.
 
     See :mod:`rastervision.pytorch_learner.dataset.classification_dataset`.
     """
 
-    def build_scenes(self, tmp_dir: str):
-        for s in self.scene_dataset.all_scenes:
+    def build_scenes(self,
+                     scene_configs: Iterable['SceneConfig'],
+                     tmp_dir: Optional[str] = None):
+        for s in scene_configs:
             if s.label_source is not None:
                 s.label_source.lazy = True
-        return super().build_scenes(tmp_dir=tmp_dir)
+        return super().build_scenes(scene_configs, tmp_dir=tmp_dir)
 
     def scene_to_dataset(self,
                          scene: Scene,
-                         transform: Optional[A.BasicTransform] = None
+                         transform: Optional[A.BasicTransform] = None,
+                         for_chipping: bool = False
                          ) -> Union[ClassificationSlidingWindowGeoDataset,
                                     ClassificationRandomWindowGeoDataset]:
-        if isinstance(self.window_opts, dict):
-            opts = self.window_opts[scene.id]
+        if isinstance(self.sampling, dict):
+            opts = self.sampling[scene.id]
         else:
-            opts = self.window_opts
+            opts = self.sampling
+
+        extra_args = {}
+        if for_chipping:
+            extra_args = dict(
+                normalize=False, to_pytorch=False, return_window=True)
 
-        if opts.method == GeoDataWindowMethod.sliding:
+        if opts.method == WindowSamplingMethod.sliding:
             ds = ClassificationSlidingWindowGeoDataset(
                 scene,
                 size=opts.size,
                 stride=opts.stride,
                 padding=opts.padding,
                 pad_direction=opts.pad_direction,
-                transform=transform)
-        elif opts.method == GeoDataWindowMethod.random:
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
+        elif opts.method == WindowSamplingMethod.random:
             ds = ClassificationRandomWindowGeoDataset(
                 scene,
                 size_lims=opts.size_lims,
                 h_lims=opts.h_lims,
                 w_lims=opts.w_lims,
                 out_size=opts.size,
                 padding=opts.padding,
                 max_windows=opts.max_windows,
                 max_sample_attempts=opts.max_sample_attempts,
                 efficient_aoi_sampling=opts.efficient_aoi_sampling,
-                transform=transform)
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
         else:
             raise NotImplementedError()
         return ds
 
 
 @register_config('classification_model')
 class ClassificationModelConfig(ModelConfig):
@@ -134,15 +151,14 @@
         return model
 
 
 @register_config('classification_learner')
 class ClassificationLearnerConfig(LearnerConfig):
     """Configure a :class:`.ClassificationLearner`."""
 
-    data: Union[ClassificationImageDataConfig, ClassificationGeoDataConfig]
     model: Optional[ClassificationModelConfig]
 
     def build(self,
               tmp_dir=None,
               model_weights_path=None,
               model_def_path=None,
               loss_def_path=None,
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/__init__.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/classification_dataset.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/classification_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             not using any labels.
         aoi_uri (Union[str, List[str]], optional): URI or list of URIs of
             GeoJSONs that specify the area-of-interest. If provided, the
             dataset will only access data from this area. Defaults to [].
         label_vector_default_class_id (Optional[int], optional): If using
             label_vector_uri and all polygons in that file belong to the same
             class and they do not contain a `class_id` property, then use this
-            argument to map all of the polgons to the appropriate class ID.
+            argument to map all of the polygons to the appropriate class ID.
             See docs for ClassInferenceTransformer for more details.
             Defaults to None.
         image_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for image data. See docs for
             RasterioSource for more details. Defaults to {}.
         label_vector_source_kw (dict, optional): Additional arguments to pass
             to the GeoJSONVectorSourceConfig used for label data, if
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/dataset.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-from typing import Union, Optional, Tuple, Any, TypeVar
-from typing_extensions import Literal
+from typing import TYPE_CHECKING, Any, Literal, Optional, Tuple, TypeVar, Union
 import logging
 
 import numpy as np
 import albumentations as A
 import torch
 from torch.utils.data import Dataset
+from shapely.ops import unary_union
 
 from rastervision.core.box import Box
 from rastervision.core.data import Scene
+from rastervision.core.data.utils import AoiSampler
 from rastervision.pytorch_learner.learner_config import PosInt, NonNegInt
 from rastervision.pytorch_learner.dataset.transform import (TransformType,
                                                             TF_TYPE_TO_TF_FUNC)
-from rastervision.pytorch_learner.dataset.utils import AoiSampler
+
+if TYPE_CHECKING:
+    from shapely.geometry import MultiPolygon, Polygon
 
 log = logging.getLogger(__name__)
 
+T = TypeVar('T')
+
+
+def _to_tuple(x: T, n: int = 2) -> Tuple[T, ...]:
+    """Convert to n-tuple if not already an n-tuple."""
+    if isinstance(x, tuple):
+        if len(x) != n:
+            raise ValueError()
+        return x
+    return tuple([x] * n)
+
 
 class AlbumentationsDataset(Dataset):
     """An adapter to use arbitrary datasets with albumentations transforms."""
 
     def __init__(self,
                  orig_dataset: Any,
                  transform: Optional[A.BasicTransform] = None,
@@ -79,45 +93,53 @@
             x = torch.from_numpy(x).float()
             # (..., H, W, C) --> (..., C, H, W)
             x = x.transpose_(-2, -1).transpose_(-3, -2)
             if y is not None:
                 y = torch.from_numpy(y)
 
         if y is None:
-            # Ideally, y should be None to semantically convery the absence of
-            # any label, but PyTorch's defauult collate function doesn't handle
+            # Ideally, y should be None to semantically convey the absence of
+            # any label, but PyTorch's default collate function doesn't handle
             # None values.
             y = torch.tensor(np.nan)
 
         return x, y
 
     def __len__(self):
         return len(self.orig_dataset)
 
 
 class ImageDataset(AlbumentationsDataset):
     """ Dataset that reads from image files. """
-    pass
 
 
 class GeoDataset(AlbumentationsDataset):
     """ Dataset that reads directly from a Scene
         (i.e. a raster source and a label source).
     """
 
-    def __init__(self,
-                 scene: Scene,
-                 transform: Optional[A.BasicTransform] = None,
-                 transform_type: Optional[TransformType] = None,
-                 normalize: bool = True,
-                 to_pytorch: bool = True):
+    def __init__(
+            self,
+            scene: Scene,
+            out_size: Optional[Union[PosInt, Tuple[PosInt, PosInt]]] = None,
+            within_aoi: bool = True,
+            transform: Optional[A.BasicTransform] = None,
+            transform_type: Optional[TransformType] = None,
+            normalize: bool = True,
+            to_pytorch: bool = True,
+            return_window: bool = False):
         """Constructor.
 
         Args:
             scene (Scene): A Scene object.
+            out_size: Resize chips to this size before returning.
+            within_aoi: If True and if the scene has an AOI, only sample
+                windows that lie fully within the AOI. If False, windows only
+                partially intersecting the AOI will also be allowed.
+                Defaults to True.
             transform (Optional[A.BasicTransform], optional): Albumentations
                 transform to apply to the windows. Defaults to None.
                 Each transform in Albumentations takes images of type uint8, and
                 sometimes other data types. The data type requirements can be
                 seen at https://albumentations.ai/docs/api_reference/augmentations/transforms/ # noqa
                 If there is a mismatch between the data type of imagery and the
                 transform requirements, a RasterTransformer should be set
@@ -125,74 +147,92 @@
                 MinMaxTransformer or StatsTransformer.
             transform_type (Optional[TransformType], optional): Type of
                 transform. Defaults to None.
             normalize (bool, optional): If True, x is normalized to [0, 1]
                 based on its data type. Defaults to True.
             to_pytorch (bool, optional): If True, x and y are converted to
                 pytorch tensors. Defaults to True.
+            return_window (bool, optional): Make __getitem__ return the window
+                coordinates used to generate the image. Defaults to False.
         """
         self.scene = scene
+        self.within_aoi = within_aoi
+        self.return_window = return_window
+        self.out_size = None
+
+        if out_size is not None:
+            self.out_size = _to_tuple(out_size)
+            transform = self.append_resize_transform(transform, self.out_size)
 
         super().__init__(
             orig_dataset=scene,
             transform=transform,
             transform_type=transform_type,
             normalize=normalize,
             to_pytorch=to_pytorch)
 
+    def append_resize_transform(
+            self, transform: A.BasicTransform | None,
+            out_size: tuple[PosInt, PosInt]) -> A.Resize | A.Compose:
+        """Get transform to use for resizing windows to out_size."""
+        resize_tf = A.Resize(*out_size, always_apply=True)
+        if transform is None:
+            transform = resize_tf
+        else:
+            transform = A.Compose([transform, resize_tf])
+        return transform
+
     def __len__(self):
         raise NotImplementedError()
 
     @classmethod
     def from_uris(cls, *args, **kwargs) -> 'GeoDataset':
         raise NotImplementedError()
 
 
-T = TypeVar('T')
-
-
-def _to_tuple(x: T, n: int = 2) -> Tuple[T, ...]:
-    """Convert to n-tuple if not already an n-tuple."""
-    if isinstance(x, tuple):
-        if len(x) != n:
-            raise ValueError()
-        return x
-    return tuple([x] * n)
-
-
 class SlidingWindowGeoDataset(GeoDataset):
     """Read the scene left-to-right, top-to-bottom, using a sliding window.
     """
 
-    def __init__(self,
-                 scene: Scene,
-                 size: Union[PosInt, Tuple[PosInt, PosInt]],
-                 stride: Union[PosInt, Tuple[PosInt, PosInt]],
-                 padding: Optional[Union[NonNegInt, Tuple[NonNegInt,
-                                                          NonNegInt]]] = None,
-                 pad_direction: Literal['both', 'start', 'end'] = 'end',
-                 transform: Optional[A.BasicTransform] = None,
-                 transform_type: Optional[TransformType] = None,
-                 normalize: bool = True,
-                 to_pytorch: bool = True):
+    def __init__(
+            self,
+            scene: Scene,
+            size: Union[PosInt, Tuple[PosInt, PosInt]],
+            stride: Union[PosInt, Tuple[PosInt, PosInt]],
+            out_size: Optional[Union[PosInt, Tuple[PosInt, PosInt]]] = None,
+            padding: Optional[Union[NonNegInt, Tuple[NonNegInt,
+                                                     NonNegInt]]] = None,
+            pad_direction: Literal['both', 'start', 'end'] = 'end',
+            within_aoi: bool = True,
+            transform: Optional[A.BasicTransform] = None,
+            transform_type: Optional[TransformType] = None,
+            normalize: bool = True,
+            to_pytorch: bool = True,
+            return_window: bool = False):
         """Constructor.
 
         Args:
             scene (Scene): A Scene object.
             size (Union[PosInt, Tuple[PosInt, PosInt]]): Window size.
             stride (Union[PosInt, Tuple[PosInt, PosInt]]): Step size between
                 windows.
+            out_size: Resize chips to this size before returning. Defaults to
+                ``None``.
             padding (Optional[Union[NonNegInt, Tuple[NonNegInt, NonNegInt]]]):
                 How many pixels the windows are allowed to overflow the sides
                 of the raster source. If None, padding is set to size // 2.
                 Defaults to None.
             pad_direction (Literal['both', 'start', 'end']): If 'end', only pad
                 ymax and xmax (bottom and right). If 'start', only pad ymin and
                 xmin (top and left). If 'both', pad all sides. Has no effect if
                 paddiong is zero. Defaults to 'end'.
+            within_aoi: If True and if the scene has an AOI, only sample
+                windows that lie fully within the AOI. If False, windows only
+                partially intersecting the AOI will also be allowed.
+                Defaults to True.
             transform (Optional[A.BasicTransform], optional): Albumentations
                 transform to apply to the windows. Defaults to None.
                 Each transform in Albumentations takes images of type uint8, and
                 sometimes other data types. The data type requirements can be
                 seen at https://albumentations.ai/docs/api_reference/augmentations/transforms/ # noqa
                 If there is a mismatch between the data type of imagery and the
                 transform requirements, a RasterTransformer should be set
@@ -200,44 +240,54 @@
                 MinMaxTransformer or StatsTransformer.
             transform_type (Optional[TransformType], optional): Type of
                 transform. Defaults to None.
             normalize (bool, optional): If True, x is normalized to [0, 1]
                 based on its data type. Defaults to True.
             to_pytorch (bool, optional): If True, x and y are converted to
                 pytorch tensors. Defaults to True.
+            return_window (bool, optional): Make __getitem__ return the window
+                coordinates used to generate the image. Defaults to False.
         """
         super().__init__(
             scene=scene,
+            out_size=out_size,
+            within_aoi=within_aoi,
             transform=transform,
             transform_type=transform_type,
             normalize=normalize,
-            to_pytorch=to_pytorch)
+            to_pytorch=to_pytorch,
+            return_window=return_window)
         self.size = _to_tuple(size)
         self.stride = _to_tuple(stride)
         self.padding = padding
         self.pad_direction = pad_direction
         self.init_windows()
 
     def init_windows(self) -> None:
         """Pre-compute windows."""
-        windows = self.scene.raster_source.extent.get_windows(
+        windows = self.scene.extent.get_windows(
             self.size,
             stride=self.stride,
             padding=self.padding,
             pad_direction=self.pad_direction)
         if len(self.scene.aoi_polygons_bbox_coords) > 0:
-            windows = Box.filter_by_aoi(windows,
-                                        self.scene.aoi_polygons_bbox_coords)
+            windows = Box.filter_by_aoi(
+                windows,
+                self.scene.aoi_polygons_bbox_coords,
+                within=self.within_aoi)
         self.windows = windows
 
     def __getitem__(self, idx: int):
         if idx >= len(self):
             raise StopIteration()
         window = self.windows[idx]
-        return super().__getitem__(window)
+        out = super().__getitem__(window)
+        if self.return_window:
+            return (out, window)
+        return out
 
     def __len__(self):
         return len(self.windows)
 
 
 class RandomWindowGeoDataset(GeoDataset):
     """Read the scene by sampling random window sizes and locations.
@@ -249,20 +299,21 @@
                  size_lims: Optional[Tuple[PosInt, PosInt]] = None,
                  h_lims: Optional[Tuple[PosInt, PosInt]] = None,
                  w_lims: Optional[Tuple[PosInt, PosInt]] = None,
                  padding: Optional[Union[NonNegInt, Tuple[NonNegInt,
                                                           NonNegInt]]] = None,
                  max_windows: Optional[NonNegInt] = None,
                  max_sample_attempts: PosInt = 100,
-                 return_window: bool = False,
                  efficient_aoi_sampling: bool = True,
+                 within_aoi: bool = True,
                  transform: Optional[A.BasicTransform] = None,
                  transform_type: Optional[TransformType] = None,
                  normalize: bool = True,
-                 to_pytorch: bool = True):
+                 to_pytorch: bool = True,
+                 return_window: bool = False):
         """Constructor.
 
         Will sample square windows if size_lims is specified. Otherwise, will
         sample rectangular windows with height and width sampled according to
         h_lims and w_lims.
 
         Args:
@@ -296,102 +347,97 @@
                 MinMaxTransformer or StatsTransformer.
             transform_type (Optional[TransformType], optional): Type of
                 transform. Defaults to None.
             max_sample_attempts (NonNegInt, optional): Max attempts when trying
                 to find a window within the AOI of the scene. Only used if the
                 scene has aoi_polygons specified. StopIteratioin is raised if
                 this is exceeded. Defaults to 100.
-            return_window (bool, optional): Make __getitem__ return the window
-                coordinates used to generate the image. Defaults to False.
             efficient_aoi_sampling (bool, optional): If the scene has AOIs,
                 sampling windows at random anywhere in the extent and then
                 checking if they fall within any of the AOIs can be very
                 inefficient. This flag enables the use of an alternate
                 algorithm that only samples window locations inside the AOIs.
                 Defaults to True.
+            within_aoi: If True and if the scene has an AOI, only sample
+                windows that lie fully within the AOI. If False, windows only
+                partially intersecting the AOI will also be allowed.
+                Defaults to True.
             transform (Optional[A.BasicTransform], optional): Albumentations
                 transform to apply to the windows. Defaults to None.
             transform_type (Optional[TransformType], optional): Type of
                 transform. Defaults to None.
             normalize (bool, optional): If True, x is normalized to [0, 1]
                 based on its data type. Defaults to True.
             to_pytorch (bool, optional): If True, x and y are converted to
                 pytorch tensors. Defaults to True.
+            return_window (bool, optional): Make __getitem__ return the window
+                coordinates used to generate the image. Defaults to False.
         """ # noqa
         has_size_lims = size_lims is not None
         has_h_lims = h_lims is not None
         has_w_lims = w_lims is not None
         if has_size_lims == (has_w_lims or has_h_lims):
             raise ValueError('Specify either size_lims or h and w lims.')
         if has_h_lims != has_w_lims:
             raise ValueError('h_lims and w_lims must both be specified')
 
-        if out_size is not None:
-            out_size = _to_tuple(out_size)
-            transform = self.get_resize_transform(transform, out_size)
-        else:
+        if out_size is None:
             log.warning(f'out_size is None, chips will not be normalized or '
                         'converted to PyTorch Tensors.')
             normalize, to_pytorch = False, False
 
         super().__init__(
             scene=scene,
+            out_size=out_size,
+            within_aoi=within_aoi,
             transform=transform,
             transform_type=transform_type,
             normalize=normalize,
-            to_pytorch=to_pytorch)
+            to_pytorch=to_pytorch,
+            return_window=return_window)
 
         if padding is None:
-            if size_lims is not None:
+            if has_size_lims:
                 max_size = size_lims[1]
                 padding = (max_size // 2, max_size // 2)
             else:
                 max_h, max_w = h_lims[1], w_lims[1]
                 padding = (max_h // 2, max_w // 2)
         padding = _to_tuple(padding)
 
         if max_windows is None:
             max_windows = np.iinfo('int').max
 
         self.size_lims = size_lims
         self.h_lims = h_lims
         self.w_lims = w_lims
         self.padding = padding
-        self.return_window = return_window
         self.max_windows = max_windows
         self.max_sample_attempts = max_sample_attempts
 
         # include padding in the extent
-        ymin, xmin, ymax, xmax = scene.raster_source.extent
+        ymin, xmin, ymax, xmax = scene.extent
         h_padding, w_padding = self.padding
         self.extent = Box(ymin - h_padding, xmin - w_padding, ymax + h_padding,
                           xmax + w_padding)
 
         self.aoi_sampler = None
-        self.aoi_polygons = self.scene.aoi_polygons_bbox_coords
-        self.has_aoi_polygons = len(self.aoi_polygons) > 0
+        aoi_polygons = self.scene.aoi_polygons_bbox_coords
+        self.has_aoi_polygons = len(aoi_polygons) > 0
         if self.has_aoi_polygons:
-            # only sample from polygons that intersect w/ the extent
             extent_polygon = self.extent.to_shapely()
-            self.aoi_polygons = [
-                p.intersection(extent_polygon) for p in self.aoi_polygons
-            ]
+            aoi: 'Polygon' | 'MultiPolygon' = unary_union(aoi_polygons)
+            # only sample from polygons that intersect w/ the extent
+            self.aoi = aoi.intersection(extent_polygon)
             if efficient_aoi_sampling:
-                self.aoi_sampler = AoiSampler(self.aoi_polygons)
-
-    def get_resize_transform(
-            self, transform: Optional[A.BasicTransform],
-            out_size: Tuple[PosInt, PosInt]) -> Union[A.Resize, A.Compose]:
-        """Get transform to use for resizing windows to out_size."""
-        resize_tf = A.Resize(*out_size, always_apply=True)
-        if transform is None:
-            transform = resize_tf
-        else:
-            transform = A.Compose([transform, resize_tf])
-        return transform
+                try:
+                    self.aoi_sampler = AoiSampler([self.aoi])
+                except ModuleNotFoundError:
+                    log.info('Ignoring efficient_aoi_sampling since triangle '
+                             'is not installed.')
 
     @property
     def min_size(self):
         if self.size_lims is not None:
             return self.size_lims[0], self.size_lims[0]
         return self.h_lims[0], self.w_lims[0]
 
@@ -430,15 +476,17 @@
         """Randomly sample a window with random size and location."""
         h, w = self.sample_window_size()
         x, y = self.sample_window_loc(h, w)
         window = Box(y, x, y + h, x + w)
         return window
 
     def sample_window(self) -> Box:
-        """If scene has AOI polygons, try to find a random window that is
+        """Sample a window with random size and location within the AOI.
+
+        If the scene has AOI polygons, try to find a random window that is
         within the AOI. Otherwise, just return the first sampled window.
 
         Raises:
             StopIteration: If unable to find a valid window within
                 self.max_sample_attempts attempts.
 
         Returns:
@@ -446,21 +494,27 @@
         """
         if not self.has_aoi_polygons:
             window = self._sample_window()
             return window
 
         for _ in range(self.max_sample_attempts):
             window = self._sample_window()
-            if Box.within_aoi(window, self.aoi_polygons):
-                return window
-        raise StopIteration('Failed to find random window within scene AOI.')
+            if self.within_aoi:
+                if Box.within_aoi(window, self.aoi):
+                    return window
+            else:
+                if Box.intersects_aoi(window, self.aoi):
+                    return window
+        raise StopIteration('Failed to find valid window within scene AOI in '
+                            f'{self.max_sample_attempts} attempts.')
 
     def __getitem__(self, idx: int):
         if idx >= len(self):
             raise StopIteration()
         window = self.sample_window()
+        out = super().__getitem__(window)
         if self.return_window:
-            return (super().__getitem__(window), window)
-        return super().__getitem__(window)
+            return (out, window)
+        return out
 
     def __len__(self):
         return self.max_windows
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/object_detection_dataset.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/object_detection_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             not using any labels.
         aoi_uri (Union[str, List[str]], optional): URI or list of URIs of
             GeoJSONs that specify the area-of-interest. If provided, the
             dataset will only access data from this area. Defaults to [].
         label_vector_default_class_id (Optional[int], optional): If using
             label_vector_uri and all polygons in that file belong to the same
             class and they do not contain a `class_id` property, then use this
-            argument to map all of the polgons to the appropriate class ID.
+            argument to map all of the polygons to the appropriate class ID.
             See docs for ClassInferenceTransformer for more details.
             Defaults to None.
         image_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for image data. See docs for
             RasterioSource for more details. Defaults to {}.
         label_vector_source_kw (dict, optional): Additional arguments to pass
             to the GeoJSONVectorSourceConfig used for label data, if
@@ -230,16 +230,16 @@
                         'Total bboxes in scene (ignoring AOI):'
                         f'{num_bboxes_in_scene}.')
 
             self.bboxes = self.labels.get_boxes()
         else:
             self.neg_probability = None
 
-    def get_resize_transform(self, transform: A.BasicTransform,
-                             out_size: Tuple[int, int]) -> A.BasicTransform:
+    def append_resize_transform(self, transform: A.BasicTransform,
+                                out_size: tuple[int, int]) -> A.BasicTransform:
         resize_tf = A.Resize(*out_size, always_apply=True)
         if transform is None:
             transform = resize_tf
         else:
             transform = A.Compose(
                 [transform, resize_tf], bbox_params=self.bbox_params)
         return transform
@@ -249,15 +249,15 @@
 
         This is done by randomly sampling one of the bounding boxes in the
         scene and drawing a random window around it.
         """
         bbox: Box = np.random.choice(self.bboxes)
         box_h, box_w = bbox.size
 
-        # check if it is possible to sample a containing widnow
+        # check if it is possible to sample a containing window
         hmax, wmax = self.max_size
         if box_h > hmax or box_w > wmax:
             raise ValueError(
                 f'Cannot sample containing window because bounding box {bbox}'
                 f'is larger than self.max_size ({self.max_size}).')
 
         # try to sample a window size that is larger than the box's size
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/regression_dataset.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/regression_dataset.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             not using any labels.
         aoi_uri (Union[str, List[str]], optional): URI or list of URIs of
             GeoJSONs that specify the area-of-interest. If provided, the
             dataset will only access data from this area. Defaults to [].
         label_vector_default_class_id (Optional[int], optional): If using
             label_vector_uri and all polygons in that file belong to the same
             class and they do not contain a `class_id` property, then use this
-            argument to map all of the polgons to the appropriate class ID.
+            argument to map all of the polygons to the appropriate class ID.
             See docs for ClassInferenceTransformer for more details.
             Defaults to None.
         image_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for image data. See docs for
             RasterioSource for more details. Defaults to {}.
         label_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for label data, if label_raster_uri is
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/transform.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,13 +229,13 @@
             x, y = out['image'], out['mask']
     if y is not None:
         y = y.astype(int)
     return x, y
 
 
 TF_TYPE_TO_TF_FUNC: Dict[TransformType, Callable] = {
-    TransformType.noop: lambda x: x,
+    TransformType.noop: lambda x, tf: x,
     TransformType.classification: classification_transformer,
     TransformType.regression: regression_transformer,
     TransformType.object_detection: object_detection_transformer,
     TransformType.semantic_segmentation: semantic_segmentation_transformer
 }
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/utils/utils.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Iterable, List, Optional, Tuple
 from os import PathLike
-from os.path import splitext
+from os.path import join, splitext
 from pathlib import Path
 from itertools import chain
 
 import numpy as np
 from torchvision.datasets.folder import (IMG_EXTENSIONS, DatasetFolder)
 from PIL import Image
 import rasterio as rio
@@ -54,20 +54,30 @@
 
 def make_image_folder_dataset(data_dir: str,
                               classes: Optional[Iterable[str]] = None
                               ) -> DatasetFolder:
     """Initializes and returns an ImageFolder.
 
     If classes is specified, ImageFolder's default class-to-index mapping
-    behavior is overriden to use the indices of classes instead.
+    behavior is overridden to use the indices of classes instead.
     """
     if classes is None:
         return DatasetFolder(
             data_dir, loader=load_image, extensions=IMG_EXTENSIONS)
 
+    from rastervision.pipeline.file_system.utils import (file_exists,
+                                                         list_paths)
+
+    class_dirs = [join(data_dir, c) for c in classes]
+    classes_present = [
+        c for c, dir in zip(classes, class_dirs)
+        if file_exists(dir, include_dir=True) and len(list_paths(dir)) > 0
+    ]
+    class_to_id = {c: classes.index(c) for c in classes_present}
+
     class ImageFolder(DatasetFolder):
         def find_classes(self,
                          directory: str) -> Tuple[List[str], Dict[str, int]]:
             """Override to force mapping from class name to class index."""
-            return classes, {c: i for (i, c) in enumerate(classes)}
+            return classes_present, class_to_id
 
     return ImageFolder(data_dir, loader=load_image, extensions=IMG_EXTENSIONS)
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/__init__.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import (Sequence, Optional)
+from typing import TYPE_CHECKING, Optional, Sequence
 from textwrap import wrap
 
 import torch
 
 from rastervision.pytorch_learner.dataset.visualizer import Visualizer  # NOQA
 from rastervision.pytorch_learner.utils import (plot_channel_groups,
                                                 channel_groups_to_imgs)
 
+if TYPE_CHECKING:
+    from matplotlib.pyplot import Axes
+
 
 class ClassificationVisualizer(Visualizer):
     """Plots samples from image classification Datasets."""
 
     def plot_xyz(self,
-                 axs: Sequence,
+                 axs: Sequence['Axes'],
                  x: torch.Tensor,
-                 y: int,
+                 y: Optional[int] = None,
                  z: Optional[int] = None,
                  plot_title: bool = True) -> None:
         channel_groups = self.get_channel_display_groups(x.shape[1])
 
         img_axes = axs[:-1]
         label_ax = axs[-1]
 
@@ -26,53 +29,68 @@
         imgs = channel_groups_to_imgs(x, channel_groups)
         plot_channel_groups(
             img_axes, imgs, channel_groups, plot_title=plot_title)
 
         # plot label
         class_names = self.class_names
         class_names = ['-\n-'.join(wrap(c, width=16)) for c in class_names]
-        if z is None:
-            # just display the class name as text
-            class_name = class_names[y]
-            label_ax.text(
-                .5,
-                .5,
-                class_name,
-                ha='center',
-                va='center',
-                fontdict={
-                    'size': 20,
-                    'family': 'sans-serif'
-                })
-            label_ax.set_xlim((0, 1))
-            label_ax.set_ylim((0, 1))
-            label_ax.axis('off')
-        else:
-            # display predicted class probabilities as a horizontal bar plot
-            # legend: green = ground truth, dark-red = wrong prediction,
-            # light-gray = other. In case predicted class matches ground truth,
-            # only one bar will be green and the others will be light-gray.
-            class_probabilities = z.softmax(dim=-1)
-            class_index_pred = z.argmax(dim=-1)
+        if y is not None and z is None:
+            self.plot_gt(label_ax, class_names, y)
+        elif z is not None:
+            self.plot_pred(label_ax, class_names, z, y=y)
+            if plot_title:
+                label_ax.set_title('Prediction')
+
+    def plot_gt(self, ax: 'Axes', class_names: Sequence[str], y: torch.Tensor):
+        """Display ground truth class names as text."""
+        class_name = class_names[y]
+        ax.text(
+            x=.5,
+            y=.5,
+            s=class_name,
+            ha='center',
+            va='center',
+            fontdict={
+                'size': 20,
+                'family': 'sans-serif'
+            })
+        ax.set_xlim((0, 1))
+        ax.set_ylim((0, 1))
+        ax.axis('off')
+
+    def plot_pred(self,
+                  ax: 'Axes',
+                  class_names: Sequence[str],
+                  z: torch.Tensor,
+                  y: Optional[torch.Tensor] = None):
+        """Plot predictions.
+
+        Plots predicted class probabilities as a horizontal bar plot. If ground
+        truth, y, is provided, the bar colors represent: green = ground truth,
+        dark-red = wrong prediction, light-gray = other. In case predicted
+        class matches ground truth, only one bar will be green and the others
+        will be light-gray.
+        """
+        class_probabilities = z.softmax(dim=-1)
+        class_index_pred = z.argmax(dim=-1)
+        bar_colors = ['lightgray'] * len(z)
+        if y is not None:
             class_index_gt = y
-            bar_colors = ['lightgray'] * len(z)
             if class_index_pred == class_index_gt:
                 bar_colors[class_index_pred] = 'green'
             else:
                 bar_colors[class_index_pred] = 'darkred'
                 bar_colors[class_index_gt] = 'green'
-            label_ax.barh(
-                y=class_names,
-                width=class_probabilities,
-                color=bar_colors,
-                edgecolor='black')
-            label_ax.set_xlim((0, 1))
-            label_ax.xaxis.grid(linestyle='--', alpha=1)
-            label_ax.set_xlabel('Probability')
-            if plot_title:
-                label_ax.set_title('Prediction')
+        ax.barh(
+            y=class_names,
+            width=class_probabilities,
+            color=bar_colors,
+            edgecolor='black')
+        ax.set_xlim((0, 1))
+        ax.xaxis.grid(linestyle='--', alpha=1)
+        ax.set_xlabel('Probability')
 
     def get_plot_ncols(self, **kwargs) -> int:
         x = kwargs['x']
         nb_img_channels = x.shape[1]
         ncols = len(self.get_channel_display_groups(nb_img_channels)) + 1
         return ncols
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,22 @@
 
     def get_collate_fn(self):
         return collate_fn
 
     def plot_xyz(self,
                  axs: Sequence,
                  x: torch.Tensor,
-                 y: BoxList,
+                 y: Optional[BoxList] = None,
                  z: Optional[BoxList] = None,
                  plot_title: bool = True) -> None:
-        y = y if z is None else z
         channel_groups = self.get_channel_display_groups(x.shape[1])
+        imgs = channel_groups_to_imgs(x, channel_groups)
 
-        class_names = self.class_names
-        class_colors = self.class_colors
+        if y is not None or z is not None:
+            y = y if z is None else z
+            class_names = self.class_names
+            class_colors = self.class_colors
+            imgs = [
+                draw_boxes(img, y, class_names, class_colors) for img in imgs
+            ]
 
-        imgs = channel_groups_to_imgs(x, channel_groups)
-        imgs = [draw_boxes(img, y, class_names, class_colors) for img in imgs]
         plot_channel_groups(axs, imgs, channel_groups, plot_title=plot_title)
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,97 @@
-from typing import (Sequence, Optional, Union)
+from typing import TYPE_CHECKING, Optional, Sequence, Union
 
 import torch
 import numpy as np
 import matplotlib.colors as mcolors
 import matplotlib.patches as mpatches
 
 from rastervision.pytorch_learner.dataset.visualizer import Visualizer  # NOQA
 from rastervision.pytorch_learner.utils import (
     color_to_triple, plot_channel_groups, channel_groups_to_imgs)
 
+if TYPE_CHECKING:
+    from matplotlib.pyplot import Axes
+    from matplotlib.colors import Colormap
+
 
 class SemanticSegmentationVisualizer(Visualizer):
     """Plots samples from semantic segmentation Datasets."""
 
     def plot_xyz(self,
                  axs: Sequence,
                  x: torch.Tensor,
-                 y: Union[torch.Tensor, np.ndarray],
+                 y: Optional[Union[torch.Tensor, np.ndarray]] = None,
                  z: Optional[torch.Tensor] = None,
                  plot_title: bool = True) -> None:
         channel_groups = self.get_channel_display_groups(x.shape[1])
 
         img_axes = axs[:len(channel_groups)]
-        label_ax = axs[len(channel_groups)]
 
         # plot image
         imgs = channel_groups_to_imgs(x, channel_groups)
         plot_channel_groups(
             img_axes, imgs, channel_groups, plot_title=plot_title)
 
+        if y is None and z is None:
+            return
+
         # plot labels
         class_colors = self.class_colors
         colors = [
             color_to_triple(c) if isinstance(c, str) else c
             for c in class_colors
         ]
         colors = np.array(colors) / 255.
         cmap = mcolors.ListedColormap(colors)
 
-        label_ax.imshow(
-            y, vmin=0, vmax=len(colors), cmap=cmap, interpolation='none')
-        if plot_title:
-            label_ax.set_title(f'Ground truth')
-        label_ax.set_xticks([])
-        label_ax.set_yticks([])
+        if y is not None:
+            label_ax: 'Axes' = axs[len(channel_groups)]
+            self.plot_gt(label_ax, y, num_classes=len(colors), cmap=cmap)
+            if plot_title:
+                label_ax.set_title('Ground truth')
 
-        # plot predictions
         if z is not None:
             pred_ax = axs[-1]
-            preds = z.argmax(dim=0)
-            pred_ax.imshow(
-                preds,
-                vmin=0,
-                vmax=len(colors),
-                cmap=cmap,
-                interpolation='none')
+            self.plot_pred(pred_ax, z, num_classes=len(colors), cmap=cmap)
             if plot_title:
-                pred_ax.set_title(f'Predicted labels')
-            pred_ax.set_xticks([])
-            pred_ax.set_yticks([])
+                pred_ax.set_title('Predicted labels')
 
         # add a legend to the rightmost subplot
         class_names = self.class_names
         if class_names:
             legend_items = [
                 mpatches.Patch(facecolor=col, edgecolor='black', label=name)
                 for col, name in zip(colors, class_names)
             ]
             axs[-1].legend(
                 handles=legend_items,
                 loc='center left',
                 bbox_to_anchor=(1., 0.5))
 
+    def plot_gt(self, ax: 'Axes', y: Union[torch.Tensor, np.ndarray],
+                num_classes: int, cmap: 'Colormap', **kwargs):
+        ax.imshow(
+            y,
+            vmin=0,
+            vmax=num_classes,
+            cmap=cmap,
+            interpolation='none',
+            **kwargs)
+        ax.set_xticks([])
+        ax.set_yticks([])
+
+    def plot_pred(self, ax: 'Axes', z: Union[torch.Tensor, np.ndarray],
+                  num_classes: int, cmap: 'Colormap', **kwargs):
+        if z.ndim == 3:
+            z = z.argmax(dim=0)
+        self.plot_gt(ax, y=z, num_classes=num_classes, cmap=cmap, **kwargs)
+
     def get_plot_ncols(self, **kwargs) -> int:
         x = kwargs['x']
         nb_img_channels = x.shape[1]
-        ncols = len(self.get_channel_display_groups(nb_img_channels)) + 1
-        z = kwargs.get('z')
-        if z is not None:
+        ncols = len(self.get_channel_display_groups(nb_img_channels))
+        if kwargs.get('y') is not None:
+            ncols += 1
+        if kwargs.get('z') is not None:
             ncols += 1
         return ncols
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/dataset/visualizer/visualizer.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import (TYPE_CHECKING, Sequence, Optional, List, Dict, Union,
                     Tuple, Any)
 from abc import ABC, abstractmethod
 
 import numpy as np
 import torch
 from torch import Tensor
-import albumentations as A
 from torch.utils.data import DataLoader
+import albumentations as A
 import matplotlib.pyplot as plt
 
 from rastervision.pipeline.file_system import make_dir
+from rastervision.core.data import ClassConfig
 from rastervision.pytorch_learner.utils import (
     deserialize_albumentation_transform, validate_albumentation_transform,
     MinMaxNormalize)
 from rastervision.pytorch_learner.learner_config import (
     RGBTuple,
     ChannelInds,
-    ensure_class_colors,
     validate_channel_display_groups,
     get_default_channel_display_groups,
 )
 
 if TYPE_CHECKING:
     from torch.utils.data import Dataset
     from matplotlib.figure import Figure
@@ -30,15 +30,15 @@
     """Base class for plotting samples from computer vision PyTorch Datasets."""
 
     scale: float = 3.
 
     def __init__(self,
                  class_names: List[str],
                  class_colors: Optional[List[Union[str, RGBTuple]]] = None,
-                 transform: Optional[Dict] = A.to_dict(MinMaxNormalize()),
+                 transform: Optional[Dict] = None,
                  channel_display_groups: Optional[Union[Dict[
                      str, ChannelInds], Sequence[ChannelInds]]] = None):
         """Constructor.
 
         Args:
             class_names: names of classes
             class_colors: Colors used to display classes. Can be color 3-tuples
@@ -56,40 +56,48 @@
                 Can be a list or tuple of groups (e.g. [(0, 1, 2), (3,)]) or a
                 dict containing title-to-group mappings
                 (e.g. {"RGB": [0, 1, 2], "IR": [3]}),
                 where each group is a list or tuple of channel indices and
                 title is a string that will be used as the title of the subplot
                 for that group.
         """
-        self.class_names = class_names
-        self.class_colors = ensure_class_colors(self.class_names, class_colors)
+        self.class_config = ClassConfig(names=class_names, colors=class_colors)
+        if transform is None:
+            transform = A.to_dict(MinMaxNormalize())
         self.transform = validate_albumentation_transform(transform)
         self._channel_display_groups = validate_channel_display_groups(
             channel_display_groups)
 
+    @property
+    def class_names(self):
+        return self.class_config.names
+
+    @property
+    def class_colors(self):
+        return self.class_config.colors
+
     @abstractmethod
     def plot_xyz(self,
                  axs,
                  x: Tensor,
-                 y: Sequence,
+                 y: Optional[Sequence] = None,
                  z: Optional[Sequence] = None,
                  plot_title: bool = True):
         """Plot image, ground truth labels, and predicted labels.
 
         Args:
             axs: matplotlib axes on which to plot
             x: image
             y: ground truth labels
             z: optional predicted labels
         """
-        pass
 
     def plot_batch(self,
                    x: Tensor,
-                   y: Sequence,
+                   y: Optional[Sequence] = None,
                    output_path: Optional[str] = None,
                    z: Optional[Sequence] = None,
                    batch_limit: Optional[int] = None,
                    show: bool = False):
         """Plot a whole batch in a grid using plot_xyz.
 
         Args:
@@ -130,26 +138,26 @@
                 plot_xyz_args = [
                     dict(params['plot_xyz_args'][i]) for _ in range(T)
                 ]
                 plot_xyz_args[0]['plot_title'] = True
                 for args in plot_xyz_args[1:]:
                     args['plot_title'] = False
                 _x = x[i]
-                _y = [y[i]] * T
+                _y = None if y is None else [y[i]] * T
                 _z = None if z is None else [z[i]] * T
                 self._plot_batch(fig, axs, plot_xyz_args, _x, y=_y, z=_z)
         else:
             raise ValueError('Expected x to have 4 or 5 dims, but found '
                              f'x.shape: {x.shape}')
 
         if show:
             plt.show()
         if output_path is not None:
             make_dir(output_path, use_dirname=True)
-            plt.savefig(output_path, bbox_inches='tight', pad_inches=0.2)
+            fig.savefig(output_path, bbox_inches='tight', pad_inches=0.2)
 
         plt.close(fig)
 
     def _plot_batch(
             self,
             fig: 'Figure',
             axs: Sequence,
@@ -163,17 +171,20 @@
 
         # apply transform, if given
         if self.transform is not None:
             tf = deserialize_albumentation_transform(self.transform)
             imgs = [tf(image=img)['image'] for img in x.numpy()]
             x = torch.from_numpy(np.stack(imgs))
 
+        if y is None:
+            y = [None] * len(x)
+        if z is None:
+            z = [None] * len(x)
         for i, row_axs in enumerate(axs):
-            _z = None if z is None else z[i]
-            self.plot_xyz(row_axs, x[i], y[i], z=_z, **plot_xyz_args[i])
+            self.plot_xyz(row_axs, x[i], y[i], z=z[i], **plot_xyz_args[i])
 
     def get_channel_display_groups(
             self, nb_img_channels: int
     ) -> Union[Dict[str, ChannelInds], Sequence[ChannelInds]]:
         # The default channel_display_groups object depends on the number of
         # channels in the image. This number is not known when the Visualizer
         # is constructed which is why it needs to be created later.
@@ -193,15 +204,15 @@
     def get_batch(self, dataset: 'Dataset', batch_sz: int = 4,
                   **kwargs) -> Tuple[Tensor, Any]:
         """Generate a batch from a dataset.
 
         This is a convenience method for generating a batch of data to plot.
 
         Args:
-            dataset (Dataset): A Pytorch Datset.
+            dataset (Dataset): A Pytorch Dataset.
             batch_sz (int): Batch size. Defaults to 4.
             **kwargs: Extra args for :class:`~torch.utils.data.DataLoader`.
 
         Returns:
             Tuple[Tensor, Any]: (x, y) tuple where x is images and y is labels.
         """
         collate_fn = self.get_collate_fn()
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/learner.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,95 @@
 from typing import (TYPE_CHECKING, Any, Callable, Dict, Iterator, List,
-                    Optional, Tuple, Union, Type)
-from typing_extensions import Literal
+                    Literal, Optional, Tuple, Union, Type)
 from abc import ABC, abstractmethod
-import os
 from os.path import join, isfile, basename, isdir
 import warnings
-import time
+from time import perf_counter
 import datetime
 import shutil
 import logging
 from subprocess import Popen
 import numbers
 from pprint import pformat
+import gc
 
 import numpy as np
 from tqdm.auto import tqdm
 
 import torch
 from torch import Tensor
 import torch.nn as nn
 from torch.utils.tensorboard import SummaryWriter
-from torch.utils.data import DataLoader
+from torch.utils.data import DataLoader, DistributedSampler
+from torch.nn.parallel import DistributedDataParallel as DDP
+import torch.distributed as dist
+import torch.multiprocessing as mp
 
+from rastervision.pipeline import rv_config_ as rv_config
+from rastervision.pipeline.utils import get_env_var
 from rastervision.pipeline.file_system import (
-    sync_to_dir, json_to_file, file_to_json, make_dir, zipdir,
-    download_if_needed, download_or_copy, sync_from_dir, get_local_path, unzip,
-    str_to_file, is_local, get_tmp_dir)
+    sync_to_dir, json_to_file, make_dir, zipdir, download_if_needed,
+    download_or_copy, sync_from_dir, get_local_path, unzip, is_local,
+    get_tmp_dir)
 from rastervision.pipeline.file_system.utils import file_exists
 from rastervision.pipeline.utils import terminate_at_exit
-from rastervision.pipeline.config import (build_config, upgrade_config,
-                                          save_pipeline_config)
+from rastervision.pipeline.config import build_config
 from rastervision.pytorch_learner.utils import (
-    get_hubconf_dir_from_cfg, aggregate_metrics, log_metrics_to_csv,
-    log_system_details, ONNXRuntimeAdapter)
+    aggregate_metrics, DDPContextManager, get_hubconf_dir_from_cfg,
+    get_learner_config_from_bundle_dir, log_metrics_to_csv, log_system_details,
+    ONNXRuntimeAdapter)
 from rastervision.pytorch_learner.dataset.visualizer import Visualizer
 
 if TYPE_CHECKING:
+    from typing import Self
     from torch.optim import Optimizer
     from torch.optim.lr_scheduler import _LRScheduler
     from torch.utils.data import Dataset, Sampler
-
-    from rastervision.pytorch_learner import (LearnerConfig,
-                                              LearnerPipelineConfig)
+    from rastervision.pytorch_learner import LearnerConfig
 
 warnings.filterwarnings('ignore')
 
 CHECKPOINTS_DIRNAME = 'checkpoints'
 MODULES_DIRNAME = 'modules'
 TRANSFORMS_DIRNAME = 'custom_albumentations_transforms'
 BUNDLE_MODEL_WEIGHTS_FILENAME = 'model.pth'
 BUNDLE_MODEL_ONNX_FILENAME = 'model.onnx'
-USE_ONNX = os.getenv('RASTERVISION_USE_ONNX', 'false').lower() in ('true', '1')
 
 log = logging.getLogger(__name__)
 
 MetricDict = Dict[str, float]
 
 
 class Learner(ABC):
     """Abstract training and prediction routines for a model.
 
     This can be subclassed to handle different computer vision tasks.
 
     The datasets, model, optimizer, and schedulers will be generated from the
-    cfg if not specified in the constructor.
+    :class:`.LearnerConfig` if not specified in the constructor.
 
-    If instantiated with training=False, the training apparatus (loss,
+    If instantiated with ``training=False``, the training apparatus (loss,
     optimizer, scheduler, logging, etc.) will not be set up and the model will
     be put into eval mode.
 
-    Note that various training and prediction methods have the side effect of
-    putting Learner.model into training or eval mode. No attempt is made to put the
-    model back into the mode it was previously in.
+    .. note::
+
+        This class supports distributed training via PyTorch DDP. If
+        instantiated as a DDP process, it will automatically read WORLD_SIZE,
+        RANK, and LOCAL_RANK environment variables. Alternatively, if
+        ``RASTERVISION_USE_DDP=YES`` (the default), and multiple GPUs are
+        detected, it will spawn DDP processes itself (one per GPU) when
+        training. DDP options that may be set via environment variables or an
+        INI file (see :ref:`raster vision config`) are:
+
+        - ``RASTERVISION_USE_DDP``: Use DDP? Default: ``YES``.
+        - ``RASTERVISION_DDP_BACKEND``: Default: ``nccl``.
+        - ``RASTERVISION_DDP_START_METHOD``: One of ``spawn``, ``fork``, or
+          ``forkserver``. Default: ``spawn``.
+
     """
 
     def __init__(self,
                  cfg: 'LearnerConfig',
                  output_dir: Optional[str] = None,
                  train_ds: Optional['Dataset'] = None,
                  valid_ds: Optional['Dataset'] = None,
@@ -133,78 +147,117 @@
             training (bool, optional): If False, the training apparatus (loss,
                 optimizer, scheduler, logging, etc.) will not be set up and the
                 model will be put into eval mode. If True, the training
                 apparatus will be set up and the model will be put into
                 training mode. Defaults to True.
         """
         self.cfg = cfg
-
-        if model is None and cfg.model is None:
+        self.training = training
+        self._onnx_mode = (model_weights_path is not None
+                           and model_weights_path.lower().endswith('.onnx'))
+        if self.onnx_mode and self.training:
+            raise ValueError('Training mode is not supported for ONNX models.')
+        if model is None and cfg.model is None and not self.onnx_mode:
             raise ValueError(
-                'cfg.model can only be None if a custom model is specified.')
+                'cfg.model can only be None if a custom model is specified '
+                'or if model_weights_path is an .onnx file.')
 
         if tmp_dir is None:
             self._tmp_dir = get_tmp_dir()
             tmp_dir = self._tmp_dir.name
         self.tmp_dir = tmp_dir
-        self.device = torch.device('cuda'
-                                   if torch.cuda.is_available() else 'cpu')
 
         self.train_ds = train_ds
         self.valid_ds = valid_ds
         self.test_ds = test_ds
 
+        self.train_dl = None
+        self.valid_dl = None
+        self.test_dl = None
+
         self.model = model
         self.loss = loss
         self.opt = optimizer
         self.epoch_scheduler = epoch_scheduler
         self.step_scheduler = step_scheduler
 
+        self.tb_process = None
+        self.tb_writer = None
+        self.tb_log_dir = None
+
+        self.setup_ddp_params()
+
+        if self.avoid_activating_cuda_runtime:
+            device = 'cuda'
+        else:
+            if torch.cuda.is_available():
+                device = 'cuda'
+            elif torch.backends.mps.is_available():
+                device = 'mps'
+            else:
+                device = 'cpu'
+
+        self.device = torch.device(device)
+
         # ---------------------------
         # Set URIs
         # ---------------------------
-        if output_dir is None and cfg.output_uri is None:
-            raise ValueError('output_dir or LearnerConfig.output_uri must '
-                             'be specified.')
-        if output_dir is not None and cfg.output_uri is not None:
-            log.warning(
-                'Both output_dir and LearnerConfig.output_uri specified. '
-                'LearnerConfig.output_uri will be ignored.')
-        if output_dir is None:
-            assert cfg.output_uri is not None
-            self.output_dir = cfg.output_uri
-            self.model_bundle_uri = cfg.get_model_bundle_uri()
-        else:
-            self.output_dir = output_dir
-            self.model_bundle_uri = join(self.output_dir, 'model-bundle.zip')
-        if is_local(self.output_dir):
-            self.output_dir_local = self.output_dir
-            make_dir(self.output_dir_local)
-        else:
-            self.output_dir_local = get_local_path(self.output_dir, tmp_dir)
-            make_dir(self.output_dir_local, force_empty=True)
-            if training and not cfg.overfit_mode:
-                self.sync_from_cloud()
-            log.info(f'Local output dir: {self.output_dir_local}')
-            log.info(f'Remote output dir: {self.output_dir}')
-
-        self.modules_dir = join(self.output_dir, MODULES_DIRNAME)
-        self.checkpoints_dir_local = join(self.output_dir_local,
-                                          CHECKPOINTS_DIRNAME)
-        make_dir(self.checkpoints_dir_local)
+        self.output_dir = None
+        self.output_dir_local = None
+        self.model_bundle_uri = None
+        self.modules_dir = None
+        self.checkpoints_dir_local = None
+
+        if self.training:
+            if output_dir is None and cfg.output_uri is None:
+                raise ValueError('output_dir or LearnerConfig.output_uri must '
+                                 'be specified in training mode.')
+            if output_dir is not None and cfg.output_uri is not None:
+                log.warning(
+                    'Both output_dir and LearnerConfig.output_uri specified. '
+                    'LearnerConfig.output_uri will be ignored.')
+            if output_dir is None:
+                assert cfg.output_uri is not None
+                self.output_dir = cfg.output_uri
+                self.model_bundle_uri = cfg.get_model_bundle_uri()
+            else:
+                self.output_dir = output_dir
+                self.model_bundle_uri = join(self.output_dir,
+                                             'model-bundle.zip')
+            if is_local(self.output_dir):
+                self.output_dir_local = self.output_dir
+                make_dir(self.output_dir_local)
+            else:
+                self.output_dir_local = get_local_path(self.output_dir,
+                                                       tmp_dir)
+                make_dir(self.output_dir_local, force_empty=True)
+                if self.training:
+                    self.sync_from_cloud()
+                log.info(f'Local output dir: {self.output_dir_local}')
+                log.info(f'Remote output dir: {self.output_dir}')
+
+            self.modules_dir = join(self.output_dir, MODULES_DIRNAME)
+            self.checkpoints_dir_local = join(self.output_dir_local,
+                                              CHECKPOINTS_DIRNAME)
+            make_dir(self.checkpoints_dir_local)
 
         # ---------------------------
-        self._onnx_mode = False
-        self.setup_model(
-            model_weights_path=model_weights_path,
-            model_def_path=model_def_path)
+        self.init_model_weights_path = model_weights_path
+        self.init_model_def_path = model_def_path
+        self.init_loss_def_path = loss_def_path
 
-        if training:
+        if not self.distributed:
+            self.setup_model(
+                model_weights_path=model_weights_path,
+                model_def_path=model_def_path)
+
+        if self.training:
             self.setup_training(loss_def_path=loss_def_path)
-            self.model.train()
+            if self.model is not None:
+                self.model.train()
         else:
             if not self.onnx_mode:
                 self.model.eval()
 
         self.visualizer = self.get_visualizer_class()(
             cfg.data.class_names, cfg.data.class_colors,
             cfg.data.plot_options.transform,
@@ -212,16 +265,16 @@
 
     @classmethod
     def from_model_bundle(cls: Type,
                           model_bundle_uri: str,
                           tmp_dir: Optional[str] = None,
                           cfg: Optional['LearnerConfig'] = None,
                           training: bool = False,
-                          use_onnx_model: bool = USE_ONNX,
-                          **kwargs) -> 'Learner':
+                          use_onnx_model: Optional[bool] = None,
+                          **kwargs) -> 'Self':
         """Create a Learner from a model bundle.
 
         .. note::
 
             This is the bundle saved in ``train/model-bundle.zip`` and not
             ``bundle/model-bundle.zip``.
 
@@ -234,15 +287,15 @@
             cfg (Optional[LearnerConfig], optional): If None, will be read from
                 the bundle. Defaults to None.
             training (bool, optional): If False, the training apparatus (loss,
                 optimizer, scheduler, logging, etc.) will not be set up and the
                 model will be put into eval mode. If True, the training
                 apparatus will be set up and the model will be put into
                 training mode. Defaults to True.
-            use_onnx_model (bool, optional): If True and training=False and a
+            use_onnx_model (Optional[bool]): If True and training=False and a
                 model.onnx file is available in the bundle, use that for
                 inference rather than the PyTorch weights. Defaults to the
                 boolean environment variable RASTERVISION_USE_ONNX if set,
                 False otherwise.
             **kwargs: Extra args for :meth:`.__init__`.
 
         Raises:
@@ -258,22 +311,15 @@
             tmp_dir = _tmp_dir.name
         model_bundle_path = download_if_needed(model_bundle_uri)
         model_bundle_dir = join(tmp_dir, 'model-bundle')
         log.info(f'Unzipping model-bundle to {model_bundle_dir}')
         unzip(model_bundle_path, model_bundle_dir)
 
         if cfg is None:
-            config_path = join(model_bundle_dir, 'pipeline-config.json')
-
-            config_dict = file_to_json(config_path)
-            config_dict = upgrade_config(config_dict)
-
-            learner_pipeline_cfg: 'LearnerPipelineConfig' = build_config(
-                config_dict)
-            cfg = learner_pipeline_cfg.learner
+            cfg = get_learner_config_from_bundle_dir(model_bundle_dir)
 
         hub_dir = join(model_bundle_dir, MODULES_DIRNAME)
         model_def_path = None
         loss_def_path = None
 
         # retrieve existing model definition, if available
         ext_cfg = cfg.model.external_def if cfg.model is not None else None
@@ -298,14 +344,17 @@
                 if not file_exists(tf['lambda_transforms_path']):
                     raise FileNotFoundError(
                         f'Custom transform definition file {tf_bundle_path} '
                         'was not found inside the bundle.')
             # config has been altered, so re-validate
             cfg = build_config(cfg.dict())
 
+        if use_onnx_model is None:
+            use_onnx_model = rv_config.get_namespace_option(
+                'rastervision', 'USE_ONNX', as_bool=True)
         onnx_mode = False
         if not training and use_onnx_model:
             onnx_path = join(model_bundle_dir, 'model.onnx')
             if file_exists(onnx_path):
                 model_weights_path = onnx_path
                 onnx_mode = True
 
@@ -342,75 +391,145 @@
     def main(self):
         """Main training sequence.
 
         This plots the dataset, runs a training and validation loop (which will
         resume if interrupted), logs stats, plots predictions, and syncs
         results to the cloud.
         """
-        log_system_details()
-        log.info(self.cfg)
-        log.info(f'Using device: {self.device}')
-        self.log_data_stats()
-        self.run_tensorboard()
+        if self.distributed:
+            with self.ddp():
+                self._main()
+        else:
+            self._main()
 
+    def _main(self):
         cfg = self.cfg
-        if not cfg.predict_mode:
-            self.plot_dataloaders(self.cfg.data.preview_batch_limit)
-            if cfg.overfit_mode:
-                self.overfit()
-            else:
-                self.train()
-                if cfg.save_model_bundle:
-                    self.save_model_bundle()
-        else:
-            self.load_checkpoint()
+        if not self.is_ddp_process or self.is_ddp_local_master:
+            if not self.avoid_activating_cuda_runtime:
+                log_system_details()
+            log.info(cfg)
+        log.info(f'Using device: {self.device}')
+
+        if not self.distributed:
+            self.run_tensorboard()
 
+        self.train()
+        if cfg.save_model_bundle:
+            if not self.is_ddp_process or self.is_ddp_master:
+                self.save_model_bundle()
         self.stop_tensorboard()
         if cfg.eval_train:
-            self.eval_model('train')
-        self.eval_model('valid')
-        self.sync_to_cloud()
+            self.validate('train')
+        self.validate('valid')
+        if not self.is_ddp_process or self.is_ddp_master:
+            self.sync_to_cloud()
 
     ###########################
     # Training and validation
     ###########################
     def train(self, epochs: Optional[int] = None):
-        """Training loop that will attempt to resume training if appropriate."""
-        start_epoch = self.get_start_epoch()
+        """Run training loop, resuming training if appropriate"""
+        start_epoch, end_epoch = self.get_start_and_end_epochs(epochs)
 
-        if epochs is None:
-            end_epoch = self.cfg.solver.num_epochs
-        else:
-            end_epoch = start_epoch + epochs
+        if start_epoch >= end_epoch:
+            log.info('Training already completed. Skipping.')
+            return
 
         if (start_epoch > 0 and start_epoch < end_epoch):
-            log.info(f'Resuming training from epoch {start_epoch}')
+            log.info('Resuming training from epoch %d', start_epoch)
 
+        if self.is_ddp_process:  # pragma: no cover
+            self._run_train_distributed(self.ddp_rank, self.ddp_world_size,
+                                        start_epoch, end_epoch)
+        elif self.distributed:  # pragma: no cover
+            log.info('Spawning %d DDP processes', self.ddp_world_size)
+            mp.start_processes(
+                self._run_train_distributed,
+                args=(self.ddp_world_size, start_epoch, end_epoch),
+                nprocs=self.ddp_world_size,
+                join=True,
+                start_method=self.ddp_start_method)
+        else:
+            self._train(start_epoch, end_epoch)
+
+    def _train(self, start_epoch: int, end_epoch: int):  # pragma: no cover
+        """Training loop."""
         self.on_train_start()
         for epoch in range(start_epoch, end_epoch):
             log.info(f'epoch: {epoch}')
+
             train_metrics = self.train_epoch(
                 optimizer=self.opt, step_scheduler=self.step_scheduler)
+
             if self.epoch_scheduler:
                 self.epoch_scheduler.step()
+
             valid_metrics = self.validate_epoch(self.valid_dl)
+
             metrics = dict(epoch=epoch, **train_metrics, **valid_metrics)
             log.info(f'metrics:\n{pformat(metrics, sort_dicts=False)}')
 
             self.on_epoch_end(epoch, metrics)
 
+    def _train_distributed(self, start_epoch: int,
+                           end_epoch: int):  # pragma: no cover
+        """Distributed training loop."""
+        if self.is_ddp_master:
+            self.on_train_start()
+
+        train_dl = self.build_dataloader('train', distributed=True)
+        val_dl = self.build_dataloader('valid', distributed=True)
+        for epoch in range(start_epoch, end_epoch):
+            log.info(f'epoch: {epoch}')
+
+            train_dl.sampler.set_epoch(epoch)
+
+            train_metrics = self.train_epoch(
+                optimizer=self.opt,
+                step_scheduler=self.step_scheduler,
+                dataloader=train_dl)
+
+            valid_metrics = self.validate_epoch(val_dl)
+
+            if self.is_ddp_master:
+                metrics = dict(epoch=epoch, **train_metrics, **valid_metrics)
+                log.info(f'metrics:\n{pformat(metrics, sort_dicts=False)}')
+                self.on_epoch_end(epoch, metrics)
+
+            if self.epoch_scheduler:
+                self.epoch_scheduler.step()
+
+            dist.barrier()
+
+    def _run_train_distributed(self, rank: int, world_size: int,
+                               *args):  # pragma: no cover
+        """Method executed by each DDP worker."""
+        with self.ddp(rank, world_size):
+            self.setup_model(
+                model_weights_path=self.init_model_weights_path,
+                model_def_path=self.init_model_def_path)
+            self.setup_training(self.init_loss_def_path)
+            self._train_distributed(*args)
+
     def train_epoch(
             self,
             optimizer: 'Optimizer',
+            dataloader: Optional[DataLoader] = None,
             step_scheduler: Optional['_LRScheduler'] = None) -> MetricDict:
         """Train for a single epoch."""
-        start = time.time()
         self.model.train()
+        if dataloader is None:
+            dataloader = self.train_dl
+        start = perf_counter()
         outputs = []
-        with tqdm(self.train_dl, desc='Training') as bar:
+        if self.ddp_rank is not None:
+            desc = f'Training (GPU={self.ddp_rank})'
+        else:
+            desc = 'Training'
+        with tqdm(self.train_dl, desc=desc) as bar:
             for batch_ind, (x, y) in enumerate(bar):
                 x = self.to_device(x, self.device)
                 y = self.to_device(y, self.device)
                 batch = (x, y)
                 optimizer.zero_grad()
                 output = self.train_step(batch, batch_ind)
                 output['train_loss'].backward()
@@ -420,15 +539,15 @@
                     output[k] = v.detach() if isinstance(v, Tensor) else v
                 outputs.append(output)
                 if step_scheduler is not None:
                     step_scheduler.step()
         if len(outputs) == 0:
             raise ValueError('Training dataset did not return any batches')
         metrics = self.train_end(outputs)
-        end = time.time()
+        end = perf_counter()
         train_time = datetime.timedelta(seconds=end - start)
         metrics['train_time'] = str(train_time)
         return metrics
 
     @abstractmethod
     def train_step(self, batch: Any, batch_ind: int) -> MetricDict:
         """Compute loss for a single training batch.
@@ -436,59 +555,98 @@
         Args:
             batch: batch data needed to compute loss
             batch_ind: index of batch within epoch
 
         Returns:
             dict with 'train_loss' as key and possibly other losses
         """
-        pass
 
     def on_train_start(self):
         """Hook that is called at start of train routine."""
-        pass
+        self.log_data_stats()
+        self.plot_dataloaders(self.cfg.data.preview_batch_limit)
 
     def train_end(self, outputs: List[Dict[str, Union[float, Tensor]]]
                   ) -> MetricDict:
-        """Aggregate the ouput of train_step at the end of the epoch.
+        """Aggregate the output of train_step at the end of the epoch.
 
         Args:
             outputs: a list of outputs of train_step
         """
-        return aggregate_metrics(outputs)
+        metrics = aggregate_metrics(outputs)
+        if self.is_ddp_process:
+            metrics = self.reduce_distributed_metrics(metrics)
+        return metrics
 
-    def eval_model(self, split: str):
-        """Evaluate model using a particular dataset split.
+    def validate(self, split: Literal['train', 'valid', 'test'] = 'valid'):
+        """Evaluate model on a particular data split."""
+        if self.is_ddp_process:  # pragma: no cover
+            self._run_validate_distributed(self.ddp_rank, self.ddp_world_size,
+                                           split)
+        elif self.distributed:  # pragma: no cover
+            log.info('Spawning DDP processes')
+            mp.start_processes(
+                self._run_validate_distributed,
+                args=(self.ddp_world_size, split),
+                nprocs=self.ddp_world_size,
+                join=True,
+                start_method=self.ddp_start_method)
+        else:
+            self._validate(split)
+
+    def _validate(self, split: Literal['train', 'valid', 'test'] = 'valid'
+                  ):  # pragma: no cover
+        """Evaluate model on a particular data split.
 
         Gets validation metrics and saves them along with prediction plots.
 
         Args:
             split: the dataset split to use: train, valid, or test.
         """
         log.info(f'Evaluating on {split} set...')
         dl = self.get_dataloader(split)
+        if dl is None:
+            self.setup_data()
+        dl = self.get_dataloader(split)
         metrics = self.validate_epoch(dl)
+        if self.is_ddp_process and not self.is_ddp_master:
+            return
         log.info(f'metrics: {metrics}')
         json_to_file(metrics,
                      join(self.output_dir_local, f'{split}_metrics.json'))
         self.plot_predictions(split, self.cfg.data.preview_batch_limit)
 
+    def _run_validate_distributed(self, rank: int, world_size: int,
+                                  *args):  # pragma: no cover
+        """Method executed by each DDP worker."""
+        with self.ddp(rank, world_size):
+            self.setup_model(
+                model_weights_path=self.init_model_weights_path,
+                model_def_path=self.init_model_def_path)
+            self.setup_training(self.init_loss_def_path)
+            self._validate(*args)
+
     def validate_epoch(self, dl: DataLoader) -> MetricDict:
         """Validate for a single epoch."""
-        start = time.time()
+        start = perf_counter()
         self.model.eval()
         outputs = []
+        if self.ddp_rank is not None:
+            desc = f'Validating (GPU={self.ddp_rank})'
+        else:
+            desc = 'Validating'
         with torch.inference_mode():
-            with tqdm(dl, desc='Validating') as bar:
+            with tqdm(dl, desc=desc) as bar:
                 for batch_ind, (x, y) in enumerate(bar):
                     x = self.to_device(x, self.device)
                     y = self.to_device(y, self.device)
                     batch = (x, y)
                     output = self.validate_step(batch, batch_ind)
                     outputs.append(output)
-        end = time.time()
+        end = perf_counter()
         validate_time = datetime.timedelta(seconds=end - start)
 
         metrics = self.validate_end(outputs)
         metrics['valid_time'] = str(validate_time)
         return metrics
 
     @abstractmethod
@@ -498,24 +656,26 @@
         Args:
             batch: batch data needed to compute validation metrics
             batch_ind: index of batch within epoch
 
         Returns:
             dict with metric names mapped to metric values
         """
-        pass
 
     def validate_end(self, outputs: List[Dict[str, Union[float, Tensor]]]
                      ) -> MetricDict:
-        """Aggregate the ouput of validate_step at the end of the epoch.
+        """Aggregate the output of validate_step at the end of the epoch.
 
         Args:
             outputs: a list of outputs of validate_step
         """
-        return aggregate_metrics(outputs)
+        metrics = aggregate_metrics(outputs)
+        if self.is_ddp_process:
+            metrics = self.reduce_distributed_metrics(metrics)
+        return metrics
 
     def on_epoch_end(self, curr_epoch: int, metrics: MetricDict) -> None:
         """Hook that is called at end of epoch.
 
         Writes metrics to CSV and TensorBoard, and saves model.
         """
         log_metrics_to_csv(self.log_path, metrics)
@@ -527,45 +687,19 @@
             self.tb_writer.flush()
 
         if self.cfg.save_all_checkpoints and curr_epoch > 0:
             checkpoint_name = f'model-ckpt-epoch-{curr_epoch - 1}.pth'
             checkpoint_path = join(self.checkpoints_dir_local, checkpoint_name)
             shutil.move(self.last_model_weights_path, checkpoint_path)
 
-        torch.save(self.model.state_dict(), self.last_model_weights_path)
+        self.save_weights(self.last_model_weights_path)
 
         if (curr_epoch + 1) % self.cfg.solver.sync_interval == 0:
             self.sync_to_cloud()
 
-    def overfit(self):
-        """Optimize model using the same batch repeatedly."""
-        self.on_overfit_start()
-
-        x, y = next(iter(self.train_dl))
-        x = self.to_device(x, self.device)
-        y = self.to_device(y, self.device)
-        batch = (x, y)
-
-        num_steps = self.cfg.solver.overfit_num_steps
-        with tqdm(range(num_steps), desc='Overfitting') as bar:
-            for step in bar:
-                loss = self.train_step(batch, step)['train_loss']
-                loss.backward()
-                self.opt.step()
-
-                if (step + 1) % 25 == 0:
-                    log.info('\nstep: {}'.format(step))
-                    log.info('train_loss: {}'.format(loss))
-
-        torch.save(self.model.state_dict(), self.last_model_weights_path)
-
-    def on_overfit_start(self):
-        """Hook that is called at start of overfit routine."""
-        pass
-
     ########################
     # Prediction/inference
     ########################
     def predict(self, x: Tensor, raw_out: bool = False) -> Any:
         """Make prediction for an image or batch of images.
 
         Args:
@@ -635,18 +769,25 @@
             whatever type the predictions are. Otherwise, the returned value is
             an iterator of tuples.
         """
 
         if return_format not in {'xyz', 'yz', 'z'}:
             raise ValueError('return_format must be one of "xyz", "yz", "z".')
 
+        cfg = self.cfg
+
+        num_workers = rv_config.get_namespace_option(
+            'rastervision',
+            'PREDICT_NUM_WORKERS',
+            default=cfg.data.num_workers)
+
         dl_kw = dict(
             collate_fn=self.get_collate_fn(),
-            batch_size=self.cfg.solver.batch_sz,
-            num_workers=self.cfg.data.num_workers,
+            batch_size=cfg.solver.batch_sz if cfg.solver else 1,
+            num_workers=int(num_workers),
             shuffle=False,
             pin_memory=True)
         dl_kw.update(dataloader_kw)
         dl = DataLoader(dataset, **dl_kw)
 
         preds = self.predict_dataloader(
             dl,
@@ -783,41 +924,168 @@
         The class ids should be the classes with the maximum probability.
         """
         raise NotImplementedError()
 
     #########
     # Setup
     #########
-    def setup_training(self, loss_def_path: Optional[str] = None) -> None:
-        cfg = self.cfg
+    def setup_ddp_params(self):
+        """Set up and validate params related to PyTorch DDP."""
 
-        self.config_path = join(self.output_dir, 'learner-config.json')
-        str_to_file(cfg.json(), self.config_path)
+        ddp_allowed = rv_config.get_namespace_option(
+            'rastervision', 'USE_DDP', True, as_bool=True)
+        self.ddp_start_method = rv_config.get_namespace_option(
+            'rastervision', 'DDP_START_METHOD', 'spawn').lower()
+
+        self.is_ddp_process = False
+        self.is_ddp_master = False
+        self.is_ddp_local_master = False
+        self.avoid_activating_cuda_runtime = False
+
+        self.ddp_world_size = get_env_var('WORLD_SIZE', None, int)
+        self.ddp_rank = get_env_var('RANK', None, int)
+        self.ddp_local_rank = get_env_var('LOCAL_RANK', None, int)
+        ddp_vars_set = all(
+            v is not None
+            for v in [self.ddp_world_size, self.ddp_rank, self.ddp_local_rank])
+
+        if not ddp_allowed or not self.training:
+            self.distributed = False
+        elif ddp_vars_set:  # pragma: no cover
+            self.distributed = True
+            self.is_ddp_process = True
+            self.is_ddp_master = self.ddp_rank == 0
+            self.is_ddp_local_master = self.ddp_local_rank == 0
+        elif self.ddp_start_method != 'spawn':
+            # If ddp_start_method is "fork" or "forkserver", the CUDA runtime
+            # must not be initialized before the fork; otherwise, a
+            # "RuntimeError: Cannot re-initialize CUDA in forked subprocess."
+            # error will be raised. We can avoid initializing it by not
+            # calling any torch.cuda functions or creating tensors on the GPU.
+            if self.ddp_world_size is None:
+                raise ValueError(
+                    'WORLD_SIZE env variable must be specified if '
+                    'RASTERVISION_DDP_START_METHOD is not "spawn".')
+            self.distributed = True
+            self.avoid_activating_cuda_runtime = True
+        elif torch.cuda.is_available():
+            dist_available = dist.is_available()
+            gpu_count = torch.cuda.device_count()
+            multi_gpus = gpu_count > 1
+            self.distributed = ddp_allowed and dist_available and multi_gpus
+            if self.distributed:
+                log.info(
+                    'Multiple GPUs detected (%d), will use DDP for training.',
+                    gpu_count)
+                world_size_is_set = self.ddp_world_size is not None
+                if not world_size_is_set:
+                    self.ddp_world_size = gpu_count
+                if world_size_is_set and self.ddp_world_size < gpu_count:
+                    log.info('Using only WORLD_SIZE=%d of total %d GPUs.',
+                             self.ddp_world_size, gpu_count)
+        else:
+            self.distributed = False
 
-        self.log_path = join(self.output_dir_local, 'log.csv')
+        if not self.distributed:
+            return
+
+        # pragma: no cover
+        if self.model is not None:
+            raise ValueError(
+                'In distributed mode, the model must be specified via '
+                'ModelConfig in LearnerConfig rather than be passed '
+                'as an instantiated object.')
+
+        dses_passed = any([self.train_ds, self.valid_ds, self.test_ds])
+        if dses_passed and self.ddp_start_method != 'fork':
+            raise ValueError(
+                'In distributed mode, if '
+                'RASTERVISION_DDP_START_METHOD != "fork", datasets must be '
+                'specified via DataConfig in LearnerConfig rather than be '
+                'passed as instantiated objects.')
+
+        if self.ddp_local_rank is not None:
+            self.device = torch.device('cuda', self.ddp_local_rank)
+
+        log.info('Using DDP')
+        log.info(f'World size: {self.ddp_world_size}')
+        log.info(f'DDP start method: {self.ddp_start_method}')
+        if self.is_ddp_process:
+            log.info(f'DDP rank: {self.ddp_rank}')
+            log.info(f'DDP local rank: {self.ddp_local_rank}')
+
+    def setup_training(self, loss_def_path: Optional[str] = None) -> None:
+        """Set up model, data, loss, optimizers and various paths.
 
-        # data
-        self.setup_data()
+        The exact behavior differs based on whether this method is called in
+        a distributed scenario.
 
-        # model
+        Args:
+            loss_def_path: A local path to a directory with a ``hubconf.py``. If
+                provided, the loss function definition is imported from here.
+                This is used when loading an external loss function from a
+                model-bundle. Defaults to ``None``.
+        """
+        cfg = self.cfg
+
+        self.config_path = join(self.output_dir_local, 'learner-config.json')
+        cfg.to_file(self.config_path)
+        self.log_path = join(self.output_dir_local, 'log.csv')
         self.last_model_weights_path = join(self.output_dir_local,
                                             'last-model.pth')
-        self.load_checkpoint()
 
-        # optimization
-        start_epoch = self.get_start_epoch()
-        self.setup_loss(loss_def_path=loss_def_path)
-        if self.opt is None:
-            self.opt = self.build_optimizer()
-        if self.step_scheduler is None:
-            self.step_scheduler = self.build_step_scheduler(start_epoch)
-        if self.epoch_scheduler is None:
-            self.epoch_scheduler = self.build_epoch_scheduler(start_epoch)
+        if not self.distributed:
+            # data
+            self.setup_data()
+            # model
+            self.load_checkpoint()
+            # optimization
+            start_epoch = self.get_start_epoch()
+            self.setup_loss(loss_def_path=loss_def_path)
+            if self.opt is None:
+                self.opt = self.build_optimizer()
+            if self.step_scheduler is None:
+                self.step_scheduler = self.build_step_scheduler(start_epoch)
+            if self.epoch_scheduler is None:
+                self.epoch_scheduler = self.build_epoch_scheduler(start_epoch)
+            self.setup_tensorboard()
+            return
 
-        self.setup_tensorboard()
+        # DDP
+        if self.is_ddp_process and dist.is_initialized():  # pragma: no cover
+            # model
+            if self.model is not None:
+                self.load_checkpoint()
+            # data
+            self.setup_data()
+            # optimization
+            start_epoch = self.get_start_epoch()
+            self.setup_loss(loss_def_path=loss_def_path)
+            if self.opt is None:
+                self.opt = self.build_optimizer()
+            if self.step_scheduler is None:
+                self.step_scheduler = self.build_step_scheduler(start_epoch)
+            if self.epoch_scheduler is None:
+                self.epoch_scheduler = self.build_epoch_scheduler(start_epoch)
+
+            if self.is_ddp_master:
+                self.setup_tensorboard()
+        else:  # pragma: no cover
+            if self.ddp_start_method == 'fork':
+                self.setup_data()
+
+    def get_start_and_end_epochs(
+            self, epochs: Optional[int] = None) -> Tuple[int, int]:
+        """Get start and end epochs given epochs."""
+        start_epoch = self.get_start_epoch()
+        if epochs is None:
+            end_epoch = self.cfg.solver.num_epochs
+        else:
+            end_epoch = start_epoch + epochs
+        return start_epoch, end_epoch
 
     def get_start_epoch(self) -> int:
         """Get start epoch.
 
         If training was interrupted, this returns the last complete epoch + 1.
         """
         start_epoch = 0
@@ -840,22 +1108,23 @@
         Args:
             model_weights_path (Optional[str], optional): Path to model
                 weights. Will be available when loading from a bundle.
                 Defaults to None.
             model_def_path (Optional[str], optional): Path to model definition.
                 Will be available when loading from a bundle. Defaults to None.
         """
-        self._onnx_mode = (model_weights_path is not None
-                           and model_weights_path.lower().endswith('.onnx'))
-        if self._onnx_mode:
+        if self.onnx_mode:
             self.model = self.load_onnx_model(model_weights_path)
             return
         if self.model is None:
             self.model = self.build_model(model_def_path=model_def_path)
         self.model.to(device=self.device)
+        if self.is_ddp_process:  # pragma: no cover
+            self.model = nn.SyncBatchNorm.convert_sync_batchnorm(self.model)
+            self.model = DDP(self.model, device_ids=[self.ddp_local_rank])
         self.load_init_weights(model_weights_path=model_weights_path)
 
     def build_model(self, model_def_path: Optional[str] = None) -> nn.Module:
         """Build a PyTorch model."""
         cfg = self.cfg
 
         in_channels = cfg.data.img_channels
@@ -863,92 +1132,161 @@
             log.warning('DataConfig.img_channels is None. Defaulting to 3.')
             in_channels = 3
 
         model = cfg.model.build(
             num_classes=cfg.data.num_classes,
             in_channels=in_channels,
             save_dir=self.modules_dir,
-            hubconf_dir=model_def_path)
+            hubconf_dir=model_def_path,
+            ddp_rank=self.ddp_local_rank)
         return model
 
-    def setup_data(self):
+    def setup_data(self, distributed: Optional[bool] = None):
         """Set datasets and dataLoaders for train, validation, and test sets.
         """
+        if distributed is None:
+            distributed = self.distributed
+
         if self.train_ds is None or self.valid_ds is None:
-            train_ds, valid_ds, test_ds = self.build_datasets()
+            if distributed:  # pragma: no cover
+                if self.is_ddp_local_master:
+                    train_ds, valid_ds, test_ds = self.build_datasets()
+                    log.debug(f'{self.ddp_rank=} Done.')
+                else:
+                    log.debug(f'{self.ddp_rank=} Waiting.')
+                dist.barrier()
+                if not self.is_ddp_local_master:
+                    train_ds, valid_ds, test_ds = self.build_datasets()
+                    log.debug(f'{self.ddp_rank=} Done.')
+                else:
+                    log.debug(f'{self.ddp_rank=} Waiting.')
+                dist.barrier()
+            else:
+                train_ds, valid_ds, test_ds = self.build_datasets()
+
             if self.train_ds is None:
                 self.train_ds = train_ds
             if self.valid_ds is None:
                 self.valid_ds = valid_ds
             if self.test_ds is None:
                 self.test_ds = test_ds
-        self.train_dl, self.valid_dl, self.test_dl = self.build_dataloaders()
+
+        log.info('Building dataloaders')
+        self.train_dl, self.valid_dl, self.test_dl = self.build_dataloaders(
+            distributed=distributed)
 
     def build_datasets(self) -> Tuple['Dataset', 'Dataset', 'Dataset']:
+        """Build Datasets for train, validation, and test splits."""
         log.info(f'Building datasets ...')
-        cfg = self.cfg
-        train_ds, val_ds, test_ds = self.cfg.data.build(
-            tmp_dir=self.tmp_dir,
-            overfit_mode=cfg.overfit_mode,
-            test_mode=cfg.test_mode)
+        train_ds, val_ds, test_ds = self.cfg.data.build(tmp_dir=self.tmp_dir)
         return train_ds, val_ds, test_ds
 
-    def build_dataloaders(self) -> Tuple[DataLoader, DataLoader, DataLoader]:
-        """Set the DataLoaders for train, validation, and test sets."""
+    def build_dataset(self,
+                      split: Literal['train', 'valid', 'test']) -> 'Dataset':
+        """Build Dataset for split."""
+        log.info('Building %s dataset ...', split)
+        ds = self.cfg.data.build_dataset(split=split, tmp_dir=self.tmp_dir)
+        return ds
+
+    def build_dataloaders(self, distributed: Optional[bool] = None
+                          ) -> Tuple[DataLoader, DataLoader, DataLoader]:
+        """Build DataLoaders for train, validation, and test splits."""
+        if distributed is None:
+            distributed = self.distributed
+
+        train_dl = self.build_dataloader('train', distributed=distributed)
+        val_dl = self.build_dataloader('valid', distributed=distributed)
+
+        test_dl = None
+        if self.test_ds is not None and len(self.test_ds) > 0:
+            test_dl = self.build_dataloader('test', distributed=distributed)
+
+        return train_dl, val_dl, test_dl
+
+    def build_dataloader(self,
+                         split: Literal['train', 'valid', 'test'],
+                         distributed: Optional[bool] = None,
+                         **kwargs) -> DataLoader:
+        """Build DataLoader for split."""
+        if distributed is None:
+            distributed = self.distributed
+
+        ds = self.get_dataset(split)
+        if ds is None:
+            ds = self.build_dataset(split)
 
         batch_sz = self.cfg.solver.batch_sz
         num_workers = self.cfg.data.num_workers
         collate_fn = self.get_collate_fn()
+        sampler = self.build_sampler(ds, split, distributed=distributed)
 
-        train_sampler = self.get_train_sampler(self.train_ds)
-        train_shuffle = train_sampler is None
-        # batchnorm layers expect batch size > 1 during training
-        train_drop_last = (len(self.train_ds) % batch_sz) == 1
-        train_dl = DataLoader(
-            self.train_ds,
-            batch_size=batch_sz,
-            shuffle=train_shuffle,
-            drop_last=train_drop_last,
-            num_workers=num_workers,
-            pin_memory=True,
-            collate_fn=collate_fn,
-            sampler=train_sampler)
+        if distributed:  # pragma: no cover
+            world_sz = self.ddp_world_size
+            if world_sz is None:
+                raise ValueError('World size not set. '
+                                 'Cannot determine per-process batch size.')
+            if world_sz > batch_sz:
+                raise ValueError(f'World size ({world_sz}) is greater '
+                                 f'than total batch size ({batch_sz}).')
+            batch_sz //= world_sz
+            log.debug('Per GPU batch size: %d', batch_sz)
 
-        val_dl = DataLoader(
-            self.valid_ds,
+        args = dict(
             batch_size=batch_sz,
-            shuffle=True,
             num_workers=num_workers,
             collate_fn=collate_fn,
-            pin_memory=True)
+            pin_memory=True,
+            multiprocessing_context='fork' if distributed else None,
+        )
+        args.update(**kwargs)
 
-        test_dl = None
-        if self.test_ds is not None and len(self.test_ds) > 0:
-            test_dl = DataLoader(
-                self.test_ds,
-                batch_size=batch_sz,
-                shuffle=True,
-                num_workers=num_workers,
-                collate_fn=collate_fn,
-                pin_memory=True)
+        if sampler is not None:
+            args['sampler'] = sampler
+        else:
+            if split == 'train':
+                args['shuffle'] = True
+                # batchnorm layers expect batch size > 1 during training
+                args['drop_last'] = (len(ds) % batch_sz) == 1
+            else:
+                args['shuffle'] = False
 
-        return train_dl, val_dl, test_dl
+        dl = DataLoader(ds, **args)
+        return dl
 
     def get_collate_fn(self) -> Optional[callable]:
         """Returns a custom collate_fn to use in DataLoader.
 
         None is returned if default collate_fn should be used.
 
         See https://pytorch.org/docs/stable/data.html#working-with-collate-fn
         """
         return None
 
-    def get_train_sampler(self, train_ds: 'Dataset') -> Optional['Sampler']:
-        """Return an optional sampler for the training dataloader."""
-        return None
+    def build_sampler(self,
+                      ds: 'Dataset',
+                      split: Literal['train', 'valid', 'test'],
+                      distributed: bool = False) -> Optional['Sampler']:
+        """Build an optional sampler for the split's dataloader."""
+        split = split.lower()
+        sampler = None
+        if split == 'train':
+            if distributed:  # pragma: no cover
+                sampler = DistributedSampler(
+                    ds,
+                    shuffle=True,
+                    num_replicas=self.ddp_world_size,
+                    rank=self.ddp_rank)
+        elif split == 'valid':
+            if distributed:  # pragma: no cover
+                sampler = DistributedSampler(
+                    ds,
+                    shuffle=False,
+                    num_replicas=self.ddp_world_size,
+                    rank=self.ddp_rank)
+        return sampler
 
     def setup_loss(self, loss_def_path: Optional[str] = None) -> None:
         """Setup self.loss.
 
         Args:
             loss_def_path (str, optional): Loss definition path. Will be
             available when loading from a bundle. Defaults to None.
@@ -986,18 +1324,17 @@
 
     ################
     # Visualization
     ################
     @abstractmethod
     def get_visualizer_class(self) -> Type[Visualizer]:
         """Returns a Visualizer class object for plotting data samples."""
-        pass
 
     def plot_predictions(self,
-                         split: str,
+                         split: Literal['train', 'valid', 'test'],
                          batch_limit: Optional[int] = None,
                          show: bool = False):
         """Plot predictions for a split.
 
         Uses the first batch for the corresponding DataLoader.
 
         Args:
@@ -1059,17 +1396,14 @@
     #########
     def save_model_bundle(self, export_onnx: bool = True):
         """Save a model bundle.
 
         This is a zip file with the model weights in .pth format and a serialized
         copy of the LearningConfig, which allows for making predictions in the future.
         """
-        from rastervision.pytorch_learner.learner_pipeline_config import (
-            LearnerPipelineConfig)
-
         if self.cfg.model is None:
             log.warning(
                 'Model was not configured via ModelConfig, and therefore, '
                 'will not be reconstructable form the model-bundle. You will '
                 'need to initialize the model yourself and pass it to '
                 'from_model_bundle().')
 
@@ -1077,37 +1411,44 @@
         model_bundle_dir = join(self.tmp_dir, 'model-bundle')
         make_dir(model_bundle_dir, force_empty=True)
 
         self._bundle_model(model_bundle_dir, export_onnx=export_onnx)
         self._bundle_modules(model_bundle_dir)
         self._bundle_transforms(model_bundle_dir)
 
-        pipeline_cfg = LearnerPipelineConfig(learner=self.cfg)
-        save_pipeline_config(pipeline_cfg,
-                             join(model_bundle_dir, 'pipeline-config.json'))
+        cfg_uri = join(model_bundle_dir, 'learner-config.json')
+        shutil.copy(self.config_path, cfg_uri)
 
         zip_path = join(self.output_dir_local, basename(self.model_bundle_uri))
         log.info(f'Saving bundle to {zip_path}.')
         zipdir(model_bundle_dir, zip_path)
 
     def _bundle_model(self, model_bundle_dir: str,
                       export_onnx: bool = True) -> None:
-        """Save model weights and copy them to bundle dir.."""
-        # pytorch
+        """Save model weights and copy them to bundle dir."""
+        model_not_set = self.model is None
+        if model_not_set:
+            self.model = self.build_model(self.init_model_def_path).cpu()
+            self.load_checkpoint()
+
         path = join(model_bundle_dir, BUNDLE_MODEL_WEIGHTS_FILENAME)
         if file_exists(self.last_model_weights_path):
             shutil.copyfile(self.last_model_weights_path, path)
         else:
-            torch.save(self.model.state_dict(), path)
+            self.save_weights(path)
 
         # ONNX
         if export_onnx:
             path = join(model_bundle_dir, BUNDLE_MODEL_ONNX_FILENAME)
             self.export_to_onnx(path)
 
+        if model_not_set:
+            self.model = None
+            gc.collect()
+
     def export_to_onnx(self,
                        path: str,
                        model: Optional['nn.Module'] = None,
                        sample_input: Optional[Tensor] = None,
                        validate_export: bool = True,
                        **kwargs) -> None:
         """Export model to ONNX format via :func:`torch.onnx.export`.
@@ -1129,28 +1470,31 @@
         Raises:
             ValueError: If sample_input is None and the Learner has no valid
                 DataLoaders.
         """
         if model is None:
             model = self.model
 
+        if isinstance(model, DDP):
+            model = model.module
+
         training_state = model.training
 
         model.eval()
         if sample_input is None:
-            for split in ['train', 'valid', 'test']:
-                dl = self.get_dataloader(split)
-                if dl is not None:
-                    break
-            else:
-                raise ValueError('sample_input not provided and Learner does '
-                                 'not have a DataLoader to get sample input '
-                                 'from.')
+            dl = self.valid_dl
+            if dl is None:
+                dl = self.build_dataloader(
+                    'valid', batch_size=1, num_workers=0, distributed=False)
             sample_input, _ = next(iter(dl))
-        sample_input = self.to_device(sample_input, self.device)
+
+        model_device = next(model.parameters()).device
+        if model_device.type == 'cuda':
+            torch.cuda.empty_cache()
+        sample_input = self.to_device(sample_input, model_device)
 
         args = dict(
             input_names=['x'],
             output_names=['out'],
             dynamic_axes={
                 'x': {
                     0: 'batch_size',
@@ -1208,14 +1552,48 @@
             tf['lambda_transforms_path'] = join('model-bundle',
                                                 TRANSFORMS_DIRNAME,
                                                 basename(tf_bundle_path))
 
     #########
     # Misc.
     #########
+    def ddp(self, rank: Optional[int] = None, world_size: Optional[int] = None
+            ) -> DDPContextManager:  # pragma: no cover
+        """Return a :class:`DDPContextManager`.
+
+        This should be used to wrap code that needs to be executed in parallel.
+        It is safe call this recursively; recusive calls will have no affect.
+
+        Note that :class:`DDPContextManager` does not start processes itself,
+        but merely initializes and destroyes DDP process groups.
+
+        Usage:
+
+        .. code-block:: python
+
+            with learner.ddp([rank], [world_size]):
+                ...
+
+        """
+        if not self.distributed:
+            raise ValueError('self.distributed is False')
+        return DDPContextManager(self, rank, world_size)
+
+    def reduce_distributed_metrics(self, metrics: dict):  # pragma: no cover
+        """Average numeric metrics across processes."""
+        for k in metrics.keys():
+            v = metrics[k]
+            if isinstance(v, (float, int)):
+                v = torch.tensor(v, device=self.device)
+            if isinstance(v, Tensor):
+                dist.reduce(v, dst=0, op=dist.ReduceOp.SUM)
+                if self.is_ddp_master:
+                    metrics[k] = (v / self.ddp_world_size).item()
+        return metrics
+
     def post_forward(self, x: Any) -> Any:
         """Post process output of call to model().
 
         Useful for when predictions are inside a structure returned by model().
         """
         return x
 
@@ -1228,43 +1606,58 @@
         Returns:
             x with extra batch dimension of length 1 if needed
         """
         if x.ndim == 3:
             x = x[None, ...]
         return x
 
-    def to_device(self, x: Any, device: str) -> Any:
+    def to_device(self, x: Any, device: Union[str, torch.device]) -> Any:
         """Load Tensors onto a device.
 
         Args:
             x: some object with Tensors in it
             device: 'cpu' or 'cuda'
 
         Returns:
             x but with any Tensors in it on the device
         """
         if isinstance(x, list):
             return [_x.to(device) if _x is not None else _x for _x in x]
         else:
             return x.to(device)
 
-    def get_dataloader(self, split: str) -> DataLoader:
+    def get_dataset(self, split: Literal['train', 'valid', 'test']
+                    ) -> Optional[DataLoader]:
+        """Get the Dataset for a split.
+
+        Args:
+            split: a split name which can be train, valid, or test
+        """
+        if split == 'train':
+            return self.train_ds
+        if split == 'valid':
+            return self.valid_ds
+        if split == 'test':
+            return self.test_ds
+        raise ValueError(f'{split} is not a valid split')
+
+    def get_dataloader(self,
+                       split: Literal['train', 'valid', 'test']) -> DataLoader:
         """Get the DataLoader for a split.
 
         Args:
             split: a split name which can be train, valid, or test
         """
         if split == 'train':
             return self.train_dl
-        elif split == 'valid':
+        if split == 'valid':
             return self.valid_dl
-        elif split == 'test':
+        if split == 'test':
             return self.test_dl
-        else:
-            raise ValueError('{} is not a valid split'.format(split))
+        raise ValueError(f'{split} is not a valid split')
 
     def normalize_input(self, x: np.ndarray) -> np.ndarray:
         """Normalize x to [0, 1].
 
         If x.dtype is a subtype of np.unsignedinteger, normalize it to
         [0, 1] using the max possible value of that dtype. Otherwise, assume
         it is in [0, 1] already and do nothing.
@@ -1295,38 +1688,49 @@
 
         if uri is None:
             return
 
         log.info(f'Loading model weights from: {uri}')
         self.load_weights(uri=uri, **args)
 
+    def save_weights(self, path: str):
+        """Save model weights to a local file."""
+        model = self.model
+        if isinstance(model, DDP):
+            model = model.module
+        torch.save(model.state_dict(), path)
+
     def load_weights(self, uri: str, **kwargs) -> None:
         """Load model weights from a file.
 
         Args:
             uri (str): URI.
             **kwargs: Extra args for :meth:`nn.Module.load_state_dict`.
         """
         weights_path = download_if_needed(uri)
-        self.model.load_state_dict(
+        model = self.model
+        if isinstance(model, DDP):
+            model = model.module
+        model.load_state_dict(
             torch.load(weights_path, map_location=self.device), **kwargs)
 
     def load_checkpoint(self):
         """Load last weights from previous run if available."""
         weights_path = self.last_model_weights_path
         if isfile(weights_path):
             log.info(f'Loading checkpoint from {weights_path}')
             args = {}
             if self.cfg.model is not None:
                 args['strict'] = self.cfg.model.load_strict
             self.load_weights(uri=weights_path, **args)
 
     def load_onnx_model(self, model_path: str) -> ONNXRuntimeAdapter:
         log.info(f'Loading ONNX model from {model_path}')
-        onnx_model = ONNXRuntimeAdapter.from_file(model_path)
+        path = download_if_needed(model_path)
+        onnx_model = ONNXRuntimeAdapter.from_file(path)
         return onnx_model
 
     def log_data_stats(self):
         """Log stats about each DataSet."""
         if self.train_ds is not None:
             log.info(f'train_ds: {len(self.train_ds)} items')
         if self.valid_ds is not None:
@@ -1348,25 +1752,23 @@
         if self.cfg.log_tensorboard:
             self.tb_log_dir = join(self.output_dir_local, 'tb-logs')
             make_dir(self.tb_log_dir)
             self.tb_writer = SummaryWriter(log_dir=self.tb_log_dir)
 
     def run_tensorboard(self):
         """Run TB server serving logged stats."""
-        if self.cfg.run_tensorboard:
+        if self.cfg.run_tensorboard:  # pragma: no cover
             log.info('Starting tensorboard process')
-            self.tb_process = Popen([
-                'tensorboard', '--bind_all',
-                '--logdir={}'.format(self.tb_log_dir)
-            ])
+            self.tb_process = Popen(
+                ['tensorboard', '--bind_all', f'--logdir={self.tb_log_dir}'])
             terminate_at_exit(self.tb_process)
 
     def stop_tensorboard(self):
         """Stop TB logging and server if it's running."""
-        if self.cfg.log_tensorboard:
+        if self.tb_writer is not None:
             self.tb_writer.close()
-            if self.cfg.run_tensorboard:
-                self.tb_process.terminate()
+        if self.tb_process is not None:  # pragma: no cover
+            self.tb_process.terminate()
 
     @property
     def onnx_mode(self) -> bool:
         return self._onnx_mode
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/learner_config.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from typing import (TYPE_CHECKING, Any, Callable, Dict, Iterable, List,
+                    Literal, Optional, Sequence, Tuple, Union)
+import os
 from os.path import join, isdir
 from enum import Enum
 import random
 import uuid
 import logging
 
-from typing import (TYPE_CHECKING, Any, Callable, Dict, Iterable, List,
-                    Optional, Sequence, Tuple, Union)
-from typing_extensions import Literal
 from pydantic import (PositiveFloat, PositiveInt as PosInt, constr, confloat,
                       conint)
 from pydantic.utils import sequence_like
 
 import albumentations as A
 import torch
 from torch import (nn, optim)
@@ -20,20 +20,22 @@
 from rastervision.pipeline.config import (Config, register_config, ConfigError,
                                           Field, validator, root_validator)
 from rastervision.pipeline.file_system import (list_paths, download_if_needed,
                                                unzip, file_exists,
                                                get_local_path, sync_from_dir)
 from rastervision.core.data import (ClassConfig, Scene, DatasetConfig as
                                     SceneDatasetConfig)
+from rastervision.core.rv_pipeline import (WindowSamplingConfig)
 from rastervision.pytorch_learner.utils import (
-    color_to_triple, validate_albumentation_transform, MinMaxNormalize,
+    validate_albumentation_transform, MinMaxNormalize,
     deserialize_albumentation_transform, get_hubconf_dir_from_cfg,
     torch_hub_load_local, torch_hub_load_github, torch_hub_load_uri)
 
 if TYPE_CHECKING:
+    from rastervision.core.data import SceneConfig
     from rastervision.pytorch_learner.learner import Learner
 
 log = logging.getLogger(__name__)
 
 default_augmentors = ['RandomRotate90', 'HorizontalFlip', 'VerticalFlip']
 augmentors = [
     'Blur', 'RandomRotate90', 'HorizontalFlip', 'VerticalFlip', 'GaussianBlur',
@@ -160,15 +162,18 @@
         has_uri = values.get('uri') is not None
         has_repo = values.get('github_repo') is not None
         if has_uri == has_repo:
             raise ConfigError(
                 'Must specify one (and only one) of github_repo and uri.')
         return values
 
-    def build(self, save_dir: str, hubconf_dir: Optional[str] = None) -> Any:
+    def build(self,
+              save_dir: str,
+              hubconf_dir: Optional[str] = None,
+              ddp_rank: Optional[int] = None) -> Any:
         """Load an external module via torch.hub.
 
         Note: Loading a PyTorch module is the typical use case, but there are
         no type restrictions on the object loaded through torch.hub.
 
         Args:
             save_dir (str, optional): The module def will be saved here.
@@ -184,30 +189,36 @@
             module = torch_hub_load_local(
                 hubconf_dir=hubconf_dir,
                 entrypoint=self.entrypoint,
                 *self.entrypoint_args,
                 **self.entrypoint_kwargs)
             return module
 
-        hubconf_dir = get_hubconf_dir_from_cfg(self, parent=save_dir)
+        dst_dir = get_hubconf_dir_from_cfg(self, parent=save_dir)
+        if ddp_rank is not None:
+            # avoid conflicts when downloading
+            os.environ['TORCH_HOME'] = f'~/.cache/torch/{ddp_rank}'
+            if ddp_rank != 0:
+                dst_dir = None
+
         if self.github_repo is not None:
             log.info(f'Fetching module definition from: {self.github_repo}')
             module = torch_hub_load_github(
                 repo=self.github_repo,
-                hubconf_dir=hubconf_dir,
                 entrypoint=self.entrypoint,
                 *self.entrypoint_args,
+                dst_dir=dst_dir,
                 **self.entrypoint_kwargs)
         else:
             log.info(f'Fetching module definition from: {self.uri}')
             module = torch_hub_load_uri(
                 uri=self.uri,
-                hubconf_dir=hubconf_dir,
                 entrypoint=self.entrypoint,
                 *self.entrypoint_args,
+                dst_dir=dst_dir,
                 **self.entrypoint_kwargs)
         return module
 
 
 def model_config_upgrader(cfg_dict, version):
     if version == 0:
         cfg_dict['backbone'] = Backbone.int_to_str(cfg_dict['backbone'])
@@ -224,15 +235,15 @@
         True,
         description=(
             'If True, use ImageNet weights. If False, use random initialization.'
         ))
     init_weights: Optional[str] = Field(
         None,
         description=('URI of PyTorch model weights used to initialize model. '
-                     'If set, this supercedes the pretrained option.'))
+                     'If set, this supersedes the pretrained option.'))
     load_strict: bool = Field(
         True,
         description=(
             'If True, the keys in the state dict referenced by init_weights '
             'must match exactly. Setting this to False can be useful if you '
             'just want to load the backbone of a model.'))
     external_def: Optional[ExternalModuleConfig] = Field(
@@ -249,14 +260,15 @@
         return self.backbone.name
 
     def build(self,
               num_classes: int,
               in_channels: int,
               save_dir: Optional[str] = None,
               hubconf_dir: Optional[str] = None,
+              ddp_rank: Optional[int] = None,
               **kwargs) -> nn.Module:
         """Build and return a model based on the config.
 
         Args:
             num_classes (int): Number of classes.
             in_channels (int, optional): Number of channels in the images that
                 will be fed into the model. Defaults to 3.
@@ -267,15 +279,15 @@
             **kwargs: Extra args for :meth:`.build_default_model`.
 
         Returns:
             A PyTorch nn.Module.
         """
         if self.external_def is not None:
             return self.build_external_model(
-                save_dir=save_dir, hubconf_dir=hubconf_dir)
+                save_dir=save_dir, hubconf_dir=hubconf_dir, ddp_rank=ddp_rank)
         return self.build_default_model(num_classes, in_channels, **kwargs)
 
     def build_default_model(self, num_classes: int, in_channels: int,
                             **kwargs) -> nn.Module:
         """Build and return the default model.
 
         Args:
@@ -286,53 +298,54 @@
         Returns:
             A PyTorch nn.Module.
         """
         raise NotImplementedError()
 
     def build_external_model(self,
                              save_dir: str,
-                             hubconf_dir: Optional[str] = None) -> nn.Module:
+                             hubconf_dir: Optional[str] = None,
+                             ddp_rank: Optional[int] = None) -> nn.Module:
         """Build and return an external model.
 
         Args:
             save_dir (str): The module def will be saved here.
             hubconf_dir (Optional[str], optional): Path to existing definition.
                 Defaults to None.
 
         Returns:
             A PyTorch nn.Module.
         """
-        return self.external_def.build(save_dir, hubconf_dir=hubconf_dir)
+        return self.external_def.build(
+            save_dir, hubconf_dir=hubconf_dir, ddp_rank=ddp_rank)
 
 
 def solver_config_upgrader(cfg_dict: dict, version: int) -> dict:
-    if version < 4:
+    if version == 3:
         # 'ignore_last_class' replaced by 'ignore_class_index' in version 4
         ignore_last_class = cfg_dict.get('ignore_last_class')
         if ignore_last_class is not None:
             if ignore_last_class is not False:
                 cfg_dict['ignore_class_index'] = -1
             del cfg_dict['ignore_last_class']
+    if version == 4:
+        # removed in version 5
+        cfg_dict.pop('test_batch_sz', None)
+        cfg_dict.pop('test_num_epochs', None)
+        cfg_dict.pop('overfit_num_steps', None)
     return cfg_dict
 
 
 @register_config('solver', upgrader=solver_config_upgrader)
 class SolverConfig(Config):
     """Config related to solver aka optimizer."""
     lr: PositiveFloat = Field(1e-4, description='Learning rate.')
     num_epochs: PosInt = Field(
         10,
         description=
         'Number of epochs (ie. sweeps through the whole training set).')
-    test_num_epochs: PosInt = Field(
-        2, description='Number of epochs to use in test mode.')
-    test_batch_sz: PosInt = Field(
-        4, description='Batch size to use in test mode.')
-    overfit_num_steps: PosInt = Field(
-        1, description='Number of optimizer steps to use in overfit mode.')
     sync_interval: PosInt = Field(
         1, description='The interval in epochs for each sync to the cloud.')
     batch_sz: PosInt = Field(32, description='Batch size.')
     one_cycle: bool = Field(
         True,
         description=
         ('If True, use triangular LR scheduler with a single cycle across all '
@@ -410,15 +423,15 @@
         """Build and return an Adam optimizer for the given model.
 
         Args:
             model (nn.Module): Model to be trained.
             **kwargs: Extra args for the optimizer constructor.
 
         Returns:
-            An Adam optimzer instance.
+            An Adam optimizer instance.
         """
         return optim.Adam(model.parameters(), lr=self.lr, **kwargs)
 
     def build_step_scheduler(self,
                              optimizer: optim.Optimizer,
                              train_ds_sz: int,
                              last_epoch: int = -1,
@@ -460,15 +473,15 @@
                 scheduler.step()
         return scheduler
 
     def build_epoch_scheduler(self,
                               optimizer: optim.Optimizer,
                               last_epoch: int = -1,
                               **kwargs) -> Optional[_LRScheduler]:
-        """Returns an LR scheduler tha changes the LR each epoch.
+        """Returns an LR scheduler that changes the LR each epoch.
 
         This is used to divide the learning rate by 10 at certain epochs.
 
         Args:
             optimizer (optim.Optimizer): Optimizer to build scheduler for.
             last_epoch (int): Last epoch. Defaults to -1.
             **kwargs: Extra args for the scheduler constructor.
@@ -577,52 +590,31 @@
     def validate_channel_display_groups(
             cls, v: Optional[Union[Dict[str, Sequence[NonNegInt]], Sequence[
                 Sequence[NonNegInt]]]]
     ) -> Optional[Dict[str, List[NonNegInt]]]:
         return validate_channel_display_groups(v)
 
 
-def ensure_class_colors(
-        class_names: List[str],
-        class_colors: Optional[List[Union[str, RGBTuple]]] = None):
-    """Ensure that class_colors is valid.
-
-    If class_names is empty, fill with random colors.
-
-    Args:
-        class_names: see DataConfig.class_names
-        class_colors: see DataConfig.class_colors
-    """
-    if class_colors is not None:
-        if len(class_names) != len(class_colors):
-            raise ConfigError(f'len(class_names) ({len(class_names)}) != '
-                              f'len(class_colors) ({len(class_colors)})\n'
-                              f'class_names: {class_names}\n'
-                              f'class_colors: {class_colors}')
-    elif len(class_names) > 0:
-        class_colors = [color_to_triple() for _ in class_names]
-    return class_colors
-
-
 def data_config_upgrader(cfg_dict: dict, version: int) -> dict:
-    if version < 2:
+    if version == 1:
         cfg_dict['type_hint'] = 'image_data'
-    elif version < 3:
+    elif version == 2:
         cfg_dict['img_channels'] = cfg_dict.get('img_channels')
+    elif version == 6:
+        class_names = cfg_dict.pop('class_names', [])
+        class_colors = cfg_dict.pop('class_colors', [])
+        cfg_dict['class_config'] = ClassConfig(
+            names=class_names, colors=class_colors)
     return cfg_dict
 
 
 @register_config('data', upgrader=data_config_upgrader)
 class DataConfig(Config):
     """Config related to dataset for training and testing."""
-    class_names: List[str] = Field([], description='Names of classes.')
-    class_colors: Optional[List[Union[str, RGBTuple]]] = Field(
-        None,
-        description=('Colors used to display classes. '
-                     'Can be color 3-tuples in list form.'))
+    class_config: ClassConfig | None = Field(None, description='Class config.')
     img_channels: Optional[PosInt] = Field(
         None, description='The number of channels of the training images.')
     img_sz: PosInt = Field(
         256,
         description=
         ('Length of a side of each image in pixels. This is the size to transform '
          'it to during training, not the size in the raw dataset.'))
@@ -659,30 +651,35 @@
     preview_batch_limit: Optional[int] = Field(
         None,
         description=
         ('Optional limit on the number of items in the preview plots produced '
          'during training.'))
 
     @property
+    def class_names(self):
+        if self.class_config is None:
+            return None
+        return self.class_config.names
+
+    @property
+    def class_colors(self):
+        if self.class_config is None:
+            return None
+        return self.class_config.colors
+
+    @property
     def num_classes(self):
-        return len(self.class_names)
+        return len(self.class_config)
 
     # validators
     _base_tf = validator(
         'base_transform', allow_reuse=True)(validate_albumentation_transform)
     _aug_tf = validator(
         'aug_transform', allow_reuse=True)(validate_albumentation_transform)
 
-    @root_validator(skip_on_failure=True)
-    def ensure_class_colors(cls, values: dict) -> dict:
-        class_names = values.get('class_names')
-        class_colors = values.get('class_colors')
-        values['class_colors'] = ensure_class_colors(class_names, class_colors)
-        return values
-
     @validator('augmentors', each_item=True)
     def validate_augmentors(cls, v: str) -> str:
         if v not in augmentors:
             raise ConfigError(f'Unsupported augmentor "{v}"')
         return v
 
     @root_validator(skip_on_failure=True)
@@ -691,25 +688,22 @@
         if plot_options is None:
             return None
         img_channels: Optional[PosInt] = values.get('img_channels')
         if img_channels is not None:
             plot_options.update(img_channels=img_channels)
         return values
 
-    def make_datasets(self) -> Tuple[Dataset, Dataset, Dataset]:
-        raise NotImplementedError()
-
     def get_custom_albumentations_transforms(self) -> List[dict]:
         """Returns all custom transforms found in this config.
 
         This should return all serialized albumentations transforms with
         a 'lambda_transforms_path' field contained in this
         config or in any of its members no matter how deeply neseted.
 
-        The pupose is to make it easier to adjust their paths all at once while
+        The purpose is to make it easier to adjust their paths all at once while
         saving to or loading from a bundle.
         """
         transforms_all = [
             self.base_transform, self.aug_transform,
             self.plot_options.transform
         ]
         transforms_with_lambdas = [
@@ -771,21 +765,25 @@
                 log.warning(
                     f'{k} is an unknown augmentor. Continuing without {k}. '
                     f'Known augmentors are: {list(augmentors_dict.keys())}')
         aug_transform = A.Compose(aug_transforms, bbox_params=bbox_params)
 
         return base_transform, aug_transform
 
-    def build(self,
-              tmp_dir: str,
-              overfit_mode: bool = False,
-              test_mode: bool = False) -> Tuple[Dataset, Dataset, Dataset]:
+    def build(self, tmp_dir: Optional[str] = None
+              ) -> Tuple[Dataset, Dataset, Dataset]:
         """Build and return train, val, and test datasets."""
         raise NotImplementedError()
 
+    def build_dataset(self,
+                      split: Literal['train', 'valid', 'test'],
+                      tmp_dir: Optional[str] = None) -> Dataset:
+        """Build and return dataset for a single split."""
+        raise NotImplementedError()
+
     def random_subset_dataset(self,
                               ds: Dataset,
                               size: Optional[int] = None,
                               fraction: Optional[Proportion] = None) -> Subset:
         if size is None and fraction is None:
             return ds
         if size is not None and fraction is not None:
@@ -805,15 +803,15 @@
     """Config related to dataset for training and testing."""
     data_format: Optional[str] = Field(
         None, description='Name of dataset format.')
     uri: Optional[Union[str, List[str]]] = Field(
         None,
         description='One of the following:\n'
         '(1) a URI of a directory containing "train", "valid", and '
-        '(optinally) "test" subdirectories;\n'
+        '(optionally) "test" subdirectories;\n'
         '(2) a URI of a zip file containing (1);\n'
         '(3) a list of (2);\n'
         '(4) a URI of a directory containing zip files containing (1).')
     group_uris: Optional[List[Union[str, List[str]]]] = Field(
         None,
         description=
         'This can be set instead of uri in order to specify groups of chips. '
@@ -858,22 +856,41 @@
                 raise ConfigError('len(group_train_sz) != len(group_uris).')
         if has_group_train_sz_rel and sequence_like(group_train_sz_rel):
             if len(group_train_sz_rel) != len(group_uris):
                 raise ConfigError(
                     'len(group_train_sz_rel) != len(group_uris).')
         return values
 
-    def make_datasets(self,
-                      train_dirs: Iterable[str],
-                      val_dirs: Iterable[str],
-                      test_dirs: Iterable[str],
-                      train_tf: Optional[A.BasicTransform] = None,
-                      val_tf: Optional[A.BasicTransform] = None,
-                      test_tf: Optional[A.BasicTransform] = None
-                      ) -> Tuple[Dataset, Dataset, Dataset]:
+    def _build_dataset(self,
+                       dirs: Iterable[str],
+                       tf: Optional[A.BasicTransform] = None
+                       ) -> Tuple[Dataset, Dataset, Dataset]:
+        """Make datasets for a single split.
+
+        Args:
+            dirs: Directories where the data is located.
+            tf: Transform for the dataset. Defaults to None.
+
+        Returns:
+            PyTorch-compatiable dataset.
+        """
+        per_dir_datasets = [self.dir_to_dataset(d, tf) for d in dirs]
+        if len(per_dir_datasets) == 0:
+            per_dir_datasets.append([])
+        combined_dataset = ConcatDataset(per_dir_datasets)
+        return combined_dataset
+
+    def _build_datasets(self,
+                        train_dirs: Iterable[str],
+                        val_dirs: Iterable[str],
+                        test_dirs: Iterable[str],
+                        train_tf: Optional[A.BasicTransform] = None,
+                        val_tf: Optional[A.BasicTransform] = None,
+                        test_tf: Optional[A.BasicTransform] = None
+                        ) -> Tuple[Dataset, Dataset, Dataset]:
         """Make training, validation, and test datasets.
 
         Args:
             train_dirs (str): Directories where training data is located.
             val_dirs (str): Directories where validation data is located.
             test_dirs (str): Directories where test data is located.
             train_tf (Optional[A.BasicTransform], optional): Transform for the
@@ -882,66 +899,66 @@
                 validation dataset. Defaults to None.
             test_tf (Optional[A.BasicTransform], optional): Transform for the
                 test dataset. Defaults to None.
 
         Returns:
             PyTorch-compatiable training, validation, and test datasets.
         """
-        train_ds_list = [self.dir_to_dataset(d, train_tf) for d in train_dirs]
-        val_ds_list = [self.dir_to_dataset(d, val_tf) for d in val_dirs]
-        test_ds_list = [self.dir_to_dataset(d, test_tf) for d in test_dirs]
-
-        for ds_list in [train_ds_list, val_ds_list, test_ds_list]:
-            if len(ds_list) == 0:
-                ds_list.append([])
-
-        train_ds = ConcatDataset(train_ds_list)
-        val_ds = ConcatDataset(val_ds_list)
-        test_ds = ConcatDataset(test_ds_list)
-
+        train_ds = self._build_dataset(train_dirs, train_tf)
+        val_ds = self._build_dataset(val_dirs, val_tf)
+        test_ds = self._build_dataset(test_dirs, test_tf)
         return train_ds, val_ds, test_ds
 
     def dir_to_dataset(self, data_dir: str,
                        transform: A.BasicTransform) -> Dataset:
         raise NotImplementedError()
 
-    def build(self,
-              tmp_dir: str,
-              overfit_mode: bool = False,
-              test_mode: bool = False) -> Tuple[Dataset, Dataset, Dataset]:
+    def build(self, tmp_dir: str) -> Tuple[Dataset, Dataset, Dataset]:
 
         if self.group_uris is None:
-            return self.get_datasets_from_uri(
-                self.uri,
-                tmp_dir=tmp_dir,
-                overfit_mode=overfit_mode,
-                test_mode=test_mode)
+            return self._get_datasets_from_uri(self.uri, tmp_dir=tmp_dir)
 
         if self.uri is not None:
             log.warning('Both DataConfig.uri and DataConfig.group_uris '
                         'specified. Only DataConfig.group_uris will be used.')
 
-        train_ds, valid_ds, test_ds = self.get_datasets_from_group_uris(
-            self.group_uris,
-            tmp_dir=tmp_dir,
-            overfit_mode=overfit_mode,
-            test_mode=test_mode)
+        train_ds, valid_ds, test_ds = self._get_datasets_from_group_uris(
+            self.group_uris, tmp_dir=tmp_dir)
 
         if self.train_sz is not None or self.train_sz_rel is not None:
             train_ds = self.random_subset_dataset(
                 train_ds, size=self.train_sz, fraction=self.train_sz_rel)
 
         return train_ds, valid_ds, test_ds
 
-    def get_datasets_from_uri(
-            self,
-            uri: Union[str, List[str]],
-            tmp_dir: str,
-            overfit_mode: bool = False,
-            test_mode: bool = False) -> Tuple[Dataset, Dataset, Dataset]:
+    def build_dataset(self,
+                      split: Literal['train', 'valid', 'test'],
+                      tmp_dir: Optional[str] = None) -> Dataset:
+
+        if self.group_uris is None:
+            ds = self._get_dataset_from_uri(
+                self.uri, split=split, tmp_dir=tmp_dir)
+            return ds
+
+        if self.uri is not None:
+            log.warning('Both DataConfig.uri and DataConfig.group_uris '
+                        'specified. Only DataConfig.group_uris will be used.')
+
+        ds = self._get_dataset_from_group_uris(
+            self.group_uris, split=split, tmp_dir=tmp_dir)
+
+        if split == 'train':
+            if self.train_sz is not None or self.train_sz_rel is not None:
+                ds = self.random_subset_dataset(
+                    ds, size=self.train_sz, fraction=self.train_sz_rel)
+
+        return ds
+
+    def _get_datasets_from_uri(self, uri: Union[str, List[str]], tmp_dir: str
+                               ) -> Tuple[Dataset, Dataset, Dataset]:
         """Get image train, validation, & test datasets from a single zip file.
 
         Args:
             uri (Union[str, List[str]]): Uri of a zip file containing the
                 images.
 
         Returns:
@@ -954,51 +971,72 @@
         test_dirs = [join(d, 'test') for d in data_dirs if isdir(d)]
 
         train_dirs = [d for d in train_dirs if isdir(d)]
         val_dirs = [d for d in val_dirs if isdir(d)]
         test_dirs = [d for d in test_dirs if isdir(d)]
 
         base_transform, aug_transform = self.get_data_transforms()
-        train_tf = (aug_transform if not overfit_mode else base_transform)
+        train_tf = aug_transform
         val_tf, test_tf = base_transform, base_transform
 
-        train_ds, val_ds, test_ds = self.make_datasets(
+        train_ds, val_ds, test_ds = self._build_datasets(
             train_dirs=train_dirs,
             val_dirs=val_dirs,
             test_dirs=test_dirs,
             train_tf=train_tf,
             val_tf=val_tf,
             test_tf=test_tf)
         return train_ds, val_ds, test_ds
 
-    def get_datasets_from_group_uris(
+    def _get_dataset_from_uri(self, uri: Union[str, List[str]],
+                              split: Literal['train', 'valid', 'test'],
+                              tmp_dir: str) -> Dataset:
+        """Get image dataset from a single zip file.
+
+        Args:
+            uri (Union[str, List[str]]): Uri of a zip file containing the
+                images.
+
+        Returns:
+            Training, validation, and test dataSets.
+        """
+        data_dirs = self.get_data_dirs(uri, unzip_dir=tmp_dir)
+
+        dirs = [join(d, split) for d in data_dirs if isdir(d)]
+        dirs = [d for d in dirs if isdir(d)]
+
+        base_transform, aug_transform = self.get_data_transforms()
+        if split == 'train':
+            tf = aug_transform
+        else:
+            tf = base_transform
+
+        ds = self._build_dataset(dirs, tf)
+        return ds
+
+    def _get_datasets_from_group_uris(
             self,
             uris: Union[str, List[str]],
             tmp_dir: str,
             group_train_sz: Optional[int] = None,
-            group_train_sz_rel: Optional[float] = None,
-            overfit_mode: bool = False,
-            test_mode: bool = False,
+            group_train_sz_rel: Optional[float] = None
     ) -> Tuple[Dataset, Dataset, Dataset]:
         train_ds_lst, valid_ds_lst, test_ds_lst = [], [], []
 
         group_sizes = None
         if group_train_sz is not None:
             group_sizes = group_train_sz
         elif group_train_sz_rel is not None:
             group_sizes = group_train_sz_rel
         if not sequence_like(group_sizes):
             group_sizes = [group_sizes] * len(uris)
 
         for uri, size in zip(uris, group_sizes):
-            train_ds, valid_ds, test_ds = self.get_datasets_from_uri(
-                uri,
-                tmp_dir=tmp_dir,
-                overfit_mode=overfit_mode,
-                test_mode=test_mode)
+            train_ds, valid_ds, test_ds = self._get_datasets_from_uri(
+                uri, tmp_dir=tmp_dir)
             if size is not None:
                 if isinstance(size, float):
                     train_ds = self.random_subset_dataset(
                         train_ds, fraction=size)
                 else:
                     train_ds = self.random_subset_dataset(train_ds, size=size)
 
@@ -1007,31 +1045,60 @@
             test_ds_lst.append(test_ds)
 
         train_ds, valid_ds, test_ds = (ConcatDataset(train_ds_lst),
                                        ConcatDataset(valid_ds_lst),
                                        ConcatDataset(test_ds_lst))
         return train_ds, valid_ds, test_ds
 
+    def _get_dataset_from_group_uris(
+            self,
+            split: Literal['train', 'valid', 'test'],
+            uris: Union[str, List[str]],
+            tmp_dir: str,
+            group_sz: Optional[int] = None,
+            group_sz_rel: Optional[float] = None) -> Dataset:
+
+        group_sizes = None
+        if group_sz is not None:
+            group_sizes = group_sz
+        elif group_sz_rel is not None:
+            group_sizes = group_sz_rel
+        if not sequence_like(group_sizes):
+            group_sizes = [group_sizes] * len(uris)
+
+        per_uri_dataset = []
+        for uri, size in zip(uris, group_sizes):
+            ds = self._get_dataset_from_uri(uri, split=split, tmp_dir=tmp_dir)
+            if size is not None:
+                if isinstance(size, float):
+                    ds = self.random_subset_dataset(ds, fraction=size)
+                else:
+                    ds = self.random_subset_dataset(ds, size=size)
+            per_uri_dataset.append(ds)
+
+        combined_dataset = ConcatDataset(per_uri_dataset)
+        return combined_dataset
+
     def get_data_dirs(self, uri: Union[str, List[str]],
                       unzip_dir: str) -> List[str]:
         """Extract data dirs from uri.
 
         Data dirs are directories containing  "train", "valid", and
-        (optinally) "test" subdirectories.
+        (optionally) "test" subdirectories.
 
         Args:
             uri (Union[str, List[str]]): A URI or a list of URIs of one of the
                 following:
 
                 (1) a URI of a directory containing "train", "valid", and
-                    (optinally) "test" subdirectories
+                    (optionally) "test" subdirectories
                 (2) a URI of a zip file containing (1)
                 (3) a list of (2)
                 (4) a URI of a directory containing zip files containing (1)
-            unzip_dir (str): Directory where zip files will be extrated to, if
+            unzip_dir (str): Directory where zip files will be extracted to, if
                 needed.
 
         Returns:
             List[str]: Paths to directories that each contain contents of one
             zip file.
         """
 
@@ -1072,15 +1139,15 @@
         return data_dirs
 
     def unzip_data(self, zip_uris: List[str], unzip_dir: str) -> List[str]:
         """Unzip dataset zip files.
 
         Args:
             zip_uris (List[str]): A list of URIs of zip files:
-            unzip_dir (str): Directory where zip files will be extrated to.
+            unzip_dir (str): Directory where zip files will be extracted to.
 
         Returns:
             List[str]: Paths to directories that each contain contents of one
             zip file.
         """
         data_dirs = []
 
@@ -1090,191 +1157,126 @@
             data_dir = join(unzip_dir, str(i))
             data_dirs.append(data_dir)
             unzip(zip_path, data_dir)
 
         return data_dirs
 
 
-class GeoDataWindowMethod(Enum):
-    sliding = 'sliding'
-    random = 'random'
-
-
-@register_config('geo_data_window')
-class GeoDataWindowConfig(Config):
-    """Configure a :class:`.GeoDataset`.
-
-    See :mod:`rastervision.pytorch_learner.dataset.dataset`.
-    """
-
-    method: GeoDataWindowMethod = Field(
-        GeoDataWindowMethod.sliding, description='')
-    size: Union[PosInt, Tuple[PosInt, PosInt]] = Field(
-        ...,
-        description='If method = sliding, this is the size of sliding window. '
-        'If method = random, this is the size that all the windows are '
-        'resized to before they are returned. If method = random and neither '
-        'size_lims nor h_lims and w_lims have been specified, then size_lims '
-        'is set to (size, size + 1).')
-    stride: Optional[Union[PosInt, Tuple[PosInt, PosInt]]] = Field(
-        None,
-        description='Stride of sliding window. Only used if method = sliding.')
-    padding: Optional[Union[NonNegInt, Tuple[NonNegInt, NonNegInt]]] = Field(
-        None,
-        description='How many pixels are windows allowed to overflow '
-        'the edges of the raster source.')
-    pad_direction: Literal['both', 'start', 'end'] = Field(
-        'end',
-        description='If "end", only pad ymax and xmax (bottom and right). '
-        'If "start", only pad ymin and xmin (top and left). If "both", '
-        'pad all sides. Has no effect if paddiong is zero. Defaults to "end".')
-    size_lims: Optional[Tuple[PosInt, PosInt]] = Field(
-        None,
-        description='[min, max) interval from which window sizes will be '
-        'uniformly randomly sampled. The upper limit is exclusive. To fix the '
-        'size to a constant value, use size_lims = (sz, sz + 1). '
-        'Only used if method = random. Specify either size_lims or '
-        'h_lims and w_lims, but not both. If neither size_lims nor h_lims '
-        'and w_lims have been specified, then this will be set to '
-        '(size, size + 1).')
-    h_lims: Optional[Tuple[PosInt, PosInt]] = Field(
-        None,
-        description='[min, max] interval from which window heights will be '
-        'uniformly randomly sampled. Only used if method = random.')
-    w_lims: Optional[Tuple[PosInt, PosInt]] = Field(
-        None,
-        description='[min, max] interval from which window widths will be '
-        'uniformly randomly sampled. Only used if method = random.')
-    max_windows: NonNegInt = Field(
-        10_000,
-        description='Max allowed reads from a GeoDataset. Only used if '
-        'method = random.')
-    max_sample_attempts: PosInt = Field(
-        100,
-        description='Max attempts when trying to find a window within the AOI '
-        'of a scene. Only used if method = random and the scene has '
-        'aoi_polygons specified.')
-    efficient_aoi_sampling: bool = Field(
-        True,
-        description='If the scene has AOIs, sampling windows at random '
-        'anywhere in the extent and then checking if they fall within any of '
-        'the AOIs can be very inefficient. This flag enables the use of an '
-        'alternate algorithm that only samples window locations inside the '
-        'AOIs. Only used if method = random and the scene has aoi_polygons '
-        'specified. Defaults to True',
-    )
-
-    @root_validator(skip_on_failure=True)
-    def validate_options(cls, values: dict) -> dict:
-        method = values.get('method')
-        size = values.get('size')
-        if method == GeoDataWindowMethod.sliding:
-            has_stride = values.get('stride') is not None
-
-            if not has_stride:
-                values['stride'] = size
-        elif method == GeoDataWindowMethod.random:
-            size_lims = values.get('size_lims')
-            h_lims = values.get('h_lims')
-            w_lims = values.get('w_lims')
-
-            has_size_lims = size_lims is not None
-            has_h_lims = h_lims is not None
-            has_w_lims = w_lims is not None
-
-            if not (has_size_lims or has_h_lims or has_w_lims):
-                size_lims = (size, size + 1)
-                has_size_lims = True
-                values['size_lims'] = size_lims
-            if has_size_lims == (has_w_lims or has_h_lims):
-                raise ConfigError('Specify either size_lims or h and w lims.')
-            if has_h_lims != has_w_lims:
-                raise ConfigError('h_lims and w_lims must both be specified')
-        return values
+def geo_data_config_upgrader(cfg_dict: dict, version: int) -> dict:
+    if version == 5:
+        cfg_dict['sampling'] = cfg_dict.pop('window_opts', {})
+    return cfg_dict
 
 
-@register_config('geo_data')
+@register_config('geo_data', upgrader=geo_data_config_upgrader)
 class GeoDataConfig(DataConfig):
     """Configure :class:`GeoDatasets <.GeoDataset>`.
 
     See :mod:`rastervision.pytorch_learner.dataset.dataset`.
     """
 
     scene_dataset: Optional['SceneDatasetConfig'] = Field(None, description='')
-    window_opts: Union[GeoDataWindowConfig, Dict[str,
-                                                 GeoDataWindowConfig]] = Field(
-                                                     {}, description='')
+    sampling: Union[WindowSamplingConfig, Dict[
+        str, WindowSamplingConfig]] = Field(
+            {}, description='Window sampling config.')
 
     def __repr_args__(self):
         ds = self.scene_dataset
         ds_repr = (f'<{len(ds.train_scenes)} train_scenes, '
                    f'{len(ds.validation_scenes)} validation_scenes, '
                    f'{len(ds.test_scenes)} test_scenes>')
-        out = [('scene_dataset', ds_repr), ('window_opts',
-                                            str(self.window_opts))]
+        out = [('scene_dataset', ds_repr), ('sampling', str(self.sampling))]
         return out
 
-    @validator('window_opts')
-    def validate_window_opts(
-            cls, v: Union[GeoDataWindowConfig, Dict[str, GeoDataWindowConfig]],
+    @validator('sampling')
+    def validate_sampling(
+            cls,
+            v: Union[WindowSamplingConfig, Dict[str, WindowSamplingConfig]],
             values: dict
-    ) -> Union[GeoDataWindowConfig, Dict[str, GeoDataWindowConfig]]:
+    ) -> Union[WindowSamplingConfig, Dict[str, WindowSamplingConfig]]:
         if isinstance(v, dict):
             if len(v) == 0:
                 return v
             scene_dataset: Optional['SceneDatasetConfig'] = values.get(
                 'scene_dataset')
             if scene_dataset is None:
-                raise ConfigError('window_opts is a non-empty dict but '
+                raise ConfigError('sampling is a non-empty dict but '
                                   'scene_dataset is None.')
             for s in scene_dataset.all_scenes:
                 if s.id not in v:
                     raise ConfigError(
                         f'Window config not found for scene {s.id}')
         return v
 
     @root_validator(skip_on_failure=True)
-    def get_class_info_from_class_config_if_needed(cls, values: dict) -> dict:
-        no_classes = len(values['class_names']) == 0
+    def get_class_config_from_dataset_if_needed(cls, values: dict) -> dict:
+        has_class_config = values.get('class_config') is not None
+        if has_class_config:
+            return values
         has_scene_dataset = values.get('scene_dataset') is not None
-        if no_classes and has_scene_dataset:
-            class_config: ClassConfig = values['scene_dataset'].class_config
-            class_config.update()
-            values['class_names'] = class_config.names
-            values['class_colors'] = class_config.colors
+        if has_scene_dataset:
+            values['class_config'] = values['scene_dataset'].class_config
         return values
 
-    def build_scenes(self, tmp_dir: str
-                     ) -> Tuple[List[Scene], List[Scene], List[Scene]]:
+    def build_scenes(self,
+                     scene_configs: Iterable['SceneConfig'],
+                     tmp_dir: Optional[str] = None) -> List[Scene]:
         """Build training, validation, and test scenes."""
+        class_config = self.scene_dataset.class_config
+        scenes = [
+            s.build(class_config, tmp_dir, use_transformers=True)
+            for s in scene_configs
+        ]
+        return scenes
+
+    def _build_dataset(self,
+                       split: Literal['train', 'valid', 'test'],
+                       tf: Optional[A.BasicTransform] = None,
+                       tmp_dir: Optional[str] = None,
+                       **kwargs) -> Tuple[Dataset, Dataset, Dataset]:
+        """Make training, validation, and test datasets.
+
+        Args:
+            split: Name of data split. One of: 'train', 'valid', 'test'.
+            tf: Transform for the
+                dataset. Defaults to None.
+            tmp_dir: Temporary directory to be used for building scenes.
+            **kwargs: Kwargs to pass to :meth:`.scene_to_dataset`.
+
+        Returns:
+            Dataset: PyTorch-compatiable dataset.
+        """
         if self.scene_dataset is None:
             raise ValueError('Cannot build scenes if scene_dataset is None.')
 
-        class_cfg = self.scene_dataset.class_config
-        train_scenes = [
-            s.build(class_cfg, tmp_dir, use_transformers=True)
-            for s in self.scene_dataset.train_scenes
-        ]
-        val_scenes = [
-            s.build(class_cfg, tmp_dir, use_transformers=True)
-            for s in self.scene_dataset.validation_scenes
-        ]
-        test_scenes = [
-            s.build(class_cfg, tmp_dir, use_transformers=True)
-            for s in self.scene_dataset.test_scenes
+        if split == 'train':
+            scene_configs = self.scene_dataset.train_scenes
+        elif split == 'valid':
+            scene_configs = self.scene_dataset.validation_scenes
+        elif split == 'test':
+            scene_configs = self.scene_dataset.test_scenes
+
+        scenes = self.build_scenes(scene_configs, tmp_dir)
+        per_scene_datasets = [
+            self.scene_to_dataset(s, tf, **kwargs) for s in scenes
         ]
 
-        return train_scenes, val_scenes, test_scenes
+        if len(per_scene_datasets) == 0:
+            per_scene_datasets.append([])
 
-    def make_datasets(self,
-                      tmp_dir: str,
-                      train_tf: Optional[A.BasicTransform] = None,
-                      val_tf: Optional[A.BasicTransform] = None,
-                      test_tf: Optional[A.BasicTransform] = None,
-                      **kwargs) -> Tuple[Dataset, Dataset, Dataset]:
+        combined_dataset = ConcatDataset(per_scene_datasets)
+
+        return combined_dataset
+
+    def _build_datasets(self,
+                        tmp_dir: Optional[str] = None,
+                        train_tf: Optional[A.BasicTransform] = None,
+                        val_tf: Optional[A.BasicTransform] = None,
+                        test_tf: Optional[A.BasicTransform] = None,
+                        **kwargs) -> Tuple[Dataset, Dataset, Dataset]:
         """Make training, validation, and test datasets.
 
         Args:
             tmp_dir (str): Temporary directory to be used for building scenes.
             train_tf (Optional[A.BasicTransform], optional): Transform for the
                 training dataset. Defaults to None.
             val_tf (Optional[A.BasicTransform], optional): Transform for the
@@ -1283,91 +1285,89 @@
                 test dataset. Defaults to None.
             **kwargs: Kwargs to pass to :meth:`.scene_to_dataset`.
 
         Returns:
             Tuple[Dataset, Dataset, Dataset]: PyTorch-compatiable training,
             validation, and test datasets.
         """
-        train_scenes, val_scenes, test_scenes = self.build_scenes(tmp_dir)
-
-        train_ds_list = [
-            self.scene_to_dataset(s, train_tf, **kwargs) for s in train_scenes
-        ]
-        val_ds_list = [
-            self.scene_to_dataset(s, val_tf, **kwargs) for s in val_scenes
-        ]
-        test_ds_list = [
-            self.scene_to_dataset(s, test_tf, **kwargs) for s in test_scenes
-        ]
-
-        for ds_list in [train_ds_list, val_ds_list, test_ds_list]:
-            if len(ds_list) == 0:
-                ds_list.append([])
-
-        train_ds = ConcatDataset(train_ds_list)
-        val_ds = ConcatDataset(val_ds_list)
-        test_ds = ConcatDataset(test_ds_list)
-
+        train_ds = self._build_dataset('train', train_tf, tmp_dir, **kwargs)
+        val_ds = self._build_dataset('valid', val_tf, tmp_dir, **kwargs)
+        test_ds = self._build_dataset('test', test_tf, tmp_dir, **kwargs)
         return train_ds, val_ds, test_ds
 
     def scene_to_dataset(self,
                          scene: Scene,
-                         transform: Optional[A.BasicTransform] = None
-                         ) -> Dataset:
+                         transform: Optional[A.BasicTransform] = None,
+                         for_chipping: bool = False) -> Dataset:
         """Make a dataset from a single scene.
         """
         raise NotImplementedError()
 
-    def build(self,
-              tmp_dir: str,
-              overfit_mode: bool = False,
-              test_mode: bool = False) -> Tuple[Dataset, Dataset, Dataset]:
+    def build_dataset(self,
+                      split: Literal['train', 'valid', 'test'],
+                      tmp_dir: Optional[str] = None) -> Dataset:
+
         base_transform, aug_transform = self.get_data_transforms()
-        train_tf = (aug_transform if not overfit_mode else base_transform)
-        val_tf, test_tf = base_transform, base_transform
+        if split == 'train':
+            tf = aug_transform
+        else:
+            tf = base_transform
+
+        ds = self._build_dataset(split, tf, tmp_dir)
+
+        if split == 'train':
+            if self.train_sz is not None or self.train_sz_rel is not None:
+                ds = self.random_subset_dataset(
+                    ds, size=self.train_sz, fraction=self.train_sz_rel)
+
+        return ds
+
+    def build(self, tmp_dir: Optional[str] = None,
+              for_chipping: bool = False) -> Tuple[Dataset, Dataset, Dataset]:
+        base_transform, aug_transform = self.get_data_transforms()
+        if for_chipping:
+            train_tf, val_tf, test_tf = None, None, None
+        else:
+            train_tf = aug_transform
+            val_tf, test_tf = base_transform, base_transform
 
-        train_ds, val_ds, test_ds = self.make_datasets(
-            tmp_dir=tmp_dir, train_tf=train_tf, val_tf=val_tf, test_tf=test_tf)
+        train_ds, val_ds, test_ds = self._build_datasets(
+            tmp_dir=tmp_dir,
+            train_tf=train_tf,
+            val_tf=val_tf,
+            test_tf=test_tf,
+            for_chipping=for_chipping)
 
         if self.train_sz is not None or self.train_sz_rel is not None:
             train_ds = self.random_subset_dataset(
                 train_ds, size=self.train_sz, fraction=self.train_sz_rel)
 
         return train_ds, val_ds, test_ds
 
 
-@register_config('learner')
+def learner_config_upgrader(cfg_dict: dict, version: int) -> dict:
+    if version == 4:
+        # removed in version 5
+        cfg_dict.pop('overfit_mode', None)
+        cfg_dict.pop('test_mode', None)
+        cfg_dict.pop('predict_mode', None)
+    return cfg_dict
+
+
+@register_config('learner', upgrader=learner_config_upgrader)
 class LearnerConfig(Config):
     """Config for Learner."""
-    model: Optional[ModelConfig]
-    solver: SolverConfig
+    model: Optional[ModelConfig] = None
+    solver: Optional[SolverConfig] = None
     data: DataConfig
 
-    predict_mode: bool = Field(
-        False,
-        description='If True, skips training, loads model, and does final eval.'
-    )
-    test_mode: bool = Field(
-        False,
-        description=
-        ('If True, uses test_num_epochs, test_batch_sz, truncated datasets with '
-         'only a single batch, image_sz that is cut in half, and num_workers = 0. '
-         'This is useful for testing that code runs correctly on CPU without '
-         'multithreading before running full job on GPU.'))
-    overfit_mode: bool = Field(
-        False,
-        description=
-        ('If True, uses half image size, and instead of doing epoch-based training, '
-         'optimizes the model using a single batch repeatedly for '
-         'overfit_num_steps number of steps.'))
     eval_train: bool = Field(
         False,
-        description=
-        ('If True, runs final evaluation on training set (in addition to test set). '
-         'Useful for debugging.'))
+        description='If True, runs final evaluation on training set '
+        '(in addition to validation set). Useful for debugging.')
     save_model_bundle: bool = Field(
         True,
         description=
         ('If True, saves a model bundle at the end of training which '
          'is zip file with model and this LearnerConfig which can be used to make '
          'predictions on new images at a later time.'))
     log_tensorboard: bool = Field(
@@ -1390,45 +1390,28 @@
         if v and not values.get('log_tensorboard'):
             raise ConfigError(
                 'Cannot run tensorboard if log_tensorboard is False')
         return v
 
     @root_validator(skip_on_failure=True)
     def validate_class_loss_weights(cls, values: dict) -> dict:
-        solver: SolverConfig = values.get('solver')
+        solver: Optional[SolverConfig] = values.get('solver')
+        if solver is None:
+            return values
         class_loss_weights = solver.class_loss_weights
         if class_loss_weights is not None:
             data: DataConfig = values.get('data')
             num_weights = len(class_loss_weights)
             num_classes = data.num_classes
             if num_weights != num_classes:
                 raise ConfigError(
                     f'class_loss_weights ({num_weights}) must be same length as '
                     f'the number of classes ({num_classes})')
         return values
 
-    @root_validator(skip_on_failure=True)
-    def update_for_mode(cls, values: dict) -> dict:
-        overfit_mode = values.get('overfit_mode')
-        test_mode = values.get('test_mode')
-        solver: SolverConfig = values.get('solver')
-        data: DataConfig = values.get('data')
-
-        if overfit_mode:
-            data.img_sz = data.img_sz // 2
-            if test_mode:
-                solver.overfit_num_steps = solver.test_overfit_num_steps
-
-        if test_mode:
-            solver.num_epochs = solver.test_num_epochs
-            solver.batch_sz = solver.test_batch_sz
-            data.num_workers = 0
-
-        return values
-
     def build(self,
               tmp_dir: Optional[str] = None,
               model_weights_path: Optional[str] = None,
               model_def_path: Optional[str] = None,
               loss_def_path: Optional[str] = None,
               training: bool = True) -> 'Learner':
         """Returns a Learner instantiated using this Config.
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/object_detection_learner.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
                     Union)
 import warnings
 
 import logging
 
 import numpy as np
 import torch
+import torch.distributed as dist
 
 from rastervision.pytorch_learner.learner import Learner
 from rastervision.pytorch_learner.object_detection_utils import (
     BoxList, TorchVisionODAdapter, compute_coco_eval, collate_fn,
     ONNXRuntimeAdapterForFasterRCNN)
 from rastervision.pytorch_learner.dataset.visualizer import (
     ObjectDetectionVisualizer)
@@ -30,15 +31,16 @@
         """Override to pass img_sz."""
         cfg = self.cfg
         model = cfg.model.build(
             num_classes=cfg.data.num_classes,
             in_channels=cfg.data.img_channels,
             save_dir=self.modules_dir,
             hubconf_dir=model_def_path,
-            img_sz=cfg.data.img_sz)
+            img_sz=cfg.data.img_sz,
+            ddp_rank=self.ddp_local_rank)
         return model
 
     def setup_model(self,
                     model_weights_path: Optional[str] = None,
                     model_def_path: Optional[str] = None) -> None:
         """Override to apply the TorchVisionODAdapter wrapper."""
         if self.model is not None:
@@ -85,14 +87,31 @@
     def validate_end(self, outputs):
         outs = []
         ys = []
         for o in outputs:
             outs.extend(o['outs'])
             ys.extend(o['ys'])
         num_class_ids = len(self.cfg.data.class_names)
+
+        if self.is_ddp_process:
+            is_master = self.is_ddp_master
+            all_outs = [None] * self.ddp_world_size
+            all_ys = [None] * self.ddp_world_size
+            dist.gather_object(
+                outs,
+                object_gather_list=(all_outs if is_master else None),
+                dst=0)
+            dist.gather_object(
+                ys, object_gather_list=(all_ys if is_master else None), dst=0)
+            if not is_master:
+                return {}
+            outs = sum(all_outs, [])
+            ys = sum(all_ys, [])
+
+        log.info(f'{self.ddp_rank} at coco eval')
         coco_eval = compute_coco_eval(outs, ys, num_class_ids)
 
         metrics = {'mAP': 0.0, 'mAP50': 0.0}
         if coco_eval is not None:
             coco_metrics = coco_eval.stats
             metrics = {'mAP': coco_metrics[0], 'mAP50': coco_metrics[1]}
         return metrics
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/object_detection_learner_config.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 import albumentations as A
 
 from torchvision.models.detection.backbone_utils import resnet_fpn_backbone
 from torchvision.models.detection.faster_rcnn import FasterRCNN
 
 from rastervision.core.data import Scene
+from rastervision.core.rv_pipeline import WindowSamplingMethod
 from rastervision.pipeline.config import (Config, register_config, Field,
                                           validator, ConfigError)
 from rastervision.pytorch_learner.learner_config import (
-    LearnerConfig, ModelConfig, Backbone, ImageDataConfig, GeoDataConfig,
-    GeoDataWindowMethod, GeoDataWindowConfig)
+    LearnerConfig, ModelConfig, Backbone, ImageDataConfig, GeoDataConfig)
 from rastervision.pytorch_learner.dataset import (
     ObjectDetectionImageDataset, ObjectDetectionSlidingWindowGeoDataset,
     ObjectDetectionRandomWindowGeoDataset)
 from rastervision.pytorch_learner.utils import adjust_conv_channels
 
 if TYPE_CHECKING:
     from rastervision.pytorch_learner.learner_config import SolverConfig
@@ -56,73 +56,51 @@
         img_dir = join(data_dir, 'img')
         annotation_uri = join(data_dir, 'labels.json')
         ds = ObjectDetectionImageDataset(
             img_dir, annotation_uri, transform=transform)
         return ds
 
 
-@register_config('object_detection_geo_data_window')
-class ObjectDetectionGeoDataWindowConfig(GeoDataWindowConfig):
-    """Configure an object detection :class:`.GeoDataset`.
-
-    See :mod:`rastervision.pytorch_learner.dataset.object_detection_dataset`.
-    """
-    ioa_thresh: float = Field(
-        0.8,
-        description='When a box is partially outside of a training chip, it '
-        'is not clear if (a clipped version) of the box should be included in '
-        'the chip. If the IOA (intersection over area) of the box with the '
-        'chip is greater than ioa_thresh, it is included in the chip. '
-        'Defaults to 0.8.')
-    clip: bool = Field(
-        False,
-        description='Clip bounding boxes to window limits when retrieving '
-        'labels for a window.')
-    neg_ratio: Optional[float] = Field(
-        None,
-        description='The ratio of negative chips (those containing no '
-        'bounding boxes) to positive chips. This can be useful if the '
-        'statistics of the background is different in positive chips. For '
-        'example, in car detection, the positive chips will always contain '
-        'roads, but no examples of rooftops since cars tend to not be near '
-        'rooftops. Defaults to None.')
-    neg_ioa_thresh: float = Field(
-        0.2,
-        description='A window will be considered negative if its max IoA with '
-        'any bounding box is less than this threshold. Defaults to 0.2.')
-
-
 @register_config('object_detection_geo_data')
 class ObjectDetectionGeoDataConfig(ObjectDetectionDataConfig, GeoDataConfig):
     """Configure object detection :class:`GeoDatasets <.GeoDataset>`.
 
     See :mod:`rastervision.pytorch_learner.dataset.object_detection_dataset`.
     """
 
     def scene_to_dataset(
             self,
             scene: Scene,
             transform: Optional[A.BasicTransform] = None,
-            bbox_params: Optional[A.BboxParams] = DEFAULT_BBOX_PARAMS
+            bbox_params: Optional[A.BboxParams] = DEFAULT_BBOX_PARAMS,
+            for_chipping: bool = False
     ) -> Union[ObjectDetectionSlidingWindowGeoDataset,
                ObjectDetectionRandomWindowGeoDataset]:
-        if isinstance(self.window_opts, dict):
-            opts = self.window_opts[scene.id]
+        if isinstance(self.sampling, dict):
+            opts = self.sampling[scene.id]
         else:
-            opts = self.window_opts
+            opts = self.sampling
+
+        extra_args = {}
+        if for_chipping:
+            extra_args = dict(
+                normalize=False, to_pytorch=False, return_window=True)
 
-        if opts.method == GeoDataWindowMethod.sliding:
+        if opts.method == WindowSamplingMethod.sliding:
             ds = ObjectDetectionSlidingWindowGeoDataset(
                 scene,
                 size=opts.size,
                 stride=opts.stride,
                 padding=opts.padding,
                 pad_direction=opts.pad_direction,
-                transform=transform)
-        elif opts.method == GeoDataWindowMethod.random:
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
+        elif opts.method == WindowSamplingMethod.random:
             ds = ObjectDetectionRandomWindowGeoDataset(
                 scene,
                 size_lims=opts.size_lims,
                 h_lims=opts.h_lims,
                 w_lims=opts.w_lims,
                 out_size=opts.size,
                 padding=opts.padding,
@@ -130,15 +108,18 @@
                 max_sample_attempts=opts.max_sample_attempts,
                 bbox_params=bbox_params,
                 ioa_thresh=opts.ioa_thresh,
                 clip=opts.clip,
                 neg_ratio=opts.neg_ratio,
                 neg_ioa_thresh=opts.neg_ioa_thresh,
                 efficient_aoi_sampling=opts.efficient_aoi_sampling,
-                transform=transform)
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
         else:
             raise NotImplementedError()
         return ds
 
 
 @register_config('object_detection_model')
 class ObjectDetectionModelConfig(ModelConfig):
@@ -218,15 +199,14 @@
         return model
 
 
 @register_config('object_detection_learner')
 class ObjectDetectionLearnerConfig(LearnerConfig):
     """Configure an :class:`.ObjectDetectionLearner`."""
 
-    data: Union[ObjectDetectionImageDataConfig, ObjectDetectionGeoDataConfig]
     model: Optional[ObjectDetectionModelConfig]
 
     def build(self,
               tmp_dir=None,
               model_weights_path=None,
               model_def_path=None,
               loss_def_path=None,
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/object_detection_utils.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/regression_learner.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,20 +35,18 @@
         model = cfg.model.build(
             num_classes=cfg.data.num_classes,
             in_channels=cfg.data.img_channels,
             save_dir=self.modules_dir,
             hubconf_dir=model_def_path,
             class_names=class_names,
             pos_class_names=pos_class_names,
-            prob_class_names=prob_class_names)
+            prob_class_names=prob_class_names,
+            ddp_rank=self.ddp_local_rank)
         return model
 
-    def on_overfit_start(self):
-        self.on_train_start()
-
     def on_train_start(self):
         ys = []
         for _, y in self.train_dl:
             ys.append(y)
         y = torch.cat(ys, dim=0)
         self.target_medians = y.median(dim=0).values.to(self.device)
 
@@ -71,16 +69,16 @@
             metrics[f'{label}_scaled_abs_error'] = scaled_abs_error[i]
 
         return metrics
 
     def prob_to_pred(self, x):
         return x
 
-    def eval_model(self, split):
-        super().eval_model(split)
+    def _validate(self, split):
+        super()._validate(split)
 
         y, out = self.predict_dataloader(
             self.get_dataloader(split), return_format='yz', raw_out=False)
 
         max_scatter_points = self.cfg.data.plot_options.max_scatter_points
         if y.shape[0] > max_scatter_points:
             scatter_inds = torch.randperm(
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/regression_learner_config.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import logging
 
 import albumentations as A
 from torch import nn
 from torchvision import models
 
 from rastervision.core.data import Scene
+from rastervision.core.rv_pipeline import WindowSamplingMethod
 from rastervision.pipeline.config import (Config, register_config, Field,
                                           ConfigError)
 from rastervision.pytorch_learner.learner_config import (
-    LearnerConfig, ModelConfig, PlotOptions, ImageDataConfig, GeoDataConfig,
-    GeoDataWindowMethod)
+    LearnerConfig, ModelConfig, PlotOptions, ImageDataConfig, GeoDataConfig)
 from rastervision.pytorch_learner.dataset import (
     RegressionImageDataset, RegressionSlidingWindowGeoDataset,
     RegressionRandomWindowGeoDataset)
 from rastervision.pytorch_learner.utils import adjust_conv_channels
 
 if TYPE_CHECKING:
     import torch
@@ -72,42 +72,54 @@
     """
 
     plot_options: Optional[RegressionPlotOptions] = Field(
         RegressionPlotOptions(), description='Options to control plotting.')
 
     def scene_to_dataset(self,
                          scene: Scene,
-                         transform: Optional[A.BasicTransform] = None
+                         transform: Optional[A.BasicTransform] = None,
+                         for_chipping: bool = False
                          ) -> Union[RegressionSlidingWindowGeoDataset,
                                     RegressionRandomWindowGeoDataset]:
-        if isinstance(self.window_opts, dict):
-            opts = self.window_opts[scene.id]
+        if isinstance(self.sampling, dict):
+            opts = self.sampling[scene.id]
         else:
-            opts = self.window_opts
+            opts = self.sampling
 
-        if opts.method == GeoDataWindowMethod.sliding:
+        extra_args = {}
+        if for_chipping:
+            extra_args = dict(
+                normalize=False, to_pytorch=False, return_window=True)
+
+        if opts.method == WindowSamplingMethod.sliding:
             ds = RegressionSlidingWindowGeoDataset(
                 scene,
                 size=opts.size,
                 stride=opts.stride,
                 padding=opts.padding,
                 pad_direction=opts.pad_direction,
-                transform=transform)
-        elif opts.method == GeoDataWindowMethod.random:
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
+        elif opts.method == WindowSamplingMethod.random:
             ds = RegressionRandomWindowGeoDataset(
                 scene,
                 size_lims=opts.size_lims,
                 h_lims=opts.h_lims,
                 w_lims=opts.w_lims,
                 out_size=opts.size,
                 padding=opts.padding,
                 max_windows=opts.max_windows,
                 max_sample_attempts=opts.max_sample_attempts,
                 efficient_aoi_sampling=opts.efficient_aoi_sampling,
-                transform=transform)
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
         else:
             raise NotImplementedError()
         return ds
 
 
 class RegressionModel(nn.Module):
     def __init__(self,
@@ -201,15 +213,14 @@
 
 
 @register_config('regression_learner')
 class RegressionLearnerConfig(LearnerConfig):
     """Configure a :class:`.RegressionLearner`."""
 
     model: Optional[RegressionModelConfig]
-    data: Union[RegressionImageDataConfig, RegressionGeoDataConfig]
 
     def build(self,
               tmp_dir,
               model_weights_path=None,
               model_def_path=None,
               loss_def_path=None,
               training=True):
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/semantic_segmentation_learner.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TYPE_CHECKING, Optional, Tuple
 import warnings
 
 import logging
 
 import torch
 from torch.nn import functional as F
+import torch.distributed as dist
 
 from rastervision.pytorch_learner.learner import Learner
 from rastervision.pytorch_learner.utils import (
     compute_conf_mat_metrics, compute_conf_mat, aggregate_metrics)
 from rastervision.pytorch_learner.dataset.visualizer import (
     SemanticSegmentationVisualizer)
 
@@ -40,16 +41,29 @@
         conf_mat = compute_conf_mat(out, y, num_labels)
 
         return {'val_loss': val_loss, 'conf_mat': conf_mat}
 
     def validate_end(self, outputs):
         metrics = aggregate_metrics(outputs, exclude_keys={'conf_mat'})
         conf_mat = sum([o['conf_mat'] for o in outputs])
-        conf_mat_metrics = compute_conf_mat_metrics(conf_mat,
-                                                    self.cfg.data.class_names)
+
+        if self.is_ddp_process:
+            metrics = self.reduce_distributed_metrics(metrics)
+            dist.reduce(conf_mat, dst=0, op=dist.ReduceOp.SUM)
+            if not self.is_ddp_master:
+                return metrics
+
+        ignored_idx = self.cfg.solver.ignore_class_index
+        if ignored_idx is not None and ignored_idx < 0:
+            ignored_idx += self.cfg.data.num_classes
+
+        class_names = self.cfg.data.class_names
+        conf_mat_metrics = compute_conf_mat_metrics(
+            conf_mat, class_names, ignore_idx=ignored_idx)
+
         metrics.update(conf_mat_metrics)
         return metrics
 
     def post_forward(self, x):
         if isinstance(x, dict):
             return x['out']
         return x
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/semantic_segmentation_learner_config.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Callable, Optional, Union
+from typing import Callable, Optional
 from os.path import join
 from enum import Enum
 import logging
 
 import albumentations as A
 from torch import nn
 from torch.utils.data import Dataset
 from torchvision import models
 
 from rastervision.core.data import Scene
+from rastervision.core.rv_pipeline import WindowSamplingMethod
 from rastervision.pipeline.config import (Config, register_config, Field,
                                           validator, ConfigError)
 from rastervision.pytorch_learner.learner_config import (
-    Backbone, LearnerConfig, ModelConfig, ImageDataConfig, GeoDataConfig,
-    GeoDataWindowMethod)
+    Backbone, LearnerConfig, ModelConfig, ImageDataConfig, GeoDataConfig)
 from rastervision.pytorch_learner.dataset import (
     SemanticSegmentationImageDataset,
     SemanticSegmentationSlidingWindowGeoDataset,
     SemanticSegmentationRandomWindowGeoDataset)
 from rastervision.pytorch_learner.utils import adjust_conv_channels
 
 log = logging.getLogger(__name__)
@@ -109,41 +109,52 @@
 
     def update(self, *args, **kwargs):
         SemanticSegmentationDataConfig.update(self)
         GeoDataConfig.update(self, *args, **kwargs)
 
     def scene_to_dataset(self,
                          scene: Scene,
-                         transform: Optional[A.BasicTransform] = None
-                         ) -> Dataset:
-        if isinstance(self.window_opts, dict):
-            opts = self.window_opts[scene.id]
+                         transform: Optional[A.BasicTransform] = None,
+                         for_chipping: bool = False) -> Dataset:
+        if isinstance(self.sampling, dict):
+            opts = self.sampling[scene.id]
         else:
-            opts = self.window_opts
+            opts = self.sampling
 
-        if opts.method == GeoDataWindowMethod.sliding:
+        extra_args = {}
+        if for_chipping:
+            extra_args = dict(
+                normalize=False, to_pytorch=False, return_window=True)
+
+        if opts.method == WindowSamplingMethod.sliding:
             ds = SemanticSegmentationSlidingWindowGeoDataset(
                 scene,
                 size=opts.size,
                 stride=opts.stride,
                 padding=opts.padding,
                 pad_direction=opts.pad_direction,
-                transform=transform)
-        elif opts.method == GeoDataWindowMethod.random:
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
+        elif opts.method == WindowSamplingMethod.random:
             ds = SemanticSegmentationRandomWindowGeoDataset(
                 scene,
                 size_lims=opts.size_lims,
                 h_lims=opts.h_lims,
                 w_lims=opts.w_lims,
                 out_size=opts.size,
                 padding=opts.padding,
                 max_windows=opts.max_windows,
                 max_sample_attempts=opts.max_sample_attempts,
                 efficient_aoi_sampling=opts.efficient_aoi_sampling,
-                transform=transform)
+                within_aoi=opts.within_aoi,
+                transform=transform,
+                **extra_args,
+            )
         else:
             raise NotImplementedError()
         return ds
 
 
 @register_config('semantic_segmentation_model')
 class SemanticSegmentationModelConfig(ModelConfig):
@@ -196,16 +207,14 @@
         return model
 
 
 @register_config('semantic_segmentation_learner')
 class SemanticSegmentationLearnerConfig(LearnerConfig):
     """Configure a :class:`.SemanticSegmentationLearner`."""
 
-    data: Union[SemanticSegmentationImageDataConfig,
-                SemanticSegmentationGeoDataConfig]
     model: Optional[SemanticSegmentationModelConfig]
 
     def build(self,
               tmp_dir=None,
               model_weights_path=None,
               model_def_path=None,
               loss_def_path=None,
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/utils/torch_hub.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/torch_hub.py`

 * *Files 22% similar despite different names*

```diff
@@ -58,96 +58,104 @@
     else:
         dir_name = _repo_name_to_dir_name(cfg.github_repo)
 
     path = join(parent, dir_name)
     return path
 
 
-def torch_hub_load_github(repo: str, hubconf_dir: str, entrypoint: str, *args,
+def torch_hub_load_github(repo: str,
+                          entrypoint: str,
+                          *args,
+                          dst_dir: Optional[str] = None,
                           **kwargs) -> Any:
     """Load an entrypoint from a github repo using :func:`torch.hub.load`.
 
     Args:
         repo (str): <repo-owner>/<erpo-name>[:tag]
-        hubconf_dir (str): Where the contents from the uri will finally
-            be saved to.
         entrypoint (str): Name of a callable present in hubconf.py.
         *args: Args to be passed to the entrypoint.
+        dst_dir: If provided, the contents of the repo are copied there.
+            Defaults to None.
         **kwargs: Keyword args to be passed to the entrypoint.
 
     Returns:
         Any: The output from calling the entrypoint.
     """
     out = torch.hub.load(
         repo,
         entrypoint,
         *args,
         source='github',
         skip_validation=True,
         **kwargs)
 
-    orig_dir = join(torch.hub.get_dir(), _repo_name_to_dir_name(repo))
-    _remove_dir(hubconf_dir)
-    shutil.move(orig_dir, hubconf_dir)
+    if dst_dir is not None:
+        orig_dir = join(torch.hub.get_dir(), _repo_name_to_dir_name(repo))
+        _remove_dir(dst_dir)
+        shutil.move(orig_dir, dst_dir)
 
     return out
 
 
-def torch_hub_load_uri(uri: str, hubconf_dir: str, entrypoint: str, *args,
+def torch_hub_load_uri(uri: str,
+                       entrypoint: str,
+                       *args,
+                       dst_dir: Optional[str] = None,
                        **kwargs) -> Any:
     """Load an entrypoint from a uri.
 
     Load an entrypoint from:
         - a local uri of a zip file, or
         - a local uri of a directory, or
         - a remote uri of zip file.
 
     The zip file should either have hubconf.py at the top level or contain
     a single sub-directory that contains hubconf.py at its top level. In the
-    latter case, the sub-directory will be copied to hubconf_dir.
+    latter case, the sub-directory will be copied to dst_dir.
 
     Args:
         uri (str): A URI.
-        hubconf_dir (str): The target directory where the contents from the uri
-            will finally be saved to.
         entrypoint (str): Name of a callable present in hubconf.py.
         *args: Args to be passed to the entrypoint.
+        dst_dir: If provided, the contents from the uri are copied there.
+            Defaults to None.
         **kwargs: Keyword args to be passed to the entrypoint.
 
     Returns:
         Any: The output from calling the entrypoint.
     """
-
     uri_path = Path(uri)
     is_zip = uri_path.suffix.lower() == '.zip'
     if is_zip:
-        # unzip
         zip_path = download_if_needed(uri)
         with get_tmp_dir() as tmp_dir:
             unzip_dir = join(tmp_dir, uri_path.stem)
             _remove_dir(unzip_dir)
             unzip(zip_path, target_dir=unzip_dir)
             unzipped_contents = list(glob(f'{unzip_dir}/*', recursive=False))
 
-            _remove_dir(hubconf_dir)
-
             # if the top level only contains a directory
             if (len(unzipped_contents) == 1) and isdir(unzipped_contents[0]):
                 sub_dir = unzipped_contents[0]
-                shutil.move(sub_dir, hubconf_dir)
+                scr_dir = sub_dir
             else:
-                shutil.move(unzip_dir, hubconf_dir)
-    # assume uri is local and attempt copying
+                scr_dir = unzip_dir
+
+            out = torch_hub_load_local(scr_dir, entrypoint, *args, **kwargs)
+
+            if dst_dir is not None:
+                _remove_dir(dst_dir)
+                shutil.move(scr_dir, dst_dir)
     else:
-        # only copy if needed
-        if realpath(uri) != realpath(hubconf_dir):
-            _remove_dir(hubconf_dir)
-            shutil.copytree(uri, hubconf_dir)
+        # assume uri is local
+        out = torch_hub_load_local(uri, entrypoint, *args, **kwargs)
+        if dst_dir is not None and realpath(uri) != realpath(dst_dir):
+            _remove_dir(dst_dir)
+            shutil.copytree(uri, dst_dir)
 
-    out = torch_hub_load_local(hubconf_dir, entrypoint, *args, **kwargs)
     return out
 
 
 def torch_hub_load_local(hubconf_dir: str, entrypoint: str, *args,
                          **kwargs) -> Any:
     """Wrapper around :func:`torch.hub.load` with ``source='local'``.
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision/pytorch_learner/utils/utils.py` & `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from typing import (Any, Dict, Sequence, Tuple, Optional, Union, List,
-                    Iterable, Container)
+from typing import (TYPE_CHECKING, Any, Dict, Sequence, Tuple, Optional, Union,
+                    List, Iterable, Container)
 from os.path import basename, join, isfile
 import logging
 
 import torch
 from torch import nn
 from torch.hub import _import_module
 import numpy as np
 from PIL import ImageColor
 import albumentations as A
 from albumentations.core.transforms_interface import ImageOnlyTransform
 import cv2
 import pandas as pd
-import onnxruntime as ort
 
-from rastervision.pipeline.file_system import get_tmp_dir
-from rastervision.pipeline.config import ConfigError
+from rastervision.pipeline.file_system.utils import (file_exists, file_to_json,
+                                                     get_tmp_dir)
+from rastervision.pipeline.config import (build_config, Config, ConfigError,
+                                          upgrade_config)
+
+if TYPE_CHECKING:
+    import onnxruntime as ort
+    from rastervision.pytorch_learner import LearnerConfig
 
 log = logging.getLogger(__name__)
 
 
 def color_to_triple(color: Optional[str] = None) -> Tuple[int, int, int]:
     """Given a PIL ImageColor string, return a triple of integers
     representing the red, green, and blue values.
@@ -38,24 +43,37 @@
         g = np.random.randint(0, 0x100)
         b = np.random.randint(0, 0x100)
         return (r, g, b)
     else:
         return ImageColor.getrgb(color)
 
 
-def compute_conf_mat(out, y, num_labels):
+def compute_conf_mat(out: torch.Tensor, y: torch.Tensor,
+                     num_labels: int) -> torch.Tensor:
     labels = torch.arange(0, num_labels).to(out.device)
-    return ((out == labels[:, None]) & (y == labels[:, None, None])).sum(
+    conf_mat = ((out == labels[:, None]) & (y == labels[:, None, None])).sum(
         dim=2, dtype=torch.float32)
+    return conf_mat
 
 
-def compute_conf_mat_metrics(conf_mat, label_names, eps=1e-6):
+def compute_conf_mat_metrics(conf_mat: torch.Tensor,
+                             label_names: list[str],
+                             ignore_idx: Optional[int] = None,
+                             eps: float = 1e-6):
     # eps is to avoid dividing by zero.
     eps = torch.tensor(eps)
     conf_mat = conf_mat.cpu()
+
+    if ignore_idx is not None:
+        keep_mask = torch.arange(len(conf_mat)) != ignore_idx
+        conf_mat = conf_mat[keep_mask, :]
+        conf_mat = conf_mat[:, keep_mask]
+        label_names = (
+            label_names[:ignore_idx] + label_names[(ignore_idx + 1):])
+
     gt_count = conf_mat.sum(dim=1)
     pred_count = conf_mat.sum(dim=0)
     total = conf_mat.sum()
     true_pos = torch.diag(conf_mat)
     precision = true_pos / torch.max(pred_count, eps)
     recall = true_pos / torch.max(gt_count, eps)
     f1 = (2 * precision * recall) / torch.max(precision + recall, eps)
@@ -67,19 +85,19 @@
         weighted_precision + weighted_recall, eps))
 
     metrics = {
         'avg_precision': weighted_precision.item(),
         'avg_recall': weighted_recall.item(),
         'avg_f1': weighted_f1.item()
     }
-    for ind, label in enumerate(label_names):
+    for i, label in enumerate(label_names):
         metrics.update({
-            '{}_precision'.format(label): precision[ind].item(),
-            '{}_recall'.format(label): recall[ind].item(),
-            '{}_f1'.format(label): f1[ind].item(),
+            f'{label}_precision': precision[i].item(),
+            f'{label}_recall': recall[i].item(),
+            f'{label}_f1': f1[i].item(),
         })
     return metrics
 
 
 def validate_albumentation_transform(tf_dict: Optional[dict]) -> dict:
     """ Validate a serialized albumentation transform by attempting to
     deserialize it.
@@ -364,15 +382,15 @@
     metrics_df.to_csv(
         csv_path, mode='a', header=(not log_file_exists), index=False)
 
 
 def aggregate_metrics(
         outputs: List[Dict[str, Union[float, torch.Tensor]]],
         exclude_keys: Container[str] = set('conf_mat')) -> Dict[str, float]:
-    """Aggregate the ouput of validate_step at the end of the epoch.
+    """Aggregate the output of validate_step at the end of the epoch.
 
     Args:
         outputs: A list of outputs of Learner.validate_step().
         exclude_keys: Keys to ignore. These will not be aggregated and will not
             be included in the output. Defaults to {'conf_mat'}.
 
     Returns:
@@ -447,21 +465,25 @@
 class ONNXRuntimeAdapter:
     """Wrapper around ONNX-runtime that behaves like a PyTorch nn.Module.
 
     That is, it implements __call__() and accepts PyTorch Tensors as inputs and
     also outputs PyTorch Tensors.
     """
 
-    def __init__(self, ort_session: ort.InferenceSession) -> None:
+    def __init__(self, ort_session: 'ort.InferenceSession') -> None:
         """Constructor.
 
         Args:
             ort_session (ort.InferenceSession): ONNX-runtime InferenceSession.
         """
         self.ort_session = ort_session
+        inputs = ort_session.get_inputs()
+        if len(inputs) > 1:
+            return ValueError('ONNX model must only take one input.')
+        self.input_key = inputs[0].name
 
     @classmethod
     def from_file(cls, path: str, providers: Optional[List[str]] = None
                   ) -> 'ONNXRuntimeAdapter':
         """Construct from file.
 
         Args:
@@ -469,21 +491,43 @@
             providers (Optional[List[str]]): ONNX-runtime execution
                 providers. See onnxruntime documentation for more details.
                 Defaults to None.
 
         Returns:
             ONNXRuntimeAdapter: An ONNXRuntimeAdapter instance.
         """
+        import onnxruntime as ort
+
         if providers is None:
             providers = ort.get_available_providers()
             log.info(f'Using ONNX execution providers: {providers}')
         ort_session = ort.InferenceSession(path, providers=providers)
         onnx_model = cls(ort_session)
         return onnx_model
 
     def __call__(self, x: Union[torch.Tensor, np.ndarray]) -> torch.Tensor:
         x = x.numpy()
-        outputs = self.ort_session.run(None, dict(x=x))
+        outputs = self.ort_session.run(None, {self.input_key: x})
         out = outputs[0]
         if isinstance(out, np.ndarray):
             out = torch.from_numpy(out)
         return out
+
+
+def get_learner_config_from_bundle_dir(
+        model_bundle_dir: str) -> 'LearnerConfig':
+    config_path = join(model_bundle_dir, 'learner-config.json')
+    if file_exists(config_path):
+        cfg = Config.from_file(config_path)
+    else:
+        # backward compatibility
+        config_path = join(model_bundle_dir, 'pipeline-config.json')
+        if not file_exists(config_path):
+            raise FileNotFoundError(
+                'Could not find a valid config file in the bundle.')
+        pipeline_cfg_dict = file_to_json(config_path)
+        cfg_dict = pipeline_cfg_dict['learner']
+        cfg_dict['plugin_versions'] = pipeline_cfg_dict['plugin_versions']
+        cfg_dict = upgrade_config(cfg_dict)
+        cfg_dict.pop('plugin_versions', None)
+        cfg = build_config(cfg_dict)
+    return cfg
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/PKG-INFO` & `rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-pytorch-learner
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds PyTorch training pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_learner-0.21.3/rastervision_pytorch_learner.egg-info/SOURCES.txt` & `rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 requirements.txt
 setup.py
 rastervision/pytorch_learner/__init__.py
 rastervision/pytorch_learner/classification_learner.py
 rastervision/pytorch_learner/classification_learner_config.py
 rastervision/pytorch_learner/learner.py
 rastervision/pytorch_learner/learner_config.py
-rastervision/pytorch_learner/learner_pipeline.py
-rastervision/pytorch_learner/learner_pipeline_config.py
 rastervision/pytorch_learner/object_detection_learner.py
 rastervision/pytorch_learner/object_detection_learner_config.py
 rastervision/pytorch_learner/object_detection_utils.py
 rastervision/pytorch_learner/regression_learner.py
 rastervision/pytorch_learner/regression_learner_config.py
 rastervision/pytorch_learner/semantic_segmentation_learner.py
 rastervision/pytorch_learner/semantic_segmentation_learner_config.py
@@ -19,23 +17,24 @@
 rastervision/pytorch_learner/dataset/classification_dataset.py
 rastervision/pytorch_learner/dataset/dataset.py
 rastervision/pytorch_learner/dataset/object_detection_dataset.py
 rastervision/pytorch_learner/dataset/regression_dataset.py
 rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py
 rastervision/pytorch_learner/dataset/transform.py
 rastervision/pytorch_learner/dataset/utils/__init__.py
-rastervision/pytorch_learner/dataset/utils/aoi_sampler.py
 rastervision/pytorch_learner/dataset/utils/utils.py
 rastervision/pytorch_learner/dataset/visualizer/__init__.py
 rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py
 rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py
 rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py
 rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py
 rastervision/pytorch_learner/dataset/visualizer/visualizer.py
 rastervision/pytorch_learner/utils/__init__.py
+rastervision/pytorch_learner/utils/distributed.py
+rastervision/pytorch_learner/utils/prediction.py
 rastervision/pytorch_learner/utils/torch_hub.py
 rastervision/pytorch_learner/utils/utils.py
 rastervision_pytorch_learner.egg-info/PKG-INFO
 rastervision_pytorch_learner.egg-info/SOURCES.txt
 rastervision_pytorch_learner.egg-info/dependency_links.txt
 rastervision_pytorch_learner.egg-info/not-zip-safe
 rastervision_pytorch_learner.egg-info/requires.txt
```

### Comparing `rastervision_pytorch_learner-0.21.3/setup.py` & `rastervision_pytorch_learner-0.30.0/setup.py`

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
 
 name = 'rastervision_pytorch_learner'
-version = '0.21.3'
+version = '0.30.0'
 description = 'A rastervision plugin that adds PyTorch training pipelines'
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

