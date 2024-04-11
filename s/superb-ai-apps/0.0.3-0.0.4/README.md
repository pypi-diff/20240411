# Comparing `tmp/superb-ai-apps-0.0.3.tar.gz` & `tmp/superb-ai-apps-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb-ai-apps-0.0.3.tar", last modified: Fri Apr  5 06:54:49 2024, max compression
+gzip compressed data, was "superb-ai-apps-0.0.4.tar", last modified: Thu Apr 11 13:22:34 2024, max compression
```

## Comparing `superb-ai-apps-0.0.3.tar` & `superb-ai-apps-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/spb_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/spb_apps/curate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/curate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/curate/superb_curate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/spb_apps/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/label/superb_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/spb_apps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-05 06:54:32.000000 superb-ai-apps-0.0.3/spb_apps/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:54:49.979259 superb-ai-apps-0.0.3/superb_ai_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 06:54:49.000000 superb-ai-apps-0.0.3/superb_ai_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 06:54:49.000000 superb-ai-apps-0.0.3/superb_ai_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:54:49.000000 superb-ai-apps-0.0.3/superb_ai_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 06:54:49.000000 superb-ai-apps-0.0.3/superb_ai_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 06:54:49.000000 superb-ai-apps-0.0.3/superb_ai_apps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/curate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/curate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/curate/superb_curate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/label/superb_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/top_level.txt
```

### Comparing `superb-ai-apps-0.0.3/setup.py` & `superb-ai-apps-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="superb-ai-apps",
-    version="0.0.3",
+    version="0.0.4",
     description="Python Package for Superb-AI Apps",
     install_requires=[
         "asttokens==2.4.1",
         "attrs==23.2.0",
         "backcall==0.2.0",
         "beautifulsoup4==4.12.3",
         "bleach==6.1.0",
```

### Comparing `superb-ai-apps-0.0.3/spb_apps/apps.py` & `superb-ai-apps-0.0.4/spb_apps/apps.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,62 +6,70 @@
 from spb_apps.label.superb_label import SuperbLabel
 from spb_apps.utils.converter import convert_yolo_bbox
 from spb_apps.utils.utils import read_info_from_zip_yolo
 
 
 class SuperbApps:
     """
-    A class to manage and interact with Superb applications Label and Curate.
+    This class manages interactions with Superb applications, specifically Label and Curate platforms.
+    It provides functionalities to download images, upload images and annotations, change project contexts,
+    and more, based on the specified platform.
     """
 
     def __init__(
         self,
         team_name: str,
         access_key: str,
         platform: str,
+        dev: bool = False,
         project_id: str = "",
         project_name: str = "",
-        dataset_name="",
+        dataset_name: str = "",
     ):
         """
-        Initializes the SuperbApps instance with necessary details and clients based on the platform.
+        Initializes the SuperbApps instance with necessary details and sets up clients for the specified platform.
 
         Args:
             team_name (str): The name of the team.
             access_key (str): The access key for authentication.
-            platform (list): A list of platforms to initialize (e.g., ['label', 'curate']).
-            project_id (str, optional): The ID of the project for labeling. Defaults to "".
-            dataset_name (str, optional): The name of the dataset for Curate. Defaults to "".
+            platform (str): The platform to initialize (either 'label' or 'curate').
+            dev (bool, optional): Flag to indicate if this is a development instance. Defaults to False.
+            project_id (str, optional): The ID of the project for labeling. Only required for 'label' platform. Defaults to "".
+            project_name (str, optional): The name of the project for labeling. Only required for 'label' platform. Defaults to "".
+            dataset_name (str, optional): The name of the dataset for Curate. Only required for 'curate' platform. Defaults to "".
         """
         self.team_name = team_name
         self.access_key = access_key
+        platform = platform.lower()
         if platform == "label":
             self.client = SuperbLabel(
                 team_name=team_name,
                 access_key=access_key,
                 project_id=project_id,
                 project_name=project_name,
             )
 
             self.label_project_name = self.client.client._project.name
         if platform == "curate":
             self.client = SuperbCurate(
                 team_name=team_name,
                 access_key=access_key,
                 dataset_name=dataset_name,
+                is_dev=dev,
             )
+            self.dataset_name = dataset_name
         self.platform = platform
 
     def download_image_by_key(self, data_key: str, path: str = None):
         """
-        Downloads an image by its data key.
+        Downloads an image using its unique data key.
 
         Args:
-            data_key (str): The data key of the image to download.
-            path (str, optional): The local file path where the image will be saved. Defaults to None.
+            data_key (str): The unique identifier for the image.
+            path (str, optional): The local file path to save the downloaded image. Defaults to None.
         """
         if self.platform == "label":
             _, label = self.client.get_labels(data_key=data_key)
             self.client.download_image(label=label[0], path=path)
         if self.platform == "curate":
             self.client.download_image(data_key=data_key, download_path=path)
 
@@ -73,17 +81,17 @@
         path: str = None,
     ):
         """
         Downloads images by applying filters such as tags, data key, and status.
 
         Args:
             tags (list, optional): A list of tags to filter images. Defaults to [].
-            data_key (str, optional): A data key to filter images. Defaults to "".
+            data_key (str, optional): A specific data key to filter images. Defaults to "".
             status (list, optional): A list of statuses to filter images. Defaults to [].
-            path (str, optional): The local file path where the images will be saved. Defaults to None.
+            path (str, optional): The local file path to save the downloaded images. Defaults to None.
         """
         from concurrent.futures import ThreadPoolExecutor
 
         if self.platform == "label":
 
             def download(label):
                 self.client.download_image(label=label, path=path)
@@ -95,39 +103,39 @@
             if count > 50:
                 with ThreadPoolExecutor(max_workers=4) as executor:
                     executor.map(download, labels)
             else:
                 for label in labels:
                     download(label)
         else:
-            print("Curate does not have filters")
+            print("Curate does not support filters for downloading images.")
 
     def get_width_height(
         self, data_hanler: spb_label.DataHandle = None, data_key: str = ""
     ) -> Tuple[int, int]:
         """
         Retrieves the width and height of an image based on its data key.
 
-        This method supports both 'label' and 'curate' platforms. It fetches the image's dimensions
-        by utilizing the respective client's method to get the width and height.
-
         Args:
-            data_key (str): The unique identifier for the image.
+            data_hanler (spb_label.DataHandle, optional): The data handler object for 'label' platform. Defaults to None.
+            data_key (str, optional): The unique identifier for the image for 'curate' platform. Defaults to "".
 
         Returns:
             Tuple[int, int]: A tuple containing the width and height of the image.
         """
         if self.platform == "label":
-            if data_hanler == None:
-                print("Label takes data handler object from spb_label")
+            if data_hanler is None:
+                print(
+                    "Label platform requires a data handler object from spb_label."
+                )
                 return
             return self.client.get_width_height(label=data_hanler)
         if self.platform == "curate":
             if data_key == "":
-                print("Curate takes data key")
+                print("Curate platform requires a data key.")
                 return
             return self.client.get_width_height(data_key=data_key)
 
     def get_labels(
         self,
         data_key: str = "",
         tags: list = [],
@@ -144,15 +152,15 @@
             assignees (list, optional): A list of assignees to filter labels. Defaults to [].
             status (list, optional): A list of statuses to filter labels. Defaults to [].
             all (bool, optional): If True, retrieves all labels ignoring other filters. Defaults to False.
 
         Returns:
             Tuple[int, List]: A tuple containing the count of labels and a list of labels.
         """
-        count, labels = self.label_client.get_labels(
+        count, labels = self.client.get_labels(
             data_key=data_key,
             tags=tags,
             assignees=assignees,
             status=status,
             all=all,
         )
 
@@ -161,41 +169,46 @@
     def change_project(self, project_name: str):
         """
         Changes the project context for the label client.
 
         Args:
             project_name (str): The name of the project to switch to.
         """
-        self.label_client.client.set_project(name=project_name)
-        self.label_project_name = self.label_client.client._project.name
+        if self.platform == "label":
+            self.client.client.set_project(name=project_name)
+            self.label_project_name = self.client.client._project.name
+        else:
+            print("Curate platform does not support changing projects.")
 
     def get_label_interface(self) -> Dict:
         """
-        Retrieves the label interface configuration.
+        Retrieves the label interface configuration for the 'label' platform.
 
         Returns:
-            Dict: The label interface configuration.
+            Dict: The label interface configuration, or prints a message if the platform is 'curate'.
         """
-        lb_interface = self.label_client.client.project.label_interface
-        return lb_interface
+        if self.platform == "label":
+            lb_interface = self.client.client.project.label_interface
+            return lb_interface
+        else:
+            print(
+                "Curate platform does not support label interface retrieval."
+            )
 
     def make_bbox(self, class_name: str, annotation: list, data_key: str = ""):
         """
         Creates a bounding box based on the specified platform ('label' or 'curate').
 
         Args:
             class_name (str): The class name associated with the bounding box.
             annotation (list): A list containing the x, y coordinates, width, and height of the bounding box.
             data_key (str, optional): The unique identifier for the image. Required for 'curate' platform.
 
         Returns:
             The result of the bounding box setting operation, which varies by platform.
-            For 'label', it returns the result of `client.bbox_setting` with class_name and annotation.
-            For 'curate', it additionally requires a data_key and returns the result of `client.bbox_setting` with data_key, class_name, and annotation.
-            If the required data_key is not provided for 'curate', it prints a message and returns None.
         """
         if self.platform == "label":
             return self.client.bbox_setting(
                 class_name=class_name, annotation=annotation
             )
         if self.platform == "curate":
             if data_key == "":
@@ -205,75 +218,130 @@
                 data_key=data_key, class_name=class_name, annotation=annotation
             )
 
     def upload_images(self, images_path: str, dataset_name: str = ""):
         """
         Uploads images to the specified platform ('label' or 'curate').
 
-        For the 'label' platform, a dataset name must be specified. If not, an error message is printed.
-        For the 'curate' platform, images are uploaded without needing a dataset name.
-
         Args:
             images_path (str): The path to the images to be uploaded.
             dataset_name (str, optional): The name of the dataset to upload the images to. Required for 'label' platform.
 
         Returns:
             The result of the image upload operation, which varies by platform.
-            For 'label', it returns the result of `client.upload_image` with images_path and dataset_name.
-            For 'curate', it returns the result of `client.curate_upload_images` with images_path.
-            If the required dataset_name is not provided for 'label', it prints a message and returns None.
         """
         if self.platform == "label":
             if dataset_name == "":
-                print("Must specify a dataset name when uploading to Label")
+                print(
+                    "Must specify a dataset name when uploading to Label platform."
+                )
                 return
             return self.client.upload_image(images_path, dataset_name)
         if self.platform == "curate":
             return self.client.curate_upload_images(images_path)
 
     def upload_annotations(
         self, data_key: str, annotations: list, format: str, classes: list = ""
-    ):
+    ) -> str:
         """
         Uploads annotations to the specified platform ('label' or 'curate') based on the provided format.
 
-        For the 'label' platform and 'yolo' format, it converts YOLO annotations to the platform's format and uploads them.
-        Requires a list of classes for 'yolo' format. If classes are not provided, it prints a message and returns None.
-
         Args:
-            data_key (str): The unique identifier for the data to which the annotations belong.
+            data_key (str): The unique identifier for the image or dataset.
             annotations (list): A list of annotations to be uploaded.
-            format (str): The format of the annotations ('yolo', etc.).
-            classes (list, optional): The list of classes associated with the annotations. Required for 'yolo' format.
+            format (str): The format of the annotations ('yolo' supported).
+            classes (list, optional): The classes associated with the annotations. Required if format is 'yolo'.
 
         Returns:
-            None. Prints a message if classes are not provided for 'yolo' format.
+            str: The status of the upload operation ('Completed', 'Skipped', or 'Failed').
         """
+        status = "Completed"
         if self.platform == "label":
             _, label = self.client.get_labels(data_key=data_key)
+            if len(label) == 0:
+                print(
+                    f"[SKIPPED] Data key: {data_key}, does not exist in project {self.label_project_name}"
+                )
+                status = "Skipped"
+                return status
             data_handler = label[0]
             if format == "yolo":
                 if classes == "":
                     print(
-                        "To upload yolo annotations, you must provide a classes."
+                        "To upload yolo annotations, you must provide classes."
                     )
-                    return
-                width, height = self.get_width_height(data_handler)
+                    status = "Failed"
+                    return status
+                width, height = self.get_width_height(
+                    data_handler=data_handler
+                )
                 converted_annotations = convert_yolo_bbox(
                     data_key, annotations, classes, width, height
                 )
                 if converted_annotations is not None:
                     self.client.upload_annotation(
                         data_handler, converted_annotations
                     )
 
-    def read_yolo_zip(self, dataset_file: str):
+        if self.platform == "curate":
+            if format == "yolo":
+                if classes == "":
+                    print(
+                        "To upload yolo annotations, you must provide classes."
+                    )
+                    status = "Failed"
+                    return status
+                bbox_annotation = []
+                try:
+                    width, height = self.get_width_height(data_key=data_key)
+                except:
+                    return "Skipped"
+                converted_annotations = convert_yolo_bbox(
+                    data_key, annotations, classes, width, height
+                )
+                if converted_annotations is not None:
+                    for anno in converted_annotations:
+                        bbox = self.client.bbox_setting(
+                            data_key,
+                            anno[0],
+                            anno[1],
+                        )
+                        bbox_annotation.append(bbox)
+
+                self.client.curate_upload_annotations(bbox_annotation)
+
+        return status
+
+    def build_label_interface(self, class_list: list, bbox: bool = True):
         """
-        Reads information from a YOLO formatted zip file.
+        Builds the label interface for the 'label' platform based on the provided class list and bbox flag.
 
         Args:
-            dataset_file (str): The path to the YOLO formatted zip file.
+            class_list (list): The list of classes to include in the label interface.
+            bbox (bool, optional): Flag to indicate if bounding boxes should be included. Defaults to True.
 
         Returns:
-            The information read from the zip file.
+            The result of the label interface building operation for 'label' platform, or prints a message for 'curate'.
+        """
+        if self.platform == "label":
+            return self.client.build_label_interface_from_yolo(
+                class_list, bbox
+            )
+        else:
+            print(
+                "Curate platform does not support building a Label Interface."
+            )
+
+    def download_image_by_slice(self, slice_name: str, download_path: str):
+        """
+        Downloads an image by its slice name to a specified path. This method is exclusive to the Curate platform.
+
+        Args:
+            slice_name (str): The name of the slice from which to download the image.
+            download_path (str): The local file path where the downloaded image will be saved.
         """
-        return read_info_from_zip_yolo(dataset_file)
+        if self.platform == "curate":
+            self.client.download_image_by_slice(
+                slice_name=slice_name, download_path=download_path
+            )
+        else:
+            print("Download by slice is only for Curate platform.")
```

### Comparing `superb-ai-apps-0.0.3/spb_apps/curate/superb_curate.py` & `superb-ai-apps-0.0.4/spb_apps/curate/superb_curate.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,74 +8,79 @@
 
 import requests
 import spb_curate
 from spb_curate.error import ConflictError
 
 from spb_apps.utils.utils import separate_batches
 
-SLEEP_INTERVAL = 5  # time in seconds to wait between loop iterations
+SLEEP_INTERVAL = 5  # Time in seconds to wait between loop iterations.
 
 
 class SuperbCurate(object):
+    """
+    A class to handle dataset curation tasks including image and annotation uploads for Superb AI.
+
+    Attributes:
+        team_name (str): Name of the team.
+        access_key (str): Access key for authentication.
+        dataset_name (str): Name of the dataset (optional).
+        slice_name (str): Name of the slice within the dataset (optional).
+        is_dev (bool): Flag to set the environment to development mode (optional).
+    """
+
     def __init__(
         self,
         team_name: str,
         access_key: str,
         dataset_name: str = "",
         slice_name: str = "",
         is_dev: bool = False,
     ):
         """
         Initializes the SuperbCurate class with team, dataset, and slice details.
         Optionally sets the environment to development mode.
 
-        :param team_name: Name of the team
-        :param access_key: Access key for authentication
-        :param dataset_name: Name of the dataset (optional)
-        :param slice_name: Name of the slice within the dataset (optional)
-        :param is_dev: Flag to set the environment to development mode (optional)
-        """
-        self.team_name: str = team_name  # Team name
-        self.access_key: str = access_key  # Access key for authentication
-        self.dataset_name: str = dataset_name  # Dataset name (optional)
-        # Set global variables in spb_curate module for team name and access key
+        Args:
+            team_name (str): Name of the team.
+            access_key (str): Access key for authentication.
+            dataset_name (str, optional): Name of the dataset.
+            slice_name (str, optional): Name of the slice within the dataset.
+            is_dev (bool, optional): Flag to set the environment to development mode.
+        """
+        self.team_name: str = team_name
+        self.access_key: str = access_key
+        self.dataset_name: str = dataset_name
         spb_curate.team_name = self.team_name
         spb_curate.access_key = self.access_key
-        # Set API base URL to development environment if in development mode
         if is_dev:
             spb_curate.api_base = "https://api.dev.superb-ai.com"
 
-        # Attempt to fetch the dataset if a dataset name is provided
-        if len(dataset_name) > 0:
+        if dataset_name:
             try:
                 self.dataset = spb_curate.fetch_dataset(name=dataset_name)
             except ConflictError:
-                # Notify the user if the dataset does not exist and needs to be created
                 print(
                     f"Dataset does not exist, Creating Dataset {dataset_name}"
                 )
                 self.dataset = spb_curate.create_dataset(
                     name=dataset_name, description="Demo dataset."
                 )
-        # Attempt to fetch the slice from the dataset if a slice name is provided
-        if len(slice_name) > 0:
-            self.slice = self.dataset.fetch_slice(
-                name=slice_name
-            )  # Fetch the slice
+
+        if slice_name:
+            self.slice = self.dataset.fetch_slice(name=slice_name)
 
     def curate_prep_images(self, images_path: list) -> List[spb_curate.Image]:
         """
-        This will prep local images for Superb Curate by creating a list of
-        Superb Curate images.
+        Prepares local images for Superb Curate by creating a list of Superb Curate images.
 
         Args:
-            images_path (list): list of paths to upload
+            images_path (list): List of paths to images to be uploaded.
 
         Returns:
-            List[spb_curate.Image]: list of curate images to upload
+            List[spb_curate.Image]: List of prepared images for upload.
         """
         curate_images: List[spb_curate.Image] = []
         for image in images_path:
             curate_images.append(
                 spb_curate.Image(
                     key=image.split("/")[-1],
                     source=spb_curate.ImageSourceLocal(asset=image),
@@ -88,163 +93,128 @@
     def curate_upload_images(self, image_path: list):
         """
         Uploads images in batches to the dataset.
 
         Args:
             image_path (list): List of image paths to upload.
         """
-        # Separate images into batches of 500
-        seperated_images = separate_batches(
+        separated_images = separate_batches(
             image_batch_size=500, to_batch_list=image_path
         )
-        total_loops = len(seperated_images)  # Total number of batches
-        for idx, sep_images in enumerate(seperated_images, start=1):
-            # Prepare images for upload
+        total_loops = len(separated_images)
+        for idx, sep_images in enumerate(separated_images, start=1):
             curate_images = self.curate_prep_images(images_path=sep_images)
-            # Create bulk image import job
             image_import_job = spb_curate.Image.create_bulk(
-                dataset_id=self.curate_dataset["id"], images=curate_images
+                dataset_id=self.dataset["id"], images=curate_images
             )
 
             print(f"created an image import job: ({idx}/{total_loops})")
-            start_time = timer()  # Start timing the upload process
+            start_time = timer()
 
             while True:
-                # Fetch the current status of the import job
                 image_import_job = spb_curate.Job.fetch(
                     id=image_import_job["id"]
                 )
                 print(
                     f"job progress: {image_import_job['progress']}", end="\r"
                 )
 
-                # Check if the job is complete
                 if image_import_job["status"] == "COMPLETE":
-                    # Print any failure details if present
                     if image_import_job["result"]["fail_detail"]:
                         print(image_import_job["result"]["fail_detail"])
                         print(image_import_job["fail_reason"])
-                    break  # Exit the loop if job is complete
+                    break
 
                 if image_import_job["status"] == "FAILED":
                     if image_import_job["result"]["fail_detail"]:
                         print(
                             "[INFO] Fail detail: ",
                             image_import_job["result"]["fail_detail"],
                         )
                         print(
                             "[INFO] Fail reason: ",
                             image_import_job["fail_reason"],
                         )
                     break
-                time.sleep(
-                    SLEEP_INTERVAL
-                )  # Wait before checking the status again
+                time.sleep(SLEEP_INTERVAL)
 
-            print(
-                f"total time: {timer() - start_time}"
-            )  # Print total upload time
+            print(f"total time: {timer() - start_time}")
 
     def curate_prep_annotations(self, annotation: list) -> List:
         """
         Prepares annotations for upload by creating a list of spb_curate.Annotation objects.
 
         Args:
             annotation (list): List of dictionaries containing annotation details.
 
         Returns:
             List[spb_curate.Annotation]: List of prepared annotations for upload.
         """
         curate_annotations: List[spb_curate.Annotation] = []
         for anno in annotation:
-            meta = anno.get(
-                "metadata", {"iscrowd": 0}
-            )  # Safely get metadata or default
+            meta = anno.get("metadata", {"iscrowd": 0})
             curate_annotations.append(
                 spb_curate.Annotation(
-                    image_key=anno[
-                        "data_key"
-                    ],  # Key of the image being annotated
-                    annotation_class=anno[
-                        "class_name"
-                    ],  # Class of the annotation
-                    annotation_type=anno[
-                        "annotation_type"
-                    ],  # Type of annotation (e.g., bounding box, segmentation)
-                    annotation_value=anno[
-                        "annotation"
-                    ],  # The actual annotation data
+                    image_key=anno["data_key"],
+                    annotation_class=anno["class_name"],
+                    annotation_type=anno["annotation_type"],
+                    annotation_value=anno["annotation"],
                     metadata=meta,
                 )
             )
 
         return curate_annotations
 
-    def curate_upload_annotations(
-        self,
-        annotation_list: list,
-    ):
+    def curate_upload_annotations(self, annotation_list: list):
         """
         Uploads annotations in batches to the dataset.
 
         Args:
-            annotation_list (list): List of annotations to upload. Format is a
-                                    list of dicts that are made up of "class_name", "annotation", "data_key", "annotation_type", "metadata" (optional)
+            annotation_list (list): List of annotations to upload.
         """
-        # Separate annotations into batches of 500 for upload
-        seperated_images = separate_batches(
+        separated_annotations = separate_batches(
             image_batch_size=500, to_batch_list=annotation_list
         )
-        for idx, sep_annotations in enumerate(seperated_images, start=1):
-            # Prepare annotations for upload
-            # Create bulk annotation import job
+        for idx, sep_annotations in enumerate(separated_annotations, start=1):
             annotation_import_job = spb_curate.Annotation.create_bulk(
-                dataset_id=self.curate_dataset[
-                    "id"
-                ],  # Dataset ID to upload annotations to
-                annotations=sep_annotations,  # Prepared annotations for upload
+                dataset_id=self.dataset["id"], annotations=sep_annotations
             )
 
             while True:
-                # Fetch the current status of the annotation import job
                 annotation_import_job = spb_curate.Job.fetch(
                     id=annotation_import_job["id"]
                 )
-
                 print(
                     f"[INFO] {(idx-1) * 500 + annotation_import_job['progress']} / {len(annotation_list)} labels updated"
                 )
 
                 if annotation_import_job["status"] == "COMPLETE":
-                    # Check for and print any failure details if present
                     if annotation_import_job["result"]["fail_detail"]:
                         print(
                             "[INFO] Fail detail: ",
                             annotation_import_job["result"]["fail_detail"],
                         )
                         print(
                             "[INFO] Fail reason: ",
                             annotation_import_job["fail_reason"],
                         )
-                    break  # Exit the loop if job is complete
+                    break
 
                 if annotation_import_job["status"] == "FAILED":
                     if annotation_import_job["result"]["fail_detail"]:
                         print(
                             "[INFO] Fail detail: ",
                             annotation_import_job["result"]["fail_detail"],
                         )
                         print(
                             "[INFO] Fail reason: ",
                             annotation_import_job["fail_reason"],
                         )
                     break
-                time.sleep(
-                    SLEEP_INTERVAL
-                )  # Wait before checking the status again
+                time.sleep(SLEEP_INTERVAL)
 
     def get_width_height(self, data_key: str) -> Tuple[int, int]:
         """
         Fetches the width and height of an image using its data key.
 
         Args:
             data_key (str): The unique identifier for the image.
@@ -256,24 +226,34 @@
         meta = image["metadata"]
         width, height = meta["_width"], meta["_height"]
         return width, height
 
     def download_image(self, data_key: str, download_path: str):
         """
         Downloads an image from the dataset using its data key.
+
+        Args:
+            data_key (str): The unique identifier for the image.
+            download_path (str): The path where the image will be downloaded.
         """
         image_url = self.dataset.fetch_images(
             key=data_key, include_image_url=True
         )[0]["image_url"]
         try:
             response = requests.get(image_url)
-            response.raise_for_status()  # Raises an HTTPError if the response status code is 4XX/5XX
-            with open(download_path, "wb") as f:
+            response.raise_for_status()
+            os.makedirs(
+                os.path.dirname(os.path.join(download_path, data_key)),
+                exist_ok=True,
+            )
+            with open(os.path.join(download_path, data_key), "wb") as f:
                 f.write(response.content)
-            print(f"[INFO] Image downloaded successfully: {download_path}")
+            print(
+                f"[INFO] Image downloaded successfully: {os.path.join(download_path, data_key)}"
+            )
         except requests.exceptions.RequestException as e:
             print(f"[ERROR] Failed to download image: {e}")
 
     def bbox_setting(
         self, data_key: str, class_name: str, annotation: list
     ) -> spb_curate.Annotation:
         """
@@ -289,18 +269,38 @@
         """
         bounding_box = spb_curate.BoundingBox(
             raw_data={
                 "x": annotation[0],
                 "y": annotation[1],
                 "width": annotation[2],
                 "height": annotation[3],
-            },
+            }
         )
         bbox_annotation = spb_curate.Annotation(
             image_key=data_key,
             annotation_class=class_name,
             annotation_type="box",
             annotation_value=bounding_box,
             metadata={},
         )
 
         return bbox_annotation
+
+    def download_image_by_slice(self, slice_name: str, download_path: str):
+        """
+        Downloads all images within a specified slice of the dataset.
+
+        This method fetches all image keys within a given slice and iteratively
+        downloads each image to the specified download path.
+
+        Args:
+            slice_name (str): The name of the slice from which to download images.
+            download_path (str): The local file path where the images will be saved.
+        """
+        slice = self.dataset.fetch_images(
+            slice=slice_name, include_image_url=True
+        )
+        # image_keys = slice.fetch_images()
+        for image in slice:
+            self.download_image(
+                data_key=image["key"], download_path=download_path
+            )
```

### Comparing `superb-ai-apps-0.0.3/spb_apps/label/superb_label.py` & `superb-ai-apps-0.0.4/spb_apps/label/superb_label.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,140 +17,133 @@
         self,
         team_name: str,
         access_key: str,
         project_id: str = "",
         project_name: str = "",
     ):
         """
-        Initializes the SuperbLabel class with necessary details for operation.
+        Initialize the SuperbLabel class with necessary details for operation.
 
-        :param team_name: The name of the team.
-        :param access_key: The access key for authentication.
-        :param project_id: The ID of the project to be set for the client.
+        Parameters:
+        - team_name (str): The name of the team.
+        - access_key (str): The access key for authentication.
+        - project_id (str, optional): The ID of the project to be set for the client. Defaults to an empty string.
+        - project_name (str, optional): The name of the project. Defaults to an empty string.
         """
-        self.team_name = (
-            team_name  # Assign the provided team name to an instance variable.
-        )
+        self.team_name = team_name
         self.client = spb_label.Client(
             team_name=team_name,
             access_key=access_key,
             project_id=project_id if project_id else None,
             project_name=project_name if project_name else None,
         )
 
     def download_export(
         self,
         input_path: str,
         export_id: str,
     ):
         """
-        Downloads an export from the server to a local path.
+        Download an export from the server to a local path.
 
-        :param input_path: The local file path where the export will be saved.
-        :param export_id: The ID of the export to download.
+        Parameters:
+        - input_path (str): The local file path where the export will be saved.
+        - export_id (str): The ID of the export to download.
         """
         print("[INFO] Checking for the export to be downloaded...")
-        download_url = self.client.get_export(
-            id=export_id
-        ).download_url  # Retrieve the download URL for the export.
-        r = requests.get(
-            download_url
-        )  # Make a GET request to the download URL.
-        if r.status_code == 200:  # Check if the request was successful.
+        download_url = self.client.get_export(id=export_id).download_url
+        r = requests.get(download_url)
+        if r.status_code == 200:
             print("Saving export to local path")
-            Path(input_path).parents[0].mkdir(
-                parents=True, exist_ok=True
-            )  # Ensure the directory exists.
-            with open(
-                input_path, "wb"
-            ) as f:  # Open the file in write-binary mode.
-                f.write(
-                    r.content
-                )  # Write the content of the response to the file.
+            Path(input_path).parents[0].mkdir(parents=True, exist_ok=True)
+            with open(input_path, "wb") as f:
+                f.write(r.content)
         else:
-            print(
-                f"Failed to download the file. Status code: {r.status_code}"
-            )  # Log failure.
+            print(f"Failed to download the file. Status code: {r.status_code}")
 
     def get_labels(
         self,
         data_key: str = "",
         tags: list = [],
         assignees: list = [],
         status: list = [],
         all: bool = False,
     ) -> Tuple[int, List]:
         """
-        Retrieves labels based on provided filters or all labels if specified.
+        Retrieve labels based on provided filters or all labels if specified.
+
+        Parameters:
+        - data_key (str, optional): Filter for a specific data key. Defaults to an empty string.
+        - tags (list, optional): Filter for specific tags. Defaults to an empty list.
+        - assignees (list, optional): Filter for specific assignees. Defaults to an empty list.
+        - status (list, optional): Filter for specific status. Defaults to an empty list.
+        - all (bool, optional): If True, ignores other filters and retrieves all labels. Defaults to False.
 
-        :param data_key: Filter for specific data key.
-        :param tags: Filter for specific tags.
-        :param assignees: Filter for specific assignees.
-        :param status: Filter for specific status.
-        :param all: If True, ignores other filters and retrieves all labels.
-        :return: A tuple containing the count of labels and a list of labels.
+        Returns:
+        Tuple[int, List]: A tuple containing the count of labels and a list of labels.
         """
-        if all:  # If retrieving all labels.
+        if all:
             next_cursor = None
             count, labels, next_cursor = self.client.get_labels(
                 cursor=next_cursor
-            )  # Retrieve all labels.
-        else:  # If using filters.
-            filter = SearchFilter(
-                project=self.client.project
-            )  # Create a search filter.
+            )
+        else:
+            filter = SearchFilter(project=self.client.project)
             if data_key:
-                filter.data_key_matches = data_key  # Set data key filter.
+                filter.data_key_matches = data_key
             if tags:
-                filter.tag_name_all = tags  # Set tags filter.
+                filter.tag_name_all = tags
             if assignees:
-                filter.assignee_is_any_one_of = (
-                    assignees  # Set assignees filter.
-                )
+                filter.assignee_is_any_one_of = assignees
             if status:
-                filter.status_is_any_one_of = status  # Set status filter.
+                filter.status_is_any_one_of = status
             next_cursor = None
             count, labels, next_cursor = self.client.get_labels(
                 filter=filter, cursor=next_cursor
-            )  # Retrieve filtered labels.
+            )
 
-        return count, labels  # Return the count and list of labels.
+        return count, labels
 
     def download_image(self, label: spb_label.DataHandle, path: str = None):
         """
-        Downloads an image associated with a label to a specified path.
+        Download an image associated with a label to a specified path.
 
-        :param label: The label data handle containing the image to download.
-        :param path: The local file path where the image will be saved. If None, defaults to the label's default path.
+        Parameters:
+        - label (spb_label.DataHandle): The label data handle containing the image to download.
+        - path (str, optional): The local file path where the image will be saved. If None, defaults to the label's default path.
         """
-        label.download_image(
-            download_to=path
-        )  # Download the image to the specified path.
+        label.download_image(download_to=path)
 
     def get_width_height(self, label: spb_label.DataHandle) -> Tuple[int, int]:
         """
-        Downloads an image associated with a label to a specified path, returns its width and height, and deletes the image.
+        Download an image associated with a label, return its width and height, and delete the image.
+
+        Parameters:
+        - label (spb_label.DataHandle): The label data handle containing the image to download.
 
-        :param label: The label data handle containing the image to download.
-        :return: A tuple containing the width and height of the downloaded image.
+        Returns:
+        Tuple[int, int]: A tuple containing the width and height of the downloaded image.
         """
         image_url = label.get_image_url()
         response = requests.get(image_url)
         img = Image.open(BytesIO(response.content))
         width, height = img.size
 
         return width, height
 
     def bbox_setting(self, class_name: str, annotation: list):
         """
-        Creates a bounding box setting for a given class name and annotation coordinates.
+        Create a bounding box setting for a given class name and annotation coordinates.
 
-        :param class_name: The class name associated with the bounding box.
-        :param annotation: A list containing the coordinates of the bounding box in the order [x, y, width, height].
-        :return: A tuple containing the class name and a dictionary with the bounding box coordinates.
+        Parameters:
+        - class_name (str): The class name associated with the bounding box.
+        - annotation (list): A list containing the coordinates of the bounding box in the order [x, y, width, height].
+
+        Returns:
+        A tuple containing the class name and a dictionary with the bounding box coordinates.
         """
         bbox = {
             "class_name": class_name,
             "annotation": {
                 "coord": {
                     "x": annotation[0],
                     "y": annotation[1],
@@ -159,66 +152,82 @@
                 }
             },
         }
 
         return bbox
 
     def upload_image(self, image_paths: list, dataset_name: str):
+        """
+        Upload images to a specified dataset.
+
+        Parameters:
+        - image_paths (list): A list of paths to the images to be uploaded.
+        - dataset_name (str): The name of the dataset to upload the images to.
+        """
         for path in image_paths:
             try:
                 self.client.upload_image(path, dataset_name)
             except ParameterException as e:
                 print(f"[ERROR]: Uploading went wrong: {e}")
 
-        return
-
     def upload_annotation(
         self, label: spb_label.DataHandle, annotations: list
     ):
+        """
+        Upload annotations for a given label.
+
+        Parameters:
+        - label (spb_label.DataHandle): The label to which the annotations will be added.
+        - annotations (list): A list of annotations to be added to the label.
+        """
         for anno in annotations:
             bbox = self.bbox_setting(anno[0], anno[1])
-            label.add_object_label(bbox)
+            label.add_object_label(
+                class_name=bbox["class_name"], annotation=bbox["annotation"]
+            )
         label.update_info()
 
-    def build_label_interface_from_yolo(
+    def build_label_interface(
         self,
-        dataset_file: str,
-        class_file_path: str,
+        class_list: list,
+        bbox: bool,
     ):
-        existing_label_interface = self.client.label_interface
+        """
+        Build and update the label interface for the project based on the provided class list and bounding box flag.
+
+        Parameters:
+        - class_list (list): A list of class names to be included in the label interface.
+        - bbox (bool): A flag indicating whether bounding boxes should be used.
+
+        Returns:
+        A tuple containing the updated label interface and a category map.
+        """
+        existing_label_interface = self.client.project.label_interface
         if existing_label_interface:
             label_interface = phy_credit.imageV2.LabelInterface.from_dict(
                 existing_label_interface
             )
             object_detection = phy_credit.imageV2.ObjectDetectionDef.from_dict(
                 existing_label_interface.get("object_detection")
             )
         else:
-            # get default label_interface and object_detection (json)
             label_interface = phy_credit.imageV2.LabelInterface.get_default()
             object_detection = (
                 phy_credit.imageV2.ObjectDetectionDef.get_default()
             )
 
-        # create class map from classes.txt and create label interface for project
         category_map = dict()
-        with open(
-            os.path.join(Path(dataset_file).parent, class_file_path), "r"
-        ) as f:
-            lines = f.readlines()
-
-        for i, line in enumerate(lines):
-            category_map[i] = line.rstrip("\n")
+        for class_name in class_list:
             bbox_suite_class_id = str(uuid4())
-            bbox_suite_class_name = category_map[i]
+            bbox_suite_class_name = class_name
 
             object_detection.add_box(
                 name=bbox_suite_class_name, id=bbox_suite_class_id
             )
 
         label_interface.set_object_detection(object_detection=object_detection)
-        print("[Classes]")
-        for value in category_map.values():
-            print(value, end=",")
-        print("")
-        print("")
+
+        self.client.update_project(
+            id=self.client.project.id,
+            label_interface=label_interface.to_dict(),
+        )
         return label_interface, category_map
```

### Comparing `superb-ai-apps-0.0.3/spb_apps/utils/converter.py` & `superb-ai-apps-0.0.4/spb_apps/utils/converter.py`

 * *Files identical despite different names*

### Comparing `superb-ai-apps-0.0.3/superb_ai_apps.egg-info/requires.txt` & `superb-ai-apps-0.0.4/superb_ai_apps.egg-info/requires.txt`

 * *Files identical despite different names*

