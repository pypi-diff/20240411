# Comparing `tmp/reqargs-1.0.0.tar.gz` & `tmp/reqargs-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqargs-1.0.0.tar", last modified: Thu Apr 11 07:19:54 2024, max compression
+gzip compressed data, was "reqargs-1.2.tar", last modified: Thu Apr 11 07:39:39 2024, max compression
```

## Comparing `reqargs-1.0.0.tar` & `reqargs-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 07:19:54.215040 reqargs-1.0.0/
--rw-rw-rw-   0        0        0      313 2024-04-11 07:19:54.214173 reqargs-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 07:19:54.205108 reqargs-1.0.0/reqargs/
--rw-rw-rw-   0        0        0       37 2023-03-26 12:23:21.000000 reqargs-1.0.0/reqargs/__init__.py
--rw-rw-rw-   0        0        0   365183 2023-03-26 12:23:21.000000 reqargs-1.0.0/reqargs/reqinstaller.py
-drwxrwxrwx   0        0        0        0 2024-04-11 07:19:54.212031 reqargs-1.0.0/reqargs.egg-info/
--rw-rw-rw-   0        0        0      313 2024-04-11 07:19:54.000000 reqargs-1.0.0/reqargs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-04-11 07:19:54.000000 reqargs-1.0.0/reqargs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 07:19:54.000000 reqargs-1.0.0/reqargs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 07:19:54.000000 reqargs-1.0.0/reqargs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 07:19:54.215040 reqargs-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-04-11 07:17:33.000000 reqargs-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:39:39.056669 reqargs-1.2/
+-rw-rw-rw-   0        0        0      311 2024-04-11 07:39:39.055636 reqargs-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 07:39:39.050635 reqargs-1.2/reqargs/
+-rw-rw-rw-   0        0        0      449 2024-04-11 07:38:08.000000 reqargs-1.2/reqargs/__init__.py
+-rw-rw-rw-   0        0        0      449 2024-04-11 07:38:22.000000 reqargs-1.2/reqargs/reqargs.py
+drwxrwxrwx   0        0        0        0 2024-04-11 07:39:39.054650 reqargs-1.2/reqargs.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 07:39:39.056669 reqargs-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-04-11 07:39:23.000000 reqargs-1.2/setup.py
```

### Comparing `reqargs-1.0.0/setup.py` & `reqargs-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 
-VERSION = '1.0.0'
+VERSION = '1.2'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="reqargs",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
```

