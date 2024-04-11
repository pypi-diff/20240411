# Comparing `tmp/dissect.sql-3.9.dev3.tar.gz` & `tmp/dissect.sql-3.9.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.sql-3.9.dev3.tar", last modified: Thu Mar 21 10:17:07 2024, max compression
+gzip compressed data, was "dissect.sql-3.9.dev4.tar", last modified: Thu Mar 28 17:22:34 2024, max compression
```

## Comparing `dissect.sql-3.9.dev3.tar` & `dissect.sql-3.9.dev4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.671195 dissect.sql-3.9.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/dissect/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/dissect/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/dissect/sql/c_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/dissect/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/dissect/sql/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/dissect/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/dissect.sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-21 10:17:07.000000 dissect.sql-3.9.dev3/dissect.sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-21 10:17:07.000000 dissect.sql-3.9.dev3/dissect.sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:17:07.000000 dissect.sql-3.9.dev3/dissect.sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:17:07.000000 dissect.sql-3.9.dev3/dissect.sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:17:07.000000 dissect.sql-3.9.dev3/dissect.sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-21 10:17:02.000000 dissect.sql-3.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/data/test.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:07.675195 dissect.sql-3.9.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/test_default_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/test_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 10:16:56.000000 dissect.sql-3.9.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.969449 dissect.sql-3.9.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-28 17:22:34.969449 dissect.sql-3.9.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.961449 dissect.sql-3.9.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.965449 dissect.sql-3.9.dev4/dissect/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/dissect/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/dissect/sql/c_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/dissect/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/dissect/sql/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/dissect/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.969449 dissect.sql-3.9.dev4/dissect.sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-03-28 17:22:34.000000 dissect.sql-3.9.dev4/dissect.sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-28 17:22:34.000000 dissect.sql-3.9.dev4/dissect.sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:22:34.000000 dissect.sql-3.9.dev4/dissect.sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:22:34.000000 dissect.sql-3.9.dev4/dissect.sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:22:34.000000 dissect.sql-3.9.dev4/dissect.sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-28 17:22:30.000000 dissect.sql-3.9.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:22:34.969449 dissect.sql-3.9.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.965449 dissect.sql-3.9.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.965449 dissect.sql-3.9.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/data/test.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:34.965449 dissect.sql-3.9.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/test_default_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:22:26.000000 dissect.sql-3.9.dev4/tox.ini
```

### Comparing `dissect.sql-3.9.dev3/LICENSE` & `dissect.sql-3.9.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/PKG-INFO` & `dissect.sql-3.9.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.sql-3.9.dev3/README.md` & `dissect.sql-3.9.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/dissect/sql/c_sqlite3.py` & `dissect.sql-3.9.dev4/dissect/sql/c_sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/dissect/sql/sqlite3.py` & `dissect.sql-3.9.dev4/dissect/sql/sqlite3.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/dissect/sql/utils.py` & `dissect.sql-3.9.dev4/dissect/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/dissect.sql.egg-info/PKG-INFO` & `dissect.sql-3.9.dev4/dissect.sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.sql
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing a parsers for the SQLite database file format, commonly used by applications to store configuration data
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.sql
 Project-URL: repository, https://github.com/fox-it/dissect.sql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.sql-3.9.dev3/dissect.sql.egg-info/SOURCES.txt` & `dissect.sql-3.9.dev4/dissect.sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/pyproject.toml` & `dissect.sql-3.9.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/data/test.sqlite` & `dissect.sql-3.9.dev4/tests/data/test.sqlite`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/docs/Makefile` & `dissect.sql-3.9.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/docs/conf.py` & `dissect.sql-3.9.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/test_default_values.py` & `dissect.sql-3.9.dev4/tests/test_default_values.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/test_row.py` & `dissect.sql-3.9.dev4/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/test_sqlite.py` & `dissect.sql-3.9.dev4/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tests/test_utils.py` & `dissect.sql-3.9.dev4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dissect.sql-3.9.dev3/tox.ini` & `dissect.sql-3.9.dev4/tox.ini`

 * *Files identical despite different names*

