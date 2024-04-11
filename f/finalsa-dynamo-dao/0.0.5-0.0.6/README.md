# Comparing `tmp/finalsa-dynamo-dao-0.0.5.tar.gz` & `tmp/finalsa-dynamo-dao-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-dynamo-dao-0.0.5.tar", last modified: Sun Mar 10 20:45:33 2024, max compression
+gzip compressed data, was "finalsa-dynamo-dao-0.0.6.tar", last modified: Thu Apr 11 01:01:11 2024, max compression
```

## Comparing `finalsa-dynamo-dao-0.0.5.tar` & `finalsa-dynamo-dao-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/base_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-10 20:45:33.000000 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-10 20:45:33.000000 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 20:45:33.000000 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-10 20:45:33.000000 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-10 20:45:33.000000 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 20:45:33.000000 finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 20:45:33.679975 finalsa-dynamo-dao-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-10 20:45:25.000000 finalsa-dynamo-dao-0.0.5/tests/test_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.919224 finalsa-dynamo-dao-0.0.6/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.919224 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:11.000000 finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 01:01:11.927224 finalsa-dynamo-dao-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:11.923224 finalsa-dynamo-dao-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-11 01:01:01.000000 finalsa-dynamo-dao-0.0.6/tests/test_dao.py
```

### Comparing `finalsa-dynamo-dao-0.0.5/LICENSE.md` & `finalsa-dynamo-dao-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.5/PKG-INFO` & `finalsa-dynamo-dao-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dynamo-dao
-Version: 0.0.5
+Version: 0.0.6
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/finalsa-dynamo-dao
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
```

### Comparing `finalsa-dynamo-dao-0.0.5/README.md` & `finalsa-dynamo-dao-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/base.py` & `finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from boto3.dynamodb.types import TypeDeserializer, TypeSerializer
 from datetime import datetime, date
-from decimal import Decimal
+from decimal import Context
 from uuid import UUID
 
 
 def clean_list(items: list):
     result = []
     for v in items:
         if not v:
@@ -24,15 +24,16 @@
 def translate_model_to_dynamo_model(dict: dict):
     serializer = TypeSerializer()
 
     def to_supported_type(v):
         if isinstance(v, datetime):
             return v.isoformat()
         if isinstance(v, float):
-            return Decimal(v)
+            r =  Context(prec=10).create_decimal_from_float(v)
+            return r
         if isinstance(v, date):
             return v.isoformat()
         if isinstance(v, UUID):
             return str(v)
         return v
     return {k: serializer.serialize(to_supported_type(v)) for k, v in dict.items()}
```

### Comparing `finalsa-dynamo-dao-0.0.5/finalsa/dynamo/dao/content/base_dao.py` & `finalsa-dynamo-dao-0.0.6/finalsa/dynamo/dao/content/base_dao.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.5/finalsa_dynamo_dao.egg-info/PKG-INFO` & `finalsa-dynamo-dao-0.0.6/finalsa_dynamo_dao.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalsa-dynamo-dao
-Version: 0.0.5
+Version: 0.0.6
 Summary: An utils package for using dynamodb
 Home-page: https://github.com/finalsa/finalsa-dynamo-dao
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: dynamodb
 Classifier: Intended Audience :: Developers
```

### Comparing `finalsa-dynamo-dao-0.0.5/setup.py` & `finalsa-dynamo-dao-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `finalsa-dynamo-dao-0.0.5/tests/test_dao.py` & `finalsa-dynamo-dao-0.0.6/tests/test_dao.py`

 * *Files identical despite different names*

