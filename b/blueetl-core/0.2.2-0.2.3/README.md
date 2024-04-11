# Comparing `tmp/blueetl-core-0.2.2.tar.gz` & `tmp/blueetl-core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueetl-core-0.2.2.tar", last modified: Mon Apr  8 13:23:03 2024, max compression
+gzip compressed data, was "blueetl-core-0.2.3.tar", last modified: Thu Apr 11 16:09:46 2024, max compression
```

## Comparing `blueetl-core-0.2.2.tar` & `blueetl-core-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.523795 blueetl-core-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/doc/source/_images/
--rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/_images/BlueETL.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.523795 blueetl-core-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/src/blueetl_core/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/src/blueetl_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_etl_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_etl_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_etl_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.567743 blueetl-core-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.555743 blueetl-core-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.559743 blueetl-core-0.2.3/doc/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/_images/BlueETL.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:09:46.567743 blueetl-core-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.555743 blueetl-core-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/src/blueetl_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/src/blueetl_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/src/blueetl_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 16:09:46.000000 blueetl-core-0.2.3/src/blueetl_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:46.563743 blueetl-core-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_etl_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_etl_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_etl_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19985 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-11 16:09:41.000000 blueetl-core-0.2.3/tox.ini
```

### Comparing `blueetl-core-0.2.2/.github/workflows/publish-sdist.yml` & `blueetl-core-0.2.3/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/.github/workflows/run-tox.yml` & `blueetl-core-0.2.3/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/CHANGELOG.rst` & `blueetl-core-0.2.3/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 0.2.3
+-------------
+
+Improvements
+~~~~~~~~~~~~
+
+- In ``blueetl_core.utils.is_subfilter()``, add the ``strict`` parameter.
+
 Version 0.2.2
 -------------
 
 Improvements
 ~~~~~~~~~~~~
 
 - In ``blueetl_core.parallel.isolated()``, execute the function in the same process if ``BLUEETL_JOBLIB_JOBS`` is set to ``1``.
```

### Comparing `blueetl-core-0.2.2/LICENSE.txt` & `blueetl-core-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/PKG-INFO` & `blueetl-core-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
```

### Comparing `blueetl-core-0.2.2/README.rst` & `blueetl-core-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/doc/Makefile` & `blueetl-core-0.2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/doc/source/_images/BlueETL.jpeg` & `blueetl-core-0.2.3/doc/source/_images/BlueETL.jpeg`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/doc/source/conf.py` & `blueetl-core-0.2.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/pyproject.toml` & `blueetl-core-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/src/blueetl_core/constants.py` & `blueetl-core-0.2.3/src/blueetl_core/constants.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/src/blueetl_core/etl.py` & `blueetl-core-0.2.3/src/blueetl_core/etl.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/src/blueetl_core/parallel.py` & `blueetl-core-0.2.3/src/blueetl_core/parallel.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/src/blueetl_core/utils.py` & `blueetl-core-0.2.3/src/blueetl_core/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,28 +128,40 @@
         return masks[0] if len(masks) == 1 else np.all(masks, axis=0)
     if is_list_like(value):
         return np.asarray(obj.isin(value))
     # more efficient than using isin with a list of one element
     return np.asarray(obj == value)
 
 
-def is_subfilter(left: dict, right: dict) -> bool:
+def is_subfilter(left: dict, right: dict, strict: bool = False) -> bool:
     """Return True if ``left`` is a subfilter of ``right``, False otherwise.
 
-    ``left`` is a subfilter of ``right`` if it's equal or more specific.
+    Args:
+        left: left filter dict.
+        right: right filter dict.
+        strict: if False, ``left`` is a subfilter of ``right`` if it's equal or more specific;
+            if True, ``left`` is a subfilter of ``right`` only if it's more specific.
 
     Examples:
         >>> print(is_subfilter({}, {}))
         True
+        >>> print(is_subfilter({}, {}, strict=True))
+        False
         >>> print(is_subfilter({}, {"key": 1}))
         False
         >>> print(is_subfilter({"key": 1}, {}))
         True
         >>> print(is_subfilter({"key": 1}, {"key": 1}))
         True
+        >>> print(is_subfilter({"key": 1}, {"key": 1}, strict=True))
+        False
+        >>> print(is_subfilter({"key": 1}, {"key": [1]}))
+        True
+        >>> print(is_subfilter({"key": 1}, {"key": [1]}, strict=True))
+        False
         >>> print(is_subfilter({"key": 1}, {"key": [1, 2]}))
         True
         >>> print(is_subfilter({"key": 1}, {"key": {"isin": [1, 2]}}))
         True
         >>> print(is_subfilter({"key": 1}, {"key": 2}))
         False
         >>> print(is_subfilter({"key": 1}, {"key": [2, 3]}))
@@ -174,15 +186,15 @@
             return obj
         if isinstance(obj, list):
             return {"isin": obj}
         # any other type of object is considered for equality with "isin"
         return {"isin": [obj]}
 
     def _is_subdict(d1: dict, d2: dict) -> bool:
-        """Return True if d1 is a subdict of d2."""
+        """Return True if d1 is a subdict of d2, or d1 and d2 are equal."""
         # mapping operator -> operation
         operators = {
             "ne": operator.eq,
             "le": operator.le,
             "lt": operator.le,
             "ge": operator.ge,
             "gt": operator.ge,
@@ -197,22 +209,27 @@
         # then d1 cannot be a subdict of d2
         for op, operation in operators.items():
             if op in d2 and (op not in d1 or not operation(d1[op], d2[op])):
                 unmatched_keys.add(op)
         L.debug("unmatched keys: %s", sorted(unmatched_keys))
         return len(unmatched_keys) == 0
 
+    # keys present in left, but missing or different in right
+    difference = set(left)
     for key in right:
         if key not in left:
             return False
         dict_left = _to_dict(left[key])
         dict_right = _to_dict(right[key])
+        if strict and dict_left == dict_right:
+            difference.remove(key)
+            continue
         if not _is_subdict(dict_left, dict_right):
             return False
-    return True
+    return not strict or len(difference) > 0
 
 
 def smart_concat(iterable, *, keys=None, copy=False, skip_empty=True, **kwargs):
     """Build and return a Series or a Dataframe from an iterable of objects with the same index.
 
     This is similar to ``pd.concat``, but the result is consistent even when the levels of the
     indexes are ordered differently, while ``pd.concat`` would blindly concatenate the indexes,
```

### Comparing `blueetl-core-0.2.2/src/blueetl_core.egg-info/PKG-INFO` & `blueetl-core-0.2.3/src/blueetl_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
```

### Comparing `blueetl-core-0.2.2/src/blueetl_core.egg-info/SOURCES.txt` & `blueetl-core-0.2.3/src/blueetl_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/tests/conftest.py` & `blueetl-core-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/tests/test_etl_dataframe.py` & `blueetl-core-0.2.3/tests/test_etl_dataframe.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/tests/test_etl_index.py` & `blueetl-core-0.2.3/tests/test_etl_index.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/tests/test_etl_series.py` & `blueetl-core-0.2.3/tests/test_etl_series.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/tests/test_parallel.py` & `blueetl-core-0.2.3/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.2/tests/test_utils.py` & `blueetl-core-0.2.3/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 @pytest.mark.parametrize(
     "left, right, expected",
     [
         ({}, {}, True),
         ({}, {"key": 1}, False),
         ({"key": 1}, {}, True),
         ({"key": 1}, {"key": 1}, True),
+        ({"key": 1}, {"key": [1]}, True),
         ({"key": 1}, {"key": [1, 2]}, True),
         ({"key": 1}, {"key": {"isin": [1, 2]}}, True),
         ({"key": 1}, {"key": 2}, False),
         ({"key": 1}, {"key": [2, 3]}, False),
         ({"key": 1}, {"key": {"isin": [2, 3]}}, False),
         ({"key1": 1, "key2": 2}, {"key1": 1}, True),
         ({"key1": 1}, {"key1": 1, "key2": 2}, False),
@@ -151,18 +152,60 @@
         ({"key": {"le": 3, "ge": 1}}, {"key": {"le": 4, "ge": 0}}, True),
         ({"key": 1}, {"key": {"eq": 1}}, True),
         ({"key": 1}, {"key": {"eq": 1, "isin": [1, 2]}}, True),
         ({"key": 1}, {"key": {"eq": 1, "isin": [2, 3]}}, False),
     ],
 )
 def test_is_subfilter(left, right, expected):
-    result = test_module.is_subfilter(left, right)
+    result = test_module.is_subfilter(left, right, strict=False)
     assert result == expected
 
 
+@pytest.mark.parametrize(
+    "left, right, expected",
+    [
+        ({}, {}, False),
+        ({}, {"key": 1}, False),
+        ({"key": 1}, {}, True),
+        ({"key": 1}, {"key": 1}, False),
+        ({"key": 1}, {"key": [1]}, False),
+        ({"key": 1}, {"key": [1, 2]}, True),
+        ({"key": 1}, {"key": {"isin": [1, 2]}}, True),
+        ({"key": 1}, {"key": 2}, False),
+        ({"key": 1}, {"key": [2, 3]}, False),
+        ({"key": 1}, {"key": {"isin": [2, 3]}}, False),
+        ({"key1": 1, "key2": 2}, {"key1": 1}, True),
+        ({"key1": 1}, {"key1": 1, "key2": 2}, False),
+        ({"key": {"isin": [1, 2]}}, {"key": 1}, False),
+        ({"key": {"ne": 3}}, {"key": {"ne": 3}}, False),
+        ({"key": {"ne": 3}}, {"key": {"ne": 4}}, False),
+        ({"key": {"gt": 3}}, {"key": {"gt": 2}}, True),
+        ({"key": {"gt": 3}}, {"key": {"gt": 3}}, False),
+        ({"key": {"gt": 3}}, {"key": {"gt": 4}}, False),
+        ({"key": {"ge": 3}}, {"key": {"ge": 2}}, True),
+        ({"key": {"ge": 3}}, {"key": {"ge": 3}}, False),
+        ({"key": {"ge": 3}}, {"key": {"ge": 4}}, False),
+        ({"key": {"lt": 3}}, {"key": {"lt": 2}}, False),
+        ({"key": {"lt": 3}}, {"key": {"lt": 3}}, False),
+        ({"key": {"lt": 3}}, {"key": {"lt": 4}}, True),
+        ({"key": {"le": 3}}, {"key": {"le": 2}}, False),
+        ({"key": {"le": 3}}, {"key": {"le": 3}}, False),
+        ({"key": {"le": 3}}, {"key": {"le": 4}}, True),
+        ({"key": {"le": 3, "ge": 1}}, {"key": {"le": 4}}, True),
+        ({"key": {"le": 3, "ge": 1}}, {"key": {"le": 4, "ge": 0}}, True),
+        ({"key": 1}, {"key": {"eq": 1}}, False),
+        ({"key": 1}, {"key": {"eq": 1, "isin": [1, 2]}}, False),
+        ({"key": 1}, {"key": {"eq": 1, "isin": [2, 3]}}, False),
+    ],
+)
+def test_is_subfilter_strict(left, right, expected):
+    result = test_module.is_subfilter(left, right, strict=True)
+    assert result is expected
+
+
 def test_smart_concat_series(series1):
     obj1 = series1.copy() + 1
     obj2 = series1.copy() + 2
     iterable = [obj1, obj2]
     expected = pd.Series(
         [1, 2, 3, 4, 2, 3, 4, 5],
         index=pd.MultiIndex.from_tuples(
```

### Comparing `blueetl-core-0.2.2/tox.ini` & `blueetl-core-0.2.3/tox.ini`

 * *Files identical despite different names*

