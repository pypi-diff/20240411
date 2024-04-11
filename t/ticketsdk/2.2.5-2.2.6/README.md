# Comparing `tmp/ticketsdk-2.2.5.tar.gz` & `tmp/ticketsdk-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.2.5.tar", last modified: Thu Apr 11 04:55:09 2024, max compression
+gzip compressed data, was "ticketsdk-2.2.6.tar", last modified: Thu Apr 11 06:31:17 2024, max compression
```

## Comparing `ticketsdk-2.2.5.tar` & `ticketsdk-2.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 04:55:09.446215 ticketsdk-2.2.5/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 04:55:09.445949 ticketsdk-2.2.5/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1442 2024-04-09 08:31:06.000000 ticketsdk-2.2.5/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 04:55:09.446373 ticketsdk-2.2.5/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 04:54:58.000000 ticketsdk-2.2.5/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 04:55:09.443771 ticketsdk-2.2.5/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.5/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.5/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.5/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 04:55:09.444718 ticketsdk-2.2.5/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.5/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3074 2024-04-11 04:54:25.000000 ticketsdk-2.2.5/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 04:55:09.444990 ticketsdk-2.2.5/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 04:55:09.000000 ticketsdk-2.2.5/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 04:55:09.000000 ticketsdk-2.2.5/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 04:55:09.000000 ticketsdk-2.2.5/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 04:55:09.000000 ticketsdk-2.2.5/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 04:55:09.000000 ticketsdk-2.2.5/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.340834 ticketsdk-2.2.6/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 06:31:17.340639 ticketsdk-2.2.6/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1511 2024-04-11 06:30:52.000000 ticketsdk-2.2.6/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-11 06:31:17.340877 ticketsdk-2.2.6/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-11 06:31:03.000000 ticketsdk-2.2.6/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.339332 ticketsdk-2.2.6/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.6/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.6/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.6/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.340115 ticketsdk-2.2.6/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3118 2024-04-09 08:03:12.000000 ticketsdk-2.2.6/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3075 2024-04-11 06:30:52.000000 ticketsdk-2.2.6/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-11 06:31:17.340421 ticketsdk-2.2.6/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-11 06:31:17.000000 ticketsdk-2.2.6/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.2.5/README.md` & `ticketsdk-2.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 ### Add new seller:
 ```
 Connection(body = {
     "partner_code":"111",
     "email":"dan5@gmail.com",
     "cs_email": "tri.nm@nandhlogistics.vn",
-    "lambda_type" :"map"
+    "lambda_type" :"map",
+    "name":"name option",
+    "company_name":"company_name option",
 }).add_new_seller()
 ```
 ### Add ticket:
 ```
 Connection(body = {
     "partner_code":"111",
     "ref_code":"test_23_03_2024",
```

### Comparing `ticketsdk-2.2.5/setup.py` & `ticketsdk-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "ticketsdk"
-version = "2.2.5"
+version = "2.2.6"
 long_desc = (
     """This SDK is a programatic inteface into the ticket APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

### Comparing `ticketsdk-2.2.5/ticketsdk/__init__.py` & `ticketsdk-2.2.6/ticketsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.5/ticketsdk/client.py` & `ticketsdk-2.2.6/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.5/ticketsdk/seller/__init__.py` & `ticketsdk-2.2.6/ticketsdk/seller/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.5/ticketsdk/validators.py` & `ticketsdk-2.2.6/ticketsdk/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         strict = True
         unknown = RAISE
 
 
 class NewSellerSchema(Schema):
     partner_code = fields.Str(required=True)
     email = fields.Str(required=True)
-    cs_email = fields.Str(required=True)
+    cs_email = fields.Str(required=False)
     lambda_type = fields.Str(required=True)
     name = fields.Str(required=False)
     company_name = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
```

