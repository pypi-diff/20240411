# Comparing `tmp/moonstreamdb-v3-0.0.1.tar.gz` & `tmp/moonstreamdb-v3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-v3-0.0.1.tar", last modified: Mon Apr  8 14:26:44 2024, max compression
+gzip compressed data, was "moonstreamdb-v3-0.0.2.tar", last modified: Thu Apr 11 12:27:41 2024, max compression
```

## Comparing `moonstreamdb-v3-0.0.1.tar` & `moonstreamdb-v3-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:44.635594 moonstreamdb-v3-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-08 14:26:44.635594 moonstreamdb-v3-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 14:26:30.000000 moonstreamdb-v3-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:44.635594 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-08 14:26:44.000000 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-08 14:26:44.000000 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:26:44.000000 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:26:34.000000 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 14:26:44.000000 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 14:26:44.000000 moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:44.635594 moonstreamdb-v3-0.0.1/moonstreamdbv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:26:30.000000 moonstreamdb-v3-0.0.1/moonstreamdbv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-08 14:26:30.000000 moonstreamdb-v3-0.0.1/moonstreamdbv3/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-08 14:26:30.000000 moonstreamdb-v3-0.0.1/moonstreamdbv3/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 14:26:30.000000 moonstreamdb-v3-0.0.1/moonstreamdbv3/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:26:44.635594 moonstreamdb-v3-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-08 14:26:30.000000 moonstreamdb-v3-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:27:32.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 12:27:41.000000 moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdbv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/moonstreamdbv3/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:27:41.601107 moonstreamdb-v3-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-11 12:27:27.000000 moonstreamdb-v3-0.0.2/setup.py
```

### Comparing `moonstreamdb-v3-0.0.1/PKG-INFO` & `moonstreamdb-v3-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.1/moonstreamdb_v3.egg-info/PKG-INFO` & `moonstreamdb-v3-0.0.2/moonstreamdb_v3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.1/moonstreamdbv3/db.py` & `moonstreamdb-v3-0.0.2/moonstreamdbv3/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.1/moonstreamdbv3/models.py` & `moonstreamdb-v3-0.0.2/moonstreamdbv3/models.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.1/setup.py` & `moonstreamdb-v3-0.0.2/setup.py`

 * *Files identical despite different names*

