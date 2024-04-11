# Comparing `tmp/ticketsdk-2.2.7.tar.gz` & `tmp/ticketsdk-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.2.7.tar", last modified: Thu Apr 11 07:06:10 2024, max compression
+gzip compressed data, was "ticketsdk-2.2.8.tar", last modified: Thu Apr 11 09:39:25 2024, max compression
```

## Comparing `ticketsdk-2.2.7.tar` & `ticketsdk-2.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.701481 ticketsdk-2.2.7/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 07:06:10.701308 ticketsdk-2.2.7/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1511 2024-04-11 06:30:52.000000 ticketsdk-2.2.7/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 07:06:10.701522 ticketsdk-2.2.7/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 07:05:48.000000 ticketsdk-2.2.7/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.700099 ticketsdk-2.2.7/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.7/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.7/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.7/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.700865 ticketsdk-2.2.7/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.7/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3075 2024-04-11 06:30:52.000000 ticketsdk-2.2.7/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 07:06:10.701132 ticketsdk-2.2.7/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 07:06:10.000000 ticketsdk-2.2.7/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.348520 ticketsdk-2.2.8/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 09:39:25.348346 ticketsdk-2.2.8/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1511 2024-04-11 06:30:52.000000 ticketsdk-2.2.8/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 09:39:25.348567 ticketsdk-2.2.8/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 09:39:11.000000 ticketsdk-2.2.8/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.347037 ticketsdk-2.2.8/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.8/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.8/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.8/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.347788 ticketsdk-2.2.8/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.8/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3089 2024-04-11 07:08:34.000000 ticketsdk-2.2.8/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 09:39:25.348168 ticketsdk-2.2.8/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 09:39:25.000000 ticketsdk-2.2.8/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.2.7/README.md` & `ticketsdk-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.7/setup.py` & `ticketsdk-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "ticketsdk"
-version = "2.2.7"
+version = "2.2.8"
 long_desc = (
     """This SDK is a programatic inteface into the ticket APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

### Comparing `ticketsdk-2.2.7/ticketsdk/__init__.py` & `ticketsdk-2.2.8/ticketsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.7/ticketsdk/client.py` & `ticketsdk-2.2.8/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.7/ticketsdk/seller/__init__.py` & `ticketsdk-2.2.8/ticketsdk/seller/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.7/ticketsdk/validators.py` & `ticketsdk-2.2.8/ticketsdk/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         strict = True
         unknown = RAISE
 
 
 class NewSellerSchema(Schema):
     partner_code = fields.Str(required=True)
     email = fields.Str(required=True)
-    cs_email = fields.Str(required=False)
+    cs_email = fields.Str(required=False, default=None)
     lambda_type = fields.Str(required=True)
     name = fields.Str(required=False)
     company_name = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
```

