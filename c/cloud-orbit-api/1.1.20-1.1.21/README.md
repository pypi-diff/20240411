# Comparing `tmp/cloud_orbit_api-1.1.20.tar.gz` & `tmp/cloud_orbit_api-1.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_orbit_api-1.1.20.tar", max compression
+gzip compressed data, was "cloud_orbit_api-1.1.21.tar", max compression
```

## Comparing `cloud_orbit_api-1.1.20.tar` & `cloud_orbit_api-1.1.21.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-04-10 07:21:02.548444 cloud_orbit_api-1.1.20/README.md
--rw-r--r--   0        0        0        0 2024-04-10 07:21:02.548444 cloud_orbit_api-1.1.20/cloud_orbit_api/__init__.py
--rw-r--r--   0        0        0     1123 2024-04-10 07:21:02.548444 cloud_orbit_api-1.1.20/cloud_orbit_api/db_factory.py
--rw-r--r--   0        0        0     2112 2024-04-10 07:21:02.548444 cloud_orbit_api-1.1.20/cloud_orbit_api/main.py
--rw-r--r--   0        0        0       90 2024-04-10 07:21:02.548444 cloud_orbit_api-1.1.20/cloud_orbit_api/models.py
--rw-r--r--   0        0        0      494 2024-04-10 07:21:14.952371 cloud_orbit_api-1.1.20/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 cloud_orbit_api-1.1.20/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-11 07:28:25.786321 cloud_orbit_api-1.1.21/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 07:28:25.786321 cloud_orbit_api-1.1.21/cloud_orbit_api/__init__.py
+-rw-r--r--   0        0        0     1123 2024-04-11 07:28:25.786321 cloud_orbit_api-1.1.21/cloud_orbit_api/db_factory.py
+-rw-r--r--   0        0        0     2112 2024-04-11 07:28:25.786321 cloud_orbit_api-1.1.21/cloud_orbit_api/main.py
+-rw-r--r--   0        0        0       90 2024-04-11 07:28:25.786321 cloud_orbit_api-1.1.21/cloud_orbit_api/models.py
+-rw-r--r--   0        0        0      494 2024-04-11 07:28:43.902350 cloud_orbit_api-1.1.21/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 cloud_orbit_api-1.1.21/PKG-INFO
```

### Comparing `cloud_orbit_api-1.1.20/cloud_orbit_api/db_factory.py` & `cloud_orbit_api-1.1.21/cloud_orbit_api/db_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_orbit_api-1.1.20/cloud_orbit_api/main.py` & `cloud_orbit_api-1.1.21/cloud_orbit_api/main.py`

 * *Files identical despite different names*

### Comparing `cloud_orbit_api-1.1.20/PKG-INFO` & `cloud_orbit_api-1.1.21/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-orbit-api
-Version: 1.1.20
+Version: 1.1.21
 Summary: This a demo project
 Author: sukruth grandhi
 Author-email: sukruthgrandhi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

