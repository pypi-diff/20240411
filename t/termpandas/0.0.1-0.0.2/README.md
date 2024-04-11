# Comparing `tmp/termpandas-0.0.1.tar.gz` & `tmp/termpandas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termpandas-0.0.1.tar", last modified: Thu Apr 11 16:49:40 2024, max compression
+gzip compressed data, was "termpandas-0.0.2.tar", last modified: Thu Apr 11 17:15:38 2024, max compression
```

## Comparing `termpandas-0.0.1.tar` & `termpandas-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-11 16:49:40.223109 termpandas-0.0.1/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      100 2024-04-11 15:50:03.000000 termpandas-0.0.1/CHANGELOG.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1076 2024-04-11 15:26:31.000000 termpandas-0.0.1/LICENSE
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       75 2024-04-11 16:34:42.000000 termpandas-0.0.1/MANIFEST.in
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      634 2024-04-11 16:49:40.223109 termpandas-0.0.1/PKG-INFO
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      510 2024-04-11 16:31:36.000000 termpandas-0.0.1/README.md
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       38 2024-04-11 16:49:40.223109 termpandas-0.0.1/setup.cfg
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      793 2024-04-11 16:04:21.000000 termpandas-0.0.1/setup.py
-drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-11 16:49:40.219109 termpandas-0.0.1/termpandas/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       31 2024-04-11 15:57:50.000000 termpandas-0.0.1/termpandas/__init__.py
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     4891 2024-04-11 15:59:06.000000 termpandas-0.0.1/termpandas/scrollable.py
-drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-11 16:49:40.223109 termpandas-0.0.1/termpandas.egg-info/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      634 2024-04-11 16:49:40.000000 termpandas-0.0.1/termpandas.egg-info/PKG-INFO
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      280 2024-04-11 16:49:40.000000 termpandas-0.0.1/termpandas.egg-info/SOURCES.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)        1 2024-04-11 16:49:40.000000 termpandas-0.0.1/termpandas.egg-info/dependency_links.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       45 2024-04-11 16:49:40.000000 termpandas-0.0.1/termpandas.egg-info/requires.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       11 2024-04-11 16:49:40.000000 termpandas-0.0.1/termpandas.egg-info/top_level.txt
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)   772130 2024-04-11 16:24:21.000000 termpandas-0.0.1/tprint.gif
+drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-11 17:15:38.430887 termpandas-0.0.2/
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      203 2024-04-11 17:15:18.000000 termpandas-0.0.2/CHANGELOG.txt
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1076 2024-04-11 15:26:31.000000 termpandas-0.0.2/LICENSE
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       75 2024-04-11 16:34:42.000000 termpandas-0.0.2/MANIFEST.in
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1200 2024-04-11 17:15:38.430887 termpandas-0.0.2/PKG-INFO
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      510 2024-04-11 16:31:36.000000 termpandas-0.0.2/README.md
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       38 2024-04-11 17:15:38.430887 termpandas-0.0.2/setup.cfg
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1030 2024-04-11 17:13:41.000000 termpandas-0.0.2/setup.py
+drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-11 17:15:38.426887 termpandas-0.0.2/termpandas/
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       31 2024-04-11 15:57:50.000000 termpandas-0.0.2/termpandas/__init__.py
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     4891 2024-04-11 15:59:06.000000 termpandas-0.0.2/termpandas/scrollable.py
+drwxrwxr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-04-11 17:15:38.430887 termpandas-0.0.2/termpandas.egg-info/
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1200 2024-04-11 17:15:38.000000 termpandas-0.0.2/termpandas.egg-info/PKG-INFO
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)      280 2024-04-11 17:15:38.000000 termpandas-0.0.2/termpandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)        1 2024-04-11 17:15:38.000000 termpandas-0.0.2/termpandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       45 2024-04-11 17:15:38.000000 termpandas-0.0.2/termpandas.egg-info/requires.txt
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       11 2024-04-11 17:15:38.000000 termpandas-0.0.2/termpandas.egg-info/top_level.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)   772130 2024-04-11 16:24:21.000000 termpandas-0.0.2/tprint.gif
```

### Comparing `termpandas-0.0.1/LICENSE` & `termpandas-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `termpandas-0.0.1/termpandas/scrollable.py` & `termpandas-0.0.2/termpandas/scrollable.py`

 * *Files identical despite different names*

### Comparing `termpandas-0.0.1/tprint.gif` & `termpandas-0.0.2/tprint.gif`

 * *Files identical despite different names*

