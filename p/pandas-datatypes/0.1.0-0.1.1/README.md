# Comparing `tmp/pandas_datatypes-0.1.0.tar.gz` & `tmp/pandas_datatypes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_datatypes-0.1.0.tar", last modified: Wed Apr 10 22:57:31 2024, max compression
+gzip compressed data, was "pandas_datatypes-0.1.1.tar", last modified: Wed Apr 10 23:29:02 2024, max compression
```

## Comparing `pandas_datatypes-0.1.0.tar` & `pandas_datatypes-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:57:31.267386 pandas_datatypes-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-10 22:57:31.267386 pandas_datatypes-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 22:57:27.000000 pandas_datatypes-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:57:31.263386 pandas_datatypes-0.1.0/pandas_datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 22:57:27.000000 pandas_datatypes-0.1.0/pandas_datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-10 22:57:27.000000 pandas_datatypes-0.1.0/pandas_datatypes/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:57:31.267386 pandas_datatypes-0.1.0/pandas_datatypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-10 22:57:31.000000 pandas_datatypes-0.1.0/pandas_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 22:57:31.000000 pandas_datatypes-0.1.0/pandas_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:57:31.000000 pandas_datatypes-0.1.0/pandas_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 22:57:31.000000 pandas_datatypes-0.1.0/pandas_datatypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 22:57:31.000000 pandas_datatypes-0.1.0/pandas_datatypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:57:31.267386 pandas_datatypes-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-10 22:57:27.000000 pandas_datatypes-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:29:02.670599 pandas_datatypes-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-10 23:29:02.670599 pandas_datatypes-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-10 23:28:58.000000 pandas_datatypes-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:29:02.666599 pandas_datatypes-0.1.1/pandas_datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 23:28:58.000000 pandas_datatypes-0.1.1/pandas_datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-10 23:28:58.000000 pandas_datatypes-0.1.1/pandas_datatypes/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:29:02.670599 pandas_datatypes-0.1.1/pandas_datatypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-10 23:29:02.000000 pandas_datatypes-0.1.1/pandas_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 23:29:02.000000 pandas_datatypes-0.1.1/pandas_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:29:02.000000 pandas_datatypes-0.1.1/pandas_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 23:29:02.000000 pandas_datatypes-0.1.1/pandas_datatypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 23:29:02.000000 pandas_datatypes-0.1.1/pandas_datatypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:29:02.670599 pandas_datatypes-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 23:28:58.000000 pandas_datatypes-0.1.1/setup.py
```

### Comparing `pandas_datatypes-0.1.0/pandas_datatypes/data_types.py` & `pandas_datatypes-0.1.1/pandas_datatypes/data_types.py`

 * *Files identical despite different names*

