# Comparing `tmp/botocore-a-la-carte-devicefarm-1.34.81.tar.gz` & `tmp/botocore-a-la-carte-devicefarm-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-devicefarm-1.34.81.tar", last modified: Wed Apr 10 01:00:01 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-devicefarm-1.34.9.tar", last modified: Thu Dec 28 01:06:42 2023, max compression
```

## Comparing `botocore-a-la-carte-devicefarm-1.34.81.tar` & `botocore-a-la-carte-devicefarm-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 01:00:01.000000 botocore-a-la-carte-devicefarm-1.34.81/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:01.352233 botocore-a-la-carte-devicefarm-1.34.81/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/
--rw-r--r--   0 runner    (1001) docker     (127)    13742 2024-04-10 00:59:41.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-10 00:59:41.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-10 00:59:41.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   238621 2024-04-10 00:59:41.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/botocore_a_la_carte_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 01:00:01.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore_a_la_carte_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 01:00:01.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore_a_la_carte_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:00:01.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore_a_la_carte_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 01:00:01.000000 botocore-a-la-carte-devicefarm-1.34.81/botocore_a_la_carte_devicefarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:00:01.356233 botocore-a-la-carte-devicefarm-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-10 01:00:01.000000 botocore-a-la-carte-devicefarm-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:42.000000 botocore-a-la-carte-devicefarm-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/
+-rw-r--r--   0 runner    (1001) docker     (127)    13742 2023-12-28 01:06:26.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42721 2023-12-28 01:06:26.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-12-28 01:06:26.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   238621 2023-12-28 01:06:26.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/botocore_a_la_carte_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-28 01:06:42.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore_a_la_carte_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-28 01:06:42.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore_a_la_carte_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:42.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore_a_la_carte_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:42.000000 botocore-a-la-carte-devicefarm-1.34.9/botocore_a_la_carte_devicefarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:42.790287 botocore-a-la-carte-devicefarm-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-28 01:06:42.000000 botocore-a-la-carte-devicefarm-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/LICENSE.txt` & `botocore-a-la-carte-devicefarm-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/PKG-INFO` & `botocore-a-la-carte-devicefarm-1.34.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-devicefarm
-Version: 1.34.81
+Version: 1.34.9
 Summary: devicefarm data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/endpoint-rule-set-1.json` & `botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/examples-1.json` & `botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/paginators-1.json` & `botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/botocore/data/devicefarm/2015-06-23/service-2.json` & `botocore-a-la-carte-devicefarm-1.34.9/botocore/data/devicefarm/2015-06-23/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/botocore_a_la_carte_devicefarm.egg-info/PKG-INFO` & `botocore-a-la-carte-devicefarm-1.34.9/botocore_a_la_carte_devicefarm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-devicefarm
-Version: 1.34.81
+Version: 1.34.9
 Summary: devicefarm data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-devicefarm-1.34.81/setup.py` & `botocore-a-la-carte-devicefarm-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-devicefarm',
-    version="1.34.81",
+    version="1.34.9",
     description='devicefarm data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/devicefarm/*/*.json'],
```

