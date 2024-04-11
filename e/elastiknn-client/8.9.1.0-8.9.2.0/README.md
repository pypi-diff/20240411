# Comparing `tmp/elastiknn-client-8.9.1.0.tar.gz` & `tmp/elastiknn-client-8.9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastiknn-client-8.9.1.0.tar", last modified: Mon Nov  6 22:51:45 2023, max compression
+gzip compressed data, was "elastiknn-client-8.9.2.0.tar", last modified: Tue Nov  7 00:39:05 2023, max compression
```

## Comparing `elastiknn-client-8.9.1.0.tar` & `elastiknn-client-8.9.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 22:51:45.077112 elastiknn-client-8.9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-11-06 22:51:45.077112 elastiknn-client-8.9.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 22:51:45.073112 elastiknn-client-8.9.1.0/elastiknn/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/elastiknn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/elastiknn/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/elastiknn/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/elastiknn/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/elastiknn/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/elastiknn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 22:51:45.073112 elastiknn-client-8.9.1.0/elastiknn_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-11-06 22:51:45.000000 elastiknn-client-8.9.1.0/elastiknn_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-06 22:51:45.000000 elastiknn-client-8.9.1.0/elastiknn_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 22:51:45.000000 elastiknn-client-8.9.1.0/elastiknn_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-06 22:51:45.000000 elastiknn-client-8.9.1.0/elastiknn_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-06 22:51:45.000000 elastiknn-client-8.9.1.0/elastiknn_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 22:51:45.077112 elastiknn-client-8.9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 22:51:45.073112 elastiknn-client-8.9.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-11-06 22:51:17.000000 elastiknn-client-8.9.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:39:05.499041 elastiknn-client-8.9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-11-07 00:39:05.499041 elastiknn-client-8.9.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:39:05.499041 elastiknn-client-8.9.2.0/elastiknn/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/elastiknn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/elastiknn/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/elastiknn/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/elastiknn/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/elastiknn/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/elastiknn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:39:05.499041 elastiknn-client-8.9.2.0/elastiknn_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-11-07 00:39:05.000000 elastiknn-client-8.9.2.0/elastiknn_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-07 00:39:05.000000 elastiknn-client-8.9.2.0/elastiknn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 00:39:05.000000 elastiknn-client-8.9.2.0/elastiknn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-07 00:39:05.000000 elastiknn-client-8.9.2.0/elastiknn_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-07 00:39:05.000000 elastiknn-client-8.9.2.0/elastiknn_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 00:39:05.499041 elastiknn-client-8.9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:39:05.499041 elastiknn-client-8.9.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-11-07 00:38:26.000000 elastiknn-client-8.9.2.0/tests/test_utils.py
```

### Comparing `elastiknn-client-8.9.1.0/PKG-INFO` & `elastiknn-client-8.9.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastiknn-client
-Version: 8.9.1.0
+Version: 8.9.2.0
 Summary: Python client for the ElastiKnn Elasticsearch plugin
 Home-page: https://github.com/alexklibisz/elastiknn
 Author: Alex Klibisz
 Author-email: aklibisz@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==8.9.0
 Requires-Dist: dataclasses-json==0.3.7
```

### Comparing `elastiknn-client-8.9.1.0/elastiknn/api.py` & `elastiknn-client-8.9.2.0/elastiknn/api.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/elastiknn/client.py` & `elastiknn-client-8.9.2.0/elastiknn/client.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/elastiknn/models.py` & `elastiknn-client-8.9.2.0/elastiknn/models.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/elastiknn/utils.py` & `elastiknn-client-8.9.2.0/elastiknn/utils.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/elastiknn_client.egg-info/PKG-INFO` & `elastiknn-client-8.9.2.0/elastiknn_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastiknn-client
-Version: 8.9.1.0
+Version: 8.9.2.0
 Summary: Python client for the ElastiKnn Elasticsearch plugin
 Home-page: https://github.com/alexklibisz/elastiknn
 Author: Alex Klibisz
 Author-email: aklibisz@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==8.9.0
 Requires-Dist: dataclasses-json==0.3.7
```

### Comparing `elastiknn-client-8.9.1.0/setup.py` & `elastiknn-client-8.9.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/tests/test_client.py` & `elastiknn-client-8.9.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/tests/test_model.py` & `elastiknn-client-8.9.2.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `elastiknn-client-8.9.1.0/tests/test_utils.py` & `elastiknn-client-8.9.2.0/tests/test_utils.py`

 * *Files identical despite different names*

