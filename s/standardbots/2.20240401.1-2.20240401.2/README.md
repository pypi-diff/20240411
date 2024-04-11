# Comparing `tmp/standardbots-2.20240401.1.tar.gz` & `tmp/standardbots-2.20240401.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standardbots-2.20240401.1.tar", last modified: Mon Apr  1 15:40:22 2024, max compression
+gzip compressed data, was "standardbots-2.20240401.2.tar", last modified: Fri Apr  5 14:19:16 2024, max compression
```

## Comparing `standardbots-2.20240401.1.tar` & `standardbots-2.20240401.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.872473 standardbots-2.20240401.1/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:40:22.872473 standardbots-2.20240401.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/standardbots/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/standardbots/auto_generated/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/auto_generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34791 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/auto_generated/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)   101836 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/auto_generated/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/standardbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:16.266593 standardbots-2.20240401.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 14:19:16.266593 standardbots-2.20240401.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:19:16.266593 standardbots-2.20240401.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 14:19:15.000000 standardbots-2.20240401.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:16.262593 standardbots-2.20240401.2/standardbots/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 14:19:04.000000 standardbots-2.20240401.2/standardbots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:16.266593 standardbots-2.20240401.2/standardbots/auto_generated/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 14:19:04.000000 standardbots-2.20240401.2/standardbots/auto_generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34791 2024-04-05 14:19:04.000000 standardbots-2.20240401.2/standardbots/auto_generated/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101836 2024-04-05 14:19:04.000000 standardbots-2.20240401.2/standardbots/auto_generated/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:19:16.266593 standardbots-2.20240401.2/standardbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 14:19:16.000000 standardbots-2.20240401.2/standardbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-05 14:19:16.000000 standardbots-2.20240401.2/standardbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:19:16.000000 standardbots-2.20240401.2/standardbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 14:19:16.000000 standardbots-2.20240401.2/standardbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 14:19:16.000000 standardbots-2.20240401.2/standardbots.egg-info/top_level.txt
```

### Comparing `standardbots-2.20240401.1/setup.py` & `standardbots-2.20240401.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: support@standardbots.com
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "standardbots"
-VERSION = "2.20240401.1"
+VERSION = "2.20240401.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `standardbots-2.20240401.1/standardbots/auto_generated/apis.py` & `standardbots-2.20240401.2/standardbots/auto_generated/apis.py`

 * *Files identical despite different names*

### Comparing `standardbots-2.20240401.1/standardbots/auto_generated/models.py` & `standardbots-2.20240401.2/standardbots/auto_generated/models.py`

 * *Files identical despite different names*

