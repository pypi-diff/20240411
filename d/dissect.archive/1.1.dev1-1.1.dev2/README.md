# Comparing `tmp/dissect.archive-1.1.dev1.tar.gz` & `tmp/dissect.archive-1.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.archive-1.1.dev1.tar", last modified: Thu Mar 28 17:21:35 2024, max compression
+gzip compressed data, was "dissect.archive-1.1.dev2.tar", last modified: Thu Apr 11 11:56:17 2024, max compression
```

## Comparing `dissect.archive-1.1.dev1.tar` & `dissect.archive-1.1.dev2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:35.869384 dissect.archive-1.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-28 17:21:35.869384 dissect.archive-1.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:35.865384 dissect.archive-1.1.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:35.865384 dissect.archive-1.1.dev1/dissect/archive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/dissect/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/dissect/archive/c_wim.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/dissect/archive/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/dissect/archive/wim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:35.869384 dissect.archive-1.1.dev1/dissect.archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-28 17:21:35.000000 dissect.archive-1.1.dev1/dissect.archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-28 17:21:35.000000 dissect.archive-1.1.dev1/dissect.archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:35.000000 dissect.archive-1.1.dev1/dissect.archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:21:35.000000 dissect.archive-1.1.dev1/dissect.archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:35.000000 dissect.archive-1.1.dev1/dissect.archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-28 17:21:29.000000 dissect.archive-1.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:35.869384 dissect.archive-1.1.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:35.869384 dissect.archive-1.1.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 17:21:21.000000 dissect.archive-1.1.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:35.869384 dissect.archive-1.1.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-28 17:21:23.000000 dissect.archive-1.1.dev1/tests/data/basic.wim.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-28 17:21:22.000000 dissect.archive-1.1.dev1/tests/test_wim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-28 17:21:22.000000 dissect.archive-1.1.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:17.557018 dissect.archive-1.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-11 11:56:17.557018 dissect.archive-1.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:17.549018 dissect.archive-1.1.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:17.553017 dissect.archive-1.1.dev2/dissect/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/dissect/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/dissect/archive/c_wim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/dissect/archive/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/dissect/archive/wim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:17.557018 dissect.archive-1.1.dev2/dissect.archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-11 11:56:17.000000 dissect.archive-1.1.dev2/dissect.archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 11:56:17.000000 dissect.archive-1.1.dev2/dissect.archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:17.000000 dissect.archive-1.1.dev2/dissect.archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:17.000000 dissect.archive-1.1.dev2/dissect.archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:17.000000 dissect.archive-1.1.dev2/dissect.archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 11:56:12.000000 dissect.archive-1.1.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:17.557018 dissect.archive-1.1.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:17.553017 dissect.archive-1.1.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:17.557018 dissect.archive-1.1.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-11 11:56:08.000000 dissect.archive-1.1.dev2/tests/data/basic.wim.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/tests/test_wim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-11 11:56:07.000000 dissect.archive-1.1.dev2/tox.ini
```

### Comparing `dissect.archive-1.1.dev1/LICENSE` & `dissect.archive-1.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/PKG-INFO` & `dissect.archive-1.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.archive
-Version: 1.1.dev1
+Version: 1.1.dev2
 Summary: A Dissect module implementing parsers for various archive and backup formats
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.archive
 Project-URL: repository, https://github.com/fox-it/dissect.archive
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.archive-1.1.dev1/README.md` & `dissect.archive-1.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/dissect/archive/c_wim.py` & `dissect.archive-1.1.dev2/dissect/archive/c_wim.py`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/dissect/archive/wim.py` & `dissect.archive-1.1.dev2/dissect/archive/wim.py`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/dissect.archive.egg-info/PKG-INFO` & `dissect.archive-1.1.dev2/dissect.archive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.archive
-Version: 1.1.dev1
+Version: 1.1.dev2
 Summary: A Dissect module implementing parsers for various archive and backup formats
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.archive
 Project-URL: repository, https://github.com/fox-it/dissect.archive
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.archive-1.1.dev1/pyproject.toml` & `dissect.archive-1.1.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/tests/conftest.py` & `dissect.archive-1.1.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/tests/data/basic.wim.gz` & `dissect.archive-1.1.dev2/tests/data/basic.wim.gz`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/tests/test_wim.py` & `dissect.archive-1.1.dev2/tests/test_wim.py`

 * *Files identical despite different names*

### Comparing `dissect.archive-1.1.dev1/tox.ini` & `dissect.archive-1.1.dev2/tox.ini`

 * *Files identical despite different names*

