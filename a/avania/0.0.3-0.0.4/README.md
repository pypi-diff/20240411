# Comparing `tmp/avania-0.0.3.tar.gz` & `tmp/avania-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.0.3.tar", last modified: Thu Apr 11 05:52:23 2024, max compression
+gzip compressed data, was "avania-0.0.4.tar", last modified: Thu Apr 11 05:55:41 2024, max compression
```

## Comparing `avania-0.0.3.tar` & `avania-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:52:23.621652 avania-0.0.3/
--rw-r--r--   0 staran     (501) staff       (20)     1742 2024-04-11 04:09:41.000000 avania-0.0.3/LICENSE
--rw-r--r--   0 staran     (501) staff       (20)      867 2024-04-11 05:52:23.621440 avania-0.0.3/PKG-INFO
--rw-r--r--   0 staran     (501) staff       (20)      662 2024-04-11 04:48:48.000000 avania-0.0.3/README.md
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:52:23.620392 avania-0.0.3/avania/
--rw-r--r--   0 staran     (501) staff       (20)       30 2024-04-11 05:21:55.000000 avania-0.0.3/avania/__init__.py
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:52:23.621247 avania-0.0.3/avania.egg-info/
--rw-r--r--   0 staran     (501) staff       (20)      867 2024-04-11 05:52:23.000000 avania-0.0.3/avania.egg-info/PKG-INFO
--rw-r--r--   0 staran     (501) staff       (20)      194 2024-04-11 05:52:23.000000 avania-0.0.3/avania.egg-info/SOURCES.txt
--rw-r--r--   0 staran     (501) staff       (20)        1 2024-04-11 05:52:23.000000 avania-0.0.3/avania.egg-info/dependency_links.txt
--rw-r--r--   0 staran     (501) staff       (20)       15 2024-04-11 05:52:23.000000 avania-0.0.3/avania.egg-info/requires.txt
--rw-r--r--   0 staran     (501) staff       (20)        7 2024-04-11 05:52:23.000000 avania-0.0.3/avania.egg-info/top_level.txt
--rw-r--r--   0 staran     (501) staff       (20)       38 2024-04-11 05:52:23.621693 avania-0.0.3/setup.cfg
--rw-r--r--   0 staran     (501) staff       (20)      352 2024-04-11 05:52:18.000000 avania-0.0.3/setup.py
+drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:55:41.733342 avania-0.0.4/
+-rw-r--r--   0 staran     (501) staff       (20)     1742 2024-04-11 04:09:41.000000 avania-0.0.4/LICENSE
+-rw-r--r--   0 staran     (501) staff       (20)     2237 2024-04-11 05:55:41.733118 avania-0.0.4/PKG-INFO
+-rw-r--r--   0 staran     (501) staff       (20)      662 2024-04-11 04:48:48.000000 avania-0.0.4/README.md
+drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:55:41.732037 avania-0.0.4/avania/
+-rw-r--r--   0 staran     (501) staff       (20)       30 2024-04-11 05:21:55.000000 avania-0.0.4/avania/__init__.py
+drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:55:41.732822 avania-0.0.4/avania.egg-info/
+-rw-r--r--   0 staran     (501) staff       (20)     2237 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/PKG-INFO
+-rw-r--r--   0 staran     (501) staff       (20)      194 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 staran     (501) staff       (20)        1 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 staran     (501) staff       (20)       15 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/requires.txt
+-rw-r--r--   0 staran     (501) staff       (20)        7 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/top_level.txt
+-rw-r--r--   0 staran     (501) staff       (20)       38 2024-04-11 05:55:41.733382 avania-0.0.4/setup.cfg
+-rw-r--r--   0 staran     (501) staff       (20)      358 2024-04-11 05:55:07.000000 avania-0.0.4/setup.py
```

### Comparing `avania-0.0.3/LICENSE` & `avania-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.0.3/PKG-INFO` & `avania-0.0.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: avania
-Version: 0.0.3
-Summary: Pays tribute to Laravel
-Author: Simon
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: numpy
-
 # Avania Framework
 
 Avania is a modern Python framework designed to provide an elegant and powerful development experience. It offers a range of components to streamline the development process, including a database ORM, a routing system, middleware support, global exception handling, and more.
 
 ## Installation
 
 You can install Avania globally using pip:
```

