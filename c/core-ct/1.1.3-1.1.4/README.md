# Comparing `tmp/core_ct-1.1.3.tar.gz` & `tmp/core_ct-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_ct-1.1.3.tar", max compression
+gzip compressed data, was "core_ct-1.1.4.tar", max compression
```

## Comparing `core_ct-1.1.3.tar` & `core_ct-1.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2024-04-11 01:05:32.636641 core_ct-1.1.3/LICENSE
--rw-r--r--   0        0        0     2593 2024-04-11 01:05:32.636641 core_ct-1.1.3/README.md
--rw-r--r--   0        0        0      981 2024-04-11 01:05:32.640641 core_ct-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/analysis.py
--rw-r--r--   0        0        0    21970 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/core.py
--rw-r--r--   0        0        0     4313 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/importers.py
--rw-r--r--   0        0        0     4454 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/slice.py
--rw-r--r--   0        0        0     7286 2024-04-11 01:05:32.640641 core_ct-1.1.3/src/core_ct/visualize.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-11 01:09:26.145899 core_ct-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2593 2024-04-11 01:09:26.145899 core_ct-1.1.4/README.md
+-rw-r--r--   0        0        0      981 2024-04-11 01:09:26.149899 core_ct-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-04-11 01:09:26.149899 core_ct-1.1.4/src/core_ct/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 01:09:26.149899 core_ct-1.1.4/src/core_ct/analysis.py
+-rw-r--r--   0        0        0    22669 2024-04-11 01:09:26.149899 core_ct-1.1.4/src/core_ct/core.py
+-rw-r--r--   0        0        0     4313 2024-04-11 01:09:26.149899 core_ct-1.1.4/src/core_ct/importers.py
+-rw-r--r--   0        0        0     4454 2024-04-11 01:09:26.149899 core_ct-1.1.4/src/core_ct/slice.py
+-rw-r--r--   0        0        0     7286 2024-04-11 01:09:26.149899 core_ct-1.1.4/src/core_ct/visualize.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.1.4/PKG-INFO
```

### Comparing `core_ct-1.1.3/LICENSE` & `core_ct-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.3/README.md` & `core_ct-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.3/pyproject.toml` & `core_ct-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-ct"
-version = "1.1.3"
+version = "1.1.4"
 description = "A Python library to assist geologists with the analysis of rock core CT scans"
 authors = [
     "Kira Hanson <khanson@mines.edu>",
     "Carla Ellefsen <cellefsen@mines.edu>",
     "Connor Sparks <csparks@mines.edu>",
     "Asa Sprow <arsprow@mines.edu>",
 ]
```

### Comparing `core_ct-1.1.3/src/core_ct/analysis.py` & `core_ct-1.1.4/src/core_ct/analysis.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.3/src/core_ct/core.py` & `core_ct-1.1.4/src/core_ct/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A class that abstracts the CT scan of a rock core."""
 
 from __future__ import annotations
 import numpy as np
+import warnings
 from typing import Callable
 from core_ct.slice import Slice
 from math import pow, sqrt
 
 # Methods
 # -------
 #     slice(self, axis, loc) -- get a 2D slice of the core
@@ -72,41 +73,49 @@
             `Slice` object containing pixel data and dimensions
 
         Raises
         ------
         ValueError
             If axis is a value other than 0, 1, or 2
         """
-        match axis:
-            case 0:
-                return Slice(
-                    data=self.data[loc],
-                    pixel_dimensions=(
-                        self.pixel_dimensions[1],
-                        self.pixel_dimensions[2],
-                    ),
-                )  # 0th and 1st
-            case 1:
-                return Slice(
-                    data=self.data[:, loc],
-                    pixel_dimensions=(
-                        self.pixel_dimensions[0],
-                        self.pixel_dimensions[2],
-                    ),
-                )
-            case 2:
-                return Slice(
-                    data=self.data[:, :, loc],
-                    pixel_dimensions=(
-                        self.pixel_dimensions[0],
-                        self.pixel_dimensions[1],
-                    ),
-                )
-            case _:
-                raise ValueError("axis must be a value between 0 and 2 (inclusive)")
+        try:
+            match axis:
+                case 0:
+                    return Slice(
+                        data=self.data[loc],
+                        pixel_dimensions=(
+                            self.pixel_dimensions[1],
+                            self.pixel_dimensions[2],
+                        ),
+                    )  # 0th and 1st
+                case 1:
+                    return Slice(
+                        data=self.data[:, loc],
+                        pixel_dimensions=(
+                            self.pixel_dimensions[0],
+                            self.pixel_dimensions[2],
+                        ),
+                    )
+                case 2:
+                    return Slice(
+                        data=self.data[:, :, loc],
+                        pixel_dimensions=(
+                            self.pixel_dimensions[0],
+                            self.pixel_dimensions[1],
+                        ),
+                    )
+                case _:
+                    raise ValueError("axis must be a value between 0 and 2 (inclusive)")
+        except IndexError as e:
+            raise IndexError(
+                f"`loc` index is out of bounds on axis {axis}, value is {loc} but "
+                f"axis size is {self.shape()[axis]}"
+                ) from e
+
+
 
     def trim(self, axis: int, loc_start: int, loc_end: int | None = None) -> Core:
         """
         Reduces the dimensions of the core along a specified axis.
 
         Get a three-dimensional slice of the core scan by trimming off a specified
         amount on the requested axis. This function is symmetrical by default.
@@ -285,14 +294,22 @@
         if y_center is None:
             y_center = int(self.data.shape[1] / 2)
         if z_center is None:
             z_center = int(self.data.shape[2] / 2)
 
         center: tuple[int, int, int] = (x_center, y_center, z_center)
 
+        # make sure all indexes are within bounds
+        for axis, idx in enumerate(center):
+            if idx >= self.shape()[axis]:
+                warnings.warn(
+                    f"Center index is out of bounds on axis {axis}, value is {idx} but "
+                    f"axis size is {self.shape()[axis]}"
+                    )
+
         starts: list[int] = [0] * 3
         ends: list[int] = [0] * 3
         for ax in range(0, 3):
             if ax == axis:
                 starts[ax] = 0
                 ends[ax] = self.data.shape[ax]
                 continue
```

### Comparing `core_ct-1.1.3/src/core_ct/importers.py` & `core_ct-1.1.4/src/core_ct/importers.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.3/src/core_ct/slice.py` & `core_ct-1.1.4/src/core_ct/slice.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.3/src/core_ct/visualize.py` & `core_ct-1.1.4/src/core_ct/visualize.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.1.3/PKG-INFO` & `core_ct-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-ct
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python library to assist geologists with the analysis of rock core CT scans
 License: MIT
 Author: Kira Hanson
 Author-email: khanson@mines.edu
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

