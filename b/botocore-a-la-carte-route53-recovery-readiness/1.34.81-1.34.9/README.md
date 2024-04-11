# Comparing `tmp/botocore-a-la-carte-route53-recovery-readiness-1.34.81.tar.gz` & `tmp/botocore-a-la-carte-route53-recovery-readiness-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-route53-recovery-readiness-1.34.81.tar", last modified: Wed Apr 10 01:00:21 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-route53-recovery-readiness-1.34.9.tar", last modified: Thu Dec 28 01:07:02 2023, max compression
```

## Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81.tar` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:21.180378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 01:00:20.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-10 01:00:21.180378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:21.176378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:21.176378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:21.176378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:21.180378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/
--rw-r--r--   0 runner    (1001) docker     (127)    13806 2024-04-10 00:59:42.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-10 00:59:42.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   108052 2024-04-10 00:59:42.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:21.180378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-10 01:00:21.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-10 01:00:21.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:00:21.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 01:00:21.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:00:21.180378 botocore-a-la-carte-route53-recovery-readiness-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-10 01:00:20.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:02.018439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:07:01.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-28 01:07:02.018439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:02.014439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:02.014439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:02.014439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:02.018439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/
+-rw-r--r--   0 runner    (1001) docker     (127)    13806 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   108052 2023-12-28 01:06:26.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:02.018439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-28 01:07:01.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-12-28 01:07:01.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:07:01.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:07:01.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:07:02.018439 botocore-a-la-carte-route53-recovery-readiness-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-28 01:07:01.000000 botocore-a-la-carte-route53-recovery-readiness-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/LICENSE.txt` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/PKG-INFO` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53-recovery-readiness
-Version: 1.34.81
+Version: 1.34.9
 Summary: route53-recovery-readiness data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/paginators-1.json` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore/data/route53-recovery-readiness/2019-12-02/service-2.json` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore/data/route53-recovery-readiness/2019-12-02/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/PKG-INFO` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-route53-recovery-readiness
-Version: 1.34.81
+Version: 1.34.9
 Summary: route53-recovery-readiness data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/botocore_a_la_carte_route53_recovery_readiness.egg-info/SOURCES.txt` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/botocore_a_la_carte_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-route53-recovery-readiness-1.34.81/setup.py` & `botocore-a-la-carte-route53-recovery-readiness-1.34.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-route53-recovery-readiness',
-    version="1.34.81",
+    version="1.34.9",
     description='route53-recovery-readiness data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/route53-recovery-readiness/*/*.json'],
```

