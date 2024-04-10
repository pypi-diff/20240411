# Comparing `tmp/MedicalImageConverter-1.3.tar.gz` & `tmp/MedicalImageConverter-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedicalImageConverter-1.3.tar", last modified: Thu Mar 28 19:46:40 2024, max compression
+gzip compressed data, was "MedicalImageConverter-1.4.tar", last modified: Wed Apr 10 23:46:05 2024, max compression
```

## Comparing `MedicalImageConverter-1.3.tar` & `MedicalImageConverter-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 19:46:40.641044 MedicalImageConverter-1.3/
--rw-rw-rw-   0        0        0    35821 2023-07-22 22:51:40.000000 MedicalImageConverter-1.3/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 19:46:40.562954 MedicalImageConverter-1.3/MedicalImageConverter/
--rw-rw-rw-   0        0        0      102 2023-07-23 20:35:17.000000 MedicalImageConverter-1.3/MedicalImageConverter/__init__.py
--rw-rw-rw-   0        0        0      690 2023-07-26 23:11:11.000000 MedicalImageConverter-1.3/MedicalImageConverter/memory.py
--rw-rw-rw-   0        0        0     1343 2024-02-23 14:56:25.000000 MedicalImageConverter-1.3/MedicalImageConverter/parsar.py
--rw-rw-rw-   0        0        0    24095 2024-03-28 19:41:53.000000 MedicalImageConverter-1.3/MedicalImageConverter/reader.py
-drwxrwxrwx   0        0        0        0 2024-03-28 19:46:40.625380 MedicalImageConverter-1.3/MedicalImageConverter.egg-info/
--rw-rw-rw-   0        0        0     4327 2024-03-28 19:46:40.000000 MedicalImageConverter-1.3/MedicalImageConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2024-03-28 19:46:40.000000 MedicalImageConverter-1.3/MedicalImageConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 19:46:40.000000 MedicalImageConverter-1.3/MedicalImageConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-03-28 19:46:40.000000 MedicalImageConverter-1.3/MedicalImageConverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4327 2024-03-28 19:46:40.625380 MedicalImageConverter-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3840 2023-09-03 04:16:10.000000 MedicalImageConverter-1.3/README.md
--rw-rw-rw-   0        0        0       97 2023-07-23 20:12:24.000000 MedicalImageConverter-1.3/pyproject.toml
--rw-rw-rw-   0        0        0      592 2024-03-28 19:46:40.641044 MedicalImageConverter-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 23:46:05.415540 MedicalImageConverter-1.4/
+-rw-rw-rw-   0        0        0    35821 2023-07-22 22:51:40.000000 MedicalImageConverter-1.4/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 23:46:05.332920 MedicalImageConverter-1.4/MedicalImageConverter/
+-rw-rw-rw-   0        0        0      102 2023-07-23 20:35:17.000000 MedicalImageConverter-1.4/MedicalImageConverter/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-07-26 23:11:11.000000 MedicalImageConverter-1.4/MedicalImageConverter/memory.py
+-rw-rw-rw-   0        0        0     1343 2024-02-23 14:56:25.000000 MedicalImageConverter-1.4/MedicalImageConverter/parsar.py
+-rw-rw-rw-   0        0        0    24481 2024-04-10 23:39:01.000000 MedicalImageConverter-1.4/MedicalImageConverter/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-10 23:46:05.392641 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/
+-rw-rw-rw-   0        0        0     4327 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-10 23:46:05.000000 MedicalImageConverter-1.4/MedicalImageConverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4327 2024-04-10 23:46:05.403593 MedicalImageConverter-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3840 2023-09-03 04:16:10.000000 MedicalImageConverter-1.4/README.md
+-rw-rw-rw-   0        0        0       97 2023-07-23 20:12:24.000000 MedicalImageConverter-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      592 2024-04-10 23:46:05.419522 MedicalImageConverter-1.4/setup.cfg
```

### Comparing `MedicalImageConverter-1.3/LICENSE.txt` & `MedicalImageConverter-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.3/MedicalImageConverter/memory.py` & `MedicalImageConverter-1.4/MedicalImageConverter/memory.py`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.3/MedicalImageConverter/parsar.py` & `MedicalImageConverter-1.4/MedicalImageConverter/parsar.py`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.3/MedicalImageConverter/reader.py` & `MedicalImageConverter-1.4/MedicalImageConverter/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,23 @@
 
                 elif t == 'ImagePositionPatient':
                     if image[0].Modality in ['US', 'CR', 'DX', 'MG', 'NM', 'XA']:
                         self.image_info.at[ii, t] = [0, 0, 0]
                     else:
                         self.image_info.at[ii, t] = image[-1].ImagePositionPatient
 
+                elif t == 'SliceThickness':
+                    if len(image) > 1:
+                        thickness = (np.asarray(image[0]['ImagePositionPatient'].value[2]).astype(float) -
+                                     np.asarray(image[1]['ImagePositionPatient'].value[2]).astype(float))
+                    else:
+                        thickness = np.asarray(image[0]['SliceThickness']).astype(float)
+
+                    self.image_info.at[ii, t] = thickness
+
                 elif t == 'Slices':
                     self.image_info.at[ii, t] = len(image)
 
                 elif t == 'DefaultWindow':
                     if (0x0028, 0x1050) in image[0] and (0x0028, 0x1051) in image[0]:
                         if image[0].Modality == 'DX':
                             self.image_info.at[ii, t] = [int(image[0].WindowCenter[0]),
@@ -418,37 +427,37 @@
             image_max = np.max(self.image_data[-1])
             self.image_info.at[ii, 'FullWindow'] = [image_min, image_max]
 
     def fix_orientation(self):
         for ii, image in enumerate(self.image_data):
             if self.image_info.at[ii, 'PatientPosition']:
                 position = self.image_info.at[ii, 'PatientPosition']
-                if position not in ['HFS', 'FFS']:
-                    rows = self.image_info.at[ii, 'Rows']
-                    columns = self.image_info.at[ii, 'Columns']
-                    spacing = self.image_info.at[ii, 'PixelSpacing']
-                    coordinates = self.image_info.at[ii, 'ImagePositionPatient']
-                    if position in ['HFDR', 'FFDR']:
-                        self.image_data[ii] = np.rot90(image, 3, (1, 2))
-
-                        new_coordinates = np.double(coordinates[0]) - spacing[0]*columns
-                        self.image_info.at[ii, 'ImagePositionPatient'][0] = new_coordinates
-                    elif position in ['HFP', 'FFP']:
-                        self.image_data[ii] = np.rot90(image, 2, (1, 2))
-
-                        new_coordinates = np.double(coordinates[0]) - spacing[0] * columns
-                        self.image_info.at[ii, 'ImagePositionPatient'][0] = new_coordinates
-
-                        new_coordinates = np.double(coordinates[1]) - spacing[1] * rows
-                        self.image_info.at[ii, 'ImagePositionPatient'][1] = new_coordinates
-                    elif position in ['HFDL', 'FFDL']:
-                        self.image_data[ii] = np.rot90(image, 1, (1, 2))
+                rows = self.image_info.at[ii, 'Rows']
+                columns = self.image_info.at[ii, 'Columns']
+                spacing = self.image_info.at[ii, 'PixelSpacing']
+                coordinates = self.image_info.at[ii, 'ImagePositionPatient']
+
+                if position in ['HFDR', 'FFDR']:
+                    self.image_data[ii] = np.rot90(image, 3, (1, 2))
+
+                    new_coordinates = np.double(coordinates[0]) - spacing[0] * (columns - 1)
+                    self.image_info.at[ii, 'ImagePositionPatient'][0] = new_coordinates
+                elif position in ['HFP', 'FFP']:
+                    self.image_data[ii] = np.rot90(image, 2, (1, 2))
+
+                    new_coordinates = np.double(coordinates[0]) - spacing[0] * (columns - 1)
+                    self.image_info.at[ii, 'ImagePositionPatient'][0] = new_coordinates
+
+                    new_coordinates = np.double(coordinates[1]) - spacing[1] * (rows - 1)
+                    self.image_info.at[ii, 'ImagePositionPatient'][1] = new_coordinates
+                elif position in ['HFDL', 'FFDL']:
+                    self.image_data[ii] = np.rot90(image, 1, (1, 2))
 
-                        new_coordinates = np.double(coordinates[1]) - spacing[1]*rows
-                        self.image_info.at[ii, 'ImagePositionPatient'][1] = new_coordinates
+                    new_coordinates = np.double(coordinates[1]) - spacing[1] * (rows - 1)
+                    self.image_info.at[ii, 'ImagePositionPatient'][1] = new_coordinates
 
     def separate_contours(self):
         """
         existing_image_info is required if the users only loads a RTSTRUCT file, this is needed to match contours with
         the image they correspond to.
 
         It is pretty gross after that. For a given ROI each contour is read-in, matched with their image, then combined
```

### Comparing `MedicalImageConverter-1.3/MedicalImageConverter.egg-info/PKG-INFO` & `MedicalImageConverter-1.4/MedicalImageConverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedicalImageConverter
-Version: 1.3
+Version: 1.4
 Summary: Reads in medical images and converts them into numpy arrays.
 Home-page: https://github.com/caleb-oconnor/MedicalImageConverter
 Author: Caleb OConnor
 Author-email: csoconnor@mdanderson.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `MedicalImageConverter-1.3/PKG-INFO` & `MedicalImageConverter-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedicalImageConverter
-Version: 1.3
+Version: 1.4
 Summary: Reads in medical images and converts them into numpy arrays.
 Home-page: https://github.com/caleb-oconnor/MedicalImageConverter
 Author: Caleb OConnor
 Author-email: csoconnor@mdanderson.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `MedicalImageConverter-1.3/README.md` & `MedicalImageConverter-1.4/README.md`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.3/setup.cfg` & `MedicalImageConverter-1.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6564 6963 616c 496d 6167 6543   = MedicalImageC
 00000020: 6f6e 7665 7274 6572 0d0a 7665 7273 696f  onverter..versio
-00000030: 6e20 3d20 312e 330d 0a61 7574 686f 7220  n = 1.3..author 
+00000030: 6e20 3d20 312e 340d 0a61 7574 686f 7220  n = 1.4..author 
 00000040: 3d20 4361 6c65 6220 4f43 6f6e 6e6f 720d  = Caleb OConnor.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6373 6f63 6f6e 6e6f 7240 6d64 616e 6465  csoconnor@mdande
 00000070: 7273 6f6e 2e6f 7267 0d0a 6465 7363 7269  rson.org..descri
 00000080: 7074 696f 6e20 3d20 5265 6164 7320 696e  ption = Reads in
 00000090: 206d 6564 6963 616c 2069 6d61 6765 7320   medical images 
 000000a0: 616e 6420 636f 6e76 6572 7473 2074 6865  and converts the
```

