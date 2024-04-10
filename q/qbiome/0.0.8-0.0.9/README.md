# Comparing `tmp/qbiome-0.0.8.tar.gz` & `tmp/qbiome-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qbiome-0.0.8.tar", last modified: Tue Apr 13 17:30:24 2021, max compression
+gzip compressed data, was "dist/qbiome-0.0.9.tar", last modified: Tue Apr 13 17:34:45 2021, max compression
```

## Comparing `qbiome-0.0.8.tar` & `qbiome-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 17:30:24.000000 qbiome-0.0.8/
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       93 2021-04-13 16:30:51.000000 qbiome-0.0.8/MANIFEST.in
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1969 2021-04-13 17:30:24.000000 qbiome-0.0.8/PKG-INFO
-drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 17:30:24.000000 qbiome-0.0.8/qbiome.egg-info/
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1969 2021-04-13 17:30:23.000000 qbiome-0.0.8/qbiome.egg-info/PKG-INFO
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      333 2021-04-13 17:30:23.000000 qbiome-0.0.8/qbiome.egg-info/SOURCES.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        1 2021-04-13 17:30:23.000000 qbiome-0.0.8/qbiome.egg-info/dependency_links.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       48 2021-04-13 17:30:23.000000 qbiome-0.0.8/qbiome.egg-info/requires.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        7 2021-04-13 17:30:23.000000 qbiome-0.0.8/qbiome.egg-info/top_level.txt
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1810 2021-04-13 17:27:55.000000 qbiome-0.0.8/setup.py
-drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 17:30:24.000000 qbiome-0.0.8/qbiome/
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 16:34:49.000000 qbiome-0.0.8/qbiome/__init__.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1026 2021-04-13 16:30:29.000000 qbiome-0.0.8/qbiome/forecaster.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     4175 2021-04-13 16:30:29.000000 qbiome-0.0.8/qbiome/qnet_orchestrator.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     8416 2021-04-13 16:30:29.000000 qbiome-0.0.8/qbiome/quantizer.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1667 2021-04-13 16:30:29.000000 qbiome-0.0.8/qbiome/mask_checker.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 16:30:29.000000 qbiome-0.0.8/qbiome/qbiome.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     4578 2021-04-13 16:30:29.000000 qbiome-0.0.8/qbiome/data_formatter.py
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      854 2021-04-13 17:27:06.000000 qbiome-0.0.8/README.rst
--rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       38 2021-04-13 17:30:24.000000 qbiome-0.0.8/setup.cfg
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 17:34:45.000000 qbiome-0.0.9/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       93 2021-04-13 16:30:51.000000 qbiome-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1969 2021-04-13 17:34:45.000000 qbiome-0.0.9/PKG-INFO
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome.egg-info/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1969 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome.egg-info/PKG-INFO
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      333 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome.egg-info/SOURCES.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        1 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome.egg-info/dependency_links.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       48 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome.egg-info/requires.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        7 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome.egg-info/top_level.txt
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1810 2021-04-13 17:27:55.000000 qbiome-0.0.9/setup.py
+drwxrwxr-x   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 17:34:45.000000 qbiome-0.0.9/qbiome/
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 16:34:49.000000 qbiome-0.0.9/qbiome/__init__.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1026 2021-04-13 16:30:29.000000 qbiome-0.0.9/qbiome/forecaster.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     4175 2021-04-13 16:30:29.000000 qbiome-0.0.9/qbiome/qnet_orchestrator.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     8416 2021-04-13 16:30:29.000000 qbiome-0.0.9/qbiome/quantizer.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     1667 2021-04-13 16:30:29.000000 qbiome-0.0.9/qbiome/mask_checker.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)        0 2021-04-13 16:30:29.000000 qbiome-0.0.9/qbiome/qbiome.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)     4578 2021-04-13 16:30:29.000000 qbiome-0.0.9/qbiome/data_formatter.py
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)      854 2021-04-13 17:27:06.000000 qbiome-0.0.9/README.rst
+-rw-rw-r--   0 ishanu    (1000) ishanu    (1000)       38 2021-04-13 17:34:45.000000 qbiome-0.0.9/setup.cfg
```

### Comparing `qbiome-0.0.8/PKG-INFO` & `qbiome-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qbiome
-Version: 0.0.8
+Version: 0.0.9
 Summary: Analyzing microbiome abundance data to infer deep structures
 Home-page: https://github.com/zeroknowledgediscovery/qbiome
 Author: zed.uchicago.edu
 Author-email: ishanu@uchicago.edu
 License: LICENSE
-Download-URL: https://github.com/zeroknowledgediscovery/qbiome/archive/0.0.8.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/qbiome/archive/0.0.9.tar.gz
 Description: ===============
         cynet
         ===============
         
         .. figure:: https://img.shields.io/pypi/dm/cynet.svg
            :alt: cynet PyPI Downloads
         .. figure:: https://img.shields.io/pypi/v/cynet.svg
```

### Comparing `qbiome-0.0.8/qbiome.egg-info/PKG-INFO` & `qbiome-0.0.9/qbiome.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qbiome
-Version: 0.0.8
+Version: 0.0.9
 Summary: Analyzing microbiome abundance data to infer deep structures
 Home-page: https://github.com/zeroknowledgediscovery/qbiome
 Author: zed.uchicago.edu
 Author-email: ishanu@uchicago.edu
 License: LICENSE
-Download-URL: https://github.com/zeroknowledgediscovery/qbiome/archive/0.0.8.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/qbiome/archive/0.0.9.tar.gz
 Description: ===============
         cynet
         ===============
         
         .. figure:: https://img.shields.io/pypi/dm/cynet.svg
            :alt: cynet PyPI Downloads
         .. figure:: https://img.shields.io/pypi/v/cynet.svg
```

### Comparing `qbiome-0.0.8/setup.py` & `qbiome-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `qbiome-0.0.8/qbiome/forecaster.py` & `qbiome-0.0.9/qbiome/forecaster.py`

 * *Files identical despite different names*

### Comparing `qbiome-0.0.8/qbiome/qnet_orchestrator.py` & `qbiome-0.0.9/qbiome/qnet_orchestrator.py`

 * *Files identical despite different names*

### Comparing `qbiome-0.0.8/qbiome/quantizer.py` & `qbiome-0.0.9/qbiome/quantizer.py`

 * *Files identical despite different names*

### Comparing `qbiome-0.0.8/qbiome/mask_checker.py` & `qbiome-0.0.9/qbiome/mask_checker.py`

 * *Files identical despite different names*

### Comparing `qbiome-0.0.8/qbiome/data_formatter.py` & `qbiome-0.0.9/qbiome/data_formatter.py`

 * *Files identical despite different names*

### Comparing `qbiome-0.0.8/README.rst` & `qbiome-0.0.9/README.rst`

 * *Files identical despite different names*

