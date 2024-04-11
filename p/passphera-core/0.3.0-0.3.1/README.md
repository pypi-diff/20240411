# Comparing `tmp/passphera-core-0.3.0.tar.gz` & `tmp/passphera-core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passphera-core-0.3.0.tar", last modified: Thu Apr 11 00:00:39 2024, max compression
+gzip compressed data, was "passphera-core-0.3.1.tar", last modified: Thu Apr 11 00:05:43 2024, max compression
```

## Comparing `passphera-core-0.3.0.tar` & `passphera-core-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:00:39.733254 passphera-core-0.3.0/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:00:39.732254 passphera-core-0.3.0/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.3.0/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:00:39.731254 passphera-core-0.3.0/passphera_core/
--rw-r--r--   0 fathi     (1000) fathi     (1000)       89 2024-04-10 23:57:17.000000 passphera-core-0.3.0/passphera_core/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      155 2024-04-10 23:57:17.000000 passphera-core-0.3.0/passphera_core/exceptions.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     7855 2024-04-10 23:57:17.000000 passphera-core-0.3.0/passphera_core/generator.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:00:39.732254 passphera-core-0.3.0/passphera_core.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      254 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-11 00:00:39.000000 passphera-core-0.3.0/passphera_core.egg-info/top_level.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-11 00:00:39.733254 passphera-core-0.3.0/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-10 23:39:37.000000 passphera-core-0.3.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:05:43.634888 passphera-core-0.3.1/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:05:43.633888 passphera-core-0.3.1/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.3.1/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:05:43.631888 passphera-core-0.3.1/passphera_core/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      139 2024-04-11 00:05:27.000000 passphera-core-0.3.1/passphera_core/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      155 2024-04-10 23:57:17.000000 passphera-core-0.3.1/passphera_core/exceptions.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     7855 2024-04-10 23:57:17.000000 passphera-core-0.3.1/passphera_core/generator.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:05:43.633888 passphera-core-0.3.1/passphera_core.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:05:43.000000 passphera-core-0.3.1/passphera_core.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      254 2024-04-11 00:05:43.000000 passphera-core-0.3.1/passphera_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-11 00:05:43.000000 passphera-core-0.3.1/passphera_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-11 00:05:43.000000 passphera-core-0.3.1/passphera_core.egg-info/top_level.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-11 00:05:43.634888 passphera-core-0.3.1/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-11 00:05:27.000000 passphera-core-0.3.1/setup.py
```

### Comparing `passphera-core-0.3.0/PKG-INFO` & `passphera-core-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.3.0/passphera_core/generator.py` & `passphera-core-0.3.1/passphera_core/generator.py`

 * *Files identical despite different names*

### Comparing `passphera-core-0.3.0/passphera_core.egg-info/PKG-INFO` & `passphera-core-0.3.1/passphera_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.3.0/setup.py` & `passphera-core-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='passphera-core',
-    version='0.3.0',
+    version='0.3.1',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     url='https://github.com/passphera/core',
     description='The core system of passphera project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['passphera_core'],
```

