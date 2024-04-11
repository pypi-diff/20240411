# Comparing `tmp/dtcv2_util-0.1.2.tar.gz` & `tmp/dtcv2_util-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtcv2_util-0.1.2.tar", last modified: Thu Mar 21 14:18:41 2024, max compression
+gzip compressed data, was "dtcv2_util-0.1.3.tar", last modified: Thu Apr 11 09:16:36 2024, max compression
```

## Comparing `dtcv2_util-0.1.2.tar` & `dtcv2_util-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 14:18:41.740350 dtcv2_util-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1897 2024-03-21 14:18:41.740350 dtcv2_util-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1588 2024-03-20 14:52:59.000000 dtcv2_util-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 14:18:41.736350 dtcv2_util-0.1.2/dtcv2_util/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-20 14:52:59.000000 dtcv2_util-0.1.2/dtcv2_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-03-20 14:52:59.000000 dtcv2_util-0.1.2/dtcv2_util/log_management.py
--rw-rw-rw-   0 root         (0) root         (0)    20362 2024-03-20 14:52:59.000000 dtcv2_util-0.1.2/dtcv2_util/meteo_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9602 2024-03-20 14:52:59.000000 dtcv2_util-0.1.2/dtcv2_util/validate_inp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 14:18:41.740350 dtcv2_util-0.1.2/dtcv2_util.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1897 2024-03-21 14:18:41.000000 dtcv2_util-0.1.2/dtcv2_util.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2024-03-21 14:18:41.000000 dtcv2_util-0.1.2/dtcv2_util.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 14:18:41.000000 dtcv2_util-0.1.2/dtcv2_util.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-21 14:18:41.000000 dtcv2_util-0.1.2/dtcv2_util.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-21 14:18:41.000000 dtcv2_util-0.1.2/dtcv2_util.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-21 14:18:41.740350 dtcv2_util-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-03-21 14:18:30.000000 dtcv2_util-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:16:36.057982 dtcv2_util-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-04-11 09:16:36.057982 dtcv2_util-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:16:36.053982 dtcv2_util-0.1.3/dtcv2_util/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/log_management.py
+-rw-rw-rw-   0 root         (0) root         (0)    20362 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/meteo_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9602 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/validate_inp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:16:36.053982 dtcv2_util-0.1.3/dtcv2_util.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-11 09:16:36.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 09:16:36.057982 dtcv2_util-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-11 09:16:25.000000 dtcv2_util-0.1.3/setup.py
```

### Comparing `dtcv2_util-0.1.2/PKG-INFO` & `dtcv2_util-0.1.3/dtcv2_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dtcv2_util
-Version: 0.1.2
+Name: dtcv2-util
+Version: 0.1.3
 Summary: Library for workflow management
 Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
 Author: Alejandra Guerrero - DTGEO
 Author-email: aguerrero@geo3bcn.csic.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dtcv2_util-0.1.2/README.md` & `dtcv2_util-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.2/dtcv2_util/log_management.py` & `dtcv2_util-0.1.3/dtcv2_util/log_management.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.2/dtcv2_util/meteo_utils.py` & `dtcv2_util-0.1.3/dtcv2_util/meteo_utils.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.2/dtcv2_util/validate_inp.py` & `dtcv2_util-0.1.3/dtcv2_util/validate_inp.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.2/dtcv2_util.egg-info/PKG-INFO` & `dtcv2_util-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dtcv2-util
-Version: 0.1.2
+Name: dtcv2_util
+Version: 0.1.3
 Summary: Library for workflow management
 Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
 Author: Alejandra Guerrero - DTGEO
 Author-email: aguerrero@geo3bcn.csic.es
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dtcv2_util-0.1.2/setup.py` & `dtcv2_util-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.2' #First version 
+VERSION = '0.1.3' #First version 
 PACKAGE_NAME = 'dtcv2_util' #For DTGEO general 
 AUTHOR = 'Alejandra Guerrero - DTGEO' 
 AUTHOR_EMAIL = 'aguerrero@geo3bcn.csic.es' 
 URL = 'https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs' 
 LICENSE = 'MIT' 
 DESCRIPTION = 'Library for workflow management' #DTC-V2
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
```

