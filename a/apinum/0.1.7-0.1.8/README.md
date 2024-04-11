# Comparing `tmp/apinum-0.1.7.tar.gz` & `tmp/apinum-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinum-0.1.7.tar", last modified: Mon Dec 11 22:21:13 2023, max compression
+gzip compressed data, was "apinum-0.1.8.tar", last modified: Thu Apr 11 05:43:38 2024, max compression
```

## Comparing `apinum-0.1.7.tar` & `apinum-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 22:21:13.687073 apinum-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-11 22:21:02.000000 apinum-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-11 22:21:13.687073 apinum-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-11 22:21:02.000000 apinum-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-11 22:21:02.000000 apinum-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 22:21:13.687073 apinum-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 22:21:13.683073 apinum-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 22:21:13.683073 apinum-0.1.7/src/apinum/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-11 22:21:02.000000 apinum-0.1.7/src/apinum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2023-12-11 22:21:02.000000 apinum-0.1.7/src/apinum/apinum.py
--rw-r--r--   0 runner    (1001) docker     (127)   144788 2023-12-11 22:21:02.000000 apinum-0.1.7/src/apinum/well_number_to_state_county.json
--rw-r--r--   0 runner    (1001) docker     (127)    49802 2023-12-11 22:21:02.000000 apinum-0.1.7/src/apinum/well_numbers.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 22:21:13.687073 apinum-0.1.7/src/apinum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-11 22:21:13.000000 apinum-0.1.7/src/apinum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-11 22:21:13.000000 apinum-0.1.7/src/apinum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 22:21:13.000000 apinum-0.1.7/src/apinum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-11 22:21:13.000000 apinum-0.1.7/src/apinum.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-11 22:21:13.000000 apinum-0.1.7/src/apinum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 22:21:13.687073 apinum-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-12-11 22:21:02.000000 apinum-0.1.7/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:43:38.804427 apinum-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 05:43:34.000000 apinum-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-11 05:43:38.804427 apinum-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-11 05:43:34.000000 apinum-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-11 05:43:34.000000 apinum-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:43:38.804427 apinum-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:43:38.800427 apinum-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:43:38.804427 apinum-0.1.8/src/apinum/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 05:43:34.000000 apinum-0.1.8/src/apinum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-11 05:43:34.000000 apinum-0.1.8/src/apinum/apinum.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144788 2024-04-11 05:43:34.000000 apinum-0.1.8/src/apinum/well_number_to_state_county.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49802 2024-04-11 05:43:34.000000 apinum-0.1.8/src/apinum/well_numbers.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:43:38.804427 apinum-0.1.8/src/apinum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-11 05:43:38.000000 apinum-0.1.8/src/apinum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-11 05:43:38.000000 apinum-0.1.8/src/apinum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:43:38.000000 apinum-0.1.8/src/apinum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 05:43:38.000000 apinum-0.1.8/src/apinum.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 05:43:38.000000 apinum-0.1.8/src/apinum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:43:38.804427 apinum-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-11 05:43:34.000000 apinum-0.1.8/tests/tests.py
```

### Comparing `apinum-0.1.7/src/apinum/apinum.py` & `apinum-0.1.8/src/apinum/apinum.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 
     # If any well numbers were found, return the most commonly occurring one
     if well_numbers:
         return max(well_numbers, key=well_numbers.count)
     else:
         return None
 
-
 # def well_number_from_las(las_path: str, extract_from_path: bool = False):
 #     """
 #     Extracts the longest API or UWI well number from a LAS file.
 
 #     Args:
 #         las_path (str): The path to the LAS file.
 #         extract_from_path (bool): If True, attempts to extract the well
```

### Comparing `apinum-0.1.7/src/apinum/well_number_to_state_county.json` & `apinum-0.1.8/src/apinum/well_number_to_state_county.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.7/src/apinum/well_numbers.json` & `apinum-0.1.8/src/apinum/well_numbers.json`

 * *Files identical despite different names*

### Comparing `apinum-0.1.7/tests/tests.py` & `apinum-0.1.8/tests/tests.py`

 * *Files identical despite different names*

