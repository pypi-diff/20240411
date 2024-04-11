# Comparing `tmp/mazegroup-0.1.3.1.tar.gz` & `tmp/mazegroup-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.3.1.tar", last modified: Wed Apr 10 19:33:33 2024, max compression
+gzip compressed data, was "mazegroup-0.1.3.2.tar", last modified: Wed Apr 10 19:50:19 2024, max compression
```

## Comparing `mazegroup-0.1.3.1.tar` & `mazegroup-0.1.3.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:33:33.770113 mazegroup-0.1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-10 19:33:33.770113 mazegroup-0.1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:33:33.766113 mazegroup-0.1.3.1/mazegroup/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/mazegroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:33:33.766113 mazegroup-0.1.3.1/mazegroup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/mazegroup/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/mazegroup/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:33:33.766113 mazegroup-0.1.3.1/mazegroup/echo/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/mazegroup/echo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/mazegroup/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/mazegroup/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:33:33.766113 mazegroup-0.1.3.1/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-10 19:33:33.000000 mazegroup-0.1.3.1/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 19:33:33.000000 mazegroup-0.1.3.1/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:33:33.000000 mazegroup-0.1.3.1/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 19:33:33.000000 mazegroup-0.1.3.1/mazegroup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 19:33:33.000000 mazegroup-0.1.3.1/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:33:33.770113 mazegroup-0.1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-10 19:33:28.000000 mazegroup-0.1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/echo/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/echo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/saves/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/saves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/setup.py
```

### Comparing `mazegroup-0.1.3.1/PKG-INFO` & `mazegroup-0.1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.3.1/README.md` & `mazegroup-0.1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.3.1/mazegroup/commands.py` & `mazegroup-0.1.3.2/mazegroup/commands.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.3.1/mazegroup/utils.py` & `mazegroup-0.1.3.2/mazegroup/utils.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.3.1/mazegroup.egg-info/PKG-INFO` & `mazegroup-0.1.3.2/mazegroup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mazegroup-0.1.3.1/setup.py` & `mazegroup-0.1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 #
 
 setup(
     name="mazegroup",
-    version="0.1.3.1",
+    version="0.1.3.2",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Genius_um",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
     packages=["mazegroup", "mazegroup/cli", "mazegroup/echo", "mazegroup/saves"], # find_packages(),
```

