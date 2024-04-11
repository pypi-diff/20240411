# Comparing `tmp/lsst-utils-26.2024.800.tar.gz` & `tmp/lsst-utils-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-utils-26.2024.800.tar", last modified: Thu Feb 22 10:43:19 2024, max compression
+gzip compressed data, was "lsst-utils-26.2024.900.tar", last modified: Thu Feb 29 10:20:57 2024, max compression
```

## Comparing `lsst-utils-26.2024.800.tar` & `lsst-utils-26.2024.900.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.169989 lsst-utils-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-22 10:43:19.169989 lsst-utils-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.157989 lsst-utils-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.157989 lsst-utils-26.2024.800/doc/lsst.utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/doc/lsst.utils/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/doc/lsst.utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.157989 lsst-utils-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.157989 lsst-utils-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.161989 lsst-utils-26.2024.800/python/lsst/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.161989 lsst-utils-26.2024.800/python/lsst/utils/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/plotting/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:43:18.000000 lsst-utils-26.2024.800/python/lsst/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/python/lsst/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.165989 lsst-utils-26.2024.800/python/lsst_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-22 10:43:19.000000 lsst-utils-26.2024.800/python/lsst_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-22 10:43:19.000000 lsst-utils-26.2024.800/python/lsst_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:19.000000 lsst-utils-26.2024.800/python/lsst_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-22 10:43:19.000000 lsst-utils-26.2024.800/python/lsst_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:43:19.000000 lsst-utils-26.2024.800/python/lsst_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:43:18.000000 lsst-utils-26.2024.800/python/lsst_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-22 10:43:19.169989 lsst-utils-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:43:19.165989 lsst-utils-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_getPackageDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_getTempFilePath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_plotting_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-02-22 10:43:07.000000 lsst-utils-26.2024.800/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.851523 lsst-utils-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.855523 lsst-utils-26.2024.900/doc/lsst.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/doc/lsst.utils/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/doc/lsst.utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.851523 lsst-utils-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.855523 lsst-utils-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.859523 lsst-utils-26.2024.900/python/lsst/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.859523 lsst-utils-26.2024.900/python/lsst/utils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/plotting/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/python/lsst/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/python/lsst_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:57.000000 lsst-utils-26.2024.900/python/lsst_utils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:57.863523 lsst-utils-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_getPackageDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_getTempFilePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_plotting_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-02-29 10:20:43.000000 lsst-utils-26.2024.900/tests/test_wrappers.py
```

### Comparing `lsst-utils-26.2024.800/LICENSE` & `lsst-utils-26.2024.900/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/PKG-INFO` & `lsst-utils-26.2024.900/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-utils-26.2024.800/README.rst` & `lsst-utils-26.2024.900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/doc/lsst.utils/CHANGES.rst` & `lsst-utils-26.2024.900/doc/lsst.utils/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/doc/lsst.utils/index.rst` & `lsst-utils-26.2024.900/doc/lsst.utils/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/pyproject.toml` & `lsst-utils-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/__init__.py` & `lsst-utils-26.2024.900/python/lsst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/_packaging.py` & `lsst-utils-26.2024.900/python/lsst/utils/_packaging.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/classes.py` & `lsst-utils-26.2024.900/python/lsst/utils/classes.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/db_auth.py` & `lsst-utils-26.2024.900/python/lsst/utils/db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/deprecated.py` & `lsst-utils-26.2024.900/python/lsst/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/doImport.py` & `lsst-utils-26.2024.900/python/lsst/utils/doImport.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/ellipsis.py` & `lsst-utils-26.2024.900/python/lsst/utils/ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/inheritDoc.py` & `lsst-utils-26.2024.900/python/lsst/utils/inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/introspection.py` & `lsst-utils-26.2024.900/python/lsst/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/iteration.py` & `lsst-utils-26.2024.900/python/lsst/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/logging.py` & `lsst-utils-26.2024.900/python/lsst/utils/logging.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/packages.py` & `lsst-utils-26.2024.900/python/lsst/utils/packages.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/plotting/limits.py` & `lsst-utils-26.2024.900/python/lsst/utils/plotting/limits.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/tests.py` & `lsst-utils-26.2024.900/python/lsst/utils/tests.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/threads.py` & `lsst-utils-26.2024.900/python/lsst/utils/threads.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/timer.py` & `lsst-utils-26.2024.900/python/lsst/utils/timer.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/usage.py` & `lsst-utils-26.2024.900/python/lsst/utils/usage.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst/utils/wrappers.py` & `lsst-utils-26.2024.900/python/lsst/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/python/lsst_utils.egg-info/PKG-INFO` & `lsst-utils-26.2024.900/python/lsst_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-utils-26.2024.800/python/lsst_utils.egg-info/SOURCES.txt` & `lsst-utils-26.2024.900/python/lsst_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_classes.py` & `lsst-utils-26.2024.900/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_db_auth.py` & `lsst-utils-26.2024.900/tests/test_db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_decorators.py` & `lsst-utils-26.2024.900/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_deprecated.py` & `lsst-utils-26.2024.900/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_doImport.py` & `lsst-utils-26.2024.900/tests/test_doImport.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_ellipsis.py` & `lsst-utils-26.2024.900/tests/test_ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_executables.py` & `lsst-utils-26.2024.900/tests/test_executables.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_getPackageDir.py` & `lsst-utils-26.2024.900/tests/test_getPackageDir.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_getTempFilePath.py` & `lsst-utils-26.2024.900/tests/test_getTempFilePath.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_import.py` & `lsst-utils-26.2024.900/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_inheritDoc.py` & `lsst-utils-26.2024.900/tests/test_inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_introspection.py` & `lsst-utils-26.2024.900/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_iteration.py` & `lsst-utils-26.2024.900/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_logging.py` & `lsst-utils-26.2024.900/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_ordering.py` & `lsst-utils-26.2024.900/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_packages.py` & `lsst-utils-26.2024.900/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_plotting_limits.py` & `lsst-utils-26.2024.900/tests/test_plotting_limits.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_threads.py` & `lsst-utils-26.2024.900/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_timer.py` & `lsst-utils-26.2024.900/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_usage.py` & `lsst-utils-26.2024.900/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_utils.py` & `lsst-utils-26.2024.900/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-utils-26.2024.800/tests/test_wrappers.py` & `lsst-utils-26.2024.900/tests/test_wrappers.py`

 * *Files identical despite different names*

