# Comparing `tmp/botocore-a-la-carte-xray-1.34.81.tar.gz` & `tmp/botocore-a-la-carte-xray-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-xray-1.34.81.tar", last modified: Wed Apr 10 01:00:23 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-xray-1.34.9.tar", last modified: Thu Dec 28 01:07:03 2023, max compression
```

## Comparing `botocore-a-la-carte-xray-1.34.81.tar` & `botocore-a-la-carte-xray-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 01:00:22.000000 botocore-a-la-carte-xray-1.34.81/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/botocore/data/xray/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-10 00:59:42.000000 botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 00:59:42.000000 botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-10 00:59:42.000000 botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   122388 2024-04-10 00:59:42.000000 botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/botocore_a_la_carte_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-10 01:00:23.000000 botocore-a-la-carte-xray-1.34.81/botocore_a_la_carte_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-10 01:00:23.000000 botocore-a-la-carte-xray-1.34.81/botocore_a_la_carte_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:00:23.000000 botocore-a-la-carte-xray-1.34.81/botocore_a_la_carte_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 01:00:23.000000 botocore-a-la-carte-xray-1.34.81/botocore_a_la_carte_xray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:00:23.056389 botocore-a-la-carte-xray-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-10 01:00:22.000000 botocore-a-la-carte-xray-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:03.746452 botocore-a-la-carte-xray-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:07:03.000000 botocore-a-la-carte-xray-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-28 01:07:03.742452 botocore-a-la-carte-xray-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:03.742452 botocore-a-la-carte-xray-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:03.742452 botocore-a-la-carte-xray-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:03.742452 botocore-a-la-carte-xray-1.34.9/botocore/data/xray/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:03.742452 botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2023-12-28 01:06:26.000000 botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-12-28 01:06:26.000000 botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   122388 2023-12-28 01:06:26.000000 botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:03.742452 botocore-a-la-carte-xray-1.34.9/botocore_a_la_carte_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-28 01:07:03.000000 botocore-a-la-carte-xray-1.34.9/botocore_a_la_carte_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-28 01:07:03.000000 botocore-a-la-carte-xray-1.34.9/botocore_a_la_carte_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:07:03.000000 botocore-a-la-carte-xray-1.34.9/botocore_a_la_carte_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:07:03.000000 botocore-a-la-carte-xray-1.34.9/botocore_a_la_carte_xray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:07:03.746452 botocore-a-la-carte-xray-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-28 01:07:03.000000 botocore-a-la-carte-xray-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-xray-1.34.81/LICENSE.txt` & `botocore-a-la-carte-xray-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-xray-1.34.81/PKG-INFO` & `botocore-a-la-carte-xray-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-xray
-Version: 1.34.81
+Version: 1.34.9
 Summary: xray data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/endpoint-rule-set-1.json` & `botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/paginators-1.json` & `botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-xray-1.34.81/botocore/data/xray/2016-04-12/service-2.json` & `botocore-a-la-carte-xray-1.34.9/botocore/data/xray/2016-04-12/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-xray-1.34.81/botocore_a_la_carte_xray.egg-info/PKG-INFO` & `botocore-a-la-carte-xray-1.34.9/botocore_a_la_carte_xray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-xray
-Version: 1.34.81
+Version: 1.34.9
 Summary: xray data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-xray-1.34.81/setup.py` & `botocore-a-la-carte-xray-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-xray',
-    version="1.34.81",
+    version="1.34.9",
     description='xray data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/xray/*/*.json'],
```

