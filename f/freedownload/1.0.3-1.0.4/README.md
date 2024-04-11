# Comparing `tmp/freedownload-1.0.3.tar.gz` & `tmp/freedownload-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedownload-1.0.3.tar", last modified: Sat Feb 24 01:56:57 2024, max compression
+gzip compressed data, was "freedownload-1.0.4.tar", last modified: Thu Apr 11 00:30:46 2024, max compression
```

## Comparing `freedownload-1.0.3.tar` & `freedownload-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 01:56:57.668963 freedownload-1.0.3/
--rw-rw-rw-   0        0        0      966 2024-02-24 01:56:57.667965 freedownload-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-24 01:56:57.575082 freedownload-1.0.3/freedownload/
--rw-rw-rw-   0        0        0     8341 2024-02-24 01:53:59.000000 freedownload-1.0.3/freedownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-02-24 01:55:01.000000 freedownload-1.0.3/freedownload/version.py
-drwxrwxrwx   0        0        0        0 2024-02-24 01:56:57.666967 freedownload-1.0.3/freedownload.egg-info/
--rw-rw-rw-   0        0        0      966 2024-02-24 01:56:57.000000 freedownload-1.0.3/freedownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-02-24 01:56:57.000000 freedownload-1.0.3/freedownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 01:56:57.000000 freedownload-1.0.3/freedownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-02-24 01:56:57.000000 freedownload-1.0.3/freedownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-24 01:56:57.000000 freedownload-1.0.3/freedownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-02-24 01:56:57.000000 freedownload-1.0.3/freedownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-02-24 01:56:57.668963 freedownload-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:30:46.286737 freedownload-1.0.4/
+-rw-rw-rw-   0        0        0      966 2024-04-11 00:30:46.285739 freedownload-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 00:30:46.249879 freedownload-1.0.4/freedownload/
+-rw-rw-rw-   0        0        0     6279 2024-04-11 00:27:54.000000 freedownload-1.0.4/freedownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-11 00:28:13.000000 freedownload-1.0.4/freedownload/version.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:30:46.283775 freedownload-1.0.4/freedownload.egg-info/
+-rw-rw-rw-   0        0        0      966 2024-04-11 00:30:45.000000 freedownload-1.0.4/freedownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-11 00:30:46.000000 freedownload-1.0.4/freedownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 00:30:45.000000 freedownload-1.0.4/freedownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-11 00:30:45.000000 freedownload-1.0.4/freedownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 00:30:45.000000 freedownload-1.0.4/freedownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-11 00:30:45.000000 freedownload-1.0.4/freedownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-11 00:30:46.286737 freedownload-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-1.0.4/setup.py
```

### Comparing `freedownload-1.0.3/PKG-INFO` & `freedownload-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `freedownload-1.0.3/README.md` & `freedownload-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `freedownload-1.0.3/freedownload.egg-info/PKG-INFO` & `freedownload-1.0.4/freedownload.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `freedownload-1.0.3/setup.py` & `freedownload-1.0.4/setup.py`

 * *Files identical despite different names*

