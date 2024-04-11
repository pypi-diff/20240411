# Comparing `tmp/SAMMEC2-0.0.3.tar.gz` & `tmp/SAMMEC2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMMEC2-0.0.3.tar", last modified: Thu Apr 11 14:32:29 2024, max compression
+gzip compressed data, was "SAMMEC2-0.0.4.tar", last modified: Thu Apr 11 14:36:26 2024, max compression
```

## Comparing `SAMMEC2-0.0.3.tar` & `SAMMEC2-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:32:29.902526 SAMMEC2-0.0.3/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:32:29.901742 SAMMEC2-0.0.3/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.3/README
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:32:29.895791 SAMMEC2-0.0.3/SAMMEC2/
--rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.3/SAMMEC2/SAMMEC2.py
--rw-r--r--   0 bso2     (1724916894) 285334988        0 2024-04-11 14:08:10.000000 SAMMEC2-0.0.3/SAMMEC2/__init__.py
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:32:29.900934 SAMMEC2-0.0.3/SAMMEC2.egg-info/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988      178 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/SOURCES.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/dependency_links.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/top_level.txt
--rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-11 14:32:29.902723 SAMMEC2-0.0.3/setup.cfg
--rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-11 14:32:13.000000 SAMMEC2-0.0.3/setup.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:36:26.463595 SAMMEC2-0.0.4/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:36:26.463145 SAMMEC2-0.0.4/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.4/README
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:36:26.458122 SAMMEC2-0.0.4/SAMMEC2/
+-rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.4/SAMMEC2/SAMMEC2.py
+-rw-r--r--   0 bso2     (1724916894) 285334988       22 2024-04-11 14:36:10.000000 SAMMEC2-0.0.4/SAMMEC2/__init__.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:36:26.462775 SAMMEC2-0.0.4/SAMMEC2.egg-info/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988      178 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/SOURCES.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/dependency_links.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/top_level.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-11 14:36:26.463679 SAMMEC2-0.0.4/setup.cfg
+-rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-11 14:36:10.000000 SAMMEC2-0.0.4/setup.py
```

### Comparing `SAMMEC2-0.0.3/SAMMEC2/SAMMEC2.py` & `SAMMEC2-0.0.4/SAMMEC2/SAMMEC2.py`

 * *Files identical despite different names*

### Comparing `SAMMEC2-0.0.3/setup.py` & `SAMMEC2-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SAMMEC2", # Replace with your own PyPI username(id)
-    version="0.0.3",
+    version="0.0.4",
     author="Banghee So",
     author_email="bso@towson.edu",
     description="SAMMEC2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bheeso/SAMME.C2",
     packages=setuptools.find_packages(),
```

