# Comparing `tmp/aett-eventstore-0.7.0.tar.gz` & `tmp/aett-eventstore-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-eventstore-0.7.0.tar", last modified: Sun Apr  7 15:47:20 2024, max compression
+gzip compressed data, was "aett-eventstore-0.8.0.tar", last modified: Thu Apr 11 04:04:38 2024, max compression
```

## Comparing `aett-eventstore-0.7.0.tar` & `aett-eventstore-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.833998 aett-eventstore-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:20.833998 aett-eventstore-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/aett/eventstore/
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/src/aett/eventstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:20.000000 aett-eventstore-0.7.0/src/aett_eventstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.829998 aett-eventstore-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_EventStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_Memento.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 15:47:13.000000 aett-eventstore-0.7.0/tests/test_Topics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:38.722809 aett-eventstore-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-11 04:04:38.722809 aett-eventstore-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:04:38.722809 aett-eventstore-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:38.718809 aett-eventstore-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:38.718809 aett-eventstore-0.8.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:38.718809 aett-eventstore-0.8.0/src/aett/eventstore/
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/src/aett/eventstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:38.722809 aett-eventstore-0.8.0/src/aett_eventstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-11 04:04:38.000000 aett-eventstore-0.8.0/src/aett_eventstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-11 04:04:38.000000 aett-eventstore-0.8.0/src/aett_eventstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:04:38.000000 aett-eventstore-0.8.0/src/aett_eventstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 04:04:38.000000 aett-eventstore-0.8.0/src/aett_eventstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 04:04:38.000000 aett-eventstore-0.8.0/src/aett_eventstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:38.722809 aett-eventstore-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/tests/test_EventStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/tests/test_Memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/tests/test_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-11 04:04:33.000000 aett-eventstore-0.8.0/tests/test_Topics.py
```

### Comparing `aett-eventstore-0.7.0/LICENSE` & `aett-eventstore-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.7.0/PKG-INFO` & `aett-eventstore-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 0.7.0
+Version: 0.8.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aett-eventstore-0.7.0/README.md` & `aett-eventstore-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.7.0/pyproject.toml` & `aett-eventstore-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.eventstore"]
 
 [project]
 name = "aett-eventstore"
-version = "0.7.0"
+version = "0.8.0"
 description = "Event store for Python"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `aett-eventstore-0.7.0/src/aett/eventstore/__init__.py` & `aett-eventstore-0.8.0/src/aett/eventstore/__init__.py`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.7.0/src/aett_eventstore.egg-info/PKG-INFO` & `aett-eventstore-0.8.0/src/aett_eventstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-eventstore
-Version: 0.7.0
+Version: 0.8.0
 Summary: Event store for Python
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aett-eventstore-0.7.0/tests/test_EventStream.py` & `aett-eventstore-0.8.0/tests/test_EventStream.py`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.7.0/tests/test_Serialization.py` & `aett-eventstore-0.8.0/tests/test_Serialization.py`

 * *Files identical despite different names*

### Comparing `aett-eventstore-0.7.0/tests/test_Topics.py` & `aett-eventstore-0.8.0/tests/test_Topics.py`

 * *Files identical despite different names*

