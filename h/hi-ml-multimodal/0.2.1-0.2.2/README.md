# Comparing `tmp/hi-ml-multimodal-0.2.1.tar.gz` & `tmp/hi-ml-multimodal-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-ml-multimodal-0.2.1.tar", last modified: Thu Apr 20 13:56:27 2023, max compression
+gzip compressed data, was "hi-ml-multimodal-0.2.2.tar", last modified: Thu Apr 11 09:29:00 2024, max compression
```

## Comparing `hi-ml-multimodal-0.2.1.tar` & `hi-ml-multimodal-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/
--rw-r--r--   0 fernando  (1000) fernando  (1000)       63 2023-03-06 16:22:52.000000 hi-ml-multimodal-0.2.1/MANIFEST.in
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4864 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4254 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/README.md
--rw-r--r--   0 fernando  (1000) fernando  (1000)      161 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/requirements_run.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       38 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/setup.cfg
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1510 2023-04-20 13:54:46.000000 hi-ml-multimodal-0.2.1/setup.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.325276 hi-ml-multimodal-0.2.1/src/
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.325276 hi-ml-multimodal-0.2.1/src/health_multimodal/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      369 2023-04-20 13:54:46.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/__init__.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.325276 hi-ml-multimodal-0.2.1/src/health_multimodal/common/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      472 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/common/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)      605 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/common/device.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5245 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/common/visualization.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/image/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1056 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/__init__.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      346 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2835 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/io.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3332 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/transforms.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3764 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/inference_engine.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      526 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     7625 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/encoder.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5725 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/model.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3731 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/modules.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4625 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/pretrained.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3186 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/resnet.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)    11818 2023-04-20 13:54:43.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/transformer.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1329 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/types.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1778 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/image/utils.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/text/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1123 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/__init__.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      346 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2617 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/io.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5045 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/inference_engine.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      575 2022-07-27 21:15:34.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)      889 2022-07-01 12:45:09.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/configuration_cxrbert.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     5785 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/modelling_cxrbert.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     2544 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/text/utils.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/
--rw-r--r--   0 fernando  (1000) fernando  (1000)      584 2022-07-27 21:15:34.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/__init__.py
--rw-r--r--   0 fernando  (1000) fernando  (1000)     7552 2023-04-12 14:44:35.000000 hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/inference_engine.py
-drwxr-xr-x   0 fernando  (1000) fernando  (1000)        0 2023-04-20 13:56:27.334885 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     4864 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/PKG-INFO
--rw-r--r--   0 fernando  (1000) fernando  (1000)     1494 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)        1 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)      161 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/requires.txt
--rw-r--r--   0 fernando  (1000) fernando  (1000)       18 2023-04-20 13:56:27.000000 hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/top_level.txt
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)       63 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/MANIFEST.in
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     5115 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/PKG-INFO
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     4254 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/README.md
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      101 2024-04-11 09:18:28.000000 hi-ml-multimodal-0.2.2/requirements_run.txt
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)       38 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/setup.cfg
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     1510 2024-04-11 09:20:31.000000 hi-ml-multimodal-0.2.2/setup.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.923621 hi-ml-multimodal-0.2.2/src/
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.923621 hi-ml-multimodal-0.2.2/src/health_multimodal/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      369 2024-04-11 09:20:31.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/__init__.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.923621 hi-ml-multimodal-0.2.2/src/health_multimodal/common/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      472 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/common/__init__.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      605 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/common/device.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     5245 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/common/visualization.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.923621 hi-ml-multimodal-0.2.2/src/health_multimodal/image/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     1056 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/__init__.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.923621 hi-ml-multimodal-0.2.2/src/health_multimodal/image/data/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      346 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/data/__init__.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     2835 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/data/io.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     3332 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/data/transforms.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     3764 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/inference_engine.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      526 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/__init__.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     7625 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/encoder.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     5725 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/model.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     3731 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/modules.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     4667 2024-04-11 09:18:28.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/pretrained.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     3346 2024-04-11 09:18:28.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/resnet.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)    11784 2024-04-11 09:18:28.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/transformer.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     1329 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/types.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     1778 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/image/utils.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/src/health_multimodal/text/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     1123 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/__init__.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/src/health_multimodal/text/data/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      346 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/data/__init__.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     2617 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/data/io.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     5045 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/inference_engine.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      575 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/__init__.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      889 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/configuration_cxrbert.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     5847 2024-04-11 09:18:28.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/modelling_cxrbert.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     2544 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/text/utils.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/src/health_multimodal/vlp/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      584 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/vlp/__init__.py
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     7552 2024-04-10 16:11:40.000000 hi-ml-multimodal-0.2.2/src/health_multimodal/vlp/inference_engine.py
+drwxr-xr-x   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        0 2024-04-11 09:29:00.927621 hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     5115 2024-04-11 09:29:00.000000 hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)     1494 2024-04-11 09:29:00.000000 hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)        1 2024-04-11 09:29:00.000000 hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)      101 2024-04-11 09:29:00.000000 hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/requires.txt
+-rw-r--r--   0 EUROPE.fperezgarcia (104237084) EUROPE.domain users (100000513)       18 2024-04-11 09:29:00.000000 hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/top_level.txt
```

### Comparing `hi-ml-multimodal-0.2.1/PKG-INFO` & `hi-ml-multimodal-0.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: hi-ml-multimodal
-Version: 0.2.1
-Summary: Microsoft Health Futures package to work with multi-modal health data
-Home-page: https://github.com/microsoft/hi-ml
-Author: Biomedical Imaging Team @ Microsoft Health Futures
-Author-email: innereyedev@microsoft.com
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 # HI-ML Multimodal Toolbox
 
 This toolbox provides models for multimodal health data.
 The code is available on [GitHub][1] and [Hugging Face 🤗][6].
 
 ## Getting started
```

### Comparing `hi-ml-multimodal-0.2.1/README.md` & `hi-ml-multimodal-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: hi-ml-multimodal
+Version: 0.2.2
+Summary: Microsoft Health Futures package to work with multi-modal health data
+Home-page: https://github.com/microsoft/hi-ml
+Author: Biomedical Imaging Team @ Microsoft Health Futures
+Author-email: innereyedev@microsoft.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+Requires-Dist: huggingface-hub
+Requires-Dist: matplotlib
+Requires-Dist: Pillow
+Requires-Dist: pydicom
+Requires-Dist: scikit-image
+Requires-Dist: SimpleITK
+Requires-Dist: timm
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: transformers
+
 # HI-ML Multimodal Toolbox
 
 This toolbox provides models for multimodal health data.
 The code is available on [GitHub][1] and [Hugging Face 🤗][6].
 
 ## Getting started
```

### Comparing `hi-ml-multimodal-0.2.1/setup.py` & `hi-ml-multimodal-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  ------------------------------------------------------------------------------------------
 
 from pathlib import Path
 from setuptools import find_namespace_packages, setup  # type: ignore
 
 
 long_description = Path("README.md").read_text(encoding="utf-8")
-version = "0.2.1"
+version = "0.2.2"
 package_name = "hi-ml-multimodal"
 install_requires = Path("requirements_run.txt").read_text().splitlines()
 
 description = "Microsoft Health Futures package to work with multi-modal health data"
 
 setup(
     name=package_name,
```

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/common/device.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/common/device.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/common/visualization.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/common/visualization.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/__init__.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/io.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/data/io.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/data/transforms.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/data/transforms.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/inference_engine.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/inference_engine.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/__init__.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/encoder.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/encoder.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/model.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/model.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/modules.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/modules.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/pretrained.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/pretrained.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import annotations
 
 import tempfile
 from pathlib import Path
 
 from torch.hub import load_state_dict_from_url
 from torchvision.datasets.utils import download_url
-from torchvision.models.resnet import model_urls
+from torchvision.models.resnet import ResNet50_Weights
 
 from .model import ImageModel
 from .types import ImageEncoderType, ImageEncoderWeightTypes
 
 
 JOINT_FEATURE_SIZE = 128
 
@@ -71,31 +71,32 @@
         img_encoder_type=ImageEncoderType.RESNET50,
         joint_feature_size=JOINT_FEATURE_SIZE,
         pretrained_model_path=resnet_checkpoint_path,
     )
     return image_model
 
 
-def get_biovil_t_image_encoder() -> ImageModel:
+def get_biovil_t_image_encoder(**kwargs) -> ImageModel:
     """Download weights from Hugging Face and instantiate the image model."""
 
     biovilt_checkpoint_path = _download_biovil_t_image_model_weights()
     model_type = ImageEncoderType.RESNET50_MULTI_IMAGE
     image_model = ImageModel(
         img_encoder_type=model_type,
         joint_feature_size=JOINT_FEATURE_SIZE,
         pretrained_model_path=biovilt_checkpoint_path,
+        **kwargs,
     )
     return image_model
 
 
 def get_imagenet_init_encoder() -> ImageModel:
     """Download ImageNet pre-trained weights and instantiate the image model."""
-
-    state_dict = load_state_dict_from_url(model_urls[ImageEncoderType.RESNET50])
+    url = ResNet50_Weights.IMAGENET1K_V1.url
+    state_dict = load_state_dict_from_url(url)
     image_model = ImageModel(
         img_encoder_type=ImageEncoderType.RESNET50,
         joint_feature_size=JOINT_FEATURE_SIZE,
         pretrained_model_path=None,
     )
     image_model.encoder.encoder.load_state_dict(state_dict)
     return image_model
```

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/resnet.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/resnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  -------------------------------------------------------------------------------------------
 
 from typing import Any, List, Tuple, Type, Union
 
 import torch
 from torch.hub import load_state_dict_from_url
-from torchvision.models.resnet import model_urls, ResNet, BasicBlock, Bottleneck
+from torchvision.models.resnet import ResNet, BasicBlock, Bottleneck
+from torchvision.models.resnet import ResNet18_Weights
+from torchvision.models.resnet import ResNet50_Weights
 
 TypeSkipConnections = Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]
 
 
 class ResNetHIML(ResNet):
     """Wrapper class of the original torchvision ResNet model.
 
@@ -45,43 +47,45 @@
         if return_intermediate_layers:
             return x0, x1, x2, x3, x4
         else:
             return x4
 
 
 def _resnet(
-    arch: str,
+    url: str,
     block: Type[Union[BasicBlock, Bottleneck]],
     layers: List[int],
     pretrained: bool,
     progress: bool,
     **kwargs: Any
 ) -> ResNetHIML:
     """Instantiate a custom :class:`ResNet` model.
 
     Adapted from :mod:`torchvision.models.resnet`.
     """
     model = ResNetHIML(block=block, layers=layers, **kwargs)
     if pretrained:
-        state_dict = load_state_dict_from_url(model_urls[arch], progress=progress)
+        state_dict = load_state_dict_from_url(url, progress=progress)
         model.load_state_dict(state_dict)
     return model
 
 
 def resnet18(pretrained: bool = False, progress: bool = True, **kwargs: Any) -> ResNetHIML:
     r"""ResNet-18 model from
     `"Deep Residual Learning for Image Recognition" <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     :param pretrained: If ``True``, returns a model pre-trained on ImageNet.
     :param progress: If ``True``, displays a progress bar of the download to ``stderr``.
     """
-    return _resnet('resnet18', BasicBlock, [2, 2, 2, 2], pretrained, progress, **kwargs)
+    url = ResNet18_Weights.IMAGENET1K_V1.url
+    return _resnet(url, BasicBlock, [2, 2, 2, 2], pretrained, progress, **kwargs)
 
 
 def resnet50(pretrained: bool = False, progress: bool = True, **kwargs: Any) -> ResNetHIML:
     r"""ResNet-50 model from
     `"Deep Residual Learning for Image Recognition" <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     :param pretrained: If ``True``, returns a model pre-trained on ImageNet
     :param progress: If ``True``, displays a progress bar of the download to ``stderr``.
     """
-    return _resnet('resnet50', Bottleneck, [3, 4, 6, 3], pretrained, progress, **kwargs)
+    url = ResNet50_Weights.IMAGENET1K_V1.url
+    return _resnet(url, Bottleneck, [3, 4, 6, 3], pretrained, progress, **kwargs)
```

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/transformer.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from dataclasses import dataclass
 from functools import partial
 from typing import Any, Callable, Optional, Set, Tuple
 
 import torch
 import torch.nn as nn
 from timm.models.layers import DropPath, Mlp, trunc_normal_
-from transformers.pytorch_utils import torch_int_div
 
 
 @dataclass
 class MultiHeadAttentionOutput:
     mha_output: torch.Tensor
     attention: Optional[torch.Tensor] = None
 
@@ -261,15 +260,15 @@
         y_embed = mask.cumsum(1, dtype=torch.float32)
         x_embed = mask.cumsum(2, dtype=torch.float32)
         if self.normalize:
             y_embed = y_embed / (y_embed[:, -1:, :] + 1e-6) * self.scale
             x_embed = x_embed / (x_embed[:, :, -1:] + 1e-6) * self.scale
 
         dim_t = torch.arange(self.embedding_dim, dtype=torch.float32)
-        dim_t = self.temperature ** (2 * torch_int_div(dim_t, 2) / self.embedding_dim)
+        dim_t = self.temperature ** (2 * torch.div(dim_t, 2, rounding_mode="floor") / self.embedding_dim)
 
         pos_x = x_embed[:, :, :, None] / dim_t
         pos_y = y_embed[:, :, :, None] / dim_t
         pos_x = torch.stack((pos_x[:, :, :, 0::2].sin(), pos_x[:, :, :, 1::2].cos()), dim=4).flatten(3)
         pos_y = torch.stack((pos_y[:, :, :, 0::2].sin(), pos_y[:, :, :, 1::2].cos()), dim=4).flatten(3)
         pos = torch.cat((pos_y, pos_x), dim=3).view(B, H * W, self.embedding_dim * 2)
```

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/model/types.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/model/types.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/image/utils.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/image/utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/__init__.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/data/io.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/data/io.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/inference_engine.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/inference_engine.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/__init__.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/configuration_cxrbert.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/configuration_cxrbert.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/model/modelling_cxrbert.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/model/modelling_cxrbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 
+from dataclasses import dataclass
 from typing import Any, Optional, Tuple, Union
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 from torch import Tensor as T
 from transformers import BertForMaskedLM
 from transformers.modeling_outputs import ModelOutput
 
 from health_multimodal.text.model.configuration_cxrbert import CXRBertConfig
 
 BERTTupleOutput = Tuple[T, T, T, T, T]
 
 
+@dataclass
 class CXRBertOutput(ModelOutput):
     last_hidden_state: torch.FloatTensor
-    logits: torch.FloatTensor
+    logits: Optional[torch.FloatTensor] = None
     cls_projected_embedding: Optional[torch.FloatTensor] = None
     hidden_states: Optional[Tuple[torch.FloatTensor]] = None
     attentions: Optional[Tuple[torch.FloatTensor]] = None
 
 
 class BertProjectionHead(nn.Module):
     """Projection head to be used with BERT CLS token.
```

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/text/utils.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/text/utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/__init__.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/vlp/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/health_multimodal/vlp/inference_engine.py` & `hi-ml-multimodal-0.2.2/src/health_multimodal/vlp/inference_engine.py`

 * *Files identical despite different names*

### Comparing `hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/PKG-INFO` & `hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: hi-ml-multimodal
-Version: 0.2.1
+Version: 0.2.2
 Summary: Microsoft Health Futures package to work with multi-modal health data
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+Requires-Dist: huggingface-hub
+Requires-Dist: matplotlib
+Requires-Dist: Pillow
+Requires-Dist: pydicom
+Requires-Dist: scikit-image
+Requires-Dist: SimpleITK
+Requires-Dist: timm
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: transformers
 
 # HI-ML Multimodal Toolbox
 
 This toolbox provides models for multimodal health data.
 The code is available on [GitHub][1] and [Hugging Face 🤗][6].
 
 ## Getting started
```

### Comparing `hi-ml-multimodal-0.2.1/src/hi_ml_multimodal.egg-info/SOURCES.txt` & `hi-ml-multimodal-0.2.2/src/hi_ml_multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

