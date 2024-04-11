# Comparing `tmp/pycommons-0.8.8.tar.gz` & `tmp/pycommons-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons-0.8.8.tar", last modified: Thu Mar  7 00:21:17 2024, max compression
+gzip compressed data, was "pycommons-0.8.9.tar", last modified: Fri Mar  8 01:18:29 2024, max compression
```

## Comparing `pycommons-0.8.8.tar` & `pycommons-0.8.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-07 00:21:17.758721 pycommons-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-03-07 00:18:39.000000 pycommons-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.750721 pycommons-0.8.8/pycommons/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.754721 pycommons-0.8.8/pycommons/dev/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.754721 pycommons-0.8.8/pycommons/dev/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19191 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/doc/doc_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/doc/index_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)    29817 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/doc/process_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/doc/setup_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.754721 pycommons-0.8.8/pycommons/dev/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/tests/compile_and_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/tests/examples_in_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/tests/examples_in_md.py
--rw-r--r--   0 runner    (1001) docker     (127)    26694 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/dev/tests/links_in_md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.754721 pycommons-0.8.8/pycommons/ds/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/ds/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/ds/immutable_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.754721 pycommons-0.8.8/pycommons/io/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/io/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/io/console.py
--rw-r--r--   0 runner    (1001) docker     (127)    40730 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/io/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/io/temp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/pycommons/math/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/math/int_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/pycommons/net/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/net/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/pycommons/processes/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/processes/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/processes/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/pycommons/strings/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/strings/chars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/strings/enforce.py
--rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/strings/string_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/strings/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-07 00:18:39.000000 pycommons-0.8.8/pycommons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/pycommons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-07 00:21:17.000000 pycommons-0.8.8/pycommons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-07 00:21:17.000000 pycommons-0.8.8/pycommons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 00:21:17.000000 pycommons-0.8.8/pycommons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 00:21:17.000000 pycommons-0.8.8/pycommons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-07 00:21:17.000000 pycommons-0.8.8/pycommons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 00:21:17.000000 pycommons-0.8.8/pycommons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-07 00:18:39.000000 pycommons-0.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-07 00:21:17.758721 pycommons-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-07 00:18:39.000000 pycommons-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:21:17.758721 pycommons-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-07 00:18:39.000000 pycommons-0.8.8/tests/test_examples_in_examples_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-07 00:18:39.000000 pycommons-0.8.8/tests/test_examples_in_readme_md.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-07 00:18:39.000000 pycommons-0.8.8/tests/test_links_in_mds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.847769 pycommons-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-03-08 01:18:29.847769 pycommons-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-03-08 01:16:15.000000 pycommons-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.839769 pycommons-0.8.9/pycommons/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.843769 pycommons-0.8.9/pycommons/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.843769 pycommons-0.8.9/pycommons/dev/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/doc/doc_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/doc/index_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32635 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/doc/process_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/doc/setup_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.843769 pycommons-0.8.9/pycommons/dev/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/tests/compile_and_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/tests/examples_in_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/tests/examples_in_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26694 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/dev/tests/links_in_md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.843769 pycommons-0.8.9/pycommons/ds/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/ds/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/ds/immutable_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.843769 pycommons-0.8.9/pycommons/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/io/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/io/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40730 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/io/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/io/temp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.843769 pycommons-0.8.9/pycommons/math/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/math/int_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.847769 pycommons-0.8.9/pycommons/net/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/net/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.847769 pycommons-0.8.9/pycommons/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/processes/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/processes/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.847769 pycommons-0.8.9/pycommons/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/strings/chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/strings/enforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/strings/string_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/strings/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-08 01:16:15.000000 pycommons-0.8.9/pycommons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.847769 pycommons-0.8.9/pycommons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-03-08 01:18:29.000000 pycommons-0.8.9/pycommons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-08 01:18:29.000000 pycommons-0.8.9/pycommons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 01:18:29.000000 pycommons-0.8.9/pycommons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 01:18:29.000000 pycommons-0.8.9/pycommons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-08 01:18:29.000000 pycommons-0.8.9/pycommons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-08 01:18:29.000000 pycommons-0.8.9/pycommons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-08 01:16:15.000000 pycommons-0.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-08 01:18:29.847769 pycommons-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-08 01:16:15.000000 pycommons-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:18:29.847769 pycommons-0.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-08 01:16:15.000000 pycommons-0.8.9/tests/test_examples_in_examples_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-08 01:16:15.000000 pycommons-0.8.9/tests/test_examples_in_readme_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-08 01:16:15.000000 pycommons-0.8.9/tests/test_links_in_mds.py
```

### Comparing `pycommons-0.8.8/PKG-INFO` & `pycommons-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycommons
-Version: 0.8.8
+Version: 0.8.9
 Summary: A package with utility functionality for Python projects.
 Home-page: https://thomasweise.github.io/pycommons
 Author: Thomas Weise
 Author-email: tweise@ustc.edu.cn
 Maintainer: Thomas Weise
 Maintainer-email: tweise@ustc.edu.cn
 License: GPL 3.0
@@ -32,19 +32,19 @@
 [![pypi downloads](https://img.shields.io/pypi/dw/pycommons.svg)](https://pypistats.org/packages/pycommons)
 [![coverage report](https://thomasweise.github.io/pycommons/tc/badge.svg)](https://thomasweise.github.io/pycommons/tc/index.html)
 
 # *pycommons:* Common Utility Functions for Python Projects.
 
 Some common utility functionality for Python projects.
 
-- [Introduction](https://thomasweise.github.io/pycommons/index.html#introduction)
-- [Installation](https://thomasweise.github.io/pycommons/index.html#installation)
-- [Examples](https://thomasweise.github.io/pycommons/index.html#examples)
-- [License](https://thomasweise.github.io/pycommons/index.html#license)
-- [Contact](https://thomasweise.github.io/pycommons/index.html#contact)
+- [Introduction](https://thomasweise.github.io/pycommons#introduction)
+- [Installation](https://thomasweise.github.io/pycommons#installation)
+- [Examples](https://thomasweise.github.io/pycommons#examples)
+- [License](https://thomasweise.github.io/pycommons#license)
+- [Contact](https://thomasweise.github.io/pycommons#contact)
 
 
 ## 1. Introduction
 
 In this project, we combine several utilities and functions that are used in our other projects.
 
 These functions have in common that they are fail-fast.
@@ -119,18 +119,18 @@
 
 ## 4. License
 
 [`pycommons`](https://thomasweise.github.io/pycommons) is a library with utilities for Python projects.
 
 Copyright (C) 2024  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
 
-Dr. Thomas Weise (see [Contact](https://thomasweise.github.io/pycommons/index.html#contact)) holds the copyright of this package.
+Dr. Thomas Weise (see [Contact](https://thomasweise.github.io/pycommons#contact)) holds the copyright of this package.
 
 `pycommons` is provided to the public as open source software under the [GNU GENERAL PUBLIC LICENSE, Version 3, 29 June 2007](https://thomasweise.github.io/pycommons/LICENSE.html).
-Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](https://thomasweise.github.io/pycommons/index.html#contact) below).
+Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](https://thomasweise.github.io/pycommons#contact) below).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 
 Please visit the [contributions guidelines](https://thomasweise.github.io/pycommons/CONTRIBUTING.html) for `pycommons` if you would like to contribute to our package.
```

### Comparing `pycommons-0.8.8/README.md` & `pycommons-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/dev/doc/__init__.py` & `pycommons-0.8.9/pycommons/dev/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/dev/doc/doc_info.py` & `pycommons-0.8.9/pycommons/dev/doc/doc_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,16 +348,16 @@
 
     >>> from os.path import join, dirname
     >>> from contextlib import redirect_stdout
     >>> from io import StringIO
     >>> with redirect_stdout(StringIO()):
     ...     s = parse_version_py(join(dirname(dirname(dirname(__file__))),
     ...         "version.py"))
-    >>> print(s)
-    0.8.8
+    >>> print(s[:s.rindex(".")])
+    0.8
 
     >>> try:
     ...     parse_version_py(None, "v")
     ... except TypeError as te:
     ...     print(te)
     descriptor '__len__' requires a 'str' object but received a 'NoneType'
```

### Comparing `pycommons-0.8.8/pycommons/dev/doc/index_rst.py` & `pycommons-0.8.9/pycommons/dev/doc/index_rst.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/dev/doc/process_md.py` & `pycommons-0.8.9/pycommons/dev/doc/process_md.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 
 #: the separators for URLs in markdown
 __MD_URL_SEPARTORS: Final[tuple[tuple[str, str, str, str], ...]] = (
     (r'\s+href\s*=\s*"\s*', r'\s*"', ' href="', '"'),
     (r"\s+href\s*=\s*'\s*", r"\s*'", ' href="', '"'),
     (r'\s+src\s*=\s*"\s*', r'\s*"', ' src="', '"'),
     (r"\s+src\s*=\s*'\s*", r"\s*'", ' src="', '"'),
-    (r'\s*=\s*"\s*', r'\s*"', '="', '"'),
-    (r"\s*=\s*'\s*", r"\s*'", '="', '"'),
     (r"\s*\]\s*\(\s*", r"\s*\)", r"](", r")"),
     (r"<\s*", r"\s*>", "<", ">"),
 )
 
 
 def __make_base_url_replacer(
         collector: Callable[[
@@ -46,116 +44,102 @@
     ...     coll.append, "https://example.com/x", "./")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x\\/?(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x\\/?(.*)\\s*>'
     >>> sub(coll[3][0], coll[3][1], " src= ' https://example.com/x/y '")
     ' src="./y"'
     >>> sub(coll[1][0], coll[1][1], " href ='http://example.com/x/y  '")
     ' href="./y"'
     >>> sub(coll[2][0], coll[2][1], ' src ="https://example.com/x/y"')
     ' src="./y"'
     >>> sub(coll[0][0], coll[0][1], '  href ="http://example.com/x/y"')
     ' href="./y"'
-    >>> sub(coll[6][0], coll[6][1], '[l](  https://example.com/x/y)')
+    >>> sub(coll[4][0], coll[4][1], '[l](  https://example.com/x/y)')
     '[l](./y)'
-    >>> sub(coll[6][0], coll[6][1], '![xx ] (http://example.com/x/y/g.jpg)')
+    >>> sub(coll[4][0], coll[4][1], '![xx ] (http://example.com/x/y/g.jpg)')
     '![xx](./y/g.jpg)'
-    >>> sub(coll[7][0], coll[7][1], '<  https://example.com/x/y >')
+    >>> sub(coll[5][0], coll[5][1], '<  https://example.com/x/y >')
     '<./y>'
     >>> sub(coll[3][0], coll[3][1], "src='https://example.com/x/y ")
     "src='https://example.com/x/y "
 
     >>> coll = list()
     >>> __make_base_url_replacer(
     ...     coll.append, "https://example.com/x/", "./")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x\\/?(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x\\/?(.*)\\s*>'
 
     >>> coll = list()
     >>> __make_base_url_replacer(
     ...     coll.append, "https://example.com/x/", "/")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x\\/?(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x\\/?(.*)\\s*>'
 
     >>> coll = list()
     >>> __make_base_url_replacer(
     ...     coll.append, "https://example.com/x/", "bb")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x(.*)\\s*>'
 
     >>> coll = list()
     >>> __make_base_url_replacer(
     ...     coll.append, "https://example.com/x", "./")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x\\/?(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x\\/?(.*)\\s*>'
 
     >>> coll = list()
     >>> __make_base_url_replacer(
     ...     coll.append, "https://example.com/x", "/")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x\\/?(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x\\/?(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x\\/?(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x\\/?(.*)\\s*>'
 
     >>> coll = list()
     >>> __make_base_url_replacer(
     ...     coll.append, "https://example.com/x", "bb")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x(.*)\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x(.*)\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x(.*)\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x(.*)\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x(.*)\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x(.*)\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x(.*)\\s*\\)'
     '<\\s*https?://example\\.com/x(.*)\\s*>'
 
     >>> try:
     ...     __make_base_url_replacer(None, "https://example.com/x", "bb")
     ... except TypeError as te:
     ...     print(te)
@@ -236,114 +220,100 @@
     ...     coll.append, "https://example.com/x.jpg", "x.jpg")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com/x\\.jpg\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com/x\\.jpg\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com/x\\.jpg\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com/x\\.jpg\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com/x\\.jpg\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com/x\\.jpg\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com/x\\.jpg\\s*\\)'
     '<\\s*https?://example\\.com/x\\.jpg\\s*>'
     >>> sub(coll[1][0], coll[1][1], " href= ' https://example.com/x.jpg '")
     ' href="x.jpg"'
     >>> sub(coll[1][0], coll[1][1], " href='https://example.com/x.jpg  '")
     ' href="x.jpg"'
     >>> sub(coll[2][0], coll[2][1], ' src="https://example.com/x.jpg"')
     ' src="x.jpg"'
     >>> sub(coll[2][0], coll[2][1], ' src="https://example.com/x.jpg"')
     ' src="x.jpg"'
-    >>> sub(coll[6][0], coll[6][1], '[l](  https://example.com/x.jpg)')
+    >>> sub(coll[4][0], coll[4][1], '[l](  https://example.com/x.jpg)')
     '[l](x.jpg)'
-    >>> sub(coll[6][0], coll[6][1], '![xx ] (https://example.com/x.jpg)')
+    >>> sub(coll[4][0], coll[4][1], '![xx ] (https://example.com/x.jpg)')
     '![xx](x.jpg)'
-    >>> sub(coll[7][0], coll[7][1], '<  https://example.com/x.jpg>')
+    >>> sub(coll[5][0], coll[5][1], '<  https://example.com/x.jpg>')
     '<x.jpg>'
 
     >>> coll = list()
     >>> __make_full_url_replacer(
     ...     coll.append, "https://example.com/", "./x")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com\\/?\\s*\\)'
     '<\\s*https?://example\\.com\\/?\\s*>'
 
     >>> coll = list()
     >>> __make_full_url_replacer(
     ...     coll.append, "https://example.com/", "/x")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com\\/?\\s*\\)'
     '<\\s*https?://example\\.com\\/?\\s*>'
 
     >>> coll = list()
     >>> __make_full_url_replacer(
     ...     coll.append, "https://example.com/", "bb")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com\\s*\\)'
     '<\\s*https?://example\\.com\\s*>'
 
     >>> coll = list()
     >>> __make_full_url_replacer(
     ...     coll.append, "https://example.com", "./x")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com\\/?\\s*\\)'
     '<\\s*https?://example\\.com\\/?\\s*>'
 
     >>> coll = list()
     >>> __make_full_url_replacer(
     ...     coll.append, "https://example.com", "/x")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com\\/?\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com\\/?\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com\\/?\\s*\\)'
     '<\\s*https?://example\\.com\\/?\\s*>'
 
     >>> coll = list()
     >>> __make_full_url_replacer(
     ...     coll.append, "https://example.com", "bb")
     >>> for k, y in coll:
     ...     print(repr(k.pattern))
     '\\s+href\\s*=\\s*"\\s*https?://example\\.com\\s*"'
     "\\s+href\\s*=\\s*'\\s*https?://example\\.com\\s*'"
     '\\s+src\\s*=\\s*"\\s*https?://example\\.com\\s*"'
     "\\s+src\\s*=\\s*'\\s*https?://example\\.com\\s*'"
-    '\\s*=\\s*"\\s*https?://example\\.com\\s*"'
-    "\\s*=\\s*'\\s*https?://example\\.com\\s*'"
     '\\s*\\]\\s*\\(\\s*https?://example\\.com\\s*\\)'
     '<\\s*https?://example\\.com\\s*>'
 
     >>> try:
     ...     __make_full_url_replacer(None, "https://example.com", "bb")
     ... except TypeError as te:
     ...     print(te)
@@ -483,18 +453,18 @@
     replacers should be an instance of typing.Iterable but is int, namely '1'.
 
     >>> coll = list()
     >>> __make_full_url_replacer(coll.append, "https://example.com",
     ...                        "https://example.com")
     >>> f = __make_replacer(coll)
     >>> try:
-    ...     f("<a ref='http://example.com' />")
+    ...     f("<a href='http://example.com' />")
     ... except ValueError as ve:
     ...     print(str(ve)[:60])
-    Endless loop: "<a ref='http://example.com' />" -> '<a ref="h
+    Endless loop: "<a href='http://example.com' />" -> '<a href=
     """
     if not isinstance(replacers, Iterable):
         raise type_error(replacers, "replacers", Iterable)
 
     pats: Final[tuple[tuple[Pattern, Callable[[Match], str] | str],
                 ...]] = tuple(replacers)
     for pattern, replacer in pats:
@@ -518,59 +488,62 @@
             if iteration > 100:
                 raise ValueError(f"Endless loop: {text!r} -> {out_str!r}.")
         return str.rstrip(out_str)  # enforce string
 
     return cast(Callable[[str], str], __func)
 
 
-def make_url_replacer(base_urls: Mapping[str, str] | None = None,
-                      full_urls: Mapping[str, str] | None = None) \
+def __make_url_replacer(base_urls: Mapping[str, str] | None = None,
+                        full_urls: Mapping[str, str] | None = None) \
         -> Callable[[str], str]:
     r"""
     Create the url replacers that fix absolute to relative URLs.
 
     :param base_urls: a mapping of basic urls to shortcuts
     :param full_urls: a mapping of full urls to abbreviations
     :returns: a single callable that can process strings and fix the URLs
         therein
+    :raises TypeError: if any of the inputs is of the wrong type
+    :raises ValueError: if any of the inputs is incorrect
 
-    >>> f = make_url_replacer(None, None)
+    >>> f = __make_url_replacer(None, None)
     >>> f("1")
     '1'
 
-    >>> f = make_url_replacer({"https://example.com/1": "./a/",
-    ...                        "https://example.com": "./"},
-    ...                       {"https://example.com/1/1.txt": "y.txt",
-    ...                        "https://example.com/x/1.txt": "z.txt"})
+    >>> f = __make_url_replacer({"https://example.com/1": "./a/",
+    ...                          "https://example.com": "./"},
+    ...                         {"https://example.com/1/1.txt": "y.txt",
+    ...                          "https://example.com/x/1.txt": "z.txt"})
     >>> f("<a href='http://example.com/1/2.txt' />")
     '<a href="./a/2.txt" />'
     >>> f("<a href='http://example.com/1' />")
     '<a href="./a/" />'
     >>> f("<a href='http://example.com' />")
     '<a href="./" />'
     >>> f("<a href='http://example.com/x.txt' />")
     '<a href="./x.txt" />'
     >>> f("<a href='http://example.com/1/1.txt' />")
     '<a href="y.txt" />'
     >>> f("<a href='http://example.com/x/1.txt' />")
     '<a href="z.txt" />'
 
     >>> try:
-    ...     make_url_replacer(1, None)
+    ...     __make_url_replacer(1, None)
     ... except TypeError as te:
     ...     print(te)
     base_urls should be an instance of typing.Mapping but is int, namely '1'.
 
     >>> try:
-    ...     make_url_replacer(None, 1)
+    ...     __make_url_replacer(None, 1)
     ... except TypeError as te:
     ...     print(te)
     full_urls should be an instance of typing.Mapping but is int, namely '1'.
     """
     keys: list[tuple[str, bool]] = []
+
     if base_urls is not None:
         if not isinstance(base_urls, Mapping):
             raise type_error(base_urls, "base_urls", Mapping)
         keys.extend((kk, False) for kk in base_urls)
     if full_urls is not None:
         if not isinstance(full_urls, Mapping):
             raise type_error(full_urls, "full_urls", Mapping)
@@ -590,129 +563,124 @@
     return __make_replacer(mappings)
 
 
 #: detects strings of the form [xyz](#123-bla) and gives \1=xyz and \2=bla
 __FIX_LINKS: Final[Pattern] = re_compile("(\\[.+?])\\(#\\d+-(.+?)\\)")
 
 
-def process_markdown(
+def __process_markdown(
         source: Iterable[str], dest: Callable[[str], Any],
         line_processor: Callable[[str], str] = lambda s: s,
         discard_until: str | None = "## 1. Introduction") -> None:
     """
     Process a markdown file in order to make it useful for distribution.
 
     This process changes the GitHub-style markdown to a format that the myst
     parser, which is used by sphinx, can render properly. This involves
     several issues:
 
     1. We discard the top-level heading.
     2. We need to move all sub-headings one step up.
     3. Furthermore, we can turn all absolute URLs pointing to the
        documentation website to local references starting with `./`.
-    4. The myst parser drops the numerical prefixes of links, i.e., it tags
-       `## 1.2. Hello` with id `hello` instead of `12-hello`. This means that
-       we need to fix all references following the pattern `[xxx](#12-hello)`
-       to `[xxx](#hello)`.
 
     :param source: the source line iterable
     :param dest: the destination callable receiving the output
     :param line_processor: an optional callable for processing lines
     :param discard_until: discard all strings until reaching this line. If
         this is `None`, all lines will be used. If this is not `None`, then
-        this will be the first line to be forwarded to `dest`
-    :param add_images_anyway: add image lines anyway, even if other stuff
+        this will be the first line to be forwarded to `dest`f
 
     >>> lp = list()
-    >>> lpp = make_url_replacer({"https://example.com/": "./"},
+    >>> lpp = __make_url_replacer({"https://example.com/": "./"},
     ...                         {"https://example.com/A": "xyz"})
     >>> src = ["![image](https://example.com/1.jp)",
     ...        "# This is `pycommons!`",
     ...        "Table of contents",
     ...        "## 1. Introduction",
     ...        "blabla bla <https://example.com/A>!",
     ...        "## 2. Some More Text",
     ...        "We [also say](https://example.com/z/hello.txt) stuff.",
     ...        "### 2.4. Code Example",
     ...        "```",
     ...        "But [not in code](https://example.com/z/hello.txt).",
     ...        "```",
     ...        "See also [here](#24-code-example)."]
-    >>> process_markdown(src, print, lpp)
+    >>> __process_markdown(src, print, lpp)
     # 1. Introduction
     blabla bla <xyz>!
     # 2. Some More Text
     We [also say](./z/hello.txt) stuff.
     ## 2.4. Code Example
     ```
     But [not in code](https://example.com/z/hello.txt).
     ```
-    See also [here](#code-example).
+    See also [here](#24-code-example).
 
     >>> try:
-    ...     process_markdown(None, print, lambda x: x, "bla")
+    ...     __process_markdown(None, print, lambda x: x, "bla")
     ... except TypeError as te:
     ...     print(te)
     source should be an instance of typing.Iterable but is None.
 
     >>> try:
-    ...     process_markdown(1, print, lambda x: x, "bla")
+    ...     __process_markdown(1, print, lambda x: x, "bla")
     ... except TypeError as te:
     ...     print(te)
     source should be an instance of typing.Iterable but is int, namely '1'.
 
     >>> try:
-    ...     process_markdown([None], print, lambda x: x, "bla")
+    ...     __process_markdown([None], print, lambda x: x, "bla")
     ... except TypeError as te:
     ...     print(te)
     descriptor 'rstrip' for 'str' objects doesn't apply to a 'NoneType' object
 
     >>> try:
-    ...     process_markdown([1], print, lambda x: x, "bla")
+    ...     __process_markdown([1], print, lambda x: x, "bla")
     ... except TypeError as te:
     ...     print(te)
     descriptor 'rstrip' for 'str' objects doesn't apply to a 'int' object
 
     >>> try:
-    ...     process_markdown([""], None, lambda x: x, "bla")
+    ...     __process_markdown([""], None, lambda x: x, "bla")
     ... except TypeError as te:
     ...     print(te)
     dest should be a callable but is None.
 
     >>> try:
-    ...     process_markdown([""], 1, lambda x: x, "bla")
+    ...     __process_markdown([""], 1, lambda x: x, "bla")
     ... except TypeError as te:
     ...     print(te)
     dest should be a callable but is int, namely '1'.
 
     >>> try:
-    ...     process_markdown([""], print, None, "bla")
+    ...     __process_markdown([""], print, None, "bla")
     ... except TypeError as te:
     ...     print(te)
     line_processor should be a callable but is None.
 
     >>> try:
-    ...     process_markdown([""], print, 1, "bla")
+    ...     __process_markdown([""], print, 1, "bla")
     ... except TypeError as te:
     ...     print(te)
     line_processor should be a callable but is int, namely '1'.
 
     >>> try:
-    ...     process_markdown([""], print, lambda x: x, 1)
+    ...     __process_markdown([""], print, lambda x: x, 1)
     ... except TypeError as te:
     ...     print(te)
     descriptor '__len__' requires a 'str' object but received a 'int'
 
     >>> try:
-    ...     process_markdown([""], print, lambda x: x, "")
+    ...     __process_markdown([""], print, lambda x: x, "")
     ... except ValueError as ve:
     ...     print(ve)
     discard_until cannot be ''.
 
-    >>> process_markdown([""], print, lambda x: x, None)
+    >>> __process_markdown([""], print, lambda x: x, None)
     <BLANKLINE>
     """
     if not isinstance(source, Iterable):
         raise type_error(source, "source", Iterable)
     if not callable(dest):
         raise type_error(dest, "dest", call=True)
     if not callable(line_processor):
@@ -754,12 +722,135 @@
         if in_code:
             if line.startswith("```"):
                 in_code = False  # toggle to non-code
         elif line.startswith("```"):
             in_code = True  # toggle to code
         elif line.startswith("#"):
             line = line[1:]  # move all sub-headings one step up
-        else:  # fix all internal urls
-            # replace links of the form "#12-bla" to "#bla"
-            line = line_processor(sub(__FIX_LINKS, "\\1(#\\2)", line))
+        else:  # e.g., fix all urls via the line processor
+            line = str.rstrip(line_processor(line))
 
         dest(line)
+
+
+def process_markdown_for_sphinx(
+        source: Iterable[str], dest: Callable[[str], Any],
+        base_urls: Mapping[str, str] | None = None,
+        full_urls: Mapping[str, str] | None = None,
+        discard_until: str | None = "## 1. Introduction") -> None:
+    """
+    Process a markdown file in order to make it useful for distribution.
+
+    This process changes the GitHub-style markdown to a format that the myst
+    parser, which is used by sphinx, can render properly. This involves
+    several issues:
+
+    1. We discard the top-level heading.
+    2. We need to move all sub-headings one step up.
+    3. Furthermore, we can turn all absolute URLs pointing to the
+       documentation website to local references starting with `./`.
+    4. The myst parser drops the numerical prefixes of links, i.e., it tags
+       `## 1.2. Hello` with id `hello` instead of `12-hello`. This means that
+       we need to fix all references following the pattern `[xxx](#12-hello)`
+       to `[xxx](#hello)`.
+
+    :param source: the source line iterable
+    :param dest: the destination callable receiving the output
+    :param base_urls: a mapping of basic urls to shortcuts
+    :param full_urls: a mapping of full urls to abbreviations
+    :param discard_until: discard all strings until reaching this line. If
+        this is `None`, all lines will be used. If this is not `None`, then
+        this will be the first line to be forwarded to `dest`
+
+    >>> lp = list()
+    >>> src = ["![image](https://example.com/1.jp)",
+    ...        "# This is `pycommons!`",
+    ...        "Table of contents",
+    ...        "## 1. Introduction",
+    ...        "blabla bla <https://example.com/A>!",
+    ...        "## 2. Some More Text",
+    ...        "We [also say](https://example.com/z/hello.txt) stuff.",
+    ...        "### 2.4. Code Example",
+    ...        "```",
+    ...        "But [not in code](https://example.com/z/hello.txt).",
+    ...        "```",
+    ...        "See also [here](#24-code-example)."]
+    >>> process_markdown_for_sphinx(src, print,
+    ...     {"https://example.com/": "./"},
+    ...     {"https://example.com/A": "xyz"})
+    # 1. Introduction
+    blabla bla <xyz>!
+    # 2. Some More Text
+    We [also say](./z/hello.txt) stuff.
+    ## 2.4. Code Example
+    ```
+    But [not in code](https://example.com/z/hello.txt).
+    ```
+    See also [here](#code-example).
+
+    >>> try:
+    ...     process_markdown_for_sphinx(None, print)
+    ... except TypeError as te:
+    ...     print(te)
+    source should be an instance of typing.Iterable but is None.
+
+    >>> try:
+    ...     process_markdown_for_sphinx(1, print)
+    ... except TypeError as te:
+    ...     print(te)
+    source should be an instance of typing.Iterable but is int, namely '1'.
+
+    >>> try:
+    ...     process_markdown_for_sphinx([None], print)
+    ... except TypeError as te:
+    ...     print(te)
+    descriptor 'rstrip' for 'str' objects doesn't apply to a 'NoneType' object
+
+    >>> try:
+    ...     process_markdown_for_sphinx([1], print)
+    ... except TypeError as te:
+    ...     print(te)
+    descriptor 'rstrip' for 'str' objects doesn't apply to a 'int' object
+
+    >>> try:
+    ...     process_markdown_for_sphinx([""], None)
+    ... except TypeError as te:
+    ...     print(te)
+    dest should be a callable but is None.
+
+    >>> try:
+    ...     process_markdown_for_sphinx([""], 1)
+    ... except TypeError as te:
+    ...     print(te)
+    dest should be a callable but is int, namely '1'.
+
+    >>> try:
+    ...     process_markdown_for_sphinx([""], print, 1, None, "bla")
+    ... except TypeError as te:
+    ...     print(te)
+    base_urls should be an instance of typing.Mapping but is int, namely '1'.
+
+    >>> try:
+    ...     process_markdown_for_sphinx([""], print, None, 1, "bla")
+    ... except TypeError as te:
+    ...     print(te)
+    full_urls should be an instance of typing.Mapping but is int, namely '1'.
+
+    >>> try:
+    ...     process_markdown_for_sphinx([""], print, None, None, 1)
+    ... except TypeError as te:
+    ...     print(te)
+    descriptor '__len__' requires a 'str' object but received a 'int'
+
+    >>> try:
+    ...     process_markdown_for_sphinx([""], print, None, None, "")
+    ... except ValueError as ve:
+    ...     print(ve)
+    discard_until cannot be ''.
+
+    >>> process_markdown_for_sphinx([""], print, None, None, None)
+    <BLANKLINE>
+    """
+    __process_markdown(source, dest, cast(
+        Callable[[str], str], lambda s, __l=__make_url_replacer(
+            base_urls, full_urls): __l(sub(__FIX_LINKS, "\\1(#\\2)",
+                                           s))), discard_until)
```

### Comparing `pycommons-0.8.8/pycommons/dev/doc/setup_doc.py` & `pycommons-0.8.9/pycommons/dev/doc/setup_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import sys
 from datetime import datetime, timezone
 from inspect import stack
 from typing import Any, Final, Iterable, Mapping
 
 from pycommons.dev.doc.doc_info import DocInfo, load_doc_info_from_setup_cfg
 from pycommons.dev.doc.index_rst import make_index_rst
-from pycommons.dev.doc.process_md import make_url_replacer, process_markdown
+from pycommons.dev.doc.process_md import (
+    process_markdown_for_sphinx,
+)
 from pycommons.io.console import logger
 from pycommons.io.path import Path, directory_path, line_writer
 from pycommons.types import check_int_range, type_error
 
 #: the default intersphinx mappings
 __DEFAULT_INTERSPHINX: Final[dict[str, tuple[str, None]]] = {
     "latexgit": ("https://thomasweise.github.io/latexgit_py/", None),
@@ -115,16 +117,15 @@
         base_urls[doc_info.doc_url] = "./"
 
     readme_out: Final[Path] = doc_path.resolve_inside("README.md")
     logger(f"Now processing {doc_info.readme_md_file!r} to {readme_out!r} "
            f"with replacers {base_urls} and {full_urls}.")
     with (doc_info.readme_md_file.open_for_read() as rd,
           readme_out.open_for_write() as wd):
-        process_markdown(rd, line_writer(wd),
-                         make_url_replacer(base_urls, full_urls))
+        process_markdown_for_sphinx(rd, line_writer(wd), base_urls, full_urls)
 
     index_rst_file: Final[Path] = doc_path.resolve_inside("index.rst")
     logger(f"Now writing index.rst file {index_rst_file!r}.")
     with index_rst_file.open_for_write() as wd:
         make_index_rst(doc_info, line_writer(wd))
 
     # enable myst header anchors
```

### Comparing `pycommons-0.8.8/pycommons/dev/tests/compile_and_run.py` & `pycommons-0.8.9/pycommons/dev/tests/compile_and_run.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/dev/tests/examples_in_dir.py` & `pycommons-0.8.9/pycommons/dev/tests/examples_in_dir.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/dev/tests/examples_in_md.py` & `pycommons-0.8.9/pycommons/dev/tests/examples_in_md.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/dev/tests/links_in_md.py` & `pycommons-0.8.9/pycommons/dev/tests/links_in_md.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/ds/cache.py` & `pycommons-0.8.9/pycommons/ds/cache.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/ds/immutable_map.py` & `pycommons-0.8.9/pycommons/ds/immutable_map.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/io/arguments.py` & `pycommons-0.8.9/pycommons/io/arguments.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/io/console.py` & `pycommons-0.8.9/pycommons/io/console.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/io/path.py` & `pycommons-0.8.9/pycommons/io/path.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/io/temp.py` & `pycommons-0.8.9/pycommons/io/temp.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/math/int_math.py` & `pycommons-0.8.9/pycommons/math/int_math.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/net/url.py` & `pycommons-0.8.9/pycommons/net/url.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/processes/python.py` & `pycommons-0.8.9/pycommons/processes/python.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/processes/shell.py` & `pycommons-0.8.9/pycommons/processes/shell.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/strings/chars.py` & `pycommons-0.8.9/pycommons/strings/chars.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/strings/enforce.py` & `pycommons-0.8.9/pycommons/strings/enforce.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/strings/string_conv.py` & `pycommons-0.8.9/pycommons/strings/string_conv.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/strings/tools.py` & `pycommons-0.8.9/pycommons/strings/tools.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons/types.py` & `pycommons-0.8.9/pycommons/types.py`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/pycommons.egg-info/PKG-INFO` & `pycommons-0.8.9/pycommons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycommons
-Version: 0.8.8
+Version: 0.8.9
 Summary: A package with utility functionality for Python projects.
 Home-page: https://thomasweise.github.io/pycommons
 Author: Thomas Weise
 Author-email: tweise@ustc.edu.cn
 Maintainer: Thomas Weise
 Maintainer-email: tweise@ustc.edu.cn
 License: GPL 3.0
@@ -32,19 +32,19 @@
 [![pypi downloads](https://img.shields.io/pypi/dw/pycommons.svg)](https://pypistats.org/packages/pycommons)
 [![coverage report](https://thomasweise.github.io/pycommons/tc/badge.svg)](https://thomasweise.github.io/pycommons/tc/index.html)
 
 # *pycommons:* Common Utility Functions for Python Projects.
 
 Some common utility functionality for Python projects.
 
-- [Introduction](https://thomasweise.github.io/pycommons/index.html#introduction)
-- [Installation](https://thomasweise.github.io/pycommons/index.html#installation)
-- [Examples](https://thomasweise.github.io/pycommons/index.html#examples)
-- [License](https://thomasweise.github.io/pycommons/index.html#license)
-- [Contact](https://thomasweise.github.io/pycommons/index.html#contact)
+- [Introduction](https://thomasweise.github.io/pycommons#introduction)
+- [Installation](https://thomasweise.github.io/pycommons#installation)
+- [Examples](https://thomasweise.github.io/pycommons#examples)
+- [License](https://thomasweise.github.io/pycommons#license)
+- [Contact](https://thomasweise.github.io/pycommons#contact)
 
 
 ## 1. Introduction
 
 In this project, we combine several utilities and functions that are used in our other projects.
 
 These functions have in common that they are fail-fast.
@@ -119,18 +119,18 @@
 
 ## 4. License
 
 [`pycommons`](https://thomasweise.github.io/pycommons) is a library with utilities for Python projects.
 
 Copyright (C) 2024  [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授)
 
-Dr. Thomas Weise (see [Contact](https://thomasweise.github.io/pycommons/index.html#contact)) holds the copyright of this package.
+Dr. Thomas Weise (see [Contact](https://thomasweise.github.io/pycommons#contact)) holds the copyright of this package.
 
 `pycommons` is provided to the public as open source software under the [GNU GENERAL PUBLIC LICENSE, Version 3, 29 June 2007](https://thomasweise.github.io/pycommons/LICENSE.html).
-Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](https://thomasweise.github.io/pycommons/index.html#contact) below).
+Terms for other licenses, e.g., for specific industrial applications, can be negotiated with Dr. Thomas Weise (who can be reached via the [contact information](https://thomasweise.github.io/pycommons#contact) below).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 
 Please visit the [contributions guidelines](https://thomasweise.github.io/pycommons/CONTRIBUTING.html) for `pycommons` if you would like to contribute to our package.
```

### Comparing `pycommons-0.8.8/pycommons.egg-info/SOURCES.txt` & `pycommons-0.8.9/pycommons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/setup.cfg` & `pycommons-0.8.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycommons-0.8.8/setup.py` & `pycommons-0.8.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """The setup and installation script."""
 
-import io
-import re
+from re import compile as re_compile
+from re import sub as re_sub
+from typing import Final, Pattern
 
 from setuptools import setup
 
 # We want to use our README.md as project description.
 # However, we must fix all the references inside.
-with io.open("README.md",
-             "rt", encoding='utf-8-sig') as reader:
+with open("README.md", encoding="utf-8-sig") as reader:
     old_lines = reader.readlines()
 
 # It seems that the markdown parser does not auto-generate anchors. This means
 # that we need to fix all references following the pattern `[xxx](#12-hello)`
 # to `[xxx]({docu_url#hello)`, where `docu_url` is the url of our
 # documentation. We do this with a regular expression `regex_search`.
-new_lines = []
+new_lines: Final[list[str]] = []
 in_code: bool = False  # we only process non-code lines
+
+# the base url where the documentation will land
+doc_url: Final[str] = "https://thomasweise.github.io/pycommons"
+# the url of our repository
+repo_url: Final[str] = "https://github.com/thomasWeise/pycommons"
+
 # detects strings of the form [xyz](#123-bla) and gives \1=xyz and \2=bla
-regex_search = re.compile("(\\[.+?])\\(#\\d+-(.+?)\\)")
-regex_repl: str = \
-    "\\1(https://thomasweise.github.io/pycommons/index.html#\\2)"
-license_old: str = \
-    "https://github.com/thomasWeise/pycommons/blob/main/LICENSE"
-license_new: str = \
-    "https://thomasweise.github.io/pycommons/LICENSE.html"
+regex_search: Final[Pattern] = re_compile("(\\[.+?])\\(#\\d+-(.+?)\\)")
+regex_repl: Final[str] = f"\\1({doc_url}#\\2)"
 
-for line in old_lines:
-    line = line.rstrip()
+# other replacements
+license_old: Final[str] = f"{repo_url}/blob/main/LICENSE"
+license_new: Final[str] = f"{doc_url}/LICENSE.html"
+
+for full_line in old_lines:
+    line: str = str.rstrip(full_line)
     if in_code:
         if line.startswith("```"):
             in_code = False  # toggle to non-code
-    else:
-        if line.startswith("```"):
-            in_code = True  # toggle to code
-        else:  # fix all internal urls
-            # replace links of the form "#12-bla" to "#bla"
-            line = re.sub(regex_search, regex_repl, line)
-            line = line.replace(license_old, license_new)
+    elif line.startswith("```"):
+        in_code = True  # toggle to code
+    else:  # fix all internal urls
+        # replace links of the form "#12-bla" to "#bla"
+        line = re_sub(regex_search, regex_repl, line)
+        line = str.replace(line, license_old, license_new)
     new_lines.append(line)
 
 # Now we can use the code in the setup.
 setup(long_description="\n".join(new_lines),
       long_description_content_type="text/markdown")
```

### Comparing `pycommons-0.8.8/tests/test_links_in_mds.py` & `pycommons-0.8.9/tests/test_links_in_mds.py`

 * *Files identical despite different names*

