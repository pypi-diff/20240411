# Comparing `tmp/valx-0.1.0.tar.gz` & `tmp/valx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valx-0.1.0.tar", last modified: Thu Apr 11 10:15:43 2024, max compression
+gzip compressed data, was "valx-0.1.1.tar", last modified: Thu Apr 11 12:27:20 2024, max compression
```

## Comparing `valx-0.1.0.tar` & `valx-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:15:43.153071 valx-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 10:15:40.000000 valx-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 10:15:43.153071 valx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-11 10:15:40.000000 valx-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:15:43.153071 valx-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 10:15:42.000000 valx-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:15:43.153071 valx-0.1.0/valx/
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-11 10:15:40.000000 valx-0.1.0/valx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:15:43.153071 valx-0.1.0/valx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 10:15:43.000000 valx-0.1.0/valx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 10:15:43.000000 valx-0.1.0/valx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:15:43.000000 valx-0.1.0/valx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 10:15:43.000000 valx-0.1.0/valx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:20.220013 valx-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 12:27:17.000000 valx-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 12:27:20.220013 valx-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-11 12:27:17.000000 valx-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:27:20.220013 valx-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 12:27:19.000000 valx-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:20.220013 valx-0.1.1/valx/
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-11 12:27:17.000000 valx-0.1.1/valx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:20.220013 valx-0.1.1/valx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 12:27:20.000000 valx-0.1.1/valx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 12:27:20.000000 valx-0.1.1/valx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:27:20.000000 valx-0.1.1/valx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 12:27:20.000000 valx-0.1.1/valx.egg-info/top_level.txt
```

### Comparing `valx-0.1.0/LICENSE` & `valx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valx-0.1.0/PKG-INFO` & `valx-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valx
-Version: 0.1.0
+Version: 0.1.1
 Summary: An open-source Python library for text cleaning tasks.
 Home-page: https://github.com/infinitode/valx
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `valx-0.1.0/README.md` & `valx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `valx-0.1.0/setup.py` & `valx-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='valx',
-    version='0.1.0',
+    version='0.1.1',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='An open-source Python library for text cleaning tasks.',
     long_description='An open-source Python library for data cleaning tasks. Includes profanity detection, and removal.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/valx',
     packages=find_packages(),
```

### Comparing `valx-0.1.0/valx/__init__.py` & `valx-0.1.1/valx/__init__.py`

 * *Files identical despite different names*

### Comparing `valx-0.1.0/valx.egg-info/PKG-INFO` & `valx-0.1.1/valx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valx
-Version: 0.1.0
+Version: 0.1.1
 Summary: An open-source Python library for text cleaning tasks.
 Home-page: https://github.com/infinitode/valx
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

