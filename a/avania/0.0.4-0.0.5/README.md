# Comparing `tmp/avania-0.0.4.tar.gz` & `tmp/avania-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.0.4.tar", last modified: Thu Apr 11 05:55:41 2024, max compression
+gzip compressed data, was "avania-0.0.5.tar", last modified: Thu Apr 11 06:11:50 2024, max compression
```

## Comparing `avania-0.0.4.tar` & `avania-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:55:41.733342 avania-0.0.4/
--rw-r--r--   0 staran     (501) staff       (20)     1742 2024-04-11 04:09:41.000000 avania-0.0.4/LICENSE
--rw-r--r--   0 staran     (501) staff       (20)     2237 2024-04-11 05:55:41.733118 avania-0.0.4/PKG-INFO
--rw-r--r--   0 staran     (501) staff       (20)      662 2024-04-11 04:48:48.000000 avania-0.0.4/README.md
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:55:41.732037 avania-0.0.4/avania/
--rw-r--r--   0 staran     (501) staff       (20)       30 2024-04-11 05:21:55.000000 avania-0.0.4/avania/__init__.py
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 05:55:41.732822 avania-0.0.4/avania.egg-info/
--rw-r--r--   0 staran     (501) staff       (20)     2237 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/PKG-INFO
--rw-r--r--   0 staran     (501) staff       (20)      194 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/SOURCES.txt
--rw-r--r--   0 staran     (501) staff       (20)        1 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/dependency_links.txt
--rw-r--r--   0 staran     (501) staff       (20)       15 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/requires.txt
--rw-r--r--   0 staran     (501) staff       (20)        7 2024-04-11 05:55:41.000000 avania-0.0.4/avania.egg-info/top_level.txt
--rw-r--r--   0 staran     (501) staff       (20)       38 2024-04-11 05:55:41.733382 avania-0.0.4/setup.cfg
--rw-r--r--   0 staran     (501) staff       (20)      358 2024-04-11 05:55:07.000000 avania-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:11:50.112424 avania-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-11 06:11:42.000000 avania-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 06:11:50.108424 avania-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 06:11:42.000000 avania-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:11:50.108424 avania-0.0.5/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 06:11:42.000000 avania-0.0.5/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:11:50.108424 avania-0.0.5/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 06:11:50.000000 avania-0.0.5/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 06:11:50.000000 avania-0.0.5/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:11:50.000000 avania-0.0.5/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 06:11:50.000000 avania-0.0.5/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 06:11:50.000000 avania-0.0.5/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:11:50.112424 avania-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 06:11:42.000000 avania-0.0.5/setup.py
```

### Comparing `avania-0.0.4/LICENSE` & `avania-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.0.4/PKG-INFO` & `avania-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
```

### Comparing `avania-0.0.4/README.md` & `avania-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.0.4/avania.egg-info/PKG-INFO` & `avania-0.0.5/avania.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
```

