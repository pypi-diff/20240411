# Comparing `tmp/im_data_manager_metadata-1.1.0-py3-none-any.whl.zip` & `tmp/im_data_manager_metadata-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 18693 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 16:08 data_manager_metadata/__init__.py
--rw-r--r--  2.0 unx     2304 b- defN 24-Apr-10 16:08 data_manager_metadata/annotation_utils.py
--rw-r--r--  2.0 unx    24263 b- defN 24-Apr-10 16:08 data_manager_metadata/data_tier_api.py
--rw-r--r--  2.0 unx     4005 b- defN 24-Apr-10 16:08 data_manager_metadata/exceptions.py
--rw-r--r--  2.0 unx    31795 b- defN 24-Apr-10 16:08 data_manager_metadata/metadata.py
--rw-r--r--  2.0 unx     1080 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4231 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      935 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/RECORD
-10 files, 68727 bytes uncompressed, 17063 bytes compressed:  75.2%
+Zip file size: 18687 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 16:48 data_manager_metadata/__init__.py
+-rw-r--r--  2.0 unx     2304 b- defN 24-Apr-11 16:48 data_manager_metadata/annotation_utils.py
+-rw-r--r--  2.0 unx    24263 b- defN 24-Apr-11 16:48 data_manager_metadata/data_tier_api.py
+-rw-r--r--  2.0 unx     4005 b- defN 24-Apr-11 16:48 data_manager_metadata/exceptions.py
+-rw-r--r--  2.0 unx    31795 b- defN 24-Apr-11 16:49 data_manager_metadata/metadata.py
+-rw-r--r--  2.0 unx     1080 b- defN 24-Apr-11 16:49 im_data_manager_metadata-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4230 b- defN 24-Apr-11 16:49 im_data_manager_metadata-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 16:49 im_data_manager_metadata-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-11 16:49 im_data_manager_metadata-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      935 b- defN 24-Apr-11 16:49 im_data_manager_metadata-2.0.0.dist-info/RECORD
+10 files, 68726 bytes uncompressed, 17057 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: data_manager_metadata/exceptions.py
 Comment: 
 
 Filename: data_manager_metadata/metadata.py
 Comment: 
 
-Filename: im_data_manager_metadata-1.1.0.dist-info/LICENSE
+Filename: im_data_manager_metadata-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: im_data_manager_metadata-1.1.0.dist-info/METADATA
+Filename: im_data_manager_metadata-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: im_data_manager_metadata-1.1.0.dist-info/WHEEL
+Filename: im_data_manager_metadata-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: im_data_manager_metadata-1.1.0.dist-info/top_level.txt
+Filename: im_data_manager_metadata-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: im_data_manager_metadata-1.1.0.dist-info/RECORD
+Filename: im_data_manager_metadata-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `im_data_manager_metadata-1.1.0.dist-info/LICENSE` & `im_data_manager_metadata-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `im_data_manager_metadata-1.1.0.dist-info/METADATA` & `im_data_manager_metadata-2.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-data-manager-metadata
-Version: 1.1.0
+Version: 2.0.0
 Summary: A framework for Informatics Matters dataset metadata
 Home-page: https://github.com/InformaticsMatters/squonk2-data-manager-metadata
 Author: Tim Dudgeon
 Author-email: tdudgeon@informaticsmatters.com
 License: MIT
 Keywords: jenkins
 Platform: any
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3, <4
 License-File: LICENSE
 Requires-Dist: PyYAML <7.0,>=6.0.1
-Requires-Dist: im-data-manager-job-decoder <2.0.0,>=1.17.2
+Requires-Dist: im-data-manager-job-decoder <3.0.0,>=2.0.0
 
 Informatics Matters Data-Manager Metadata
 =========================================
 
 A metadata framework package for the Data Tier Data Manager service.
 The ``im-data-manager-metadata`` package is a set of utilities
 employed by the `Informatics Matters`_ Data-Manager service
```

## Comparing `im_data_manager_metadata-1.1.0.dist-info/RECORD` & `im_data_manager_metadata-2.0.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 data_manager_metadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_manager_metadata/annotation_utils.py,sha256=n20sznImYFS_PvZbk3jQFKqnBzUvCd2r2X9mr0_XWgw,2304
 data_manager_metadata/data_tier_api.py,sha256=SAjBXIfcQarPImsyzE4yBo2DKaB2m-BrunoAF0HkHq0,24263
 data_manager_metadata/exceptions.py,sha256=ofGgCf2LAct76d7fRM7Fb5827-uhjW5fpiqwvBvdXoM,4005
 data_manager_metadata/metadata.py,sha256=J-lkSZIbbY5Wc6I8CYcC0ixM8KkSn7-JiU9WaSWM8Uc,31795
-im_data_manager_metadata-1.1.0.dist-info/LICENSE,sha256=aPo-a09Zp9KzKrL5Spr6s59gb3b4cro7mJ3igSBbqrQ,1080
-im_data_manager_metadata-1.1.0.dist-info/METADATA,sha256=On6f2vE4jLOXp7EC1GybuQ86kze66McwTSMGjYGrY-0,4231
-im_data_manager_metadata-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-im_data_manager_metadata-1.1.0.dist-info/top_level.txt,sha256=ayBYnZrfzouPELqGB79YSQ0oyvL6RonH4kGerlGt5yk,22
-im_data_manager_metadata-1.1.0.dist-info/RECORD,,
+im_data_manager_metadata-2.0.0.dist-info/LICENSE,sha256=aPo-a09Zp9KzKrL5Spr6s59gb3b4cro7mJ3igSBbqrQ,1080
+im_data_manager_metadata-2.0.0.dist-info/METADATA,sha256=TWfCqTbvwtGH4UUWFd8DIK3mO8RKytKvHwJf_Thlx6A,4230
+im_data_manager_metadata-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+im_data_manager_metadata-2.0.0.dist-info/top_level.txt,sha256=ayBYnZrfzouPELqGB79YSQ0oyvL6RonH4kGerlGt5yk,22
+im_data_manager_metadata-2.0.0.dist-info/RECORD,,
```

