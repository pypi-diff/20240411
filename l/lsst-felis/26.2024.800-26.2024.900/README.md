# Comparing `tmp/lsst-felis-26.2024.800.tar.gz` & `tmp/lsst-felis-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-felis-26.2024.800.tar", last modified: Thu Feb 22 10:42:21 2024, max compression
+gzip compressed data, was "lsst-felis-26.2024.900.tar", last modified: Thu Feb 29 10:20:00 2024, max compression
```

## Comparing `lsst-felis-26.2024.800.tar` & `lsst-felis-26.2024.900.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:21.848844 lsst-felis-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-22 10:42:21.848844 lsst-felis-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:21.840844 lsst-felis-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:21.844844 lsst-felis-26.2024.800/python/felis/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:21.844844 lsst-felis-26.2024.800/python/felis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/db/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    17704 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/felis/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/python/felis/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:21.848844 lsst-felis-26.2024.800/python/lsst_felis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:21.000000 lsst-felis-26.2024.800/python/lsst_felis.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-22 10:42:21.848844 lsst-felis-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:21.848844 lsst-felis-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19080 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-02-22 10:42:05.000000 lsst-felis-26.2024.800/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.960162 lsst-felis-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.964162 lsst-felis-26.2024.900/python/felis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.964162 lsst-felis-26.2024.900/python/felis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/db/sqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17704 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/felis/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/python/felis/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/python/lsst_felis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:00.000000 lsst-felis-26.2024.900/python/lsst_felis.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 10:20:00.968162 lsst-felis-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:00.964162 lsst-felis-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19080 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-02-29 10:19:51.000000 lsst-felis-26.2024.900/tests/test_validation.py
```

### Comparing `lsst-felis-26.2024.800/LICENSE` & `lsst-felis-26.2024.900/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/PKG-INFO` & `lsst-felis-26.2024.900/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `lsst-felis-26.2024.800/README.rst` & `lsst-felis-26.2024.900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/pyproject.toml` & `lsst-felis-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/__init__.py` & `lsst-felis-26.2024.900/python/felis/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/check.py` & `lsst-felis-26.2024.900/python/felis/check.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/cli.py` & `lsst-felis-26.2024.900/python/felis/cli.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/datamodel.py` & `lsst-felis-26.2024.900/python/felis/datamodel.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/db/sqltypes.py` & `lsst-felis-26.2024.900/python/felis/db/sqltypes.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/simple.py` & `lsst-felis-26.2024.900/python/felis/simple.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/sql.py` & `lsst-felis-26.2024.900/python/felis/sql.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/tap.py` & `lsst-felis-26.2024.900/python/felis/tap.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/types.py` & `lsst-felis-26.2024.900/python/felis/types.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/utils.py` & `lsst-felis-26.2024.900/python/felis/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/validation.py` & `lsst-felis-26.2024.900/python/felis/validation.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/felis/visitor.py` & `lsst-felis-26.2024.900/python/felis/visitor.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/python/lsst_felis.egg-info/PKG-INFO` & `lsst-felis-26.2024.900/python/lsst_felis.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `lsst-felis-26.2024.800/python/lsst_felis.egg-info/SOURCES.txt` & `lsst-felis-26.2024.900/python/lsst_felis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_check.py` & `lsst-felis-26.2024.900/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_cli.py` & `lsst-felis-26.2024.900/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_datamodel.py` & `lsst-felis-26.2024.900/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_simple.py` & `lsst-felis-26.2024.900/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_sql.py` & `lsst-felis-26.2024.900/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_tap.py` & `lsst-felis-26.2024.900/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_utils.py` & `lsst-felis-26.2024.900/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-felis-26.2024.800/tests/test_validation.py` & `lsst-felis-26.2024.900/tests/test_validation.py`

 * *Files identical despite different names*

