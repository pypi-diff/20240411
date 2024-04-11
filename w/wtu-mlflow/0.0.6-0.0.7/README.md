# Comparing `tmp/wtu-mlflow-0.0.6.tar.gz` & `tmp/wtu-mlflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtu-mlflow-0.0.6.tar", last modified: Thu Apr 11 06:10:55 2024, max compression
+gzip compressed data, was "wtu-mlflow-0.0.7.tar", last modified: Thu Apr 11 10:46:44 2024, max compression
```

## Comparing `wtu-mlflow-0.0.6.tar` & `wtu-mlflow-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hbjs       (501) staff       (20)        0 2024-04-11 06:10:55.113551 wtu-mlflow-0.0.6/
--rw-r--r--   0 hbjs       (501) staff       (20)     2177 2024-04-11 06:10:55.113400 wtu-mlflow-0.0.6/PKG-INFO
--rw-r--r--   0 hbjs       (501) staff       (20)     1485 2024-03-26 06:02:23.000000 wtu-mlflow-0.0.6/README.md
--rw-r--r--   0 hbjs       (501) staff       (20)       38 2024-04-11 06:10:55.113597 wtu-mlflow-0.0.6/setup.cfg
--rw-r--r--   0 hbjs       (501) staff       (20)      772 2024-04-11 06:10:43.000000 wtu-mlflow-0.0.6/setup.py
-drwxr-xr-x   0 hbjs       (501) staff       (20)        0 2024-04-11 06:10:55.112699 wtu-mlflow-0.0.6/wtu_mlflow/
--rw-r--r--   0 hbjs       (501) staff       (20)      153 2024-04-09 06:40:25.000000 wtu-mlflow-0.0.6/wtu_mlflow/__init__.py
--rw-r--r--   0 hbjs       (501) staff       (20)     2523 2024-04-11 06:08:53.000000 wtu-mlflow-0.0.6/wtu_mlflow/base_mlflow_client.py
--rw-r--r--   0 hbjs       (501) staff       (20)      559 2024-04-01 07:08:25.000000 wtu-mlflow-0.0.6/wtu_mlflow/env_checker.py
--rw-r--r--   0 hbjs       (501) staff       (20)     3254 2024-04-11 06:10:10.000000 wtu-mlflow-0.0.6/wtu_mlflow/onnx_client.py
--rw-r--r--   0 hbjs       (501) staff       (20)     3322 2024-04-11 06:09:39.000000 wtu-mlflow-0.0.6/wtu_mlflow/torch_client.py
-drwxr-xr-x   0 hbjs       (501) staff       (20)        0 2024-04-11 06:10:55.113213 wtu-mlflow-0.0.6/wtu_mlflow.egg-info/
--rw-r--r--   0 hbjs       (501) staff       (20)     2177 2024-04-11 06:10:55.000000 wtu-mlflow-0.0.6/wtu_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 hbjs       (501) staff       (20)      322 2024-04-11 06:10:55.000000 wtu-mlflow-0.0.6/wtu_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 hbjs       (501) staff       (20)        1 2024-04-11 06:10:55.000000 wtu-mlflow-0.0.6/wtu_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 hbjs       (501) staff       (20)       78 2024-04-11 06:10:55.000000 wtu-mlflow-0.0.6/wtu_mlflow.egg-info/requires.txt
--rw-r--r--   0 hbjs       (501) staff       (20)       11 2024-04-11 06:10:55.000000 wtu-mlflow-0.0.6/wtu_mlflow.egg-info/top_level.txt
+drwxr-xr-x   0 hbjs       (501) staff       (20)        0 2024-04-11 10:46:44.046489 wtu-mlflow-0.0.7/
+-rw-r--r--   0 hbjs       (501) staff       (20)     2177 2024-04-11 10:46:44.046354 wtu-mlflow-0.0.7/PKG-INFO
+-rw-r--r--   0 hbjs       (501) staff       (20)     1485 2024-03-26 06:02:23.000000 wtu-mlflow-0.0.7/README.md
+-rw-r--r--   0 hbjs       (501) staff       (20)       38 2024-04-11 10:46:44.046532 wtu-mlflow-0.0.7/setup.cfg
+-rw-r--r--   0 hbjs       (501) staff       (20)      800 2024-04-11 10:46:42.000000 wtu-mlflow-0.0.7/setup.py
+drwxr-xr-x   0 hbjs       (501) staff       (20)        0 2024-04-11 10:46:44.045177 wtu-mlflow-0.0.7/wtu_mlflow/
+-rw-r--r--   0 hbjs       (501) staff       (20)      153 2024-04-09 06:40:25.000000 wtu-mlflow-0.0.7/wtu_mlflow/__init__.py
+-rw-r--r--   0 hbjs       (501) staff       (20)     2523 2024-04-11 06:08:53.000000 wtu-mlflow-0.0.7/wtu_mlflow/base_mlflow_client.py
+-rw-r--r--   0 hbjs       (501) staff       (20)      559 2024-04-01 07:08:25.000000 wtu-mlflow-0.0.7/wtu_mlflow/env_checker.py
+-rw-r--r--   0 hbjs       (501) staff       (20)     3254 2024-04-11 06:10:10.000000 wtu-mlflow-0.0.7/wtu_mlflow/onnx_client.py
+-rw-r--r--   0 hbjs       (501) staff       (20)     3322 2024-04-11 06:09:39.000000 wtu-mlflow-0.0.7/wtu_mlflow/torch_client.py
+drwxr-xr-x   0 hbjs       (501) staff       (20)        0 2024-04-11 10:46:44.046164 wtu-mlflow-0.0.7/wtu_mlflow.egg-info/
+-rw-r--r--   0 hbjs       (501) staff       (20)     2177 2024-04-11 10:46:44.000000 wtu-mlflow-0.0.7/wtu_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 hbjs       (501) staff       (20)      322 2024-04-11 10:46:44.000000 wtu-mlflow-0.0.7/wtu_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 hbjs       (501) staff       (20)        1 2024-04-11 10:46:44.000000 wtu-mlflow-0.0.7/wtu_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 hbjs       (501) staff       (20)       73 2024-04-11 10:46:44.000000 wtu-mlflow-0.0.7/wtu_mlflow.egg-info/requires.txt
+-rw-r--r--   0 hbjs       (501) staff       (20)       11 2024-04-11 10:46:44.000000 wtu-mlflow-0.0.7/wtu_mlflow.egg-info/top_level.txt
```

### Comparing `wtu-mlflow-0.0.6/PKG-INFO` & `wtu-mlflow-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtu-mlflow
-Version: 0.0.6
+Version: 0.0.7
 Summary: W-Train Utils for MLflow
 Home-page: https://github.com/WIM-Corporation/w-train-utils-mlflow
 Author: hbjs
 Author-email: hbjs97@naver.com
 License: UNKNOWN
 Description: # wtrainclient
```

### Comparing `wtu-mlflow-0.0.6/README.md` & `wtu-mlflow-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wtu-mlflow-0.0.6/wtu_mlflow/base_mlflow_client.py` & `wtu-mlflow-0.0.7/wtu_mlflow/base_mlflow_client.py`

 * *Files identical despite different names*

### Comparing `wtu-mlflow-0.0.6/wtu_mlflow/env_checker.py` & `wtu-mlflow-0.0.7/wtu_mlflow/env_checker.py`

 * *Files identical despite different names*

### Comparing `wtu-mlflow-0.0.6/wtu_mlflow/onnx_client.py` & `wtu-mlflow-0.0.7/wtu_mlflow/onnx_client.py`

 * *Files identical despite different names*

### Comparing `wtu-mlflow-0.0.6/wtu_mlflow/torch_client.py` & `wtu-mlflow-0.0.7/wtu_mlflow/torch_client.py`

 * *Files identical despite different names*

### Comparing `wtu-mlflow-0.0.6/wtu_mlflow.egg-info/PKG-INFO` & `wtu-mlflow-0.0.7/wtu_mlflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtu-mlflow
-Version: 0.0.6
+Version: 0.0.7
 Summary: W-Train Utils for MLflow
 Home-page: https://github.com/WIM-Corporation/w-train-utils-mlflow
 Author: hbjs
 Author-email: hbjs97@naver.com
 License: UNKNOWN
 Description: # wtrainclient
```

