# Comparing `tmp/lsst-resources-26.2024.400.tar.gz` & `tmp/lsst-resources-26.2024.500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-resources-26.2024.400.tar", last modified: Thu Jan 25 10:34:54 2024, max compression
+gzip compressed data, was "lsst-resources-26.2024.500.tar", last modified: Thu Feb  1 10:58:10 2024, max compression
```

## Comparing `lsst-resources-26.2024.400.tar` & `lsst-resources-26.2024.500.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.562063 lsst-resources-26.2024.400/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-01-25 10:34:54.562063 lsst-resources-26.2024.400/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.554063 lsst-resources-26.2024.400/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.554063 lsst-resources-26.2024.400/doc/lsst.resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/doc/lsst.resources/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/doc/lsst.resources/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/doc/lsst.resources/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.554063 lsst-resources-26.2024.400/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.554063 lsst-resources-26.2024.400/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.558063 lsst-resources-26.2024.400/python/lsst/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.558063 lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    57609 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/_resourcePath.py
--rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70041 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/packageresource.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20076 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/schemeless.py
--rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/python/lsst/resources/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst/resources/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.562063 lsst-resources-26.2024.400/python/lsst_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 10:34:54.000000 lsst-resources-26.2024.400/python/lsst_resources.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-25 10:34:54.562063 lsst-resources-26.2024.400/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 10:34:54.562063 lsst-resources-26.2024.400/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38967 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-01-25 10:34:41.000000 lsst-resources-26.2024.400/tests/test_schemeless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/doc/lsst.resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/doc/lsst.resources/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/doc/lsst.resources/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/doc/lsst.resources/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.703503 lsst-resources-26.2024.500/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.707503 lsst-resources-26.2024.500/python/lsst/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.707503 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57585 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/_resourcePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70041 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/packageresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20076 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/schemeless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/python/lsst/resources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst/resources/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/python/lsst_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 10:58:10.000000 lsst-resources-26.2024.500/python/lsst_resources.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 10:58:10.711503 lsst-resources-26.2024.500/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38967 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-01 10:57:59.000000 lsst-resources-26.2024.500/tests/test_schemeless.py
```

### Comparing `lsst-resources-26.2024.400/LICENSE` & `lsst-resources-26.2024.500/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/PKG-INFO` & `lsst-resources-26.2024.500/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 26.2024.400
+Version: 26.2024.500
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -26,15 +26,15 @@
 Requires-Dist: astropy>=4.0; extra == "https"
 Requires-Dist: requests>=2.26.0; extra == "https"
 Requires-Dist: urllib3>=1.25.10; extra == "https"
 Requires-Dist: defusedxml; extra == "https"
 Provides-Extra: gs
 Requires-Dist: google-cloud-storage; extra == "gs"
 Provides-Extra: test
-Requires-Dist: moto>=1.3; extra == "test"
+Requires-Dist: moto!=5.0.0,>=1.3; extra == "test"
 Requires-Dist: pytest>=3.2; extra == "test"
 Requires-Dist: pytest-openfiles>=0.5.0; extra == "test"
 Requires-Dist: responses>=0.12.0; extra == "test"
 
 # lsst.resources
 
 [![pypi](https://img.shields.io/pypi/v/lsst-resources.svg)](https://pypi.org/project/lsst-resources/)
```

### Comparing `lsst-resources-26.2024.400/README.md` & `lsst-resources-26.2024.500/README.md`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/doc/lsst.resources/CHANGES.rst` & `lsst-resources-26.2024.500/doc/lsst.resources/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/doc/lsst.resources/index.rst` & `lsst-resources-26.2024.500/doc/lsst.resources/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/pyproject.toml` & `lsst-resources-26.2024.500/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "urllib3 >= 1.25.10",
     "defusedxml",
 ]
 gs = [
     "google-cloud-storage",
 ]
 test = [
-    "moto >= 1.3",
+    "moto >= 1.3,!=5.0.0",
     "pytest >= 3.2",
     "pytest-openfiles >= 0.5.0",
     "responses >= 0.12.0",
 ]
 
 [tool.setuptools.packages.find]
 where = ["python"]
```

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/__init__.py` & `lsst-resources-26.2024.500/python/lsst/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_baseResourceHandle.py` & `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_baseResourceHandle.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,92 +41,74 @@
     `.BaseResourceHandle`.
 
     Any class that satisfies this protocol can be used in any context where a
     `.BaseResourceHandle` is expected.
     """
 
     @abstractproperty
-    def mode(self) -> str:
-        ...
+    def mode(self) -> str: ...
 
     @abstractmethod
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
     @abstractproperty
-    def closed(self) -> bool:
-        ...
+    def closed(self) -> bool: ...
 
     @abstractmethod
-    def fileno(self) -> int:
-        ...
+    def fileno(self) -> int: ...
 
     @abstractmethod
-    def flush(self) -> None:
-        ...
+    def flush(self) -> None: ...
 
     @abstractproperty
-    def isatty(self) -> bool | Callable[[], bool]:
-        ...
+    def isatty(self) -> bool | Callable[[], bool]: ...
 
     @abstractmethod
-    def readable(self) -> bool:
-        ...
+    def readable(self) -> bool: ...
 
     @abstractmethod
-    def readline(self, size: int = -1) -> U:
-        ...
+    def readline(self, size: int = -1) -> U: ...
 
     @abstractmethod
-    def readlines(self, hint: int = -1) -> Iterable[U]:
-        ...
+    def readlines(self, hint: int = -1) -> Iterable[U]: ...
 
     @abstractmethod
     def seek(self, offset: int, whence: int = SEEK_SET, /) -> int:
         pass
 
     @abstractmethod
-    def seekable(self) -> bool:
-        ...
+    def seekable(self) -> bool: ...
 
     @abstractmethod
-    def tell(self) -> int:
-        ...
+    def tell(self) -> int: ...
 
     @abstractmethod
-    def truncate(self, size: int | None = None) -> int:
-        ...
+    def truncate(self, size: int | None = None) -> int: ...
 
     @abstractmethod
-    def writable(self) -> bool:
-        ...
+    def writable(self) -> bool: ...
 
     @abstractmethod
-    def writelines(self, lines: Iterable[U], /) -> None:
-        ...
+    def writelines(self, lines: Iterable[U], /) -> None: ...
 
     @abstractmethod
-    def read(self, size: int = -1) -> U:
-        ...
+    def read(self, size: int = -1) -> U: ...
 
     @abstractmethod
-    def write(self, b: U, /) -> int:
-        ...
+    def write(self, b: U, /) -> int: ...
 
-    def __enter__(self: S) -> S:
-        ...
+    def __enter__(self: S) -> S: ...
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
         /,
-    ) -> bool | None:
-        ...
+    ) -> bool | None: ...
 
 
 class BaseResourceHandle(ABC, ResourceHandleProtocol[U]):
     """Base class interface for the handle like interface of
     `~lsst.resources.ResourcePath` subclasses.
 
     Parameters
```

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_fileResourceHandle.py` & `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_fileResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_httpResourceHandle.py` & `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_httpResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py` & `lsst-resources-26.2024.500/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/_resourcePath.py` & `lsst-resources-26.2024.500/python/lsst/resources/_resourcePath.py`

 * *Files 0% similar despite different names*

```diff
@@ -1267,36 +1267,33 @@
     @overload
     @classmethod
     def findFileResources(
         cls,
         candidates: Iterable[ResourcePathExpression],
         file_filter: str | re.Pattern | None,
         grouped: Literal[True],
-    ) -> Iterator[Iterator[ResourcePath]]:
-        ...
+    ) -> Iterator[Iterator[ResourcePath]]: ...
 
     @overload
     @classmethod
     def findFileResources(
         cls,
         candidates: Iterable[ResourcePathExpression],
         *,
         grouped: Literal[True],
-    ) -> Iterator[Iterator[ResourcePath]]:
-        ...
+    ) -> Iterator[Iterator[ResourcePath]]: ...
 
     @overload
     @classmethod
     def findFileResources(
         cls,
         candidates: Iterable[ResourcePathExpression],
         file_filter: str | re.Pattern | None = None,
         grouped: Literal[False] = False,
-    ) -> Iterator[ResourcePath]:
-        ...
+    ) -> Iterator[ResourcePath]: ...
 
     @classmethod
     def findFileResources(
         cls,
         candidates: Iterable[ResourcePathExpression],
         file_filter: str | re.Pattern | None = None,
         grouped: bool = False,
```

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/file.py` & `lsst-resources-26.2024.500/python/lsst/resources/file.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/gs.py` & `lsst-resources-26.2024.500/python/lsst/resources/gs.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/http.py` & `lsst-resources-26.2024.500/python/lsst/resources/http.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/location.py` & `lsst-resources-26.2024.500/python/lsst/resources/location.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/mem.py` & `lsst-resources-26.2024.500/python/lsst/resources/mem.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/packageresource.py` & `lsst-resources-26.2024.500/python/lsst/resources/packageresource.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/s3.py` & `lsst-resources-26.2024.500/python/lsst/resources/s3.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/s3utils.py` & `lsst-resources-26.2024.500/python/lsst/resources/s3utils.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/schemeless.py` & `lsst-resources-26.2024.500/python/lsst/resources/schemeless.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/tests.py` & `lsst-resources-26.2024.500/python/lsst/resources/tests.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/python/lsst/resources/utils.py` & `lsst-resources-26.2024.500/python/lsst/resources/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         yield None
 
 
 class TransactionProtocol(Protocol):
     """Protocol for type checking transaction interface."""
 
     @contextlib.contextmanager
-    def undoWith(self, name: str, undoFunc: Callable, *args: Any, **kwargs: Any) -> Iterator[None]:
-        ...
+    def undoWith(self, name: str, undoFunc: Callable, *args: Any, **kwargs: Any) -> Iterator[None]: ...
 
 
 def makeTestTempDir(default_base: str | None = None) -> str:
     """Create a temporary directory for test usage.
 
     The directory will be created within ``LSST_RESOURCES_TEST_TMP`` if that
     environment variable is set, falling back to ``LSST_RESOURCES_TMPDIR``
```

### Comparing `lsst-resources-26.2024.400/python/lsst_resources.egg-info/PKG-INFO` & `lsst-resources-26.2024.500/python/lsst_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 26.2024.400
+Version: 26.2024.500
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -26,15 +26,15 @@
 Requires-Dist: astropy>=4.0; extra == "https"
 Requires-Dist: requests>=2.26.0; extra == "https"
 Requires-Dist: urllib3>=1.25.10; extra == "https"
 Requires-Dist: defusedxml; extra == "https"
 Provides-Extra: gs
 Requires-Dist: google-cloud-storage; extra == "gs"
 Provides-Extra: test
-Requires-Dist: moto>=1.3; extra == "test"
+Requires-Dist: moto!=5.0.0,>=1.3; extra == "test"
 Requires-Dist: pytest>=3.2; extra == "test"
 Requires-Dist: pytest-openfiles>=0.5.0; extra == "test"
 Requires-Dist: responses>=0.12.0; extra == "test"
 
 # lsst.resources
 
 [![pypi](https://img.shields.io/pypi/v/lsst-resources.svg)](https://pypi.org/project/lsst-resources/)
```

### Comparing `lsst-resources-26.2024.400/python/lsst_resources.egg-info/SOURCES.txt` & `lsst-resources-26.2024.500/python/lsst_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_file.py` & `lsst-resources-26.2024.500/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_gs.py` & `lsst-resources-26.2024.500/tests/test_gs.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_http.py` & `lsst-resources-26.2024.500/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_location.py` & `lsst-resources-26.2024.500/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_mem.py` & `lsst-resources-26.2024.500/tests/test_mem.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_resource.py` & `lsst-resources-26.2024.500/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `lsst-resources-26.2024.400/tests/test_s3.py` & `lsst-resources-26.2024.500/tests/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 from lsst.resources.s3 import S3ResourcePath
 from lsst.resources.s3utils import clean_test_environment_for_s3
 from lsst.resources.tests import GenericReadWriteTestCase, GenericTestCase
 
 try:
     import boto3
     import botocore
-    from moto import mock_s3
+
+    try:
+        from moto import mock_aws  # v5
+    except ImportError:
+        from moto import mock_s3 as mock_aws
 except ImportError:
     boto3 = None
 
-    def mock_s3(cls):
-        """No-op decorator in case moto mock_s3 can not be imported."""
+    def mock_aws(cls):
+        """No-op decorator in case moto mock_aws can not be imported."""
         return cls
 
 
 class GenericS3TestCase(GenericTestCase, unittest.TestCase):
     """Generic tests of S3 URIs."""
 
     scheme = "s3"
@@ -43,21 +47,21 @@
 @unittest.skipIf(not boto3, "Warning: boto3 AWS SDK not found!")
 class S3ReadWriteTestCase(GenericReadWriteTestCase, unittest.TestCase):
     """Tests of reading and writing S3 URIs."""
 
     scheme = "s3"
     netloc = "my_2nd_bucket"
 
-    mock_s3 = mock_s3()
+    mock_aws = mock_aws()
     """The mocked s3 interface from moto."""
 
     def setUp(self):
         self.enterContext(clean_test_environment_for_s3())
         # Enable S3 mocking of tests.
-        self.mock_s3.start()
+        self.mock_aws.start()
 
         # MOTO needs to know that we expect Bucket bucketname to exist
         s3 = boto3.resource("s3")
         s3.create_bucket(Bucket=self.netloc)
 
         super().setUp()
 
@@ -73,15 +77,15 @@
             else:
                 raise
 
         bucket = s3.Bucket(self.netloc)
         bucket.delete()
 
         # Stop the S3 mock.
-        self.mock_s3.stop()
+        self.mock_aws.stop()
 
         S3ResourcePath.use_threads = None
 
         super().tearDown()
 
     def test_bucket_fail(self):
         # Deliberately create URI with unknown bucket.
```

### Comparing `lsst-resources-26.2024.400/tests/test_s3utils.py` & `lsst-resources-26.2024.500/tests/test_s3utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 import os
 import unittest
 from unittest import mock
 
 try:
     import boto3
     from botocore.exceptions import ParamValidationError
-    from moto import mock_s3
+
+    try:
+        from moto import mock_aws  # v5
+    except ImportError:
+        from moto import mock_s3 as mock_aws
 except ImportError:
     boto3 = None
 
 from lsst.resources import ResourcePath
 from lsst.resources.location import Location
 from lsst.resources.s3utils import bucketExists, clean_test_environment_for_s3, getS3Client, s3CheckFileExists
 
@@ -40,15 +44,15 @@
     """Test for the S3 related utilities."""
 
     bucketName = "test_bucket_name"
     fileName = "testFileName"
 
     def setUp(self):
         self.enterContext(clean_test_environment_for_s3())
-        self.enterContext(mock_s3())
+        self.enterContext(mock_aws())
 
         self.client = getS3Client()
         try:
             self.client.create_bucket(Bucket=self.bucketName)
             self.client.put_object(Bucket=self.bucketName, Key=self.fileName, Body=b"test content")
         except self.client.exceptions.BucketAlreadyExists:
             pass
```

### Comparing `lsst-resources-26.2024.400/tests/test_schemeless.py` & `lsst-resources-26.2024.500/tests/test_schemeless.py`

 * *Files identical despite different names*

