# Comparing `tmp/prusek_spheroid-4.7.tar.gz` & `tmp/prusek_spheroid-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-4.7.tar", last modified: Wed Apr 10 14:45:12 2024, max compression
+gzip compressed data, was "prusek_spheroid-4.8.tar", last modified: Thu Apr 11 04:47:42 2024, max compression
```

## Comparing `prusek_spheroid-4.7.tar` & `prusek_spheroid-4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 14:45:12.346092 prusek_spheroid-4.7/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 14:45:12.345871 prusek_spheroid-4.7/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-4.7/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 14:45:12.344825 prusek_spheroid-4.7/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.7/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    52159 2024-04-10 08:13:09.000000 prusek_spheroid-4.7/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-4.7/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.7/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.7/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.7/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.7/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.7/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.7/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.7/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.7/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-10 14:45:12.345642 prusek_spheroid-4.7/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9116 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-10 14:45:12.000000 prusek_spheroid-4.7/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-10 14:45:12.346142 prusek_spheroid-4.7/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-10 14:44:58.000000 prusek_spheroid-4.7/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-11 04:47:42.493340 prusek_spheroid-4.8/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9112 2024-04-11 04:47:42.493126 prusek_spheroid-4.8/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8540 2024-04-10 14:46:55.000000 prusek_spheroid-4.8/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-11 04:47:42.491897 prusek_spheroid-4.8/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19403 2024-04-09 19:07:14.000000 prusek_spheroid-4.8/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    52459 2024-04-11 04:47:16.000000 prusek_spheroid-4.8/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-4.8/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-4.8/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-4.8/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7199 2024-04-04 16:33:02.000000 prusek_spheroid-4.8/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-4.8/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-4.8/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-4.8/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-4.8/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-4.8/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-11 04:47:42.492908 prusek_spheroid-4.8/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9112 2024-04-11 04:47:42.000000 prusek_spheroid-4.8/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-11 04:47:42.000000 prusek_spheroid-4.8/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-11 04:47:42.000000 prusek_spheroid-4.8/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-11 04:47:42.000000 prusek_spheroid-4.8/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-11 04:47:42.000000 prusek_spheroid-4.8/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-11 04:47:42.493386 prusek_spheroid-4.8/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-11 04:47:30.000000 prusek_spheroid-4.8/setup.py
```

### Comparing `prusek_spheroid-4.7/PKG-INFO` & `prusek_spheroid-4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.7
+Version: 4.8
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -76,15 +76,15 @@
 
 Prusek-Spheroid is a sophisticated Python package equipped with a user-friendly graphical interface (GUI) that facilitates image segmentation and optimization tasks. This guide provides an overview of the GUI functionalities and how to use them effectively. The whole program is based on the knowledge of segmentations of several (approximately 15 to 20) spheroids. Based on these segmentations, the program learns to segment the remaining spheroid images in the dataset (project). So far the only possible formats in which the segmentations can be loaded are the COCO 1.0 format or loading masks and corresponding images. This is the format supported by the CVAT (Computer Vision Annotation Tool) platform.
 
 ### Using the Spheroid Segmentation GUI
 
 The Prusek-Spheroid GUI is designed to be intuitive, providing a range of functionalities for effective image segmentation. Here’s a detailed overview of the key elements:
 
-1. **Input File and Folder Selection**: These two sections are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files.
+1. **Input File and Folder Selection**: These two tabs are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files.
 
 2. **Output Folder Selection**: After processing, the results will be saved in the selected output folder. This feature allows you to specify where you want the segmented images and other outputs to be stored. If selected, the properties of the contours are also saved in the resulting folder as an excel file. Furthermore, the JSON file with the optimal parameters is also saved in the selected output folder in the "IoU" subfolder.
 
 3. **Project Name Field**: Here, you enter the name of your project. This name will be used for organizing and saving the results in a structured manner.
 
 4. **'I Already Know the Parameters' Checkbox**: If you have pre-determined parameters from a previous Gradient descent project, you can use this checkbox. It's useful when you want to segment images using already optimized parameters without going through the Gradient descent process again. Is also recommended to use when knowing the parameters from a visually similar project. The learned parameters are usually located in the "IoU" pad in the output directory as a JSON file.
```

### Comparing `prusek_spheroid-4.7/README.md` & `prusek_spheroid-4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 Prusek-Spheroid is a sophisticated Python package equipped with a user-friendly graphical interface (GUI) that facilitates image segmentation and optimization tasks. This guide provides an overview of the GUI functionalities and how to use them effectively. The whole program is based on the knowledge of segmentations of several (approximately 15 to 20) spheroids. Based on these segmentations, the program learns to segment the remaining spheroid images in the dataset (project). So far the only possible formats in which the segmentations can be loaded are the COCO 1.0 format or loading masks and corresponding images. This is the format supported by the CVAT (Computer Vision Annotation Tool) platform.
 
 ### Using the Spheroid Segmentation GUI
 
 The Prusek-Spheroid GUI is designed to be intuitive, providing a range of functionalities for effective image segmentation. Here’s a detailed overview of the key elements:
 
-1. **Input File and Folder Selection**: These two sections are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files.
+1. **Input File and Folder Selection**: These two tabs are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files.
 
 2. **Output Folder Selection**: After processing, the results will be saved in the selected output folder. This feature allows you to specify where you want the segmented images and other outputs to be stored. If selected, the properties of the contours are also saved in the resulting folder as an excel file. Furthermore, the JSON file with the optimal parameters is also saved in the selected output folder in the "IoU" subfolder.
 
 3. **Project Name Field**: Here, you enter the name of your project. This name will be used for organizing and saving the results in a structured manner.
 
 4. **'I Already Know the Parameters' Checkbox**: If you have pre-determined parameters from a previous Gradient descent project, you can use this checkbox. It's useful when you want to segment images using already optimized parameters without going through the Gradient descent process again. Is also recommended to use when knowing the parameters from a visually similar project. The learned parameters are usually located in the "IoU" pad in the output directory as a JSON file.
```

### Comparing `prusek_spheroid-4.7/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-4.8/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/GUI.py` & `prusek_spheroid-4.8/prusek_spheroid/GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1036,21 +1036,25 @@
             return
 
         if self.loaded_parameters is None:
             if current_tab == self.coco_tab:
                 annotation_address = self.coco_annotation_path.get()
                 annotation_address = fm.unzip(annotation_address)
                 annotations_address, images_address = update_addresses(annotation_address)
+                print(f"Loading annotations JSON from: {annotations_address}")
+                print(f"Loading reference Images from: {images_address}")
                 annotation_data = fm.load_annotations(
                     os.path.join(annotations_address, 'instances_default.json'), images_address)
                 print(f"Loaded {len(annotation_data)} annotated images")
             elif current_tab == self.mask_tab:
-                mask_adress = self.masks_annotation_path.get()
+                mask_address = self.masks_annotation_path.get()
                 images_address = self.image_dataset_path.get()
-                annotation_data = fm.load_masks_from_images(mask_adress, images_address)
+                print(f"Loading reference Masks from: {mask_address}")
+                print(f"Loading reference Images from: {images_address}")
+                annotation_data = fm.load_masks_from_images(mask_address, images_address)
                 print(f"Loaded {len(annotation_data)} annotated images")
         else:
             annotation_data = None
 
         dataset_address = self.dataset_path.get()
         output_address = self.output_path.get()
```

### Comparing `prusek_spheroid-4.7/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-4.8/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-4.8/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/conversion.py` & `prusek_spheroid-4.8/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/file_management.py` & `prusek_spheroid-4.8/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/image_processing.py` & `prusek_spheroid-4.8/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/merge_directories.py` & `prusek_spheroid-4.8/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/methods.py` & `prusek_spheroid-4.8/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/metrics.py` & `prusek_spheroid-4.8/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-4.8/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-4.8/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 4.7
+Version: 4.8
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -76,15 +76,15 @@
 
 Prusek-Spheroid is a sophisticated Python package equipped with a user-friendly graphical interface (GUI) that facilitates image segmentation and optimization tasks. This guide provides an overview of the GUI functionalities and how to use them effectively. The whole program is based on the knowledge of segmentations of several (approximately 15 to 20) spheroids. Based on these segmentations, the program learns to segment the remaining spheroid images in the dataset (project). So far the only possible formats in which the segmentations can be loaded are the COCO 1.0 format or loading masks and corresponding images. This is the format supported by the CVAT (Computer Vision Annotation Tool) platform.
 
 ### Using the Spheroid Segmentation GUI
 
 The Prusek-Spheroid GUI is designed to be intuitive, providing a range of functionalities for effective image segmentation. Here’s a detailed overview of the key elements:
 
-1. **Input File and Folder Selection**: These two sections are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files.
+1. **Input File and Folder Selection**: These two tabs are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files.
 
 2. **Output Folder Selection**: After processing, the results will be saved in the selected output folder. This feature allows you to specify where you want the segmented images and other outputs to be stored. If selected, the properties of the contours are also saved in the resulting folder as an excel file. Furthermore, the JSON file with the optimal parameters is also saved in the selected output folder in the "IoU" subfolder.
 
 3. **Project Name Field**: Here, you enter the name of your project. This name will be used for organizing and saving the results in a structured manner.
 
 4. **'I Already Know the Parameters' Checkbox**: If you have pre-determined parameters from a previous Gradient descent project, you can use this checkbox. It's useful when you want to segment images using already optimized parameters without going through the Gradient descent process again. Is also recommended to use when knowing the parameters from a visually similar project. The learned parameters are usually located in the "IoU" pad in the output directory as a JSON file.
```

### Comparing `prusek_spheroid-4.7/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-4.8/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-4.7/setup.py` & `prusek_spheroid-4.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="4.7",
+    version="4.8",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

