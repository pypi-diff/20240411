# Comparing `tmp/rg3py-0.0.7-py3-none-win_amd64.whl.zip` & `tmp/rg3py-0.0.8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7957277 bytes, number of entries: 7
--rw-r--r--  2.0 unx      921 b- defN 24-Apr-08 18:35 rg3py/__init__.py
--rw-r--r--  2.0 unx 20624384 b- defN 24-Apr-08 18:35 rg3py/rg3py.pyd
--rw-r--r--  2.0 unx     8432 b- defN 24-Apr-08 18:35 rg3py/rg3py.pyi
--rw-r--r--  2.0 unx     4821 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      510 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/RECORD
-7 files, 20639172 bytes uncompressed, 7956389 bytes compressed:  61.5%
+Zip file size: 7957290 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      921 b- defN 24-Apr-11 17:15 rg3py/__init__.py
+-rw-r--r--  2.0 unx 20624384 b- defN 24-Apr-11 17:15 rg3py/rg3py.pyd
+-rw-r--r--  2.0 unx     8432 b- defN 24-Apr-11 17:15 rg3py/rg3py.pyi
+-rw-r--r--  2.0 unx     4917 b- defN 24-Apr-11 17:15 rg3py-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-11 17:15 rg3py-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-11 17:15 rg3py-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      510 b- defN 24-Apr-11 17:15 rg3py-0.0.8.dist-info/RECORD
+7 files, 20639268 bytes uncompressed, 7956402 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: rg3py/rg3py.pyd
 Comment: 
 
 Filename: rg3py/rg3py.pyi
 Comment: 
 
-Filename: rg3py-0.0.7.dist-info/METADATA
+Filename: rg3py-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: rg3py-0.0.7.dist-info/WHEEL
+Filename: rg3py-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: rg3py-0.0.7.dist-info/top_level.txt
+Filename: rg3py-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: rg3py-0.0.7.dist-info/RECORD
+Filename: rg3py-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rg3py-0.0.7.dist-info/METADATA` & `rg3py-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: rg3py
-Version: 0.0.7
+Version: 0.0.8
 Summary: RG3 is a C/C++ analyzer framework
 Author: DronCode
 Author-email: alexandrleutin@gmail.com
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

