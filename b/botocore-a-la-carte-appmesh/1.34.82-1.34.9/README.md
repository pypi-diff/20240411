# Comparing `tmp/botocore-a-la-carte-appmesh-1.34.82.tar.gz` & `tmp/botocore-a-la-carte-appmesh-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-appmesh-1.34.82.tar", last modified: Thu Apr 11 01:00:46 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-appmesh-1.34.9.tar", last modified: Thu Dec 28 01:06:40 2023, max compression
```

## Comparing `botocore-a-la-carte-appmesh-1.34.82.tar` & `botocore-a-la-carte-appmesh-1.34.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.232757 botocore-a-la-carte-appmesh-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 01:00:45.000000 botocore-a-la-carte-appmesh-1.34.82/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 01:00:46.232757 botocore-a-la-carte-appmesh-1.34.82/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.228757 botocore-a-la-carte-appmesh-1.34.82/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.228757 botocore-a-la-carte-appmesh-1.34.82/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.228757 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.228757 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/
--rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    73589 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.228757 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   239752 2024-04-11 01:00:33.000000 botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:46.232757 botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 01:00:46.000000 botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 01:00:46.000000 botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:46.000000 botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 01:00:46.000000 botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:00:46.232757 botocore-a-la-carte-appmesh-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 01:00:45.000000 botocore-a-la-carte-appmesh-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:40.000000 botocore-a-la-carte-appmesh-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    17628 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    73589 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   239752 2023-12-28 01:06:26.000000 botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-28 01:06:40.000000 botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-28 01:06:40.000000 botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:40.000000 botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:40.000000 botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:40.458269 botocore-a-la-carte-appmesh-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-28 01:06:40.000000 botocore-a-la-carte-appmesh-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-appmesh-1.34.82/LICENSE.txt` & `botocore-a-la-carte-appmesh-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/PKG-INFO` & `botocore-a-la-carte-appmesh-1.34.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appmesh
-Version: 1.34.82
+Version: 1.34.9
 Summary: appmesh data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/paginators-1.json` & `botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2018-10-01/service-2.json` & `botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2018-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/paginators-1.json` & `botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore/data/appmesh/2019-01-25/service-2.json` & `botocore-a-la-carte-appmesh-1.34.9/botocore/data/appmesh/2019-01-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/PKG-INFO` & `botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-appmesh
-Version: 1.34.82
+Version: 1.34.9
 Summary: appmesh data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-appmesh-1.34.82/botocore_a_la_carte_appmesh.egg-info/SOURCES.txt` & `botocore-a-la-carte-appmesh-1.34.9/botocore_a_la_carte_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-appmesh-1.34.82/setup.py` & `botocore-a-la-carte-appmesh-1.34.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-appmesh',
-    version="1.34.82",
+    version="1.34.9",
     description='appmesh data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/appmesh/*/*.json'],
```

