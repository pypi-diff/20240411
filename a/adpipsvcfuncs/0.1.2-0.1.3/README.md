# Comparing `tmp/adpipsvcfuncs-0.1.2.tar.gz` & `tmp/adpipsvcfuncs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipsvcfuncs-0.1.2.tar", last modified: Wed Apr 10 17:05:51 2024, max compression
+gzip compressed data, was "adpipsvcfuncs-0.1.3.tar", last modified: Thu Apr 11 18:52:04 2024, max compression
```

## Comparing `adpipsvcfuncs-0.1.2.tar` & `adpipsvcfuncs-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:05:51.716328 adpipsvcfuncs-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-10 17:04:57.000000 adpipsvcfuncs-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-10 17:05:51.712328 adpipsvcfuncs-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-10 17:04:57.000000 adpipsvcfuncs-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:05:51.712328 adpipsvcfuncs-0.1.2/adpipsvcfuncs/
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:04:57.000000 adpipsvcfuncs-0.1.2/adpipsvcfuncs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      969 2024-04-10 17:04:57.000000 adpipsvcfuncs-0.1.2/adpipsvcfuncs/adpipsvcfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:05:51.712328 adpipsvcfuncs-0.1.2/adpipsvcfuncs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-10 17:05:51.000000 adpipsvcfuncs-0.1.2/adpipsvcfuncs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-10 17:05:51.000000 adpipsvcfuncs-0.1.2/adpipsvcfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:05:51.000000 adpipsvcfuncs-0.1.2/adpipsvcfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-10 17:05:51.000000 adpipsvcfuncs-0.1.2/adpipsvcfuncs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 17:05:51.716328 adpipsvcfuncs-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      424 2024-04-10 17:04:57.000000 adpipsvcfuncs-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:52:04.782391 adpipsvcfuncs-0.1.3/adpipsvcfuncs/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs/adpipsvcfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-11 18:52:04.000000 adpipsvcfuncs-0.1.3/adpipsvcfuncs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 18:52:04.786392 adpipsvcfuncs-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      424 2024-04-11 18:51:10.000000 adpipsvcfuncs-0.1.3/setup.py
```

### Comparing `adpipsvcfuncs-0.1.2/LICENSE` & `adpipsvcfuncs-0.1.3/LICENSE`

 * *Files identical despite different names*

