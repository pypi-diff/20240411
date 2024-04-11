# Comparing `tmp/diracx-api-0.0.1a8.tar.gz` & `tmp/diracx-api-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-api-0.0.1a8.tar", last modified: Thu Nov 30 08:39:35 2023, max compression
+gzip compressed data, was "diracx-api-0.0.1a9.tar", last modified: Sun Jan 28 09:11:23 2024, max compression
```

## Comparing `diracx-api-0.0.1a8.tar` & `diracx-api-0.0.1a9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:35.444975 diracx-api-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-11-30 08:39:35.444975 diracx-api-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:39:35.444975 diracx-api-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:35.440975 diracx-api-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:35.440975 diracx-api-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:35.440975 diracx-api-0.0.1a8/src/diracx/api/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/src/diracx/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/src/diracx/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/src/diracx/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/src/diracx/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:35.440975 diracx-api-0.0.1a8/src/diracx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-11-30 08:39:35.000000 diracx-api-0.0.1a8/src/diracx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-11-30 08:39:35.000000 diracx-api-0.0.1a8/src/diracx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:39:35.000000 diracx-api-0.0.1a8/src/diracx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-30 08:39:35.000000 diracx-api-0.0.1a8/src/diracx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:39:35.000000 diracx-api-0.0.1a8/src/diracx_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:35.440975 diracx-api-0.0.1a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-11-30 08:39:21.000000 diracx-api-0.0.1a8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:23.753151 diracx-api-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-28 09:11:23.753151 diracx-api-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:11:23.753151 diracx-api-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:23.749151 diracx-api-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:23.749151 diracx-api-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:23.749151 diracx-api-0.0.1a9/src/diracx/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/src/diracx/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/src/diracx/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/src/diracx/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/src/diracx/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:23.753151 diracx-api-0.0.1a9/src/diracx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-28 09:11:23.000000 diracx-api-0.0.1a9/src/diracx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-28 09:11:23.000000 diracx-api-0.0.1a9/src/diracx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:11:23.000000 diracx-api-0.0.1a9/src/diracx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-28 09:11:23.000000 diracx-api-0.0.1a9/src/diracx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:11:23.000000 diracx-api-0.0.1a9/src/diracx_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:23.753151 diracx-api-0.0.1a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-01-28 09:11:11.000000 diracx-api-0.0.1a9/tests/test_utils.py
```

### Comparing `diracx-api-0.0.1a8/PKG-INFO` & `diracx-api-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-api
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-api-0.0.1a8/pyproject.toml` & `diracx-api-0.0.1a9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -39,7 +39,10 @@
 addopts = [
     "-v",
     "--cov=diracx.api", "--cov-report=term-missing",
     "-pdiracx.testing",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

### Comparing `diracx-api-0.0.1a8/src/diracx/api/jobs.py` & `diracx-api-0.0.1a9/src/diracx/api/jobs.py`

 * *Files identical despite different names*

### Comparing `diracx-api-0.0.1a8/src/diracx/api/utils.py` & `diracx-api-0.0.1a9/src/diracx/api/utils.py`

 * *Files identical despite different names*

### Comparing `diracx-api-0.0.1a8/src/diracx_api.egg-info/PKG-INFO` & `diracx-api-0.0.1a9/src/diracx_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-api
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-api-0.0.1a8/tests/test_jobs.py` & `diracx-api-0.0.1a9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `diracx-api-0.0.1a8/tests/test_utils.py` & `diracx-api-0.0.1a9/tests/test_utils.py`

 * *Files identical despite different names*

