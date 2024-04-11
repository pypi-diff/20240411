# Comparing `tmp/diracx-db-0.0.1a8.tar.gz` & `tmp/diracx-db-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-db-0.0.1a8.tar", last modified: Thu Nov 30 08:40:26 2023, max compression
+gzip compressed data, was "diracx-db-0.0.1a9.tar", last modified: Sun Jan 28 09:12:13 2024, max compression
```

## Comparing `diracx-db-0.0.1a8.tar` & `diracx-db-0.0.1a9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.045542 diracx-db-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.045542 diracx-db-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.049542 diracx-db-0.0.1a8/src/diracx/db/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.049542 diracx-db-0.0.1a8/src/diracx/db/os/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/os/job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/os/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.049542 diracx-db-0.0.1a8/src/diracx/db/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.049542 diracx-db-0.0.1a8/src/diracx/db/sql/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/auth/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/auth/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.049542 diracx-db-0.0.1a8/src/diracx/db/sql/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/dummy/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/dummy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.049542 diracx-db-0.0.1a8/src/diracx/db/sql/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/jobs/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/jobs/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/jobs/status_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/src/diracx/db/sql/sandbox_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/sandbox_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/sandbox_metadata/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/sandbox_metadata/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/src/diracx/db/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/src/diracx_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-11-30 08:40:26.000000 diracx-db-0.0.1a8/src/diracx_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-30 08:40:26.000000 diracx-db-0.0.1a8/src/diracx_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:40:26.000000 diracx-db-0.0.1a8/src/diracx_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-30 08:40:26.000000 diracx-db-0.0.1a8/src/diracx_db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-30 08:40:26.000000 diracx-db-0.0.1a8/src/diracx_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:40:26.000000 diracx-db-0.0.1a8/src/diracx_db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/auth/test_authorization_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/auth/test_device_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/auth/test_refresh_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/tests/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/jobs/test_jobDB.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/jobs/test_jobLoggingDB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:26.053542 diracx-db-0.0.1a8/tests/opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/opensearch/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/opensearch/test_index_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/opensearch/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/test_dummyDB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2023-11-30 08:39:21.000000 diracx-db-0.0.1a8/tests/test_sandbox_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.453004 diracx-db-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.453004 diracx-db-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/os/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/os/job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/os/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/sql/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/auth/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/auth/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/sql/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/dummy/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/dummy/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/sql/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29876 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/jobs/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/jobs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/jobs/status_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.457004 diracx-db-0.0.1a9/src/diracx/db/sql/sandbox_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/sandbox_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/sandbox_metadata/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/sandbox_metadata/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/src/diracx/db/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/src/diracx_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-28 09:12:13.000000 diracx-db-0.0.1a9/src/diracx_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-01-28 09:12:13.000000 diracx-db-0.0.1a9/src/diracx_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:12:13.000000 diracx-db-0.0.1a9/src/diracx_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-28 09:12:13.000000 diracx-db-0.0.1a9/src/diracx_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-28 09:12:13.000000 diracx-db-0.0.1a9/src/diracx_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:12:13.000000 diracx-db-0.0.1a9/src/diracx_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/auth/test_authorization_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/auth/test_device_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/auth/test_refresh_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/tests/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/jobs/test_jobDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/jobs/test_jobLoggingDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:13.461004 diracx-db-0.0.1a9/tests/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/opensearch/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/opensearch/test_index_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/opensearch/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/test_dummyDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-01-28 09:11:11.000000 diracx-db-0.0.1a9/tests/test_sandbox_metadata.py
```

### Comparing `diracx-db-0.0.1a8/PKG-INFO` & `diracx-db-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-db
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-db-0.0.1a8/pyproject.toml` & `diracx-db-0.0.1a9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -52,7 +52,10 @@
 addopts = [
     "-v",
     "--cov=diracx.db", "--cov-report=term-missing",
     "-pdiracx.testing", "-pdiracx.testing.osdb",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

### Comparing `diracx-db-0.0.1a8/src/diracx/db/__main__.py` & `diracx-db-0.0.1a9/src/diracx/db/__main__.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/os/job_parameters.py` & `diracx-db-0.0.1a9/src/diracx/db/os/job_parameters.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/os/utils.py` & `diracx-db-0.0.1a9/src/diracx/db/os/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 from opensearchpy import AsyncOpenSearch
 
 from diracx.core.exceptions import InvalidQueryError
 from diracx.core.extensions import select_from_extension
 from diracx.db.exceptions import DBUnavailable
 
-OS_DATE_FORMAT = "%Y-%m-%dT%H:%M:%S.%f%z"
-
 logger = logging.getLogger(__name__)
 
 
 class OpenSearchDBError(Exception):
     pass
 
 
@@ -180,15 +178,17 @@
 
         # Dates are returned as strings, convert them to Python datetimes
         for hit in hits:
             for field_name in hit:
                 if field_name not in self.fields:
                     continue
                 if self.fields[field_name]["type"] == "date":
-                    hit[field_name] = datetime.strptime(hit[field_name], OS_DATE_FORMAT)
+                    hit[field_name] = datetime.strptime(
+                        hit[field_name], "%Y-%m-%dT%H:%M:%S.%f%z"
+                    )
 
         return hits
 
 
 def require_type(operator, field_name, field_type, allowed_types):
     if field_type not in allowed_types:
         raise InvalidQueryError(
```

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/auth/db.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/auth/db.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/auth/schema.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/auth/schema.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/dummy/db.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/dummy/db.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/dummy/schema.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/dummy/schema.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/jobs/db.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/jobs/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,15 +384,15 @@
         classAdReq = ClassAd("[]")
         retVal = {}
         retVal["JobID"] = job_id
 
         classAdJob.insertAttributeInt("JobID", job_id)
 
         try:
-            result = self._checkAndPrepareJob(
+            result = await self._checkAndPrepareJob(
                 job_id,
                 classAdJob,
                 classAdReq,
                 jobAttrs["Owner"],
                 jobAttrs["OwnerGroup"],
                 new_job_attributes,
                 classAdJob.getAttributeString("VirtualOrganization"),
@@ -417,31 +417,29 @@
 
         jobAttrs["Status"] = JobStatus.RECEIVED
 
         jobAttrs["MinorStatus"] = JobMinorStatus.RESCHEDULED
 
         jobAttrs["ApplicationStatus"] = "Unknown"
 
-        jobAttrs["ApplicationNumStatus"] = 0
+        jobAttrs["LastUpdateTime"] = datetime.now(tz=timezone.utc)
 
-        jobAttrs["LastUpdateTime"] = str(datetime.utcnow())
-
-        jobAttrs["RescheduleTime"] = str(datetime.utcnow())
+        jobAttrs["RescheduleTime"] = datetime.now(tz=timezone.utc)
 
         reqJDL = classAdReq.asJDL()
         classAdJob.insertAttributeInt("JobRequirements", reqJDL)
 
         jobJDL = classAdJob.asJDL()
 
         # Replace the JobID placeholder if any
         jobJDL = jobJDL.replace("%j", str(job_id))
 
-        result = self.setJobJDL(job_id, jobJDL)
+        result = await self.setJobJDL(job_id, jobJDL)
 
-        result = self.setJobAttributes(job_id, jobAttrs)
+        result = await self.setJobAttributes(job_id, jobAttrs)
 
         retVal["InputData"] = classAdJob.lookupAttribute("InputData")
         retVal["RescheduleCounter"] = reschedule_counter
         retVal["Status"] = JobStatus.RECEIVED
         retVal["MinorStatus"] = JobMinorStatus.RESCHEDULED
 
         return retVal
@@ -665,17 +663,21 @@
 
     async def get_tq_infos_for_jobs(
         self, job_ids: list[int]
     ) -> set[tuple[int, str, str, str]]:
         """
         Get the task queue info for given jobs
         """
-        stmt = select(
-            TaskQueues.TQId, TaskQueues.Owner, TaskQueues.OwnerGroup, TaskQueues.VO
-        ).where(JobsQueue.JobId.in_(job_ids))
+        stmt = (
+            select(
+                TaskQueues.TQId, TaskQueues.Owner, TaskQueues.OwnerGroup, TaskQueues.VO
+            )
+            .join(JobsQueue, TaskQueues.TQId == JobsQueue.TQId)
+            .where(JobsQueue.JobId.in_(job_ids))
+        )
         return set(
             (int(row[0]), str(row[1]), str(row[2]), str(row[3]))
             for row in (await self.conn.execute(stmt)).all()
         )
 
     async def get_owner_for_task_queue(self, tq_id: int) -> dict[str, str]:
         """
```

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/jobs/schema.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/jobs/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,52 +56,39 @@
         Integer,
         ForeignKey("JobJDLs.JobID", ondelete="CASCADE"),
         primary_key=True,
         default=0,
     )
     JobType = Column("JobType", String(32), default="user")
     JobGroup = Column("JobGroup", String(32), default="00000000")
-    JobSplitType = Column(
-        "JobSplitType", Enum("Single", "Master", "Subjob", "DAGNode"), default="Single"
-    )
-    MasterJobID = Column("MasterJobID", Integer, default=0)
     Site = Column("Site", String(100), default="ANY")
     JobName = Column("JobName", String(128), default="Unknown")
     Owner = Column("Owner", String(64), default="Unknown")
     OwnerGroup = Column("OwnerGroup", String(128), default="Unknown")
     VO = Column("VO", String(32))
     SubmissionTime = NullColumn("SubmissionTime", DateTime)
     RescheduleTime = NullColumn("RescheduleTime", DateTime)
     LastUpdateTime = NullColumn("LastUpdateTime", DateTime)
     StartExecTime = NullColumn("StartExecTime", DateTime)
     HeartBeatTime = NullColumn("HeartBeatTime", DateTime)
     EndExecTime = NullColumn("EndExecTime", DateTime)
     Status = Column("Status", String(32), default="Received")
     MinorStatus = Column("MinorStatus", String(128), default="Unknown")
     ApplicationStatus = Column("ApplicationStatus", String(255), default="Unknown")
-    ApplicationNumStatus = Column("ApplicationNumStatus", Integer, default=0)
     UserPriority = Column("UserPriority", Integer, default=0)
-    SystemPriority = Column("SystemPriority", Integer, default=0)
     RescheduleCounter = Column("RescheduleCounter", Integer, default=0)
     VerifiedFlag = Column("VerifiedFlag", EnumBackedBool(), default=False)
-    DeletedFlag = Column("DeletedFlag", EnumBackedBool(), default=False)
-    KilledFlag = Column("KilledFlag", EnumBackedBool(), default=False)
-    FailedFlag = Column("FailedFlag", EnumBackedBool(), default=False)
-    ISandboxReadyFlag = Column("ISandboxReadyFlag", EnumBackedBool(), default=False)
-    OSandboxReadyFlag = Column("OSandboxReadyFlag", EnumBackedBool(), default=False)
-    RetrievedFlag = Column("RetrievedFlag", EnumBackedBool(), default=False)
     # TODO: Should this be True/False/"Failed"? Or True/False/Null?
     AccountedFlag = Column(
         "AccountedFlag", Enum("True", "False", "Failed"), default="False"
     )
 
     __table_args__ = (
         Index("JobType", "JobType"),
         Index("JobGroup", "JobGroup"),
-        Index("JobSplitType", "JobSplitType"),
         Index("Site", "Site"),
         Index("Owner", "Owner"),
         Index("OwnerGroup", "OwnerGroup"),
         Index("Status", "Status"),
         Index("MinorStatus", "MinorStatus"),
         Index("ApplicationStatus", "ApplicationStatus"),
         Index("StatusSite", "Status", "Site"),
@@ -208,15 +195,14 @@
     __table_args__ = (PrimaryKeyConstraint("JobID", "SeqNum"),)
 
 
 class TaskQueues(TaskQueueDBBase):
     __tablename__ = "tq_TaskQueues"
     TQId = Column(Integer, primary_key=True)
     Owner = Column(String(255), nullable=False)
-    OwnerDN = Column(String(255))
     OwnerGroup = Column(String(32), nullable=False)
     VO = Column(String(32), nullable=False)
     CPUTime = Column(BigInteger, nullable=False)
     Priority = Column(Float, nullable=False)
     Enabled = Column(Boolean, nullable=False, default=0)
     __table_args__ = (Index("TQOwner", "Owner", "OwnerGroup", "CPUTime"),)
```

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/jobs/status_utility.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/jobs/status_utility.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/sandbox_metadata/db.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/sandbox_metadata/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
     async def upsert_owner(self, user: UserInfo) -> int:
         """Get the id of the owner from the database"""
         # TODO: Follow https://github.com/DIRACGrid/diracx/issues/49
         stmt = sqlalchemy.select(sb_Owners.OwnerID).where(
             sb_Owners.Owner == user.preferred_username,
             sb_Owners.OwnerGroup == user.dirac_group,
-            # TODO: Add VO
+            sb_Owners.VO == user.vo,
         )
         result = await self.conn.execute(stmt)
         if owner_id := result.scalar_one_or_none():
             return owner_id
 
         stmt = sqlalchemy.insert(sb_Owners).values(
             Owner=user.preferred_username,
             OwnerGroup=user.dirac_group,
+            VO=user.vo,
         )
         result = await self.conn.execute(stmt)
         return result.lastrowid
 
     @staticmethod
     def get_pfn(bucket_name: str, user: UserInfo, sandbox_info: SandboxInfo) -> str:
         """Get the sandbox's user namespaced and content addressed PFN"""
```

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/sandbox_metadata/schema.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/sandbox_metadata/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 class sb_Owners(Base):
     __tablename__ = "sb_Owners"
     OwnerID = Column(Integer, autoincrement=True)
     Owner = Column(String(32))
     OwnerGroup = Column(String(32))
+    VO = Column(String(64))
     __table_args__ = (PrimaryKeyConstraint("OwnerID"),)
 
 
 class sb_SandBoxes(Base):
     __tablename__ = "sb_SandBoxes"
     SBId = Column(Integer, autoincrement=True)
     OwnerId = Column(Integer)
```

### Comparing `diracx-db-0.0.1a8/src/diracx/db/sql/utils.py` & `diracx-db-0.0.1a9/src/diracx/db/sql/utils.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/src/diracx_db.egg-info/PKG-INFO` & `diracx-db-0.0.1a9/src/diracx_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-db
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-db-0.0.1a8/src/diracx_db.egg-info/SOURCES.txt` & `diracx-db-0.0.1a9/src/diracx_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/auth/test_authorization_flow.py` & `diracx-db-0.0.1a9/tests/auth/test_authorization_flow.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/auth/test_device_flow.py` & `diracx-db-0.0.1a9/tests/auth/test_device_flow.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/auth/test_refresh_token.py` & `diracx-db-0.0.1a9/tests/auth/test_refresh_token.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/jobs/test_jobDB.py` & `diracx-db-0.0.1a9/tests/jobs/test_jobDB.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/jobs/test_jobLoggingDB.py` & `diracx-db-0.0.1a9/tests/jobs/test_jobLoggingDB.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/opensearch/test_connection.py` & `diracx-db-0.0.1a9/tests/opensearch/test_connection.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/opensearch/test_index_template.py` & `diracx-db-0.0.1a9/tests/opensearch/test_index_template.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/opensearch/test_search.py` & `diracx-db-0.0.1a9/tests/opensearch/test_search.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/test_dummyDB.py` & `diracx-db-0.0.1a9/tests/test_dummyDB.py`

 * *Files identical despite different names*

### Comparing `diracx-db-0.0.1a8/tests/test_sandbox_metadata.py` & `diracx-db-0.0.1a9/tests/test_sandbox_metadata.py`

 * *Files identical despite different names*

