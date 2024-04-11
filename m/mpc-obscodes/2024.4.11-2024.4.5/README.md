# Comparing `tmp/mpc_obscodes-2024.4.11.tar.gz` & `tmp/mpc_obscodes-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2024.4.11.tar", last modified: Thu Apr 11 02:23:07 2024, max compression
+gzip compressed data, was "mpc_obscodes-2024.4.5.tar", last modified: Fri Apr  5 02:22:26 2024, max compression
```

## Comparing `mpc_obscodes-2024.4.11.tar` & `mpc_obscodes-2024.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:23:07.316976 mpc_obscodes-2024.4.11/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-11 02:23:07.316976 mpc_obscodes-2024.4.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:23:07.316976 mpc_obscodes-2024.4.11/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)   253456 2024-04-11 02:23:02.000000 mpc_obscodes-2024.4.11/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 02:23:02.000000 mpc_obscodes-2024.4.11/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:23:07.316976 mpc_obscodes-2024.4.11/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-11 02:22:59.000000 mpc_obscodes-2024.4.11/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:23:07.316976 mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-11 02:23:07.000000 mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 02:23:07.000000 mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:23:07.000000 mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 02:23:07.000000 mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 02:23:07.000000 mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 02:23:02.000000 mpc_obscodes-2024.4.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:23:07.316976 mpc_obscodes-2024.4.11/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.240371 mpc_obscodes-2024.4.5/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253345 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/setup.cfg
```

### Comparing `mpc_obscodes-2024.4.11/PKG-INFO` & `mpc_obscodes-2024.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.4.11
+Version: 2024.4.5
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.4.11/README.md` & `mpc_obscodes-2024.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes/compare.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes/fetch.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996009577015164%*

 * *Differences: {'delete': "['Y84']"}*

```diff
@@ -14278,20 +14278,14 @@
     },
     "Y66": {
         "Longitude": 343.49053,
         "Name": "Two-Meter Twin Telescope, TTT2, Teide",
         "cos": 0.881484,
         "sin": 0.471429
     },
-    "Y84": {
-        "Longitude": 358.11972,
-        "Name": "Observatoire de Saint Domineuc",
-        "cos": 0.665503,
-        "sin": 0.743909
-    },
     "Y85": {
         "Longitude": 351.85389,
         "Name": "Magalofes Observatory, Fene",
         "cos": 0.727084,
         "sin": 0.684321
     },
     "Y86": {
```

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.11/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.4.11
+Version: 2024.4.5
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.4.11/pyproject.toml` & `mpc_obscodes-2024.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2024.04.11"
+version = "2024.04.05"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

