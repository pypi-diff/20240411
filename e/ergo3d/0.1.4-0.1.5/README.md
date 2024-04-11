# Comparing `tmp/ergo3d-0.1.4.tar.gz` & `tmp/ergo3d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ergo3d-0.1.4.tar", last modified: Wed Apr 10 03:23:08 2024, max compression
+gzip compressed data, was "ergo3d-0.1.5.tar", last modified: Thu Apr 11 20:32:16 2024, max compression
```

## Comparing `ergo3d-0.1.4.tar` & `ergo3d-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.433895 ergo3d-0.1.4/
--rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      467 2024-04-10 03:23:08.433895 ergo3d-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2024-04-10 03:22:46.000000 ergo3d-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.417779 ergo3d-0.1.4/ergo3d/
--rw-rw-rw-   0        0        0       46 2024-04-04 19:41:29.000000 ergo3d-0.1.4/ergo3d/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.425874 ergo3d-0.1.4/ergo3d/camera/
--rw-rw-rw-   0        0        0     6865 2024-04-09 23:07:34.000000 ergo3d-0.1.4/ergo3d/camera/Camera.py
--rw-rw-rw-   0        0        0    13438 2024-04-02 22:55:21.000000 ergo3d-0.1.4/ergo3d/camera/FLIR_camera.py
--rw-rw-rw-   0        0        0       51 2024-04-04 19:41:29.000000 ergo3d-0.1.4/ergo3d/camera/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.433895 ergo3d-0.1.4/ergo3d/geometry/
--rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/CoordinateSystem3D.py
--rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/JointAngles.py
--rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/Plane.py
--rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.4/ergo3d/geometry/Point.py
--rw-rw-rw-   0        0        0      105 2024-04-04 19:41:29.000000 ergo3d-0.1.4/ergo3d/geometry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:23:08.417779 ergo3d-0.1.4/ergo3d.egg-info/
--rw-rw-rw-   0        0        0      467 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 03:23:08.000000 ergo3d-0.1.4/ergo3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 03:23:08.433895 ergo3d-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-10 03:22:46.000000 ergo3d-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:32:16.196585 ergo3d-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-04-11 20:32:16.195586 ergo3d-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2024-04-10 03:22:46.000000 ergo3d-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 20:32:16.174377 ergo3d-0.1.5/ergo3d/
+-rw-rw-rw-   0        0        0       46 2024-04-04 19:41:29.000000 ergo3d-0.1.5/ergo3d/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:32:16.185512 ergo3d-0.1.5/ergo3d/camera/
+-rw-rw-rw-   0        0        0     6963 2024-04-10 04:40:29.000000 ergo3d-0.1.5/ergo3d/camera/Camera.py
+-rw-rw-rw-   0        0        0    14554 2024-04-10 04:57:06.000000 ergo3d-0.1.5/ergo3d/camera/FLIR_camera.py
+-rw-rw-rw-   0        0        0       51 2024-04-04 19:41:29.000000 ergo3d-0.1.5/ergo3d/camera/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:32:16.194580 ergo3d-0.1.5/ergo3d/geometry/
+-rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.5/ergo3d/geometry/CoordinateSystem3D.py
+-rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.5/ergo3d/geometry/JointAngles.py
+-rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.5/ergo3d/geometry/Plane.py
+-rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.5/ergo3d/geometry/Point.py
+-rw-rw-rw-   0        0        0      105 2024-04-04 19:41:29.000000 ergo3d-0.1.5/ergo3d/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:32:16.180456 ergo3d-0.1.5/ergo3d.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-04-11 20:32:16.000000 ergo3d-0.1.5/ergo3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-04-11 20:32:16.000000 ergo3d-0.1.5/ergo3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:32:16.000000 ergo3d-0.1.5/ergo3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-11 20:32:16.000000 ergo3d-0.1.5/ergo3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 20:32:16.000000 ergo3d-0.1.5/ergo3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:32:16.196585 ergo3d-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-11 20:32:14.000000 ergo3d-0.1.5/setup.py
```

### Comparing `ergo3d-0.1.4/LICENSE` & `ergo3d-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.4/README.md` & `ergo3d-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.4/ergo3d/camera/Camera.py` & `ergo3d-0.1.5/ergo3d/camera/Camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Axis angle to quaternion, for SMPL mostly
         :param axis: (3,)
         :param angle: None or float
         :return:
         """
         axis_norm = np.linalg.norm(axis)
         angle = axis_norm if angle is None else angle
-        axis = axis / axis_norm if axis_norm > 1e-8 else np.array([0, 0, 0])
+        axis = axis / axis_norm if axis_norm > 1e-8 else np.array([0, 0, 0])  # todo: sin(x/2)/x ~= 1/2 - (x**2)/48 for small angle x < 1e6
         w = np.cos(angle / 2.0)
         xyz = axis * np.sin(angle / 2.0)
         return np.array([w, xyz[0], xyz[1], xyz[2]])
 
     @staticmethod
     def axis_angle_from_quaternion(quaternion, one_output=True):
         """
@@ -62,15 +62,15 @@
         :param one_output: True: put angle as the norm of the axis vector
         :return:
         """
         w, x, y, z = quaternion
         angle = 2 * np.arccos(w)
         sin_theta_over_two = np.sqrt(1 - w * w)
         # To avoid division by zero, check if sin(theta/2) is close to zero
-        axis = np.array([x, y, z]) / sin_theta_over_two if sin_theta_over_two > 1e-8 else np.array([1, 0, 0]) # If the angle is close to 0, direction does not matter
+        axis = np.array([x, y, z]) / sin_theta_over_two if sin_theta_over_two > 1e-8 else np.array([1, 0, 0]) # If the angle is close to 0, direction does not matter  # todo: small angle approximation
         return axis * angle if one_output else [axis, angle]
 
     @staticmethod
     def quaternion_multiply(q1, q2):
         """
         Multiply two quaternions.
```

### Comparing `ergo3d-0.1.4/ergo3d/camera/FLIR_camera.py` & `ergo3d-0.1.5/ergo3d/camera/FLIR_camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,44 @@
 from .Camera import *
 
+
+def batch_load_from_xcp(xcp_filename):
+    # Read the xcp file as xml
+    with open(xcp_filename, 'r') as f:
+        xml_string = f.read()
+    root = ET.fromstring(xml_string)
+    cameras = []
+    for child in root:
+        if child.attrib['DISPLAY_TYPE'] == 'VideoInputDevice:Blackfly S BFS-U3-23S3C':
+            camera = FLIR_Camera()
+            camera.load_vicon_xcp(child)
+            cameras.append(camera)
+    return cameras
+
+
+def load_csv(csv_filename):
+    df = pd.read_csv(csv_filename, skiprows=[0, 1, 2,3, 4], header=None)
+    header_df = pd.read_csv(csv_filename, skiprows=[0, 1], nrows=1, header=None)
+    # remove nan in the header
+    # iterate over header_df
+    header = ['Frame', 'Sub Frame']
+    axis = ['X', 'Y', 'Z']
+    joint_names = []
+    for x in header_df.iloc[0]:
+        # print(x)
+        if type(x) == str:
+            joint_name = x.split(':')[-1]
+            joint_names.append(joint_name)
+            for ax in axis:
+                header.append(f'{joint_name}-{ax}')
+    # add header to df
+    df.columns = header
+    return df, joint_names
+
+
 class FLIR_Camera(Camera):
     def __init__(self):
         super().__init__()
 
     def load_vicon_xcp(self, xcp_element):
         # Read the xcp file as xml
         self.DEVICEID = xcp_element.attrib['DEVICEID']
```

### Comparing `ergo3d-0.1.4/ergo3d/geometry/CoordinateSystem3D.py` & `ergo3d-0.1.5/ergo3d/geometry/CoordinateSystem3D.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.4/ergo3d/geometry/JointAngles.py` & `ergo3d-0.1.5/ergo3d/geometry/JointAngles.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.4/ergo3d/geometry/Plane.py` & `ergo3d-0.1.5/ergo3d/geometry/Plane.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.4/ergo3d/geometry/Point.py` & `ergo3d-0.1.5/ergo3d/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.4/setup.py` & `ergo3d-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ergo3d',  # Name of your package
-    version='0.1.4',  # Version number
+    version='0.1.5',  # Version number
     description='A Python package for 3D ergonomic calculations.',  # Short description of your package
     url='https://github.com/LeyangWen/ergo3d',  # URL for your package's homepage
     author='Leyang Wen',  # Your name
     author_email='wenleyan@umich.edu',  # Your email
     license='MIT',  # License type for your package
     packages=find_packages(),  # Automatically find all packages and subpackages
     install_requires=[  # List of dependencies
```

