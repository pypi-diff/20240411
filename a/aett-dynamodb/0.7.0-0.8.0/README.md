# Comparing `tmp/aett-dynamodb-0.7.0.tar.gz` & `tmp/aett-dynamodb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-dynamodb-0.7.0.tar", last modified: Sun Apr  7 15:47:16 2024, max compression
+gzip compressed data, was "aett-dynamodb-0.8.0.tar", last modified: Thu Apr 11 04:04:39 2024, max compression
```

## Comparing `aett-dynamodb-0.7.0.tar` & `aett-dynamodb-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.562626 aett-dynamodb-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.562626 aett-dynamodb-0.7.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/src/aett/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-07 15:47:11.000000 aett-dynamodb-0.7.0/src/aett/dynamodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.566626 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:16.000000 aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:39.117841 aett-dynamodb-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 04:04:33.000000 aett-dynamodb-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 04:04:33.000000 aett-dynamodb-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-11 04:04:39.117841 aett-dynamodb-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-11 04:04:33.000000 aett-dynamodb-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 04:04:33.000000 aett-dynamodb-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:04:39.117841 aett-dynamodb-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:39.113841 aett-dynamodb-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:39.113841 aett-dynamodb-0.8.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:39.113841 aett-dynamodb-0.8.0/src/aett/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-04-11 04:04:33.000000 aett-dynamodb-0.8.0/src/aett/dynamodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:39.113841 aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-11 04:04:39.000000 aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-11 04:04:39.000000 aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:04:39.000000 aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 04:04:39.000000 aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 04:04:39.000000 aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/top_level.txt
```

### Comparing `aett-dynamodb-0.7.0/LICENSE` & `aett-dynamodb-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-dynamodb-0.7.0/PKG-INFO` & `aett-dynamodb-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 0.7.0
+Version: 0.8.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.7.0
-Requires-Dist: boto3[crt]~=1.34.79
+Requires-Dist: aett-domain>=0.8.0
+Requires-Dist: boto3[crt]~=1.34.82
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett-dynamodb-0.7.0/README.md` & `aett-dynamodb-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aett-dynamodb-0.7.0/pyproject.toml` & `aett-dynamodb-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.dynamodb"]
 
 [project]
 name = "aett-dynamodb"
-version = "0.7.0"
+version = "0.8.0"
 description = "DynamoDB connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "dynamodb"]
 dependencies = [
-    'aett-domain >= 0.7.0',
-    'boto3[crt]~=1.34.79'
+    'aett-domain >= 0.8.0',
+    'boto3[crt]~=1.34.82'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
 
 [project.urls]
```

### Comparing `aett-dynamodb-0.7.0/src/aett/dynamodb/__init__.py` & `aett-dynamodb-0.8.0/src/aett/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `aett-dynamodb-0.7.0/src/aett_dynamodb.egg-info/PKG-INFO` & `aett-dynamodb-0.8.0/src/aett_dynamodb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-dynamodb
-Version: 0.7.0
+Version: 0.8.0
 Summary: DynamoDB connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,16 +29,16 @@
 Keywords: events,event store,dynamodb
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.7.0
-Requires-Dist: boto3[crt]~=1.34.79
+Requires-Dist: aett-domain>=0.8.0
+Requires-Dist: boto3[crt]~=1.34.82
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

