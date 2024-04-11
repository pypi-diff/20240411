# Comparing `tmp/prusek_spheroid-4.6.tar.gz` & `tmp/prusek_spheroid-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-4.6.tar", last modified: Wed Apr 10 08:13:45 2024, max compression
+gzip compressed data, was "prusek_spheroid-4.7.tar", last modified: Wed Apr 10 14:45:12 2024, max compression
```

## Comparing `prusek_spheroid-4.6.tar` & `prusek_spheroid-4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 08:13:45.051813 prusek_spheroid-4.6/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 08:13:45.051483 prusek_spheroid-4.6/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.6/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 08:13:45.050274 prusek_spheroid-4.6/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.6/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    52159 2024-04-10 08:13:09.000000 prusek_spheroid-4.6/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12428 2024-04-06 18:03:18.000000 prusek_spheroid-4.6/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.6/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.6/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.6/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.6/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.6/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.6/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.6/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.6/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 08:13:45.051252 prusek_spheroid-4.6/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 08:13:45.000000 prusek_spheroid-4.6/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-10 08:13:45.000000 prusek_spheroid-4.6/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-10 08:13:45.000000 prusek_spheroid-4.6/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-10 08:13:45.000000 prusek_spheroid-4.6/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-10 08:13:45.000000 prusek_spheroid-4.6/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-10 08:13:45.051866 prusek_spheroid-4.6/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-10 08:13:41.000000 prusek_spheroid-4.6/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 14:45:12.346092 prusek_spheroid-4.7/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 14:45:12.345871 prusek_spheroid-4.7/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.7/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 14:45:12.344825 prusek_spheroid-4.7/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.7/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    52159 2024-04-10 08:13:09.000000 prusek_spheroid-4.7/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-4.7/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.7/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.7/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.7/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.7/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.7/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.7/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.7/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.7/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 14:45:12.345642 prusek_spheroid-4.7/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-10 14:45:12.346142 prusek_spheroid-4.7/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-10 14:44:58.000000 prusek_spheroid-4.7/setup.py
```

### Comparing `prusek_spheroid-4.6/PKG-INFO` & `prusek_spheroid-4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.6
+Version: 4.7
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-4.6/README.md` & `prusek_spheroid-4.7/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-4.7/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/GUI.py` & `prusek_spheroid-4.7/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-4.7/prusek_spheroid/GradientDescentGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         self.data = data  # data by měla být seznamem trojic
 
     def __len__(self):
         return len(self.data)
 
     def __getitem__(self, idx):
         mask, image, name = self.data[idx]
+        if mask is None or image is None or name is None:
+            raise ValueError(f"Data at index {idx} contains None. Please check the input dataset.")
         return mask, image, name
 
 
 class GradientDescent:
     def __init__(self, annotation_data, outputAddress, projekt, algorithm, learning_rate,
                  num_iterations, delta, batch_size, f, progress_window=None, contours_state=None,
                  detect_corrupted=True):
```

### Comparing `prusek_spheroid-4.6/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-4.7/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/conversion.py` & `prusek_spheroid-4.7/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/file_management.py` & `prusek_spheroid-4.7/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/image_processing.py` & `prusek_spheroid-4.7/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/merge_directories.py` & `prusek_spheroid-4.7/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/methods.py` & `prusek_spheroid-4.7/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/metrics.py` & `prusek_spheroid-4.7/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-4.7/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-4.7/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.6
+Version: 4.7
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-4.6/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-4.7/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.6/setup.py` & `prusek_spheroid-4.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="4.6",
+    version="4.7",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

