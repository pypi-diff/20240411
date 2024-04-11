# Comparing `tmp/diracx-testing-0.0.1a8.tar.gz` & `tmp/diracx-testing-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-testing-0.0.1a8.tar", last modified: Thu Nov 30 08:40:51 2023, max compression
+gzip compressed data, was "diracx-testing-0.0.1a9.tar", last modified: Sun Jan 28 09:12:38 2024, max compression
```

## Comparing `diracx-testing-0.0.1a8.tar` & `diracx-testing-0.0.1a9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:51.425829 diracx-testing-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-11-30 08:40:51.425829 diracx-testing-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-testing-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-30 08:39:21.000000 diracx-testing-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:40:51.425829 diracx-testing-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:51.421829 diracx-testing-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:51.421829 diracx-testing-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:51.421829 diracx-testing-0.0.1a8/src/diracx/testing/
--rw-r--r--   0 runner    (1001) docker     (127)    14173 2023-11-30 08:39:21.000000 diracx-testing-0.0.1a8/src/diracx/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-11-30 08:39:21.000000 diracx-testing-0.0.1a8/src/diracx/testing/osdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:51.425829 diracx-testing-0.0.1a8/src/diracx_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-11-30 08:40:51.000000 diracx-testing-0.0.1a8/src/diracx_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-11-30 08:40:51.000000 diracx-testing-0.0.1a8/src/diracx_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:40:51.000000 diracx-testing-0.0.1a8/src/diracx_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-30 08:40:51.000000 diracx-testing-0.0.1a8/src/diracx_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:40:51.000000 diracx-testing-0.0.1a8/src/diracx_testing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-testing-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-28 09:11:11.000000 diracx-testing-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/src/diracx/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)    19026 2024-01-28 09:11:11.000000 diracx-testing-0.0.1a9/src/diracx/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-01-28 09:11:11.000000 diracx-testing-0.0.1a9/src/diracx/testing/osdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:38.144932 diracx-testing-0.0.1a9/src/diracx_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-28 09:12:38.000000 diracx-testing-0.0.1a9/src/diracx_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-28 09:12:38.000000 diracx-testing-0.0.1a9/src/diracx_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:12:38.000000 diracx-testing-0.0.1a9/src/diracx_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-28 09:12:38.000000 diracx-testing-0.0.1a9/src/diracx_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:12:38.000000 diracx-testing-0.0.1a9/src/diracx_testing.egg-info/top_level.txt
```

### Comparing `diracx-testing-0.0.1a8/PKG-INFO` & `diracx-testing-0.0.1a9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: diracx-testing
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytest-cov
+Requires-Dist: pytest-xdist
 Provides-Extra: testing
 Requires-Dist: diracx-testing; extra == "testing"
```

### Comparing `diracx-testing-0.0.1a8/pyproject.toml` & `diracx-testing-0.0.1a9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Distributed Computing",
 ]
 dependencies = [
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
+    "pytest-xdist",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 testing = [
     "diracx-testing",
 ]
```

### Comparing `diracx-testing-0.0.1a8/src/diracx/testing/osdb.py` & `diracx-testing-0.0.1a9/src/diracx/testing/osdb.py`

 * *Files identical despite different names*

### Comparing `diracx-testing-0.0.1a8/src/diracx_testing.egg-info/PKG-INFO` & `diracx-testing-0.0.1a9/src/diracx_testing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: diracx-testing
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: TODO
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytest-cov
+Requires-Dist: pytest-xdist
 Provides-Extra: testing
 Requires-Dist: diracx-testing; extra == "testing"
```

