# Comparing `tmp/openvino_model_api-0.1.9.tar.gz` & `tmp/openvino_model_api-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino_model_api-0.1.9.tar", last modified: Wed Jan 31 03:32:51 2024, max compression
+gzip compressed data, was "openvino_model_api-0.1.9.1.tar", last modified: Thu Apr 11 23:38:28 2024, max compression
```

## Comparing `openvino_model_api-0.1.9.tar` & `openvino_model_api-0.1.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-01-31 03:32:51.135666 openvino_model_api-0.1.9/
--rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     7439 2024-01-31 03:32:51.135666 openvino_model_api-0.1.9/PKG-INFO
-drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-01-31 03:32:51.135666 openvino_model_api-0.1.9/openvino_model_api.egg-info/
--rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     7439 2024-01-31 03:32:51.000000 openvino_model_api-0.1.9/openvino_model_api.egg-info/PKG-INFO
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     3802 2024-01-31 03:32:51.000000 openvino_model_api-0.1.9/openvino_model_api.egg-info/SOURCES.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        1 2024-01-31 03:32:51.000000 openvino_model_api-0.1.9/openvino_model_api.egg-info/dependency_links.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      211 2024-01-31 03:32:51.000000 openvino_model_api-0.1.9/openvino_model_api.egg-info/requires.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        9 2024-01-31 03:32:51.000000 openvino_model_api-0.1.9/openvino_model_api.egg-info/top_level.txt
--rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)       38 2024-01-31 03:32:51.135666 openvino_model_api-0.1.9/setup.cfg
--rwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)     1785 2024-01-31 03:28:14.000000 openvino_model_api-0.1.9/setup.py
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-04-11 23:38:28.789264 openvino_model_api-0.1.9.1/
+-rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     7441 2024-04-11 23:38:28.789264 openvino_model_api-0.1.9.1/PKG-INFO
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2024-04-11 23:38:28.789264 openvino_model_api-0.1.9.1/openvino_model_api.egg-info/
+-rw-r--r--   0 vsovraso  (1002) vsovraso  (1002)     7441 2024-04-11 23:38:28.000000 openvino_model_api-0.1.9.1/openvino_model_api.egg-info/PKG-INFO
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     3802 2024-04-11 23:38:28.000000 openvino_model_api-0.1.9.1/openvino_model_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        1 2024-04-11 23:38:28.000000 openvino_model_api-0.1.9.1/openvino_model_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      211 2024-04-11 23:38:28.000000 openvino_model_api-0.1.9.1/openvino_model_api.egg-info/requires.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        9 2024-04-11 23:38:28.000000 openvino_model_api-0.1.9.1/openvino_model_api.egg-info/top_level.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)       38 2024-04-11 23:38:28.789264 openvino_model_api-0.1.9.1/setup.cfg
+-rwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)     1787 2024-04-11 22:13:08.000000 openvino_model_api-0.1.9.1/setup.py
```

### Comparing `openvino_model_api-0.1.9/PKG-INFO` & `openvino_model_api-0.1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openvino_model_api
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Model API: model wrappers and pipelines for inference with OpenVINO
 Home-page: https://github.com/openvinotoolkit/model_api
 Author: Intel(R) Corporation
 License: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.16.6
 Requires-Dist: opencv-python
 Requires-Dist: scipy>=1.5.4
-Requires-Dist: openvino>=2023.0.0
-Requires-Dist: openvino-dev>=2023.0.0
+Requires-Dist: openvino<=2023.3.0
+Requires-Dist: openvino-dev<=2023.3.0
 Provides-Extra: ovms
 Requires-Dist: ovmsclient; extra == "ovms"
 Provides-Extra: tests
 Requires-Dist: httpx; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: openvino-dev[onnx,pytorch,tensorflow2]; extra == "tests"
 Requires-Dist: ultralytics<=8.0.205,>=8.0.114; extra == "tests"
```

### Comparing `openvino_model_api-0.1.9/openvino_model_api.egg-info/PKG-INFO` & `openvino_model_api-0.1.9.1/openvino_model_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openvino_model_api
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Model API: model wrappers and pipelines for inference with OpenVINO
 Home-page: https://github.com/openvinotoolkit/model_api
 Author: Intel(R) Corporation
 License: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.16.6
 Requires-Dist: opencv-python
 Requires-Dist: scipy>=1.5.4
-Requires-Dist: openvino>=2023.0.0
-Requires-Dist: openvino-dev>=2023.0.0
+Requires-Dist: openvino<=2023.3.0
+Requires-Dist: openvino-dev<=2023.3.0
 Provides-Extra: ovms
 Requires-Dist: ovmsclient; extra == "ovms"
 Provides-Extra: tests
 Requires-Dist: httpx; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: openvino-dev[onnx,pytorch,tensorflow2]; extra == "tests"
 Requires-Dist: ultralytics<=8.0.205,>=8.0.114; extra == "tests"
```

### Comparing `openvino_model_api-0.1.9/openvino_model_api.egg-info/SOURCES.txt` & `openvino_model_api-0.1.9.1/openvino_model_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvino_model_api-0.1.9/setup.py` & `openvino_model_api-0.1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from setuptools import find_packages, setup
 
 SETUP_DIR = Path(__file__).resolve().parent
 
 setup(
     name="openvino_model_api",
-    version="0.1.9",
+    version="0.1.9.1",
     description="Model API: model wrappers and pipelines for inference with OpenVINO",
     author="Intel(R) Corporation",
     url="https://github.com/openvinotoolkit/model_api",
     packages=find_packages(SETUP_DIR),
     package_dir={"openvino": str(SETUP_DIR / "openvino")},
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
```

