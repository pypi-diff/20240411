# Comparing `tmp/dagster-wandb-0.23.0.tar.gz` & `tmp/dagster-wandb-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.23.0.tar", last modified: Thu Apr  4 19:55:11 2024, max compression
+gzip compressed data, was "dagster-wandb-0.23.1.tar", last modified: Thu Apr 11 18:16:18 2024, max compression
```

## Comparing `dagster-wandb-0.23.0.tar` & `dagster-wandb-0.23.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      665 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      151 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.103917 dagster-wandb-0.23.0/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34086 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.107917 dagster-wandb-0.23.0/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5153 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2272 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      774 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/dagster_wandb/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2744 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/utils/errors.py
--rw-r--r--   0 root         (0) root         (0)     7890 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/utils/pickling.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.103917 dagster-wandb-0.23.0/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      665 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      607 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1359 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:18.022858 dagster-wandb-0.23.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-11 18:16:18.022858 dagster-wandb-0.23.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:18.014858 dagster-wandb-0.23.1/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34086 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:18.018858 dagster-wandb-0.23.1/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5153 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      774 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:18.022858 dagster-wandb-0.23.1/dagster_wandb/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/utils/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7890 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/utils/pickling.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:18.018858 dagster-wandb-0.23.1/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-11 18:16:17.000000 dagster-wandb-0.23.1/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      607 2024-04-11 18:16:17.000000 dagster-wandb-0.23.1/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:16:17.000000 dagster-wandb-0.23.1/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:16:17.000000 dagster-wandb-0.23.1/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 18:16:17.000000 dagster-wandb-0.23.1/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-11 18:16:17.000000 dagster-wandb-0.23.1/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-11 18:16:18.026858 dagster-wandb-0.23.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-11 18:04:20.000000 dagster-wandb-0.23.1/setup.py
```

### Comparing `dagster-wandb-0.23.0/LICENSE` & `dagster-wandb-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/PKG-INFO` & `dagster-wandb-0.23.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-wandb-0.23.0/dagster_wandb/__init__.py` & `dagster-wandb-0.23.1/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/io_manager.py` & `dagster-wandb-0.23.1/dagster_wandb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/launch/configs.py` & `dagster-wandb-0.23.1/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/launch/ops.py` & `dagster-wandb-0.23.1/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/resources.py` & `dagster-wandb-0.23.1/dagster_wandb/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/types.py` & `dagster-wandb-0.23.1/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/utils/errors.py` & `dagster-wandb-0.23.1/dagster_wandb/utils/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb/utils/pickling.py` & `dagster-wandb-0.23.1/dagster_wandb/utils/pickling.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.23.1/dagster_wandb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-wandb-0.23.0/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.23.1/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.23.0/setup.py` & `dagster-wandb-0.23.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.0",
+        "dagster==1.7.1",
         "wandb>=0.15.11,<1.0",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```
