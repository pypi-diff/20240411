# Comparing `tmp/donetools-0.0.5.tar.gz` & `tmp/donetools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donetools-0.0.5.tar", last modified: Mon Apr  8 13:19:44 2024, max compression
+gzip compressed data, was "donetools-0.0.6.tar", last modified: Thu Apr 11 08:57:16 2024, max compression
```

## Comparing `donetools-0.0.5.tar` & `donetools-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:19:44.944650 donetools-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 13:19:44.944650 donetools-0.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:19:44.944650 donetools-0.0.5/donetools/
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 07:14:03.000000 donetools-0.0.5/donetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      622 2024-04-08 07:07:04.000000 donetools-0.0.5/donetools/info.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-08 13:19:33.000000 donetools-0.0.5/donetools/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:19:44.944650 donetools-0.0.5/donetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-08 13:19:44.000000 donetools-0.0.5/donetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-08 13:19:44.000000 donetools-0.0.5/donetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:19:44.000000 donetools-0.0.5/donetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-08 13:19:44.000000 donetools-0.0.5/donetools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      457 2024-04-08 13:19:41.000000 donetools-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:19:44.944650 donetools-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:57:16.352984 donetools-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 08:57:16.352984 donetools-0.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:57:16.352984 donetools-0.0.6/donetools/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 07:14:03.000000 donetools-0.0.6/donetools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      684 2024-04-10 15:11:13.000000 donetools-0.0.6/donetools/info.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-04-11 08:56:20.000000 donetools-0.0.6/donetools/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:57:16.352984 donetools-0.0.6/donetools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-11 08:56:40.000000 donetools-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 08:57:16.352984 donetools-0.0.6/setup.cfg
```

### Comparing `donetools-0.0.5/LICENSE` & `donetools-0.0.6/LICENSE`

 * *Files identical despite different names*

