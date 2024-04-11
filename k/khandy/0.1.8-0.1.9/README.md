# Comparing `tmp/khandy-0.1.8.tar.gz` & `tmp/khandy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khandy-0.1.8.tar", last modified: Tue Mar 19 12:48:50 2024, max compression
+gzip compressed data, was "khandy-0.1.9.tar", last modified: Tue Mar 19 14:56:06 2024, max compression
```

## Comparing `khandy-0.1.8.tar` & `khandy-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.336554 khandy-0.1.8/
--rw-rw-rw-   0        0        0     1012 2024-03-19 12:48:50.335557 khandy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-10-09 15:29:43.000000 khandy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.300735 khandy-0.1.8/khandy/
--rw-rw-rw-   0        0        0      437 2023-10-07 16:43:18.000000 khandy-0.1.8/khandy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.317932 khandy-0.1.8/khandy/boxes/
--rw-rw-rw-   0        0        0      366 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/__init__.py
--rw-rw-rw-   0        0        0     2534 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_and_indices.py
--rw-rw-rw-   0        0        0     1156 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_clip.py
--rw-rw-rw-   0        0        0     2436 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_coder.py
--rw-rw-rw-   0        0        0     3540 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_convert.py
--rw-rw-rw-   0        0        0     6629 2023-10-09 15:08:54.000000 khandy-0.1.8/khandy/boxes/boxes_filter.py
--rw-rw-rw-   0        0        0     7587 2023-06-10 13:37:49.000000 khandy-0.1.8/khandy/boxes/boxes_overlap.py
--rw-rw-rw-   0        0        0     4694 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_transform_flip.py
--rw-rw-rw-   0        0        0     5268 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_transform_rotate.py
--rw-rw-rw-   0        0        0     3201 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_transform_scale.py
--rw-rw-rw-   0        0        0     4730 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_transform_translate.py
--rw-rw-rw-   0        0        0      685 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/boxes/boxes_utils.py
--rw-rw-rw-   0        0        0     6061 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/dict_utils.py
--rw-rw-rw-   0        0        0     5746 2023-05-06 13:34:07.000000 khandy-0.1.8/khandy/draw_utils.py
--rw-rw-rw-   0        0        0     2202 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/feature_utils.py
--rw-rw-rw-   0        0        0     3874 2024-02-19 11:43:34.000000 khandy-0.1.8/khandy/file_io_utils.py
--rw-rw-rw-   0        0        0    22242 2024-03-11 16:30:27.000000 khandy-0.1.8/khandy/fs_utils.py
--rw-rw-rw-   0        0        0      712 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/hash_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.327065 khandy-0.1.8/khandy/image/
--rw-rw-rw-   0        0        0      204 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/image/__init__.py
--rw-rw-rw-   0        0        0     2127 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/image/align_and_crop.py
--rw-rw-rw-   0        0        0     5115 2023-03-27 11:12:38.000000 khandy-0.1.8/khandy/image/crop_or_pad.py
--rw-rw-rw-   0        0        0     1864 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/image/flip.py
--rw-rw-rw-   0        0        0     2009 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/image/image_hash.py
--rw-rw-rw-   0        0        0    15138 2024-02-19 12:24:00.000000 khandy-0.1.8/khandy/image/misc.py
--rw-rw-rw-   0        0        0     6955 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/image/resize.py
--rw-rw-rw-   0        0        0     2422 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/image/rotate.py
--rw-rw-rw-   0        0        0     2061 2023-03-27 11:12:38.000000 khandy-0.1.8/khandy/image/translate.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.329058 khandy-0.1.8/khandy/label/
--rw-rw-rw-   0        0        0       25 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/label/__init__.py
--rw-rw-rw-   0        0        0    20678 2024-02-19 11:42:06.000000 khandy-0.1.8/khandy/label/detect.py
--rw-rw-rw-   0        0        0    10849 2024-02-19 16:02:47.000000 khandy-0.1.8/khandy/misc.py
--rw-rw-rw-   0        0        0     7763 2024-03-13 13:45:20.000000 khandy-0.1.8/khandy/numpy_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.332566 khandy-0.1.8/khandy/points/
--rw-rw-rw-   0        0        0       91 2023-10-07 17:32:35.000000 khandy-0.1.8/khandy/points/__init__.py
--rw-rw-rw-   0        0        0      632 2023-12-31 02:09:31.000000 khandy-0.1.8/khandy/points/pts_letterbox.py
--rw-rw-rw-   0        0        0      941 2023-10-07 17:32:19.000000 khandy-0.1.8/khandy/points/pts_misc.py
--rw-rw-rw-   0        0        0      943 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/points/pts_transform_scale.py
--rw-rw-rw-   0        0        0     3835 2024-03-08 16:16:49.000000 khandy-0.1.8/khandy/seq_utils.py
--rw-rw-rw-   0        0        0     2048 2024-02-19 11:42:06.000000 khandy-0.1.8/khandy/split_utils.py
--rw-rw-rw-   0        0        0     4366 2024-03-19 10:49:45.000000 khandy-0.1.8/khandy/text_utils.py
--rw-rw-rw-   0        0        0     3208 2023-05-06 13:18:28.000000 khandy-0.1.8/khandy/time_utils.py
--rw-rw-rw-   0        0        0       52 2023-03-10 15:10:32.000000 khandy-0.1.8/khandy/version.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:48:50.334561 khandy-0.1.8/khandy.egg-info/
--rw-rw-rw-   0        0        0     1012 2024-03-19 12:48:50.000000 khandy-0.1.8/khandy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2024-03-19 12:48:50.000000 khandy-0.1.8/khandy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 12:48:50.000000 khandy-0.1.8/khandy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-10 15:10:59.000000 khandy-0.1.8/khandy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2024-03-19 12:48:50.000000 khandy-0.1.8/khandy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-19 12:48:50.000000 khandy-0.1.8/khandy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 12:48:50.336554 khandy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1574 2024-03-19 12:44:29.000000 khandy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.072760 khandy-0.1.9/
+-rw-rw-rw-   0        0        0     1326 2024-03-19 14:56:06.071763 khandy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2024-03-19 14:55:36.000000 khandy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.030718 khandy-0.1.9/khandy/
+-rw-rw-rw-   0        0        0      437 2023-10-07 16:43:18.000000 khandy-0.1.9/khandy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.051656 khandy-0.1.9/khandy/boxes/
+-rw-rw-rw-   0        0        0      366 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/__init__.py
+-rw-rw-rw-   0        0        0     2534 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_and_indices.py
+-rw-rw-rw-   0        0        0     1156 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_clip.py
+-rw-rw-rw-   0        0        0     2436 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_coder.py
+-rw-rw-rw-   0        0        0     3540 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_convert.py
+-rw-rw-rw-   0        0        0     6629 2023-10-09 15:08:54.000000 khandy-0.1.9/khandy/boxes/boxes_filter.py
+-rw-rw-rw-   0        0        0     7587 2023-06-10 13:37:49.000000 khandy-0.1.9/khandy/boxes/boxes_overlap.py
+-rw-rw-rw-   0        0        0     4694 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_transform_flip.py
+-rw-rw-rw-   0        0        0     5268 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_transform_rotate.py
+-rw-rw-rw-   0        0        0     3201 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_transform_scale.py
+-rw-rw-rw-   0        0        0     4730 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_transform_translate.py
+-rw-rw-rw-   0        0        0      685 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/boxes/boxes_utils.py
+-rw-rw-rw-   0        0        0     6061 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/dict_utils.py
+-rw-rw-rw-   0        0        0     5746 2023-05-06 13:34:07.000000 khandy-0.1.9/khandy/draw_utils.py
+-rw-rw-rw-   0        0        0     2202 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/feature_utils.py
+-rw-rw-rw-   0        0        0     3874 2024-02-19 11:43:34.000000 khandy-0.1.9/khandy/file_io_utils.py
+-rw-rw-rw-   0        0        0    22242 2024-03-11 16:30:27.000000 khandy-0.1.9/khandy/fs_utils.py
+-rw-rw-rw-   0        0        0      712 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/hash_utils.py
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.062285 khandy-0.1.9/khandy/image/
+-rw-rw-rw-   0        0        0      204 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/image/__init__.py
+-rw-rw-rw-   0        0        0     2127 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/image/align_and_crop.py
+-rw-rw-rw-   0        0        0     5115 2023-03-27 11:12:38.000000 khandy-0.1.9/khandy/image/crop_or_pad.py
+-rw-rw-rw-   0        0        0     1864 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/image/flip.py
+-rw-rw-rw-   0        0        0     2009 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/image/image_hash.py
+-rw-rw-rw-   0        0        0    15138 2024-02-19 12:24:00.000000 khandy-0.1.9/khandy/image/misc.py
+-rw-rw-rw-   0        0        0     6955 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/image/resize.py
+-rw-rw-rw-   0        0        0     2422 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/image/rotate.py
+-rw-rw-rw-   0        0        0     2061 2023-03-27 11:12:38.000000 khandy-0.1.9/khandy/image/translate.py
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.064780 khandy-0.1.9/khandy/label/
+-rw-rw-rw-   0        0        0       25 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/label/__init__.py
+-rw-rw-rw-   0        0        0    20678 2024-02-19 11:42:06.000000 khandy-0.1.9/khandy/label/detect.py
+-rw-rw-rw-   0        0        0    10849 2024-02-19 16:02:47.000000 khandy-0.1.9/khandy/misc.py
+-rw-rw-rw-   0        0        0     7763 2024-03-13 13:45:20.000000 khandy-0.1.9/khandy/numpy_utils.py
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.068773 khandy-0.1.9/khandy/points/
+-rw-rw-rw-   0        0        0       91 2023-10-07 17:32:35.000000 khandy-0.1.9/khandy/points/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-12-31 02:09:31.000000 khandy-0.1.9/khandy/points/pts_letterbox.py
+-rw-rw-rw-   0        0        0      941 2023-10-07 17:32:19.000000 khandy-0.1.9/khandy/points/pts_misc.py
+-rw-rw-rw-   0        0        0      943 2023-03-10 15:10:32.000000 khandy-0.1.9/khandy/points/pts_transform_scale.py
+-rw-rw-rw-   0        0        0     3835 2024-03-08 16:16:49.000000 khandy-0.1.9/khandy/seq_utils.py
+-rw-rw-rw-   0        0        0     2048 2024-02-19 11:42:06.000000 khandy-0.1.9/khandy/split_utils.py
+-rw-rw-rw-   0        0        0     4366 2024-03-19 10:49:45.000000 khandy-0.1.9/khandy/text_utils.py
+-rw-rw-rw-   0        0        0     3208 2023-05-06 13:18:28.000000 khandy-0.1.9/khandy/time_utils.py
+-rw-rw-rw-   0        0        0       52 2024-03-19 14:55:47.000000 khandy-0.1.9/khandy/version.py
+drwxrwxrwx   0        0        0        0 2024-03-19 14:56:06.070766 khandy-0.1.9/khandy.egg-info/
+-rw-rw-rw-   0        0        0     1326 2024-03-19 14:56:05.000000 khandy-0.1.9/khandy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2024-03-19 14:56:05.000000 khandy-0.1.9/khandy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 14:56:05.000000 khandy-0.1.9/khandy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-10 15:10:59.000000 khandy-0.1.9/khandy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2024-03-19 14:56:05.000000 khandy-0.1.9/khandy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-03-19 14:56:05.000000 khandy-0.1.9/khandy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-19 14:56:06.072760 khandy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2024-03-19 14:24:00.000000 khandy-0.1.9/setup.py
```

### Comparing `khandy-0.1.8/PKG-INFO` & `khandy-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khandy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Handy Utilities for Computer Vision
 Home-page: https://github.com/quarrying/khandy
 Author: quarryman
 Author-email: quarrying@qq.com
 Maintainer: quarryman
 Maintainer-email: quarrying@qq.com
 License: MIT
@@ -22,24 +22,37 @@
 Requires-Dist: requests
 
 ## Overview
 Handy utilities mainly for computer vision
 
 
 ## Installation
+
+khandy requires Python 3.8 or higher. 
+
+### Install the latest stable version from PyPI
+```sh
+pip install -U khandy
 ```
+
+### Install the latest version from the master branch on GitHub
+```sh
+pip install -U git+https://github.com/quarrying/khandy.git
+```
+
+### Install the latest version locally
+```sh
 git clone https://github.com/quarrying/khandy.git
 cd khandy
 pip install -e .
 ```
 
 
 ## Dependencies
-One of the principles of this project is to ensure minimal dependencies.
+One of the principles of this project is to ensure minimal dependencies. Now only depends:
 
-- Python 3.5+
 - NumPy 1.11+
 - OpenCV 2.0+
 - Pillow
 - lxml
 - requests
```

### Comparing `khandy-0.1.8/khandy/boxes/boxes_and_indices.py` & `khandy-0.1.9/khandy/boxes/boxes_and_indices.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_clip.py` & `khandy-0.1.9/khandy/boxes/boxes_clip.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_coder.py` & `khandy-0.1.9/khandy/boxes/boxes_coder.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_convert.py` & `khandy-0.1.9/khandy/boxes/boxes_convert.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_filter.py` & `khandy-0.1.9/khandy/boxes/boxes_filter.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_overlap.py` & `khandy-0.1.9/khandy/boxes/boxes_overlap.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_transform_flip.py` & `khandy-0.1.9/khandy/boxes/boxes_transform_flip.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_transform_rotate.py` & `khandy-0.1.9/khandy/boxes/boxes_transform_rotate.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_transform_scale.py` & `khandy-0.1.9/khandy/boxes/boxes_transform_scale.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_transform_translate.py` & `khandy-0.1.9/khandy/boxes/boxes_transform_translate.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/boxes/boxes_utils.py` & `khandy-0.1.9/khandy/boxes/boxes_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/dict_utils.py` & `khandy-0.1.9/khandy/dict_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/draw_utils.py` & `khandy-0.1.9/khandy/draw_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/feature_utils.py` & `khandy-0.1.9/khandy/feature_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/file_io_utils.py` & `khandy-0.1.9/khandy/file_io_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/fs_utils.py` & `khandy-0.1.9/khandy/fs_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/hash_utils.py` & `khandy-0.1.9/khandy/hash_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/align_and_crop.py` & `khandy-0.1.9/khandy/image/align_and_crop.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/crop_or_pad.py` & `khandy-0.1.9/khandy/image/crop_or_pad.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/flip.py` & `khandy-0.1.9/khandy/image/flip.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/image_hash.py` & `khandy-0.1.9/khandy/image/image_hash.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/misc.py` & `khandy-0.1.9/khandy/image/misc.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/resize.py` & `khandy-0.1.9/khandy/image/resize.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/rotate.py` & `khandy-0.1.9/khandy/image/rotate.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/image/translate.py` & `khandy-0.1.9/khandy/image/translate.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/label/detect.py` & `khandy-0.1.9/khandy/label/detect.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/misc.py` & `khandy-0.1.9/khandy/misc.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/numpy_utils.py` & `khandy-0.1.9/khandy/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/points/pts_letterbox.py` & `khandy-0.1.9/khandy/points/pts_letterbox.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/points/pts_misc.py` & `khandy-0.1.9/khandy/points/pts_misc.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/points/pts_transform_scale.py` & `khandy-0.1.9/khandy/points/pts_transform_scale.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/seq_utils.py` & `khandy-0.1.9/khandy/seq_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/split_utils.py` & `khandy-0.1.9/khandy/split_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/text_utils.py` & `khandy-0.1.9/khandy/text_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy/time_utils.py` & `khandy-0.1.9/khandy/time_utils.py`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/khandy.egg-info/PKG-INFO` & `khandy-0.1.9/khandy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khandy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Handy Utilities for Computer Vision
 Home-page: https://github.com/quarrying/khandy
 Author: quarryman
 Author-email: quarrying@qq.com
 Maintainer: quarryman
 Maintainer-email: quarrying@qq.com
 License: MIT
@@ -22,24 +22,37 @@
 Requires-Dist: requests
 
 ## Overview
 Handy utilities mainly for computer vision
 
 
 ## Installation
+
+khandy requires Python 3.8 or higher. 
+
+### Install the latest stable version from PyPI
+```sh
+pip install -U khandy
 ```
+
+### Install the latest version from the master branch on GitHub
+```sh
+pip install -U git+https://github.com/quarrying/khandy.git
+```
+
+### Install the latest version locally
+```sh
 git clone https://github.com/quarrying/khandy.git
 cd khandy
 pip install -e .
 ```
 
 
 ## Dependencies
-One of the principles of this project is to ensure minimal dependencies.
+One of the principles of this project is to ensure minimal dependencies. Now only depends:
 
-- Python 3.5+
 - NumPy 1.11+
 - OpenCV 2.0+
 - Pillow
 - lxml
 - requests
```

### Comparing `khandy-0.1.8/khandy.egg-info/SOURCES.txt` & `khandy-0.1.9/khandy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khandy-0.1.8/setup.py` & `khandy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     version=get_version(),
     description='Handy Utilities for Computer Vision',
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     keywords='computer vision',
     packages=find_packages(),
-    
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Utilities',
     ],
     url='https://github.com/quarrying/khandy',
```

