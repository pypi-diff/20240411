# Comparing `tmp/botocore-a-la-carte-forecastquery-1.34.81.tar.gz` & `tmp/botocore-a-la-carte-forecastquery-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-forecastquery-1.34.81.tar", last modified: Wed Apr 10 00:59:58 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-forecastquery-1.34.9.tar", last modified: Thu Dec 28 01:06:48 2023, max compression
```

## Comparing `botocore-a-la-carte-forecastquery-1.34.81.tar` & `botocore-a-la-carte-forecastquery-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:59:58.692214 botocore-a-la-carte-forecastquery-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 00:59:58.000000 botocore-a-la-carte-forecastquery-1.34.81/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 00:59:58.692214 botocore-a-la-carte-forecastquery-1.34.81/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:59:58.688214 botocore-a-la-carte-forecastquery-1.34.81/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:59:58.688214 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:59:58.688214 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:59:58.692214 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/
--rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-10 00:59:41.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 00:59:41.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 00:59:41.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-10 00:59:41.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:59:58.692214 botocore-a-la-carte-forecastquery-1.34.81/botocore_a_la_carte_forecastquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 00:59:58.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore_a_la_carte_forecastquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-10 00:59:58.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore_a_la_carte_forecastquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:59:58.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore_a_la_carte_forecastquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 00:59:58.000000 botocore-a-la-carte-forecastquery-1.34.81/botocore_a_la_carte_forecastquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:59:58.692214 botocore-a-la-carte-forecastquery-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-10 00:59:58.000000 botocore-a-la-carte-forecastquery-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:48.190329 botocore-a-la-carte-forecastquery-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:47.000000 botocore-a-la-carte-forecastquery-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-28 01:06:48.190329 botocore-a-la-carte-forecastquery-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:48.186329 botocore-a-la-carte-forecastquery-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:48.186329 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:48.186329 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:48.186329 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2023-12-28 01:06:26.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2023-12-28 01:06:26.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:48.190329 botocore-a-la-carte-forecastquery-1.34.9/botocore_a_la_carte_forecastquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-28 01:06:48.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore_a_la_carte_forecastquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-28 01:06:48.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore_a_la_carte_forecastquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:48.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore_a_la_carte_forecastquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:48.000000 botocore-a-la-carte-forecastquery-1.34.9/botocore_a_la_carte_forecastquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:48.190329 botocore-a-la-carte-forecastquery-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-28 01:06:47.000000 botocore-a-la-carte-forecastquery-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-forecastquery-1.34.81/LICENSE.txt` & `botocore-a-la-carte-forecastquery-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecastquery-1.34.81/PKG-INFO` & `botocore-a-la-carte-forecastquery-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-forecastquery
-Version: 1.34.81
+Version: 1.34.9
 Summary: forecastquery data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/endpoint-rule-set-1.json` & `botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecastquery-1.34.81/botocore/data/forecastquery/2018-06-26/service-2.json` & `botocore-a-la-carte-forecastquery-1.34.9/botocore/data/forecastquery/2018-06-26/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-forecastquery-1.34.81/botocore_a_la_carte_forecastquery.egg-info/PKG-INFO` & `botocore-a-la-carte-forecastquery-1.34.9/botocore_a_la_carte_forecastquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-forecastquery
-Version: 1.34.81
+Version: 1.34.9
 Summary: forecastquery data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-forecastquery-1.34.81/setup.py` & `botocore-a-la-carte-forecastquery-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-forecastquery',
-    version="1.34.81",
+    version="1.34.9",
     description='forecastquery data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/forecastquery/*/*.json'],
```

