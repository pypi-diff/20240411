# Comparing `tmp/diracx-client-0.0.1a8.tar.gz` & `tmp/diracx-client-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-client-0.0.1a8.tar", last modified: Thu Nov 30 08:40:00 2023, max compression
+gzip compressed data, was "diracx-client-0.0.1a9.tar", last modified: Sun Jan 28 09:11:48 2024, max compression
```

## Comparing `diracx-client-0.0.1a8.tar` & `diracx-client-0.0.1a9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.741257 diracx-client-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-11-30 08:40:00.741257 diracx-client-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:40:00.741257 diracx-client-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.733257 diracx-client-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.733257 diracx-client-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.733257 diracx-client-0.0.1a8/src/diracx/client/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    80974 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.737257 diracx-client-0.0.1a8/src/diracx/client/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.737257 diracx-client-0.0.1a8/src/diracx/client/aio/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81992 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/operations/_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/aio/operations/_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.737257 diracx-client-0.0.1a8/src/diracx/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/models/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    38365 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/models/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/models/_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.737257 diracx-client-0.0.1a8/src/diracx/client/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   103712 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/operations/_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/operations/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/src/diracx/client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.737257 diracx-client-0.0.1a8/src/diracx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-11-30 08:40:00.000000 diracx-client-0.0.1a8/src/diracx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-11-30 08:40:00.000000 diracx-client-0.0.1a8/src/diracx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:40:00.000000 diracx-client-0.0.1a8/src/diracx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-30 08:40:00.000000 diracx-client-0.0.1a8/src/diracx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:40:00.000000 diracx-client-0.0.1a8/src/diracx_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:00.737257 diracx-client-0.0.1a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-11-30 08:39:21.000000 diracx-client-0.0.1a8/tests/test_regenerate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.617078 diracx-client-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.617078 diracx-client-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.617078 diracx-client-0.0.1a9/src/diracx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80974 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/src/diracx/client/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/src/diracx/client/aio/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81992 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/operations/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/aio/operations/_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/src/diracx/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/models/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38365 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/models/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/models/_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/src/diracx/client/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103712 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/operations/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/operations/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/src/diracx/client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/src/diracx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-28 09:11:48.000000 diracx-client-0.0.1a9/src/diracx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-28 09:11:48.000000 diracx-client-0.0.1a9/src/diracx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:11:48.000000 diracx-client-0.0.1a9/src/diracx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-28 09:11:48.000000 diracx-client-0.0.1a9/src/diracx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:11:48.000000 diracx-client-0.0.1a9/src/diracx_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:48.621078 diracx-client-0.0.1a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-28 09:11:11.000000 diracx-client-0.0.1a9/tests/test_regenerate.py
```

### Comparing `diracx-client-0.0.1a8/PKG-INFO` & `diracx-client-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-client
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

### Comparing `diracx-client-0.0.1a8/pyproject.toml` & `diracx-client-0.0.1a9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -43,7 +43,10 @@
 addopts = [
     "-v",
     "--cov=diracx.client", "--cov-report=term-missing",
     "-pdiracx.testing",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

### Comparing `diracx-client-0.0.1a8/src/diracx/client/__init__.py` & `diracx-client-0.0.1a9/src/diracx/client/__init__.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/_client.py` & `diracx-client-0.0.1a9/src/diracx/client/_client.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/_configuration.py` & `diracx-client-0.0.1a9/src/diracx/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/_patch.py` & `diracx-client-0.0.1a9/src/diracx/client/_patch.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/_serialization.py` & `diracx-client-0.0.1a9/src/diracx/client/_serialization.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/_vendor.py` & `diracx-client-0.0.1a9/src/diracx/client/_vendor.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/__init__.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/_client.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/_configuration.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/_patch.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/_vendor.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/operations/__init__.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/operations/_operations.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/aio/operations/_patch.py` & `diracx-client-0.0.1a9/src/diracx/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/models/__init__.py` & `diracx-client-0.0.1a9/src/diracx/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/models/_enums.py` & `diracx-client-0.0.1a9/src/diracx/client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/models/_models.py` & `diracx-client-0.0.1a9/src/diracx/client/models/_models.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/models/_patch.py` & `diracx-client-0.0.1a9/src/diracx/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/operations/__init__.py` & `diracx-client-0.0.1a9/src/diracx/client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/operations/_operations.py` & `diracx-client-0.0.1a9/src/diracx/client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx/client/operations/_patch.py` & `diracx-client-0.0.1a9/src/diracx/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/src/diracx_client.egg-info/PKG-INFO` & `diracx-client-0.0.1a9/src/diracx_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-client
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

### Comparing `diracx-client-0.0.1a8/src/diracx_client.egg-info/SOURCES.txt` & `diracx-client-0.0.1a9/src/diracx_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diracx-client-0.0.1a8/tests/test_regenerate.py` & `diracx-client-0.0.1a9/tests/test_regenerate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import subprocess
 from pathlib import Path
 
 import git
+import pytest
 
 import diracx.client
 
+pytestmark = pytest.mark.enabled_dependencies([])
+# pytestmark = pytest.mark.enabled_dependencies(["ConfigSource", "AuthSettings"])
+
+
+@pytest.fixture
+def test_client(client_factory):
+    with client_factory.unauthenticated() as client:
+        yield client
+
 
 def test_regenerate_client(test_client, tmp_path):
     """Regenerate the AutoREST client and run pre-commit checks on it
 
     This test is skipped by default, and can be enabled by passing
     --regenerate-client to pytest. It is intended to be run manually
     when the API changes.
```

