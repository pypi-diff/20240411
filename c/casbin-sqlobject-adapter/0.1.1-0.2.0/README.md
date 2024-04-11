# Comparing `tmp/casbin_sqlobject_adapter-0.1.1.tar.gz` & `tmp/casbin_sqlobject_adapter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\casbin_sqlobject_adapter-0.1.1.tar", last modified: Sat Jun 13 12:41:23 2020, max compression
+gzip compressed data, was "casbin_sqlobject_adapter-0.2.0.tar", last modified: Thu Apr 11 17:01:42 2024, max compression
```

## Comparing `casbin_sqlobject_adapter-0.1.1.tar` & `casbin_sqlobject_adapter-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-06-13 12:41:23.598223 casbin_sqlobject_adapter-0.1.1/
--rw-rw-rw-   0        0        0     3430 2020-06-13 12:41:23.596224 casbin_sqlobject_adapter-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2163 2020-06-13 10:35:27.000000 casbin_sqlobject_adapter-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2020-06-13 12:41:23.572241 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter/
--rw-rw-rw-   0        0        0       41 2020-06-13 12:29:43.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter/__init__.py
--rw-rw-rw-   0        0        0     2320 2020-06-13 12:29:43.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter/adapter.py
-drwxrwxrwx   0        0        0        0 2020-06-13 12:41:23.590226 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter.egg-info/
--rw-rw-rw-   0        0        0     3430 2020-06-13 12:41:23.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2020-06-13 12:41:23.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-13 12:41:23.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2020-06-13 12:41:23.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2020-06-13 12:41:23.000000 casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-13 12:41:23.599222 casbin_sqlobject_adapter-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1146 2020-06-13 12:30:49.000000 casbin_sqlobject_adapter-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:42.926538 casbin_sqlobject_adapter-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 17:01:12.000000 casbin_sqlobject_adapter-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-11 17:01:42.926538 casbin_sqlobject_adapter-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-11 17:01:12.000000 casbin_sqlobject_adapter-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:42.922538 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 17:01:12.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-11 17:01:12.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:42.926538 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-11 17:01:42.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 17:01:42.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:01:42.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 17:01:42.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 17:01:42.000000 casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-11 17:01:41.000000 casbin_sqlobject_adapter-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 17:01:12.000000 casbin_sqlobject_adapter-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:01:42.926538 casbin_sqlobject_adapter-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:42.926538 casbin_sqlobject_adapter-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-11 17:01:12.000000 casbin_sqlobject_adapter-0.2.0/tests/test_adapter.py
```

### Comparing `casbin_sqlobject_adapter-0.1.1/README.md` & `casbin_sqlobject_adapter-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 SQLObject Adapter for PyCasbin
 ====
 
-[![Build Status](https://www.travis-ci.org/pycasbin/sqlobject-adapter.svg?branch=master)](https://www.travis-ci.org/pycasbin/sqlobject-adapter)
+[![GitHub Action](https://github.com/pycasbin/sqlobject-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/sqlobject-adapter/actions)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/sqlobject-adapter/badge.svg)](https://coveralls.io/github/pycasbin/sqlobject-adapter)
 [![Version](https://img.shields.io/pypi/v/casbin_sqlobject_adapter.svg)](https://pypi.org/project/casbin_sqlobject_adapter/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin_sqlobject_adapter.svg)](https://pypi.org/project/casbin_sqlobject_adapter/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/casbin_sqlobject_adapter.svg)](https://pypi.org/project/casbin_sqlobject_adapter/)
 [![Download](https://img.shields.io/pypi/dm/casbin_sqlobject_adapter.svg)](https://pypi.org/project/casbin_sqlobject_adapter/)
 [![License](https://img.shields.io/pypi/l/casbin_sqlobject_adapter.svg)](https://pypi.org/project/casbin_sqlobject_adapter/)
```

### Comparing `casbin_sqlobject_adapter-0.1.1/casbin_sqlobject_adapter/adapter.py` & `casbin_sqlobject_adapter-0.2.0/casbin_sqlobject_adapter/adapter.py`

 * *Files identical despite different names*

