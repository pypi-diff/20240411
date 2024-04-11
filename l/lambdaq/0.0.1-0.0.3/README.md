# Comparing `tmp/lambdaq-0.0.1-py3-none-any.whl.zip` & `tmp/lambdaq-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
 Zip file size: 7056 bytes, number of entries: 16
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-10 16:33 lambdaq/VERSION
--rw-r--r--  2.0 unx      244 b- defN 24-Apr-10 16:11 lambdaq/__init__.py
--rw-r--r--  2.0 unx     2651 b- defN 24-Apr-10 16:27 lambdaq/event_handler.py
--rw-r--r--  2.0 unx      961 b- defN 24-Apr-10 16:13 lambdaq/handle_event.py
--rw-r--r--  2.0 unx       89 b- defN 24-Apr-10 11:31 lambdaq/logging.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 12:46 lambdaq/py.typed
--rw-r--r--  2.0 unx      215 b- defN 24-Apr-10 11:31 lambdaq/types/__init__.py
--rw-r--r--  2.0 unx       59 b- defN 24-Apr-10 11:31 lambdaq/types/message.py
--rw-r--r--  2.0 unx      167 b- defN 24-Apr-10 11:32 lambdaq/types/message_handler.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 10:46 lambdaq/types/py.typed
--rw-r--r--  2.0 unx       61 b- defN 24-Apr-10 11:31 lambdaq/types/response.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-10 16:33 lambdaq-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4129 b- defN 24-Apr-10 16:33 lambdaq-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 16:33 lambdaq-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-10 16:33 lambdaq-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1236 b- defN 24-Apr-10 16:33 lambdaq-0.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-11 06:59 lambdaq/VERSION
+-rw-r--r--  2.0 unx      244 b- defN 24-Apr-11 06:59 lambdaq/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 24-Apr-11 06:59 lambdaq/event_handler.py
+-rw-r--r--  2.0 unx      961 b- defN 24-Apr-11 06:59 lambdaq/handle_event.py
+-rw-r--r--  2.0 unx       89 b- defN 24-Apr-11 06:59 lambdaq/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 06:59 lambdaq/py.typed
+-rw-r--r--  2.0 unx      215 b- defN 24-Apr-11 06:59 lambdaq/types/__init__.py
+-rw-r--r--  2.0 unx       59 b- defN 24-Apr-11 06:59 lambdaq/types/message.py
+-rw-r--r--  2.0 unx      167 b- defN 24-Apr-11 06:59 lambdaq/types/message_handler.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 06:59 lambdaq/types/py.typed
+-rw-r--r--  2.0 unx       61 b- defN 24-Apr-11 06:59 lambdaq/types/response.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-Apr-11 06:59 lambdaq-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4129 b- defN 24-Apr-11 06:59 lambdaq-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 06:59 lambdaq-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-11 06:59 lambdaq-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1236 b- defN 24-Apr-11 06:59 lambdaq-0.0.3.dist-info/RECORD
 16 files, 10991 bytes uncompressed, 5014 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: lambdaq/types/py.typed
 Comment: 
 
 Filename: lambdaq/types/response.py
 Comment: 
 
-Filename: lambdaq-0.0.1.dist-info/LICENSE
+Filename: lambdaq-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: lambdaq-0.0.1.dist-info/METADATA
+Filename: lambdaq-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: lambdaq-0.0.1.dist-info/WHEEL
+Filename: lambdaq-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: lambdaq-0.0.1.dist-info/top_level.txt
+Filename: lambdaq-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: lambdaq-0.0.1.dist-info/RECORD
+Filename: lambdaq-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lambdaq/VERSION

```diff
@@ -1 +1 @@
-0.0.1
+0.0.3
```

## Comparing `lambdaq-0.0.1.dist-info/LICENSE` & `lambdaq-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lambdaq-0.0.1.dist-info/METADATA` & `lambdaq-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaq
-Version: 0.0.1
+Version: 0.0.3
 Summary: Helps you write Amazon Web Services Lambda functions called by Step Functions via SQS
 Author: Cariad Eccleston
 Author-email: cariad@cariad.earth
 License: MIT
 Project-URL: Project, https://github.com/cariad/lambdaq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lambdaq-0.0.1.dist-info/RECORD` & `lambdaq-0.0.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-lambdaq/VERSION,sha256=5mNQReHSR47EynEtjA4d_O-Lt7Wx6OO7Vg03_jmannI,6
+lambdaq/VERSION,sha256=TKwna27F1Mcc2Wyi57di6xJUOa28hyHeVhMQbRNF_i0,6
 lambdaq/__init__.py,sha256=Z9fGKOKW5-rfWA0tVrdwVckK-uM9oSbHaS84HjFHDPQ,244
 lambdaq/event_handler.py,sha256=1hKeD3o2Jge9ha4zwU0kT10RYp2IykdoJyJeVox_PyY,2651
 lambdaq/handle_event.py,sha256=aQuDwIhlRai6TnybW1lBspPppXeEYLJE5qoVP0H7LmE,961
 lambdaq/logging.py,sha256=CRfvNy4vKBdAt2viao5lTtDFRrsq6tti9AjvBkCgu3s,89
 lambdaq/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lambdaq/types/__init__.py,sha256=R4k_2OeLdvKbyffFw3jWbZYuaWfDW9NThoNpnrXCspw,215
 lambdaq/types/message.py,sha256=ryIJnCraE0BDK2d_suET0VkN_MjvCIcjJE2cKxksiqo,59
 lambdaq/types/message_handler.py,sha256=3EMvfatnRPrPbMwGCNTmWBT4iVxdqajEBsmmX9aJDSs,167
 lambdaq/types/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lambdaq/types/response.py,sha256=IKagKXpdVEhAurqdXDrDvNUGXTj67bYGQQrHQoTAXRk,61
-lambdaq-0.0.1.dist-info/LICENSE,sha256=4g0rxlvaGRJXe119BmPUqMzp-9r5q7R4oRnrncQJWvU,1073
-lambdaq-0.0.1.dist-info/METADATA,sha256=l8mfRwGHzBQbHmqvJC0ALjH2fLMMlvkIQWDG5Ok_TJ8,4129
-lambdaq-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-lambdaq-0.0.1.dist-info/top_level.txt,sha256=43SyedRqVg0zyo4GDd6Cvr-v3LPzw-Z7WaxrRhpv07A,8
-lambdaq-0.0.1.dist-info/RECORD,,
+lambdaq-0.0.3.dist-info/LICENSE,sha256=4g0rxlvaGRJXe119BmPUqMzp-9r5q7R4oRnrncQJWvU,1073
+lambdaq-0.0.3.dist-info/METADATA,sha256=L0zbcpPGCARyANQGAfNduKCnJu0iMBqjwrydpawDfAE,4129
+lambdaq-0.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+lambdaq-0.0.3.dist-info/top_level.txt,sha256=43SyedRqVg0zyo4GDd6Cvr-v3LPzw-Z7WaxrRhpv07A,8
+lambdaq-0.0.3.dist-info/RECORD,,
```

