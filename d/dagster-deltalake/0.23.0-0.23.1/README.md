# Comparing `tmp/dagster-deltalake-0.23.0.tar.gz` & `tmp/dagster-deltalake-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-0.23.0.tar", last modified: Thu Apr  4 19:51:36 2024, max compression
+gzip compressed data, was "dagster-deltalake-0.23.1.tar", last modified: Thu Apr 11 18:11:29 2024, max compression
```

## Comparing `dagster-deltalake-0.23.0.tar` & `dagster-deltalake-0.23.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      707 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/dagster_deltalake/
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6650 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/config.py
--rw-r--r--   0 root         (0) root         (0)     9940 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/handler.py
--rw-r--r--   0 root         (0) root         (0)     9439 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/py.typed
--rw-r--r--   0 root         (0) root         (0)     1694 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/
--rw-r--r--   0 root         (0) root         (0)      707 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1408 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:11:29.504929 dagster-deltalake-0.23.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-11 18:11:29.504929 dagster-deltalake-0.23.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:11:29.500929 dagster-deltalake-0.23.1/dagster_deltalake/
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6650 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/config.py
+-rw-r--r--   0 root         (0) root         (0)     9940 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/handler.py
+-rw-r--r--   0 root         (0) root         (0)     9439 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1694 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/dagster_deltalake/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:11:29.504929 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-11 18:11:29.000000 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-11 18:11:29.000000 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:11:29.000000 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:11:29.000000 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-11 18:11:29.000000 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-11 18:11:29.000000 dagster-deltalake-0.23.1/dagster_deltalake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-11 18:11:29.504929 dagster-deltalake-0.23.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-11 18:04:20.000000 dagster-deltalake-0.23.1/setup.py
```

### Comparing `dagster-deltalake-0.23.0/LICENSE` & `dagster-deltalake-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.0/PKG-INFO` & `dagster-deltalake-0.23.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for Deltalake-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-0.23.0/dagster_deltalake/__init__.py` & `dagster-deltalake-0.23.1/dagster_deltalake/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.0/dagster_deltalake/config.py` & `dagster-deltalake-0.23.1/dagster_deltalake/config.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.0/dagster_deltalake/handler.py` & `dagster-deltalake-0.23.1/dagster_deltalake/handler.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.0/dagster_deltalake/io_manager.py` & `dagster-deltalake-0.23.1/dagster_deltalake/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.0/dagster_deltalake/resource.py` & `dagster-deltalake-0.23.1/dagster_deltalake/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.23.0/dagster_deltalake.egg-info/PKG-INFO` & `dagster-deltalake-0.23.1/dagster_deltalake.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for Deltalake-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-0.23.0/setup.py` & `dagster-deltalake-0.23.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "deltalake>=0.15",
-        "dagster==1.7.0",
+        "dagster==1.7.1",
     ],
     extras_require={
         "pandas": ["pandas"],
     },
     zip_safe=False,
 )
```

