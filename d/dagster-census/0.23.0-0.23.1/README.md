# Comparing `tmp/dagster-census-0.23.0.tar.gz` & `tmp/dagster-census-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-census-0.23.0.tar", last modified: Thu Apr  4 19:54:55 2024, max compression
+gzip compressed data, was "dagster-census-0.23.1.tar", last modified: Thu Apr 11 18:18:27 2024, max compression
```

## Comparing `dagster-census-0.23.0.tar` & `dagster-census-0.23.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:55.411813 dagster-census-0.23.0/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-census-0.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-04 19:44:08.000000 dagster-census-0.23.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      705 2024-04-04 19:54:55.411813 dagster-census-0.23.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:55.407813 dagster-census-0.23.0/dagster_census/
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-04 19:44:08.000000 dagster-census-0.23.0/dagster_census/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3551 2024-04-04 19:44:08.000000 dagster-census-0.23.0/dagster_census/ops.py
--rw-r--r--   0 root         (0) root         (0)    10798 2024-04-04 19:44:08.000000 dagster-census-0.23.0/dagster_census/resources.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-04-04 19:44:08.000000 dagster-census-0.23.0/dagster_census/types.py
--rw-r--r--   0 root         (0) root         (0)     1325 2024-04-04 19:44:08.000000 dagster-census-0.23.0/dagster_census/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-census-0.23.0/dagster_census/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:55.407813 dagster-census-0.23.0/dagster_census.egg-info/
--rw-r--r--   0 root         (0) root         (0)      705 2024-04-04 19:54:55.000000 dagster-census-0.23.0/dagster_census.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2024-04-04 19:54:55.000000 dagster-census-0.23.0/dagster_census.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:55.000000 dagster-census-0.23.0/dagster_census.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:55.000000 dagster-census-0.23.0/dagster_census.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-04 19:54:55.000000 dagster-census-0.23.0/dagster_census.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-04 19:54:55.000000 dagster-census-0.23.0/dagster_census.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-04 19:54:55.411813 dagster-census-0.23.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1291 2024-04-04 19:44:08.000000 dagster-census-0.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:27.943721 dagster-census-0.23.1/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-census-0.23.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-11 18:04:20.000000 dagster-census-0.23.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-11 18:18:27.943721 dagster-census-0.23.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:27.939721 dagster-census-0.23.1/dagster_census/
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-11 18:04:20.000000 dagster-census-0.23.1/dagster_census/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2024-04-11 18:04:20.000000 dagster-census-0.23.1/dagster_census/ops.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2024-04-11 18:04:20.000000 dagster-census-0.23.1/dagster_census/resources.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-11 18:04:20.000000 dagster-census-0.23.1/dagster_census/types.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-04-11 18:04:20.000000 dagster-census-0.23.1/dagster_census/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-census-0.23.1/dagster_census/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:27.943721 dagster-census-0.23.1/dagster_census.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-11 18:18:27.000000 dagster-census-0.23.1/dagster_census.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2024-04-11 18:18:27.000000 dagster-census-0.23.1/dagster_census.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:18:27.000000 dagster-census-0.23.1/dagster_census.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:18:27.000000 dagster-census-0.23.1/dagster_census.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-11 18:18:27.000000 dagster-census-0.23.1/dagster_census.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-11 18:18:27.000000 dagster-census-0.23.1/dagster_census.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-11 18:18:27.943721 dagster-census-0.23.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-04-11 18:04:20.000000 dagster-census-0.23.1/setup.py
```

### Comparing `dagster-census-0.23.0/LICENSE` & `dagster-census-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.0/PKG-INFO` & `dagster-census-0.23.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.23.0/dagster_census/ops.py` & `dagster-census-0.23.1/dagster_census/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.0/dagster_census/resources.py` & `dagster-census-0.23.1/dagster_census/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.0/dagster_census/types.py` & `dagster-census-0.23.1/dagster_census/types.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.0/dagster_census/utils.py` & `dagster-census-0.23.1/dagster_census/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-census-0.23.0/dagster_census.egg-info/PKG-INFO` & `dagster-census-0.23.1/dagster_census.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-census
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for integrating Census with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-census
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-census-0.23.0/setup.py` & `dagster-census-0.23.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_census_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.0"],
+    install_requires=["dagster==1.7.1"],
     zip_safe=False,
 )
```

