# Comparing `tmp/roktools-6.0.0.tar.gz` & `tmp/roktools-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.0.0.tar", max compression
+gzip compressed data, was "roktools-6.0.1.tar", max compression
```

## Comparing `roktools-6.0.0.tar` & `roktools-6.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-11 08:26:15.718863 roktools-6.0.0/LICENSE
--rw-r--r--   0        0        0     1485 2024-04-11 08:26:15.718863 roktools-6.0.0/README.md
--rw-r--r--   0        0        0     1162 2024-04-11 08:26:15.718863 roktools-6.0.0/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/decorator.py
--rw-r--r--   0        0        0      927 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/file.py
--rw-r--r--   0        0        0    33609 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-04-11 08:26:15.758862 roktools-6.0.0/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1878 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9505 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-04-11 08:26:15.762862 roktools-6.0.0/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5898 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-04-11 08:26:15.762862 roktools-6.0.0/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    29707 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/rinex.py
--rwxr-xr-x   0        0        0     1083 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/tensorial.py
--rw-r--r--   0        0        0    11293 2024-04-11 08:26:15.718863 roktools-6.0.0/roktools/time.py
--rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 roktools-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-11 08:36:41.085389 roktools-6.0.1/LICENSE
+-rw-r--r--   0        0        0     1480 2024-04-11 08:36:41.085389 roktools-6.0.1/README.md
+-rw-r--r--   0        0        0     1162 2024-04-11 08:36:41.085389 roktools-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/decorator.py
+-rw-r--r--   0        0        0      927 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/file.py
+-rw-r--r--   0        0        0    33609 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:36:41.125389 roktools-6.0.1/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1878 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9505 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:36:41.125389 roktools-6.0.1/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5898 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:36:41.125389 roktools-6.0.1/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-04-11 08:36:41.085389 roktools-6.0.1/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    29707 2024-04-11 08:36:41.089389 roktools-6.0.1/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1083 2024-04-11 08:36:41.089389 roktools-6.0.1/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-04-11 08:36:41.089389 roktools-6.0.1/roktools/tensorial.py
+-rw-r--r--   0        0        0    11293 2024-04-11 08:36:41.089389 roktools-6.0.1/roktools/time.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 roktools-6.0.1/PKG-INFO
```

### Comparing `roktools-6.0.0/LICENSE` & `roktools-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/README.md` & `roktools-6.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Python tools used in internal Rokubun projects. This repository contains the following modules:
 
 - `logger`, a module that extends basic Python logging
 - `geodetic`, to perform basic geodetic transformation (Cartesian to Geodetic,
   Cartesian to Local Tangential Plane, ...)
 
-
 ## Installation
 
 pip install roktools
 
 ## Modules
 
 ### Logger
@@ -40,8 +39,8 @@
 ```
 
 
 ## Deployment to PyPi
 
 The project is published automatically using internal Gitlab CI on each commit to master to PyPi repository [roktools](https://pypi.org/project/roktools/)
 
-    
+
```

### Comparing `roktools-6.0.0/pyproject.toml` & `roktools-6.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.0.0"
+version = "6.0.1"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.0.0/roktools/cl.py` & `roktools-6.0.1/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/file.py` & `roktools-6.0.1/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/geodetic.py` & `roktools-6.0.1/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/gnss/edit.py` & `roktools-6.0.1/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/gnss/observables.py` & `roktools-6.0.1/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/gnss/residuals.py` & `roktools-6.0.1/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/gnss/types.py` & `roktools-6.0.1/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/logger.py` & `roktools-6.0.1/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/orbit/kepler.py` & `roktools-6.0.1/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/orbit/tle.py` & `roktools-6.0.1/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/parsers/rtklib/stats.py` & `roktools-6.0.1/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/rinex.py` & `roktools-6.0.1/roktools/rinex.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/stats.py` & `roktools-6.0.1/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/tensorial.py` & `roktools-6.0.1/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/roktools/time.py` & `roktools-6.0.1/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.0/PKG-INFO` & `roktools-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.0.0
+Version: 6.0.1
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -17,15 +17,14 @@
 
 Python tools used in internal Rokubun projects. This repository contains the following modules:
 
 - `logger`, a module that extends basic Python logging
 - `geodetic`, to perform basic geodetic transformation (Cartesian to Geodetic,
   Cartesian to Local Tangential Plane, ...)
 
-
 ## Installation
 
 pip install roktools
 
 ## Modules
 
 ### Logger
@@ -55,9 +54,9 @@
 ```
 
 
 ## Deployment to PyPi
 
 The project is published automatically using internal Gitlab CI on each commit to master to PyPi repository [roktools](https://pypi.org/project/roktools/)
 
-    
+
```

