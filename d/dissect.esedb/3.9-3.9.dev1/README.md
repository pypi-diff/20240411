# Comparing `tmp/dissect.esedb-3.9.tar.gz` & `tmp/dissect.esedb-3.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.esedb-3.9.tar", last modified: Tue Sep 26 13:10:36 2023, max compression
+gzip compressed data, was "dissect.esedb-3.9.dev1.tar", last modified: Mon Sep  4 17:20:43 2023, max compression
```

## Comparing `dissect.esedb-3.9.tar` & `dissect.esedb-3.9.dev1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.680239 dissect.esedb-3.9/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-09-26 13:10:18.000000 dissect.esedb-3.9/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2023-09-26 13:10:18.000000 dissect.esedb-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-26 13:10:18.000000 dissect.esedb-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2023-09-26 13:10:36.680239 dissect.esedb-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-09-26 13:10:18.000000 dissect.esedb-3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.664238 dissect.esedb-3.9/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.672238 dissect.esedb-3.9/dissect/esedb/
--rwxr-xr-x   0 runner    (1001) docker     (127)      308 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23922 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/c_esedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/cursor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3357 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/esedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/lcmapstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/page.py
--rw-r--r--   0 runner    (1001) docker     (127)    18033 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/record.py
--rw-r--r--   0 runner    (1001) docker     (127)   819383 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/sorting_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.672238 dissect.esedb-3.9/dissect/esedb/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/tools/impacket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/tools/sru.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-09-26 13:10:18.000000 dissect.esedb-3.9/dissect/esedb/tools/ual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.668238 dissect.esedb-3.9/dissect.esedb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2023-09-26 13:10:36.000000 dissect.esedb-3.9/dissect.esedb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-09-26 13:10:36.000000 dissect.esedb-3.9/dissect.esedb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 13:10:36.000000 dissect.esedb-3.9/dissect.esedb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-09-26 13:10:36.000000 dissect.esedb-3.9/dissect.esedb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-26 13:10:36.000000 dissect.esedb-3.9/dissect.esedb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-09-26 13:10:18.000000 dissect.esedb-3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 13:10:36.680239 dissect.esedb-3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.672238 dissect.esedb-3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.676239 dissect.esedb-3.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    56705 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/Current.mdb.gz
--rw-r--r--   0 runner    (1001) docker     (127)    52655 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/SRUDB.dat.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)     9771 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/basic.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)     9913 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/binary.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)    10431 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/default.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)    12993 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/index.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)  2009304 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/large.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)    12291 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/multi.edb.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)    11790 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/data/text.edb.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 13:10:36.676239 dissect.esedb-3.9/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15519 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/test_esedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/test_sru.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tests/test_ual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-09-26 13:10:18.000000 dissect.esedb-3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.663970 dissect.esedb-3.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (999)      314 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (999)    11341 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)       48 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     3715 2023-09-04 17:20:43.663970 dissect.esedb-3.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2601 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.647968 dissect.esedb-3.9.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.655969 dissect.esedb-3.9.dev1/dissect/esedb/
+-rwxr-xr-x   0 runner    (1001) docker     (999)      308 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    23922 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/c_esedb.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2047 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/compression.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4528 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/cursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)     3357 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/esedb.py
+-rw-r--r--   0 runner    (1001) docker     (999)      162 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8991 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/index.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6972 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/lcmapstring.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7977 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/page.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18033 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/record.py
+-rw-r--r--   0 runner    (1001) docker     (999)   819383 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/sorting_table.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10945 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/table.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.655969 dissect.esedb-3.9.dev1/dissect/esedb/tools/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2138 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/tools/impacket.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5776 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/tools/sru.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2959 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/dissect/esedb/tools/ual.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.651969 dissect.esedb-3.9.dev1/dissect.esedb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3715 2023-09-04 17:20:43.000000 dissect.esedb-3.9.dev1/dissect.esedb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-09-04 17:20:43.000000 dissect.esedb-3.9.dev1/dissect.esedb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 17:20:43.000000 dissect.esedb-3.9.dev1/dissect.esedb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       65 2023-09-04 17:20:43.000000 dissect.esedb-3.9.dev1/dissect.esedb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        8 2023-09-04 17:20:43.000000 dissect.esedb-3.9.dev1/dissect.esedb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     1537 2023-09-04 17:20:31.000000 dissect.esedb-3.9.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 17:20:43.663970 dissect.esedb-3.9.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.655969 dissect.esedb-3.9.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.659969 dissect.esedb-3.9.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (999)    56705 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/Current.mdb.gz
+-rw-r--r--   0 runner    (1001) docker     (999)    52655 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/SRUDB.dat.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)     9771 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/basic.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)     9913 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/binary.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)    10431 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/default.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)    12993 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/index.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)  2009304 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/large.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)    12291 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/multi.edb.gz
+-rwxr-xr-x   0 runner    (1001) docker     (999)    11790 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/data/text.edb.gz
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:20:43.663970 dissect.esedb-3.9.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (999)      749 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (999)      785 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (999)       90 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    15519 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/test_esedb.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3203 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1097 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (999)      150 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/test_sru.py
+-rw-r--r--   0 runner    (1001) docker     (999)      399 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tests/test_ual.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1751 2023-09-04 17:20:26.000000 dissect.esedb-3.9.dev1/tox.ini
```

### Comparing `dissect.esedb-3.9/LICENSE` & `dissect.esedb-3.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/PKG-INFO` & `dissect.esedb-3.9.dev1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.esedb
-Version: 3.9
+Version: 3.9.dev1
 Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
 Project-URL: repository, https://github.com/fox-it/dissect.esedb
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,14 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
-Requires-Dist: dissect.cstruct<4.0.dev,>=3.4.dev
-Requires-Dist: dissect.util<4.0.dev,>=3.5.dev
 
 # dissect.esedb
 
 A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in
 Active Directory, Exchange and Windows Update. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.esedb/index.html).
```

### Comparing `dissect.esedb-3.9/README.md` & `dissect.esedb-3.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/c_esedb.py` & `dissect.esedb-3.9.dev1/dissect/esedb/c_esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/compression.py` & `dissect.esedb-3.9.dev1/dissect/esedb/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/cursor.py` & `dissect.esedb-3.9.dev1/dissect/esedb/cursor.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/esedb.py` & `dissect.esedb-3.9.dev1/dissect/esedb/esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/index.py` & `dissect.esedb-3.9.dev1/dissect/esedb/index.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/lcmapstring.py` & `dissect.esedb-3.9.dev1/dissect/esedb/lcmapstring.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/page.py` & `dissect.esedb-3.9.dev1/dissect/esedb/page.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/record.py` & `dissect.esedb-3.9.dev1/dissect/esedb/record.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/sorting_table.py` & `dissect.esedb-3.9.dev1/dissect/esedb/sorting_table.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/table.py` & `dissect.esedb-3.9.dev1/dissect/esedb/table.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/tools/impacket.py` & `dissect.esedb-3.9.dev1/dissect/esedb/tools/impacket.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/tools/sru.py` & `dissect.esedb-3.9.dev1/dissect/esedb/tools/sru.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect/esedb/tools/ual.py` & `dissect.esedb-3.9.dev1/dissect/esedb/tools/ual.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/dissect.esedb.egg-info/PKG-INFO` & `dissect.esedb-3.9.dev1/dissect.esedb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.esedb
-Version: 3.9
+Version: 3.9.dev1
 Summary: A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in Active Directory, Exchange and Windows Update
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.esedb
 Project-URL: repository, https://github.com/fox-it/dissect.esedb
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,14 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYRIGHT
-Requires-Dist: dissect.cstruct<4.0.dev,>=3.4.dev
-Requires-Dist: dissect.util<4.0.dev,>=3.5.dev
 
 # dissect.esedb
 
 A Dissect module implementing a parser for Microsofts Extensible Storage Engine Database (ESEDB), used for example in
 Active Directory, Exchange and Windows Update. For more information, please see [the
 documentation](https://docs.dissect.tools/en/latest/projects/dissect.esedb/index.html).
```

### Comparing `dissect.esedb-3.9/dissect.esedb.egg-info/SOURCES.txt` & `dissect.esedb-3.9.dev1/dissect.esedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/pyproject.toml` & `dissect.esedb-3.9.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -46,7 +46,8 @@
 [tool.setuptools]
 license-files = ["LICENSE", "COPYRIGHT"]
 
 [tool.setuptools.packages.find]
 include = ["dissect.*"]
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
```

### Comparing `dissect.esedb-3.9/tests/conftest.py` & `dissect.esedb-3.9.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/Current.mdb.gz` & `dissect.esedb-3.9.dev1/tests/data/Current.mdb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/SRUDB.dat.gz` & `dissect.esedb-3.9.dev1/tests/data/SRUDB.dat.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/basic.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/basic.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/binary.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/binary.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/default.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/default.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/index.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/index.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/large.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/large.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/multi.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/multi.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/data/text.edb.gz` & `dissect.esedb-3.9.dev1/tests/data/text.edb.gz`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/docs/Makefile` & `dissect.esedb-3.9.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/docs/conf.py` & `dissect.esedb-3.9.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/test_esedb.py` & `dissect.esedb-3.9.dev1/tests/test_esedb.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/test_index.py` & `dissect.esedb-3.9.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tests/test_record.py` & `dissect.esedb-3.9.dev1/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `dissect.esedb-3.9/tox.ini` & `dissect.esedb-3.9.dev1/tox.ini`

 * *Files identical despite different names*

