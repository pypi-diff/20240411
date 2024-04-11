# Comparing `tmp/aett-postgres-0.7.0.tar.gz` & `tmp/aett-postgres-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aett-postgres-0.7.0.tar", last modified: Sun Apr  7 15:47:16 2024, max compression
+gzip compressed data, was "aett-postgres-0.8.0.tar", last modified: Thu Apr 11 04:04:35 2024, max compression
```

## Comparing `aett-postgres-0.7.0.tar` & `aett-postgres-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.082473 aett-postgres-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.082473 aett-postgres-0.7.0/src/aett/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/src/aett/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-07 15:47:10.000000 aett-postgres-0.7.0/src/aett/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:16.086473 aett-postgres-0.7.0/src/aett_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 15:47:16.000000 aett-postgres-0.7.0/src/aett_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:35.465915 aett-postgres-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 04:04:29.000000 aett-postgres-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 04:04:29.000000 aett-postgres-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-11 04:04:35.465915 aett-postgres-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-11 04:04:29.000000 aett-postgres-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-11 04:04:29.000000 aett-postgres-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:04:35.465915 aett-postgres-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:35.461915 aett-postgres-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:35.461915 aett-postgres-0.8.0/src/aett/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:35.461915 aett-postgres-0.8.0/src/aett/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-11 04:04:29.000000 aett-postgres-0.8.0/src/aett/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:04:35.461915 aett-postgres-0.8.0/src/aett_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-11 04:04:35.000000 aett-postgres-0.8.0/src/aett_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-11 04:04:35.000000 aett-postgres-0.8.0/src/aett_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:04:35.000000 aett-postgres-0.8.0/src/aett_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 04:04:35.000000 aett-postgres-0.8.0/src/aett_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 04:04:35.000000 aett-postgres-0.8.0/src/aett_postgres.egg-info/top_level.txt
```

### Comparing `aett-postgres-0.7.0/LICENSE` & `aett-postgres-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aett-postgres-0.7.0/PKG-INFO` & `aett-postgres-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 0.7.0
+Version: 0.8.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.7.0
+Requires-Dist: aett-domain>=0.8.0
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

### Comparing `aett-postgres-0.7.0/README.md` & `aett-postgres-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aett-postgres-0.7.0/pyproject.toml` & `aett-postgres-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 include = ["aett.postgres"]
 
 [project]
 name = "aett-postgres"
-version = "0.7.0"
+version = "0.8.0"
 description = "Postgres connector for aett event store"
 readme = "README.md"
 authors = [{ name = "Jacob Reimers", email = "pypi@reimers.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["events", "event store", "postgres"]
 dependencies = [
-    'aett-domain >= 0.7.0',
+    'aett-domain >= 0.8.0',
     'psycopg-binary~=3.1.18'
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "behave"]
```

### Comparing `aett-postgres-0.7.0/src/aett/postgres/__init__.py` & `aett-postgres-0.8.0/src/aett/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `aett-postgres-0.7.0/src/aett_postgres.egg-info/PKG-INFO` & `aett-postgres-0.8.0/src/aett_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aett-postgres
-Version: 0.7.0
+Version: 0.8.0
 Summary: Postgres connector for aett event store
 Author-email: Jacob Reimers <pypi@reimers.io>
 License: MIT License
         
         Copyright (c) 2024 python_eventstore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,15 +29,15 @@
 Keywords: events,event store,postgres
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aett-domain>=0.7.0
+Requires-Dist: aett-domain>=0.8.0
 Requires-Dist: psycopg-binary~=3.1.18
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: behave; extra == "dev"
 
 # Æt (Aett) is an Event Store for Python
```

