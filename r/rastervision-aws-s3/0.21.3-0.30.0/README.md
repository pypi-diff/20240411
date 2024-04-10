# Comparing `tmp/rastervision_aws_s3-0.21.3.tar.gz` & `tmp/rastervision_aws_s3-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_aws_s3-0.21.3.tar", last modified: Tue Oct 17 19:14:41 2023, max compression
+gzip compressed data, was "rastervision_aws_s3-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
```

## Comparing `rastervision_aws_s3-0.21.3.tar` & `rastervision_aws_s3-0.30.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.763311 rastervision_aws_s3-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      550 2023-10-17 19:14:41.763311 rastervision_aws_s3-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.759311 rastervision_aws_s3-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.759311 rastervision_aws_s3-0.21.3/rastervision/aws_s3/
--rw-rw-r--   0 root         (0) root         (0)      421 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.21.3/rastervision/aws_s3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10519 2023-09-08 19:48:40.000000 rastervision_aws_s3-0.21.3/rastervision/aws_s3/s3_file_system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.763311 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/
--rw-r--r--   0 root         (0) root         (0)      550 2023-10-17 19:14:41.000000 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-10-17 19:14:41.000000 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       72 2023-10-17 19:14:41.000000 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:41.000000 rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       73 2023-10-17 13:37:07.000000 rastervision_aws_s3-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:41.763311 rastervision_aws_s3-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1129 2023-10-17 13:37:07.000000 rastervision_aws_s3-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/rastervision/aws_s3/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      421 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.30.0/rastervision/aws_s3/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10519 2024-04-07 00:38:15.000000 rastervision_aws_s3-0.30.0/rastervision/aws_s3/s3_file_system.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      363 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       40 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       75 2024-04-10 21:55:10.000000 rastervision_aws_s3-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1717 2024-04-10 21:55:10.000000 rastervision_aws_s3-0.30.0/setup.py
```

### Comparing `rastervision_aws_s3-0.21.3/PKG-INFO` & `rastervision_aws_s3-0.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_aws_s3
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds an AWS S3 file system
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_s3-0.21.3/rastervision/aws_s3/s3_file_system.py` & `rastervision_aws_s3-0.30.0/rastervision/aws_s3/s3_file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_aws_s3-0.21.3/rastervision_aws_s3.egg-info/PKG-INFO` & `rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-aws-s3
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds an AWS S3 file system
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

