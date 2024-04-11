# Comparing `tmp/cntracer-1.1.65-cp39-cp39-win_amd64.whl.zip` & `tmp/cntracer-1.7.10-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 115624 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   340480 b- defN 23-Oct-12 09:09 cntracer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 23-Oct-12 09:09 cntracer-1.1.65.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      234 b- defN 23-Oct-12 09:09 cntracer-1.1.65.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Oct-12 09:09 cntracer-1.1.65.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Oct-12 09:09 cntracer-1.1.65.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      481 b- defN 23-Oct-12 09:09 cntracer-1.1.65.dist-info/RECORD
-6 files, 343486 bytes uncompressed, 114754 bytes compressed:  66.6%
+Zip file size: 155729 bytes, number of entries: 8
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-11 05:11 cntracer.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-11 05:11 cntracer-1.7.10.dist-info/
+-rwxr-xr-x  2.0 unx   563712 b- defN 24-Apr-11 05:11 cntracer.cpython-311-aarch64-linux-gnu.so
+-rw-r--r--  2.0 unx      223 b- defN 24-Apr-11 05:11 cntracer-1.7.10.dist-info/METADATA
+-rw-r--r--  2.0 unx     2182 b- defN 24-Apr-11 05:11 cntracer-1.7.10.dist-info/LICENSE
+-rw-r--r--  2.0 unx      154 b- defN 24-Apr-11 05:11 cntracer-1.7.10.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-11 05:11 cntracer-1.7.10.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      501 b- defN 24-Apr-11 05:11 cntracer-1.7.10.dist-info/RECORD
+8 files, 566781 bytes uncompressed, 154599 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
-Filename: cntracer.cp39-win_amd64.pyd
+Filename: cntracer.libs/
 Comment: 
 
-Filename: cntracer-1.1.65.dist-info/LICENSE
+Filename: cntracer-1.7.10.dist-info/
 Comment: 
 
-Filename: cntracer-1.1.65.dist-info/METADATA
+Filename: cntracer.cpython-311-aarch64-linux-gnu.so
 Comment: 
 
-Filename: cntracer-1.1.65.dist-info/WHEEL
+Filename: cntracer-1.7.10.dist-info/METADATA
 Comment: 
 
-Filename: cntracer-1.1.65.dist-info/top_level.txt
+Filename: cntracer-1.7.10.dist-info/LICENSE
 Comment: 
 
-Filename: cntracer-1.1.65.dist-info/RECORD
+Filename: cntracer-1.7.10.dist-info/WHEEL
+Comment: 
+
+Filename: cntracer-1.7.10.dist-info/top_level.txt
+Comment: 
+
+Filename: cntracer-1.7.10.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `cntracer-1.1.65.dist-info/LICENSE` & `cntracer-1.7.10.dist-info/LICENSE`

 * *Files identical despite different names*

