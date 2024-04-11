# Comparing `tmp/fd2py-1.0.tar.gz` & `tmp/fd2py-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fd2py-1.0.tar", last modified: Thu Apr 11 06:27:21 2024, max compression
+gzip compressed data, was "fd2py-1.1.tar", last modified: Thu Apr 11 06:41:47 2024, max compression
```

## Comparing `fd2py-1.0.tar` & `fd2py-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:27:21.390554 fd2py-1.0/
--rw-rw-rw-   0        0        0      425 2024-04-11 06:27:21.389552 fd2py-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 06:27:21.388549 fd2py-1.0/fd2py.egg-info/
--rw-rw-rw-   0        0        0      425 2024-04-11 06:27:21.000000 fd2py-1.0/fd2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      133 2024-04-11 06:27:21.000000 fd2py-1.0/fd2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:27:21.000000 fd2py-1.0/fd2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:27:21.000000 fd2py-1.0/fd2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4635 2024-04-11 05:22:51.000000 fd2py-1.0/fd2py.py
--rw-rw-rw-   0        0        0       42 2024-04-11 06:27:21.390554 fd2py-1.0/setup.cfg
--rw-rw-rw-   0        0        0      461 2024-04-11 06:27:06.000000 fd2py-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:41:47.011911 fd2py-1.1/
+-rw-rw-rw-   0        0        0      425 2024-04-11 06:41:47.010907 fd2py-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 06:41:47.009805 fd2py-1.1/fd2py.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-04-11 06:41:46.000000 fd2py-1.1/fd2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2024-04-11 06:41:46.000000 fd2py-1.1/fd2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:41:46.000000 fd2py-1.1/fd2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-11 06:41:46.000000 fd2py-1.1/fd2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4635 2024-04-11 05:22:51.000000 fd2py-1.1/fd2py.py
+-rw-rw-rw-   0        0        0       42 2024-04-11 06:41:47.011911 fd2py-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      487 2024-04-11 06:41:39.000000 fd2py-1.1/setup.py
```

### Comparing `fd2py-1.0/fd2py.py` & `fd2py-1.1/fd2py.py`

 * *Files identical despite different names*

