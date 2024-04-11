# Comparing `tmp/ticketsdk-2.2.6.tar.gz` & `tmp/ticketsdk-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.2.6.tar", last modified: Thu Apr 11 06:31:17 2024, max compression
+gzip compressed data, was "ticketsdk-2.2.7.tar", last modified: Thu Apr 11 07:06:10 2024, max compression
```

## Comparing `ticketsdk-2.2.6.tar` & `ticketsdk-2.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.340834 ticketsdk-2.2.6/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 06:31:17.340639 ticketsdk-2.2.6/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1511 2024-04-11 06:30:52.000000 ticketsdk-2.2.6/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 06:31:17.340877 ticketsdk-2.2.6/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 06:31:03.000000 ticketsdk-2.2.6/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.339332 ticketsdk-2.2.6/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.6/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.6/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.6/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.340115 ticketsdk-2.2.6/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.6/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3075 2024-04-11 06:30:52.000000 ticketsdk-2.2.6/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.340421 ticketsdk-2.2.6/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.701481 ticketsdk-2.2.7/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 07:06:10.701308 ticketsdk-2.2.7/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1511 2024-04-11 06:30:52.000000 ticketsdk-2.2.7/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 07:06:10.701522 ticketsdk-2.2.7/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 07:05:48.000000 ticketsdk-2.2.7/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.700099 ticketsdk-2.2.7/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.7/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.7/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.7/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.700865 ticketsdk-2.2.7/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.7/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3075 2024-04-11 06:30:52.000000 ticketsdk-2.2.7/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.701132 ticketsdk-2.2.7/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.2.6/README.md` & `ticketsdk-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.6/setup.py` & `ticketsdk-2.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "ticketsdk"
-version = "2.2.6"
+version = "2.2.7"
 long_desc = (
     """This SDK is a programatic inteface into the ticket APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

### Comparing `ticketsdk-2.2.6/ticketsdk/__init__.py` & `ticketsdk-2.2.7/ticketsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.6/ticketsdk/client.py` & `ticketsdk-2.2.7/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.6/ticketsdk/seller/__init__.py` & `ticketsdk-2.2.7/ticketsdk/seller/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.6/ticketsdk/validators.py` & `ticketsdk-2.2.7/ticketsdk/validators.py`

 * *Files identical despite different names*

