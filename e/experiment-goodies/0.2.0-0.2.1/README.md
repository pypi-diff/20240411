# Comparing `tmp/experiment_goodies-0.2.0.tar.gz` & `tmp/experiment_goodies-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_goodies-0.2.0.tar", max compression
+gzip compressed data, was "experiment_goodies-0.2.1.tar", max compression
```

## Comparing `experiment_goodies-0.2.0.tar` & `experiment_goodies-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1172 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-21 12:43:40.830253 experiment_goodies-0.2.0/experiment_goodies/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/experiment_goodies/geo/__init__.py
--rw-r--r--   0        0        0     7728 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/experiment_goodies/geo/raster.py
--rw-r--r--   0        0        0     5571 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/experiment_goodies/geo/vector.py
--rw-r--r--   0        0        0      268 2024-03-21 12:43:40.830253 experiment_goodies-0.2.0/experiment_goodies/logger/__init__.py
--rw-r--r--   0        0        0     4189 2024-04-10 14:47:21.255719 experiment_goodies-0.2.0/experiment_goodies/logger/experiment_logger.py
--rw-r--r--   0        0        0     5850 2024-03-21 12:43:40.830253 experiment_goodies-0.2.0/experiment_goodies/logger/rainbow_logger.py
--rw-r--r--   0        0        0     1101 2024-04-10 14:47:21.255719 experiment_goodies-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 experiment_goodies-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1172 2024-03-21 18:20:53.347022 experiment_goodies-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-21 12:43:40.830253 experiment_goodies-0.2.1/experiment_goodies/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:20:53.347022 experiment_goodies-0.2.1/experiment_goodies/geo/__init__.py
+-rw-r--r--   0        0        0     7896 2024-04-11 03:58:45.858601 experiment_goodies-0.2.1/experiment_goodies/geo/raster.py
+-rw-r--r--   0        0        0     5571 2024-03-21 18:20:53.347022 experiment_goodies-0.2.1/experiment_goodies/geo/vector.py
+-rw-r--r--   0        0        0      268 2024-03-21 12:43:40.830253 experiment_goodies-0.2.1/experiment_goodies/logger/__init__.py
+-rw-r--r--   0        0        0     4189 2024-04-10 14:47:21.255719 experiment_goodies-0.2.1/experiment_goodies/logger/experiment_logger.py
+-rw-r--r--   0        0        0     5850 2024-03-21 12:43:40.830253 experiment_goodies-0.2.1/experiment_goodies/logger/rainbow_logger.py
+-rw-r--r--   0        0        0     1101 2024-04-11 21:29:03.311823 experiment_goodies-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 experiment_goodies-0.2.1/PKG-INFO
```

### Comparing `experiment_goodies-0.2.0/README.md` & `experiment_goodies-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.0/experiment_goodies/geo/raster.py` & `experiment_goodies-0.2.1/experiment_goodies/geo/raster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Literal
 
 import affine
 import numpy as np
 import rasterio
 from geopandas import GeoSeries
 from rasterio.mask import mask
 from rasterio.merge import merge
@@ -99,24 +99,29 @@
                 "transform": out_transform,
             }
         )
     with rasterio.open(output_path, "w", **profile) as dst:
         dst.write(masked_array)
 
 
-def merge_rasters_into_mosaic(raster_paths: list[str], mosaic_path: str):
+def merge_rasters_into_mosaic(
+    raster_paths: list[str],
+    mosaic_path: str,
+    method: Literal["first", "last", "min", "max"] = "max",
+):
     """Merges a list of rasters into a single mosaic. Assumes all input rasters are in the same CRS
     This function is a simple wrapper around rasterio.merge.merge, see https://rasterio.readthedocs.io/en/stable/api/rasterio.merge.html
     for more complex functionalities.
 
     Args:
         paths (list[str]): list of rasters to merge
         mosaic_path (str): output mosaic path
+        method (str): which method to use for merging. Defaults to "max"
     """
-    mosaic, output_trf = merge(raster_paths)
+    mosaic, output_trf = merge(raster_paths, method=method)
     with rasterio.open(raster_paths[0]) as ref_src:
         ref_meta = ref_src.meta
     output_meta = ref_meta.copy()
     output_meta.update(
         {
             "driver": "GTiff",
             "height": mosaic.shape[1],
```

### Comparing `experiment_goodies-0.2.0/experiment_goodies/geo/vector.py` & `experiment_goodies-0.2.1/experiment_goodies/geo/vector.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.0/experiment_goodies/logger/experiment_logger.py` & `experiment_goodies-0.2.1/experiment_goodies/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.0/experiment_goodies/logger/rainbow_logger.py` & `experiment_goodies-0.2.1/experiment_goodies/logger/rainbow_logger.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.2.0/pyproject.toml` & `experiment_goodies-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "experiment-goodies"
-version = "0.2.0"
+version = "0.2.1"
 description = "Useful helpers, callbacks and more for experimenting with ml models"
 authors = ["Javier Smith <javier.smith.dlc@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 logutils = "^0.3.5"
```

### Comparing `experiment_goodies-0.2.0/PKG-INFO` & `experiment_goodies-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-goodies
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful helpers, callbacks and more for experimenting with ml models
 Author: Javier Smith
 Author-email: javier.smith.dlc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

