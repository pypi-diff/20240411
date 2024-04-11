# Comparing `tmp/Avania-0.0.0.tar.gz` & `tmp/avania-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Avania-0.0.0.tar", last modified: Thu Apr 11 03:30:00 2024, max compression
+gzip compressed data, was "avania-0.0.1.tar", last modified: Thu Apr 11 03:30:44 2024, max compression
```

## Comparing `Avania-0.0.0.tar` & `avania-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 03:30:00.156018 Avania-0.0.0/
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 03:30:00.155480 Avania-0.0.0/Avania.egg-info/
--rw-r--r--   0 staran     (501) staff       (20)      166 2024-04-11 03:30:00.000000 Avania-0.0.0/Avania.egg-info/PKG-INFO
--rw-r--r--   0 staran     (501) staff       (20)      199 2024-04-11 03:30:00.000000 Avania-0.0.0/Avania.egg-info/SOURCES.txt
--rw-r--r--   0 staran     (501) staff       (20)        1 2024-04-11 03:30:00.000000 Avania-0.0.0/Avania.egg-info/dependency_links.txt
--rw-r--r--   0 staran     (501) staff       (20)       15 2024-04-11 03:30:00.000000 Avania-0.0.0/Avania.egg-info/requires.txt
--rw-r--r--   0 staran     (501) staff       (20)       12 2024-04-11 03:30:00.000000 Avania-0.0.0/Avania.egg-info/top_level.txt
--rw-r--r--   0 staran     (501) staff       (20)     1074 2024-04-11 03:00:42.000000 Avania-0.0.0/LICENSE
--rw-r--r--   0 staran     (501) staff       (20)      166 2024-04-11 03:30:00.155762 Avania-0.0.0/PKG-INFO
--rw-r--r--   0 staran     (501) staff       (20)        0 2024-04-11 02:59:31.000000 Avania-0.0.0/README.md
-drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 03:30:00.155212 Avania-0.0.0/example_pkg/
--rw-r--r--   0 staran     (501) staff       (20)        0 2024-04-11 02:58:48.000000 Avania-0.0.0/example_pkg/__init__.py
--rw-r--r--   0 staran     (501) staff       (20)       38 2024-04-11 03:30:00.156060 Avania-0.0.0/setup.cfg
--rw-r--r--   0 staran     (501) staff       (20)      256 2024-04-11 03:29:57.000000 Avania-0.0.0/setup.py
+drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 03:30:44.401584 avania-0.0.1/
+-rw-r--r--   0 staran     (501) staff       (20)     1074 2024-04-11 03:00:42.000000 avania-0.0.1/LICENSE
+-rw-r--r--   0 staran     (501) staff       (20)      166 2024-04-11 03:30:44.401359 avania-0.0.1/PKG-INFO
+-rw-r--r--   0 staran     (501) staff       (20)        0 2024-04-11 02:59:31.000000 avania-0.0.1/README.md
+drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 03:30:44.401121 avania-0.0.1/avania.egg-info/
+-rw-r--r--   0 staran     (501) staff       (20)      166 2024-04-11 03:30:44.000000 avania-0.0.1/avania.egg-info/PKG-INFO
+-rw-r--r--   0 staran     (501) staff       (20)      199 2024-04-11 03:30:44.000000 avania-0.0.1/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 staran     (501) staff       (20)        1 2024-04-11 03:30:44.000000 avania-0.0.1/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 staran     (501) staff       (20)       15 2024-04-11 03:30:44.000000 avania-0.0.1/avania.egg-info/requires.txt
+-rw-r--r--   0 staran     (501) staff       (20)       12 2024-04-11 03:30:44.000000 avania-0.0.1/avania.egg-info/top_level.txt
+drwxr-xr-x   0 staran     (501) staff       (20)        0 2024-04-11 03:30:44.400963 avania-0.0.1/example_pkg/
+-rw-r--r--   0 staran     (501) staff       (20)        0 2024-04-11 02:58:48.000000 avania-0.0.1/example_pkg/__init__.py
+-rw-r--r--   0 staran     (501) staff       (20)       38 2024-04-11 03:30:44.401621 avania-0.0.1/setup.cfg
+-rw-r--r--   0 staran     (501) staff       (20)      256 2024-04-11 03:30:41.000000 avania-0.0.1/setup.py
```

### Comparing `Avania-0.0.0/LICENSE` & `avania-0.0.1/LICENSE`

 * *Files identical despite different names*

