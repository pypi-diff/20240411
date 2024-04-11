# Comparing `tmp/valor-client-0.20.1.tar.gz` & `tmp/valor-client-0.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor-client-0.20.1.tar", last modified: Fri Apr  5 21:44:28 2024, max compression
+gzip compressed data, was "valor-client-0.20.2.tar", last modified: Thu Apr 11 03:42:48 2024, max compression
```

## Comparing `valor-client-0.20.1.tar` & `valor-client-0.20.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.513570 valor-client-0.20.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 21:44:23.000000 valor-client-0.20.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 21:44:28.513570 valor-client-0.20.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 21:44:23.000000 valor-client-0.20.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:44:28.513570 valor-client-0.20.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 21:44:23.000000 valor-client-0.20.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.505570 valor-client-0.20.1/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-05 21:44:23.000000 valor-client-0.20.1/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    53715 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.509570 valor-client-0.20.1/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    46702 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-05 21:44:23.000000 valor-client-0.20.1/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:44:28.513570 valor-client-0.20.1/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 21:44:28.000000 valor-client-0.20.1/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.704584 valor-client-0.20.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 03:42:41.000000 valor-client-0.20.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-11 03:42:48.704584 valor-client-0.20.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-11 03:42:41.000000 valor-client-0.20.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:42:48.704584 valor-client-0.20.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 03:42:41.000000 valor-client-0.20.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.696584 valor-client-0.20.2/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12523 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-11 03:42:41.000000 valor-client-0.20.2/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53932 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.700584 valor-client-0.20.2/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.704584 valor-client-0.20.2/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58814 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-11 03:42:41.000000 valor-client-0.20.2/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:42:48.704584 valor-client-0.20.2/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-11 03:42:48.000000 valor-client-0.20.2/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-11 03:42:48.000000 valor-client-0.20.2/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:42:48.000000 valor-client-0.20.2/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 03:42:48.000000 valor-client-0.20.2/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 03:42:48.000000 valor-client-0.20.2/valor_client.egg-info/top_level.txt
```

### Comparing `valor-client-0.20.1/LICENSE` & `valor-client-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/PKG-INFO` & `valor-client-0.20.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.20.1
+Version: 0.20.2
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor-client-0.20.1/pyproject.toml` & `valor-client-0.20.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/conftest.py` & `valor-client-0.20.2/unit-tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Tuple
 
 import numpy as np
 import pytest
 
 from valor import Label
-from valor.schemas import BoundingBox, BoundingPolygon, Raster
+from valor.schemas import Box, Polygon, Raster
 
 
 @pytest.fixture
 def labels() -> List[Label]:
     return [
         Label(key="k1", value="v1"),
         Label(key="k2", value="v2"),
@@ -23,21 +23,21 @@
         (10, 10),
         (0, 10),
         (0, 0),
     ]
 
 
 @pytest.fixture
-def bbox() -> BoundingBox:
-    return BoundingBox.from_extrema(xmin=0, xmax=10, ymin=0, ymax=10)
+def bbox() -> Box:
+    return Box.from_extrema(xmin=0, xmax=10, ymin=0, ymax=10)
 
 
 @pytest.fixture
-def polygon(box_points) -> BoundingPolygon:
-    return BoundingPolygon([box_points])
+def polygon(box_points) -> Polygon:
+    return Polygon([box_points])
 
 
 @pytest.fixture
 def raster_raw_mask() -> np.ndarray:
     """
     Creates a 2d numpy of bools of shape:
     | T  F |
```

### Comparing `valor-client-0.20.1/unit-tests/coretypes/test_core.py` & `valor-client-0.20.2/unit-tests/coretypes/test_core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 
 import pytest
 
 from valor import Annotation, Datum, GroundTruth, Label, Prediction, enums
-from valor.schemas import Score
+from valor.schemas import Float, Polygon
 
 
 def test_datum():
     Datum(uid="123")
     Datum(uid="123", metadata={})
     Datum(uid="123", metadata={"name": 1})
 
@@ -52,50 +52,49 @@
         task_type=enums.TaskType.CLASSIFICATION, labels=labels, metadata={}
     )
     Annotation(
         task_type=enums.TaskType.CLASSIFICATION,
         labels=labels,
         metadata=metadata,
     )
+    Annotation(
+        task_type=enums.TaskType.OBJECT_DETECTION,
+        labels=labels,
+        polygon=bbox,  # bbox is a constrained polygon so this is valid usage
+    )
 
     # test `__post_init__`
     with pytest.raises(ValueError) as e:
         Annotation(task_type="something", labels=labels)  # type: ignore
     assert "TaskType" in str(e)
-    with pytest.raises(TypeError) as e:
-        Annotation(
-            task_type=enums.TaskType.OBJECT_DETECTION,
-            labels=labels,
-            bounding_box=polygon,
-        )
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         Annotation(
             task_type=enums.TaskType.OBJECT_DETECTION,
             labels=labels,
-            polygon=bbox,
+            bounding_box=Polygon([[(0, 0), (1, 0), (1, 1), (0, 0)]]),  # type: ignore
         )
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         Annotation(
             task_type=enums.TaskType.OBJECT_DETECTION,
             labels=labels,
             raster=bbox,
         )
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION,
             labels=labels,
             metadata=[1234],  # type: ignore
         )
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION,
             labels=labels,
             metadata={1: 1},  # type: ignore
         )
-    with pytest.raises(ValueError) as e:
+    with pytest.raises(ValueError):
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION,
             labels=labels,
             metadata={"test": None},  # type: ignore
         )
 
 
@@ -113,48 +112,46 @@
     # test `__post_init__`
     with pytest.raises(ValueError) as e:
         Annotation(task_type="soemthing", labels=[l1])  # type: ignore
     assert "TaskType" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=l1)  # type: ignore
     assert "List[Label]" in str(e)
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION, labels=[l1, l2, "label"]  # type: ignore
         )
-    assert "Label" in str(e)
 
 
 def test_prediction_annotation():
     l1 = Label(key="test", value="value")
     l2 = Label(key="test", value="other")
     l3 = Label(key="other", value="value")
 
     s1 = copy.deepcopy(l1)
-    s1.score = Score(0.5)
+    s1.score = Float.nullable(0.5)
     s2 = copy.deepcopy(l2)
-    s2.score = Score(0.5)
+    s2.score = Float.nullable(0.5)
     s3 = copy.deepcopy(l3)
-    s3.score = Score(1.0)
+    s3.score = Float.nullable(1.0)
 
     # valid
     Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=[s1, s2, s3])
 
     # test `__post_init__`
     with pytest.raises(ValueError) as e:
         Annotation(task_type="something", labels=[s1, s2, s3])  # type: ignore
     assert "TaskType" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=s1)  # type: ignore
     assert "List[Label]" in str(e)
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION, labels=[s1, s2, "label"]  # type: ignore
         )
-    assert "Label" in str(e)
 
 
 def test_groundtruth():
     label = Label(key="test", value="value")
     datum = Datum(uid="somefile")
     gts = [
         Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=[label]),
@@ -164,32 +161,30 @@
     # valid
     GroundTruth(
         datum=datum,
         annotations=gts,
     )
 
     # test `__post_init__`
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         GroundTruth(
             datum="datum",  # type: ignore
             annotations=gts,
         )
-    assert "Datum" in str(e)
     with pytest.raises(TypeError) as e:
         GroundTruth(
             datum=datum,
             annotations=gts[0],  # type: ignore
         )
     assert "List[Annotation]" in str(e)
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError):
         GroundTruth(
             datum=datum,
             annotations=[gts[0], gts[1], "annotation"],  # type: ignore
         )
-    assert "Annotation" in str(e)
 
     # test equalities
     with pytest.raises(TypeError):
         _ = (
             GroundTruth(
                 datum=datum,
                 annotations=gts,
@@ -219,51 +214,49 @@
 
     # valid
     Prediction(datum=datum, annotations=pds)
 
     string = str(Prediction(datum=datum, annotations=pds))
     assert (
         string
-        == "{'datum': {'uid': 'somefile', 'metadata': {}}, 'annotations': [{'task_type': 'classification', 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'metadata': {}, 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}, {'task_type': 'classification', 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'metadata': {}, 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}]}"
+        == "{'datum': {'uid': 'somefile', 'metadata': {}}, 'annotations': [{'task_type': 'classification', 'metadata': {}, 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}, {'task_type': 'classification', 'metadata': {}, 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}]}"
     )
     assert "dataset_name" not in string
 
     # test `__post_init__`
+    with pytest.raises(TypeError):
+        Prediction(datum="datum", annotations=pds)  # type: ignore
     with pytest.raises(TypeError) as e:
-        Prediction.create(datum="datum", annotations=pds)  # type: ignore
-    assert "Datum" in str(e)
-    with pytest.raises(TypeError) as e:
-        Prediction.create(
+        Prediction(
             datum=datum,
             annotations=pds[0],  # type: ignore
         )
     assert "List[Annotation]" in str(e)
 
-    with pytest.raises(TypeError) as e:
-        Prediction.create(
+    with pytest.raises(TypeError):
+        Prediction(
             datum=datum,
             annotations=[pds[0], pds[1], "annotation"],  # type: ignore
         )
-    assert "Annotation" in str(e)
 
     with pytest.raises(ValueError) as e:
-        Prediction.create(
+        Prediction(
             datum=datum,
             annotations=[
-                Annotation.create(
+                Annotation(
                     task_type=enums.TaskType.CLASSIFICATION,
                     labels=[
-                        Label.create(key="test", value="value", score=0.8),
-                        Label.create(key="test", value="other", score=0.1),
+                        Label(key="test", value="value", score=0.8),
+                        Label(key="test", value="other", score=0.1),
                     ],
                 )
             ],
         )
     assert "for label key test got scores summing to 0.9" in str(e)
 
     # test equalities
     with pytest.raises(TypeError):
-        _ = Prediction.create(datum=datum, annotations=pds) == 1
+        _ = Prediction(datum=datum, annotations=pds) == 1
 
-    assert Prediction.create(
+    assert Prediction(datum=datum, annotations=pds) == Prediction(
         datum=datum, annotations=pds
-    ) == Prediction.create(datum=datum, annotations=pds)
+    )
```

### Comparing `valor-client-0.20.1/unit-tests/coretypes/test_evaluation.py` & `valor-client-0.20.2/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/coretypes/test_filtering.py` & `valor-client-0.20.2/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/schemas/test_filters.py` & `valor-client-0.20.2/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/schemas/test_geojson.py` & `valor-client-0.20.2/unit-tests/schemas/test_geojson.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from valor.schemas import BoundingBox, MultiPolygon, Point, Polygon, Raster
+from valor.schemas import Box, MultiPolygon, Point, Polygon, Raster
 
 
 def test_point():
     # valid
     p1 = Point((1, 1))
     p2 = Point((1.0, 1.0))
     p3 = Point((1.0, 0.99))
@@ -70,26 +70,24 @@
     p1 = (-1, -2)
     p2 = (10, -2)
     p3 = (10, 11)
     p4 = (-1, 11)
     coords = [[p1, p2, p3, p4, p1]]
 
     # test validation
-    BoundingBox(coords)
+    Box(coords)
     with pytest.raises(TypeError) as e:
-        BoundingBox(polygon=p1)  # type: ignore
+        Box(polygon=p1)  # type: ignore
     with pytest.raises(ValueError) as e:
-        BoundingBox([[p1, p2, p3, p4]])
+        Box([[p1, p2, p3, p4]])
     assert "at least 4 points with the first point being repeated" in str(e)
 
     # test classmethod `from_extrema`
     assert (
-        BoundingBox.from_extrema(
-            xmin=-1, xmax=10, ymin=-2, ymax=11
-        ).get_value()
+        Box.from_extrema(xmin=-1, xmax=10, ymin=-2, ymax=11).get_value()
         == coords
     )
 
 
 def test_multipolygon():
     p1 = (0, 0)
     p2 = (5, 0)
@@ -122,17 +120,17 @@
     Raster({"mask": mask1, "geometry": multipoly1.get_value()})
     Raster.from_numpy(mask=mask1)
     Raster.from_geometry(geometry=poly1, height=10, width=10)
     Raster.from_geometry(geometry=multipoly1, height=10, width=10)
 
     # test validation
     with pytest.raises(TypeError):
-        assert Raster({"mask": "test", "geometry": None})
+        assert Raster({"mask": "test", "geometry": None})  # type: ignore testing
     with pytest.raises(TypeError) as e:
-        assert Raster(123)
+        assert Raster(123)  # type: ignore - testing
 
     # test classmethod `from_numpy`
     mask2 = np.ones((10, 10, 10)) == 1
     mask3 = np.ones((10, 10))
     with pytest.raises(ValueError) as e:
         Raster.from_numpy(mask2)
     assert "raster only supports 2d arrays" in str(e)
```

### Comparing `valor-client-0.20.1/unit-tests/schemas/test_label.py` & `valor-client-0.20.2/unit-tests/schemas/test_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 def test_label():
     # valid
     l1 = Label(key="test", value="value")
 
     # test validation
     with pytest.raises(TypeError):
-        assert Label(key=123, value="123")
+        assert Label(key=123, value="123")  # type: ignore - testing
     with pytest.raises(TypeError):
-        assert Label(key="123", value=123)
+        assert Label(key="123", value=123)  # type: ignore - testing
 
     # test member fn `tuple`
     assert l1.tuple() == ("test", "value", None)
 
     # test member fn `__eq__`
     l2 = Label(key="test", value="value")
     assert l1 == l2
```

### Comparing `valor-client-0.20.1/unit-tests/symbolic/collections/test_dictionary.py` & `valor-client-0.20.2/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/symbolic/collections/test_static_collection.py` & `valor-client-0.20.2/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import pytest
 
 from valor.schemas import List as SymbolicList
 from valor.schemas.symbolic.collections import StaticCollection
-from valor.schemas.symbolic.types import Bool, Float, Integer, String, Symbol
+from valor.schemas.symbolic.types import Bool, Float, Integer, String
 
 
 def test_static_collection_init():
     class A(StaticCollection):
         w: Integer
         x: Float
         y: String
         z: Bool
 
     # test that kwargs are required
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         A()
 
 
 def test_static_collection_symbol():
     class A(StaticCollection):
         w: Integer
         x: Float
         y: String
         z: Bool
 
     # test that the 'symbolic' classmethod is the same as passing a symbol
     symA = A.symbolic()
-    assert symA.to_dict() == A(symbol=Symbol(name="a")).to_dict()
+    assert symA.to_dict() == A.symbolic(name="a").to_dict()
 
     # test symbolic usage
     assert symA.to_dict() == {
         "type": "symbol",
         "value": {
             "owner": None,
             "name": "a",
@@ -84,36 +84,26 @@
         x: Float
         y: String
         z: Bool
 
     encoding = {"w": 101, "x": 0.123, "y": "foobar", "z": True}
 
     # test that casting to symbolics is implicit
-    v1 = A.definite(w=101, x=0.123, y="foobar", z=True)
-    v2 = A.definite(
-        w=Integer(101), x=Float(0.123), y=String("foobar"), z=Bool(True)
-    )
-    v3 = A.definite(w=101, x=Float(0.123), y=String("foobar"), z=True)
+    v1 = A(w=101, x=0.123, y="foobar", z=True)
+    v2 = A(w=Integer(101), x=Float(0.123), y=String("foobar"), z=Bool(True))
+    v3 = A(w=101, x=Float(0.123), y=String("foobar"), z=True)
     assert v1.to_dict() == v2.to_dict()
     assert v1.to_dict() == v3.to_dict()
 
     # test that kwargs can be loaded by dictionary
-    v4 = A.definite(**encoding)
+    v4 = A(**encoding)
     v5 = A(**encoding)
     assert v1.to_dict() == v4.to_dict()
     assert v1.to_dict() == v5.to_dict()
 
-    # test 'definite' classmethod strips symbol
-    assert (
-        v1.to_dict()
-        == A.definite(
-            w=101, x=0.123, y="foobar", z=True, symbol=Symbol(name="test")
-        ).to_dict()
-    )
-
     # test dictionary generation
     assert v1.to_dict() == {
         "type": "a",
         "value": {"w": 101, "x": 0.123, "y": "foobar", "z": True},
     }
 
     # test value members
```

### Comparing `valor-client-0.20.1/unit-tests/symbolic/collections/test_structures.py` & `valor-client-0.20.2/unit-tests/symbolic/collections/test_structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,63 +17,55 @@
     Point,
     Polygon,
     String,
     Symbol,
     Time,
     Variable,
 )
-from valor.schemas.symbolic.collections import (
-    Dictionary,
-    DictionaryValue,
-    _get_atomic_type_by_name,
-    _get_atomic_type_by_value,
-)
 from valor.schemas.symbolic.operators import (
     AppendableFunction,
     TwoArgumentFunction,
 )
+from valor.schemas.symbolic.types import (
+    Dictionary,
+    DictionaryValue,
+    _get_type_by_value,
+    get_type_by_name,
+)
 
 
-def test__get_atomic_type_by_value():
-    assert _get_atomic_type_by_value(True) is Bool
-    assert _get_atomic_type_by_value("hello world") is String
-    assert _get_atomic_type_by_value(int(1)) is Integer
-    assert _get_atomic_type_by_value(float(3.14)) is Float
+def test__get_type_by_value():
+    assert _get_type_by_value(True) is Bool
+    assert _get_type_by_value("hello world") is String
+    assert _get_type_by_value(int(1)) is Integer
+    assert _get_type_by_value(float(3.14)) is Float
     assert (
-        _get_atomic_type_by_value(datetime.datetime(year=2024, month=1, day=1))
+        _get_type_by_value(datetime.datetime(year=2024, month=1, day=1))
         is DateTime
     )
+    assert _get_type_by_value(datetime.date(year=2024, month=1, day=1)) is Date
     assert (
-        _get_atomic_type_by_value(datetime.date(year=2024, month=1, day=1))
-        is Date
-    )
-    assert (
-        _get_atomic_type_by_value(datetime.time(hour=1, minute=1, second=1))
-        is Time
-    )
-    assert (
-        _get_atomic_type_by_value(datetime.timedelta(seconds=100)) is Duration
+        _get_type_by_value(datetime.time(hour=1, minute=1, second=1)) is Time
     )
-    assert _get_atomic_type_by_value((1, 1)) is Point
-    assert _get_atomic_type_by_value([(1, 1)]) is MultiPoint
-    assert _get_atomic_type_by_value([(1, 1), (2, 2)]) is LineString
-    assert _get_atomic_type_by_value([[(1, 1), (2, 2)]]) is MultiLineString
+    assert _get_type_by_value(datetime.timedelta(seconds=100)) is Duration
+    assert _get_type_by_value((1, 1)) is Point
+    assert _get_type_by_value([(1, 1)]) is MultiPoint
+    assert _get_type_by_value([(1, 1), (2, 2)]) is LineString
+    assert _get_type_by_value([[(1, 1), (2, 2)]]) is MultiLineString
+    assert _get_type_by_value([[(1, 1), (2, 2), (0, 1), (1, 1)]]) is Polygon
     assert (
-        _get_atomic_type_by_value([[(1, 1), (2, 2), (0, 1), (1, 1)]])
-        is Polygon
-    )
-    assert (
-        _get_atomic_type_by_value([[[(1, 1), (2, 2), (0, 1), (1, 1)]]])
+        _get_type_by_value([[[(1, 1), (2, 2), (0, 1), (1, 1)]]])
         is MultiPolygon
     )
+    assert _get_type_by_value({"randomvalue": "idk"}) is Dictionary
     with pytest.raises(NotImplementedError):
-        assert _get_atomic_type_by_value({"randomvalue": "idk"})
+        assert _get_type_by_value(set()).__name__
 
 
-def test__get_atomic_type_by_name():
+def test_get_type_by_name():
     types_ = [
         Bool,
         String,
         Integer,
         Float,
         DateTime,
         Date,
@@ -86,17 +78,18 @@
         Polygon,
         MultiPolygon,
     ]
     for type_ in types_:
         type_name = type_.__name__
         assert issubclass(type_, Variable)
         assert isinstance(type_name, str)
-        assert _get_atomic_type_by_name(type_name) is type_
+        assert get_type_by_name(type_name) is type_
+        assert get_type_by_name(f"list[{type_name}]") is List[type_]
     with pytest.raises(NotImplementedError):
-        assert _get_atomic_type_by_name("some_nonexistent_type")
+        assert get_type_by_name("some_nonexistent_type")
 
 
 def get_function_name(fn: str) -> str:
     fns = {
         "__eq__": "eq",
         "__ne__": "ne",
         "__and__": "and",
@@ -117,16 +110,16 @@
 
 def _test_to_dict(objcls, value):
     # test __init__
     assert objcls(value).to_dict() == {
         "type": objcls.__name__.lower(),
         "value": objcls(value).encode_value(),
     }
-    # test definite
-    assert objcls.definite(value).to_dict() == {
+    # test value
+    assert objcls(value).to_dict() == {
         "type": objcls.__name__.lower(),
         "value": objcls(value).encode_value(),
     }
     # test symbolic
     assert objcls.symbolic().to_dict() == {
         "type": "symbol",
         "value": {
@@ -201,15 +194,15 @@
             "name": "list[float]",
             "key": None,
             "attribute": None,
         },
     }
 
     # test creating valued lists
-    variable = List[Float].definite([0.1, 0.2, 0.3])
+    variable = List[Float]([0.1, 0.2, 0.3])
     assert variable.__str__() == "[0.1, 0.2, 0.3]"
     assert variable.to_dict() == {
         "type": "list[float]",
         "value": [0.1, 0.2, 0.3],
     }
 
     # test setting value in list by index
@@ -248,15 +241,15 @@
                 "attribute": None,
             },
         },
         "rhs": {"type": "list[float]", "value": [0.1, 0.2, 0.3]},
     }
 
     # test decode from json dict
-    assert List[Float].decode_value([0.1, 0.2, 0.3]).get_value() == [
+    assert List[Float].decode_value([0.1, 0.2, 0.3]).get_value() == [  # type: ignore
         0.1,
         0.2,
         0.3,
     ]
 
     # test comparison between valued variable and value
     assert (variable == [0.1, 0.2, 0.3]).to_dict() == {
@@ -268,29 +261,23 @@
     with pytest.raises(TypeError):
         assert List[String](String("hello"))
 
     # test setting list item to unsupported type
     with pytest.raises(TypeError):
         assert List[Integer]([String("hello")])
 
-    # test that type wrapper is not implemented
-    with pytest.raises(NotImplementedError):
-        List()[0]
-    with pytest.raises(NotImplementedError):
-        List()[0] = 1
-    with pytest.raises(NotImplementedError):
-        iter(List())
-    with pytest.raises(NotImplementedError):
-        len(List())
+    # test that untyped wrapper is not implemented
+    with pytest.raises(TypeError):
+        List()  # type: ignore - intentionally missing args
 
 
 def test_dictionary_value():
     # test cannot hold a value
-    with pytest.raises(NotImplementedError):
-        DictionaryValue.definite(1)
+    with pytest.raises(ValueError):
+        DictionaryValue(1)  # type: ignore - intentionally incorrect
 
     # test symbol cannot already attribute
     with pytest.raises(ValueError) as e:
         DictionaryValue(
             symbol=Symbol(name="a", attribute="c", owner="d", key="b"),
         )
     assert "attribute" in str(e)
@@ -388,22 +375,30 @@
         "__gt__",
         "__ge__",
         "__lt__",
         "__le__",
         "__and__",
         "__or__",
         "__xor__",
-        "is_none",
-        "is_not_none",
         "intersects",
         "inside",
         "outside",
     ]:
         _test_unsupported(objcls, permutations, op)
 
+    # test nullable
+    v1 = objcls.nullable(None)
+    assert v1.get_value() is None
+    assert v1.is_none().get_value() is True  # type: ignore - always a bool
+    assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
+    v2 = objcls.nullable(permutations[0][0])
+    assert v2.get_value() is not None
+    assert v2.is_none().get_value() is False  # type: ignore - always a bool
+    assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
+
     # test encoding
     assert {
         "k0": {"type": "bool", "value": True},
         "k1": {"type": "string", "value": "v1"},
         "k2": {"type": "integer", "value": 123},
         "k3": {"type": "float", "value": 1.24},
         "k4": {"type": "datetime", "value": "2024-01-01T00:00:00"},
```

### Comparing `valor-client-0.20.1/unit-tests/symbolic/test_operators.py` & `valor-client-0.20.2/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/symbolic/types/test_schemas.py` & `valor-client-0.20.2/unit-tests/symbolic/types/test_schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,13 @@
+import typing
+
 import numpy as np
 import pytest
 
-from valor.schemas import (
-    BoundingBox,
-    BoundingPolygon,
-    Embedding,
-    Raster,
-    Score,
-    TaskTypeEnum,
-)
+from valor.schemas import Box, Embedding, Float, Raster, TaskTypeEnum
 from valor.schemas.symbolic.operators import (
     AppendableFunction,
     TwoArgumentFunction,
 )
 
 
 def get_function_name(fn: str) -> str:
@@ -38,41 +33,44 @@
 def _test_encoding(objcls, value, encoded_value):
     assert (
         objcls(value).to_dict() == objcls.decode_value(encoded_value).to_dict()
     )
     assert encoded_value == objcls(value).encode_value()
 
 
-def _test_to_dict(objcls, value):
+def _test_to_dict(objcls, value, type_name: typing.Optional[str] = None):
+    type_name = type_name if type_name else objcls.__name__.lower()
     # test __init__
     assert objcls(value).to_dict() == {
-        "type": objcls.__name__.lower(),
+        "type": type_name,
         "value": objcls(value).encode_value(),
     }
-    # test definite
-    assert objcls.definite(value).to_dict() == {
-        "type": objcls.__name__.lower(),
+    # test value
+    assert objcls(value).to_dict() == {
+        "type": type_name,
         "value": objcls(value).encode_value(),
     }
     # test symbolic
     assert objcls.symbolic().to_dict() == {
         "type": "symbol",
         "value": {
             "owner": None,
-            "name": objcls.__name__.lower(),
+            "name": type_name,
             "key": None,
             "attribute": None,
         },
     }
 
 
-def _test_generic(objcls, permutations, op):
+def _test_generic(
+    objcls, permutations, op, type_name: typing.Optional[str] = None
+):
     """Tests expressions that can only be resolved to JSON."""
     for a, _ in permutations:
-        A = objcls(a)
+        A = objcls.nullable(a)
         C = objcls.symbolic()
         # test variable -> builtin against variable -> variable
         assert (
             C.__getattribute__(op)(a).to_dict()
             == C.__getattribute__(op)(A).to_dict()
         )
         # test commutative propery (this will fail)
@@ -82,15 +80,15 @@
                 a.__getattribute__(op)(C)
                 # function exists, but is not commutative
                 if type(a.__getattribute__(op)(A)) not in {objcls, type(a)}:
                     raise AssertionError("NotImplementedType")
             except AttributeError as e:
                 raise AssertionError(e)
         # test instance dictionary generation
-        _test_to_dict(objcls, a)
+        _test_to_dict(objcls, a, type_name)
         # test functional dictionary generation
         expr = C.__getattribute__(op)(a)
         expr_dict = expr.to_dict()
         if issubclass(type(expr), AppendableFunction):
             assert len(expr_dict) == 2
             assert expr_dict["op"] == get_function_name(op)
             assert expr_dict["args"] == [
@@ -102,15 +100,19 @@
             assert expr_dict["op"] == get_function_name(op)
             assert expr_dict["lhs"] == C.to_dict()
             assert expr_dict["rhs"] == A.to_dict()
         else:
             raise AssertionError
 
 
-def _test_resolvable(objcls, permutations, op):
+def _test_resolvable(
+    objcls, permutations, op, type_name: typing.Optional[str] = None
+):
+    type_name = type_name if type_name else objcls.__name__.lower()
+
     # test expressions that can be simplified to a 'Bool'
     for a, b in permutations:
         A = objcls(a)
         B = objcls(b)
 
         # determine truth
         truth = a.__getattribute__(op)(b)
@@ -119,72 +121,78 @@
         assert A.__getattribute__(op)(b).get_value() is truth
         # test variable -> variable against truth
         assert A.__getattribute__(op)(B).get_value() is truth
         # test dictionary generation
         dictA = A.to_dict()
         assert A.get_value() == a
         assert len(dictA) == 2
-        assert dictA["type"] == objcls.__name__.lower()
+        assert dictA["type"] == type_name
         assert dictA["value"] == A.encode_value()
     # test expressions that cannot be simplified
-    _test_generic(objcls, permutations, op)
+    _test_generic(objcls, permutations, op, type_name=type_name)
 
 
 def _test_unsupported(objcls, permutations, op):
     for a, b in permutations:
         with pytest.raises(AttributeError):
             objcls(a).__getattribute__(op)(b)
 
 
 def test_score():
-    objcls = Score
+    objcls = Float
 
     # test supported methods
     permutations = [
         (0.9, 0.1),
         (0.9, 0.9),
         (0.1, 0.9),
         (0.1, 0.1),
     ]
     unresolvable_permutations = [
         (0.9, None),
         (None, 0.9),
     ]
     for op in ["__eq__", "__ne__", "__gt__", "__ge__", "__lt__", "__le__"]:
-        _test_resolvable(objcls, permutations, op)
-        _test_generic(objcls, unresolvable_permutations, op)
+        _test_resolvable(objcls, permutations, op, type_name="float")
+        with pytest.raises(TypeError):
+            _test_generic(
+                objcls, unresolvable_permutations, op, type_name="float"
+            )
+
         with pytest.raises((AssertionError, TypeError)):
-            _test_resolvable(objcls, unresolvable_permutations, op)
+            _test_resolvable(
+                objcls,
+                unresolvable_permutations,
+                op,
+                type_name="float",
+            )
 
     # test nullable
-    assert Score(1.0).is_none().get_value() is False  # type: ignore - always returns bool
-    assert Score(1.0).is_not_none().get_value() is True  # type: ignore - always returns bool
-    assert Score(None).is_none().get_value() is True  # type: ignore - always returns bool
-    assert Score(None).is_not_none().get_value() is False  # type: ignore - always returns bool
+    v1 = objcls.nullable(None)
+    assert v1.get_value() is None
+    assert v1.is_none().get_value() is True  # type: ignore - always a bool
+    assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
+    v2 = objcls.nullable(permutations[0][0])
+    assert v2.get_value() is not None
+    assert v2.is_none().get_value() is False  # type: ignore - always a bool
+    assert v2.is_not_none().get_value() is True  # type: ignore - always a boolnullable(None).is_not_none().get_value() is False  # type: ignore - always returns bool
 
     # test unsupported methods
     for op in [
         "__and__",
         "__or__",
         "__xor__",
         "intersects",
         "inside",
         "outside",
     ]:
         _test_unsupported(objcls, permutations, op)
 
     # test encoding
     _test_encoding(objcls, 0.2, 0.2)
-    _test_encoding(objcls, None, None)
-
-    # test that score is bounded to the range 0.0 <= score <= 1.0
-    with pytest.raises(ValueError):
-        Score(-0.01)
-    with pytest.raises(ValueError):
-        Score(1.01)
 
 
 def test_tasktypeenum():
     from valor.enums import TaskType
 
     objcls = TaskTypeEnum
 
@@ -203,22 +211,30 @@
         "__gt__",
         "__ge__",
         "__lt__",
         "__le__",
         "__and__",
         "__or__",
         "__xor__",
-        "is_none",
-        "is_not_none",
         "intersects",
         "inside",
         "outside",
     ]:
         _test_unsupported(objcls, permutations, op)
 
+    # test nullable
+    v1 = objcls.nullable(None)
+    assert v1.get_value() is None
+    assert v1.is_none().get_value() is True  # type: ignore - always a bool
+    assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
+    v2 = objcls.nullable(permutations[0][0])
+    assert v2.get_value() is not None
+    assert v2.is_none().get_value() is False  # type: ignore - always a bool
+    assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
+
     # test encoding
     _test_encoding(
         objcls, TaskType.CLASSIFICATION, TaskType.CLASSIFICATION.value
     )
     _test_encoding(
         objcls, TaskType.OBJECT_DETECTION, TaskType.OBJECT_DETECTION.value
     )
@@ -226,48 +242,50 @@
         objcls,
         TaskType.SEMANTIC_SEGMENTATION,
         TaskType.SEMANTIC_SEGMENTATION.value,
     )
     _test_encoding(objcls, TaskType.EMBEDDING, TaskType.EMBEDDING.value)
 
 
-def test_bounding_box():
-    objcls = BoundingBox
+def test_box():
+    objcls = Box
     value = [[(0, 2), (1, 2), (1, 3), (0, 3), (0, 2)]]
     other = [[(1, 2), (2, 2), (2, 3), (1, 3), (1, 2)]]
 
     # test __init__
     assert objcls(value).get_value() == value
 
     # test 'from_extrema' classmethod
     assert objcls.from_extrema(0, 1, 2, 3).get_value() == value
 
     # test dictionary generation
     assert objcls.from_extrema(0, 1, 2, 3).to_dict() == {
-        "type": "boundingbox",
+        "type": "box",
         "value": value,
     }
 
     # test permutations
     permutations = [
         (value, value),
         (value, other),
         (other, other),
         (other, value),
-        (value, None),
-        (None, value),
     ]
     for op in ["intersects", "inside", "outside"]:
         _test_generic(objcls, permutations, op)
 
     # test nullable
-    assert objcls.from_extrema(0, 1, 2, 3).is_none().get_value() is False  # type: ignore - always returns bool
-    assert objcls.from_extrema(0, 1, 2, 3).is_not_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_not_none().get_value() is False  # type: ignore - always returns bool
+    v1 = objcls.nullable(None)
+    assert v1.get_value() is None
+    assert v1.is_none().get_value() is True  # type: ignore - always a bool
+    assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
+    v2 = objcls.nullable(permutations[0][0])
+    assert v2.get_value() is not None
+    assert v2.is_none().get_value() is False  # type: ignore - always a bool
+    assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
 
     # test unsupported methods
     for op in [
         "__eq__",
         "__ne__",
         "__gt__",
         "__ge__",
@@ -277,141 +295,89 @@
         "__or__",
         "__xor__",
     ]:
         _test_unsupported(objcls, permutations, op)
 
     # test encoding
     _test_encoding(objcls, value, value)
-    _test_encoding(objcls, None, None)
 
     # test validate box must define 5 points with first == last
     with pytest.raises(ValueError):
-        BoundingBox([[(0, 0)]])
+        Box([[(0, 0)]])
     with pytest.raises(ValueError):
-        BoundingBox(value[:-1])
+        Box(value[:-1])
     value[0][-1] = (10, 10)
     with pytest.raises(ValueError):
-        BoundingBox(value)
-
-
-def test_bounding_polygon():
-    objcls = BoundingPolygon
-    value = [[(0, 2), (1, 2), (1, 3), (0, 3), (0, 2)]]
-    other = [[(1, 2), (2, 2), (2, 3), (1, 3), (1, 2)]]
-
-    # test __init__
-    assert objcls(value).get_value() == value
-
-    # test dictionary generation
-    assert objcls(value).to_dict() == {
-        "type": "boundingpolygon",
-        "value": value,
-    }
-
-    # test permutations
-    permutations = [
-        (value, value),
-        (value, other),
-        (other, other),
-        (other, value),
-        (value, None),
-        (None, value),
-    ]
-    for op in ["intersects", "inside", "outside"]:
-        _test_generic(objcls, permutations, op)
-
-    # test nullable
-    assert objcls(value).is_none().get_value() is False  # type: ignore - always returns bool
-    assert objcls(value).is_not_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_not_none().get_value() is False  # type: ignore - always returns bool
-
-    # test unsupported methods
-    for op in [
-        "__eq__",
-        "__ne__",
-        "__gt__",
-        "__ge__",
-        "__lt__",
-        "__le__",
-        "__and__",
-        "__or__",
-        "__xor__",
-    ]:
-        _test_unsupported(objcls, permutations, op)
-
-    # test encoding
-    _test_encoding(objcls, value, value)
-    _test_encoding(objcls, None, None)
+        Box(value)
 
 
 def test_raster():
     objcls = Raster
 
     bitmask1 = np.full((10, 10), True)
     bitmask2 = np.full((10, 10), False)
-    geom = BoundingBox.from_extrema(0, 1, 2, 3)
+    geom = Box.from_extrema(0, 1, 2, 3)
 
     value = {"mask": bitmask1, "geometry": None}
     other = {"mask": bitmask2, "geometry": geom.get_value()}
 
     encoded_value = {
         "mask": "iVBORw0KGgoAAAANSUhEUgAAAAoAAAAKAQAAAAClSfIQAAAAEElEQVR4nGP8f5CJgQEXAgAzSQHUW1CW8QAAAABJRU5ErkJggg==",
         "geometry": None,
     }
 
     # test encoding
     _test_encoding(objcls, value, encoded_value)
-    _test_encoding(objcls, None, None)
 
     # test permutations
     permutations = [
         (value, value),
         (value, other),
         (other, other),
         (other, value),
-        (value, None),
-        (None, value),
     ]
     for op in ["intersects", "inside", "outside"]:
         _test_generic(objcls, permutations, op)
 
     # test nullable
-    assert objcls(value).is_none().get_value() is False  # type: ignore - always returns bool
-    assert objcls(value).is_not_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_not_none().get_value() is False  # type: ignore - always returns bool
-    assert Raster(None)
+    v1 = objcls.nullable(None)
+    assert v1.get_value() is None
+    assert v1.is_none().get_value() is True  # type: ignore - always a bool
+    assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
+    v2 = objcls.nullable(permutations[0][0])
+    assert v2.get_value() is not None
+    assert v2.is_none().get_value() is False  # type: ignore - always a bool
+    assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
 
     # test 'from_numpy' classmethod
     assert Raster.from_numpy(bitmask1).to_dict() == Raster(value).to_dict()
 
     # test 'from_geometry' classmethod
     assert (
         Raster.from_geometry(geom, 10, 10).to_dict() == Raster(other).to_dict()
     )
 
     # test type validation
     with pytest.raises(TypeError):
-        Raster(123)
+        Raster(123)  # type: ignore
     with pytest.raises(ValueError):
         Raster({})
     with pytest.raises(TypeError):
-        Raster({"mask": 123, "geometry": None})
+        Raster({"mask": 123, "geometry": None})  # type: ignore
     with pytest.raises(ValueError) as e:
         Raster({"mask": np.zeros((10,)), "geometry": None})
     assert "2d arrays" in str(e)
     with pytest.raises(ValueError) as e:
         Raster({"mask": np.zeros((10, 10, 10)), "geometry": None})
     assert "2d arrays" in str(e)
     with pytest.raises(ValueError) as e:
         Raster({"mask": np.zeros((10, 10)), "geometry": None})
     assert "bool" in str(e)
     with pytest.raises(TypeError):
-        Raster({"mask": bitmask1, "geometry": 123})
+        Raster({"mask": bitmask1, "geometry": 123})  # type: ignore
 
     # test property 'area'
     assert objcls.symbolic().area.is_symbolic
     assert objcls.symbolic().area.to_dict() == {
         "type": "symbol",
         "value": {
             "owner": None,
@@ -425,16 +391,14 @@
     with pytest.raises(ValueError):
         objcls(value).area
 
     # test property 'array'
     assert (bitmask1 == Raster(value).array).all()
     with pytest.warns(RuntimeWarning):
         Raster(other).array
-    with pytest.warns(RuntimeWarning):
-        Raster(None).array
 
     # test property 'array' is not available to symbols
     with pytest.raises(TypeError):
         Raster.symbolic().array
 
 
 def test_embedding():
@@ -453,25 +417,27 @@
 
     # test permutations
     permutations = [
         (value, value),
         (value, other),
         (other, other),
         (other, value),
-        (value, None),
-        (None, value),
     ]
     for op in ["intersects", "inside", "outside"]:
         _test_generic(objcls, permutations, op)
 
     # test nullable
-    assert objcls(value).is_none().get_value() is False  # type: ignore - always returns bool
-    assert objcls(value).is_not_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_none().get_value() is True  # type: ignore - always returns bool
-    assert objcls(None).is_not_none().get_value() is False  # type: ignore - always returns bool
+    v1 = objcls.nullable(None)
+    assert v1.get_value() is None
+    assert v1.is_none().get_value() is True  # type: ignore - always a bool
+    assert v1.is_not_none().get_value() is False  # type: ignore - always a bool
+    v2 = objcls.nullable(permutations[0][0])
+    assert v2.get_value() is not None
+    assert v2.is_none().get_value() is False  # type: ignore - always a bool
+    assert v2.is_not_none().get_value() is True  # type: ignore - always a bool
 
     # test unsupported methods
     for op in [
         "__eq__",
         "__ne__",
         "__gt__",
         "__ge__",
@@ -481,15 +447,14 @@
         "__or__",
         "__xor__",
     ]:
         _test_unsupported(objcls, permutations, op)
 
     # test encoding
     _test_encoding(objcls, value, value)
-    _test_encoding(objcls, None, None)
 
 
 def test_label():
     pass
 
 
 def test_annotation():
```

### Comparing `valor-client-0.20.1/unit-tests/test_client.py` & `valor-client-0.20.2/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/unit-tests/test_viz.py` & `valor-client-0.20.2/unit-tests/test_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import PIL.Image
 import pytest
 
 from valor import Annotation, GroundTruth, Label
 from valor.enums import TaskType
 from valor.metatypes import ImageMetadata
-from valor.schemas import BoundingPolygon, MultiPolygon, Polygon, Raster
+from valor.schemas import MultiPolygon, Polygon, Raster
 from valor.viz import (
     _polygons_to_binary_mask,
     create_combined_segmentation_mask,
     draw_detections_on_image,
 )
 
 
@@ -172,15 +172,15 @@
     detections = [
         GroundTruth(
             datum=ImageMetadata.create("test", 300, 300).datum,
             annotations=[
                 Annotation(
                     task_type=TaskType.OBJECT_DETECTION,
                     labels=[Label(key="k", value="v")],
-                    polygon=BoundingPolygon(bounding_poly.get_value()),
+                    polygon=Polygon(bounding_poly.get_value()),
                 )
             ],
         ),
     ]
     img = PIL.Image.new("RGB", (300, 300))
 
     img = draw_detections_on_image(detections, img)
```

### Comparing `valor-client-0.20.1/valor/__init__.py` & `valor-client-0.20.2/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/client.py` & `valor-client-0.20.2/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/coretypes.py` & `valor-client-0.20.2/valor/coretypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import datetime
 import json
 import time
-import warnings
 from dataclasses import asdict, dataclass
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from valor.client import ClientConnection, connect, get_connection
 from valor.enums import AnnotationType, EvaluationStatus, TableStatus, TaskType
 from valor.exceptions import ClientException
 from valor.schemas import (
     Annotation,
     Datum,
@@ -76,37 +75,32 @@
     """
 
     datum: Datum = Datum.symbolic(owner="groundtruth", name="datum")
     annotations: SymbolicList[Annotation] = SymbolicList[Annotation].symbolic(
         owner="groundtruth", name="annotations"
     )
 
-    @classmethod
-    def create(
-        cls,
+    def __init__(
+        self,
+        *,
         datum: Datum,
         annotations: List[Annotation],
-        **_,
     ):
         """
         Creates a ground truth.
 
         Parameters
         ----------
         datum : Datum
-            The `Datum` associated with the `GroundTruth`.
+            The datum that the ground truth is operating over.
         annotations : List[Annotation]
-            The list of `Annotations` associated with the `GroundTruth`.
+            The list of ground truth annotations.
         """
-        return cls.definite(
-            datum=datum,
-            annotations=annotations,
-        )
+        super().__init__(datum=datum, annotations=annotations)
 
-    def __post_init__(self):
         for annotation in self.annotations:
             for label in annotation.labels:
                 if label.score.get_value() is not None:
                     raise ValueError(
                         "GroundTruth labels should not have scores."
                     )
 
@@ -139,40 +133,33 @@
     """
 
     datum: Datum = Datum.symbolic(owner="prediction", name="datum")
     annotations: SymbolicList[Annotation] = SymbolicList[Annotation].symbolic(
         owner="prediction", name="annotations"
     )
 
-    @classmethod
-    def create(
-        cls,
+    def __init__(
+        self,
+        *,
         datum: Datum,
         annotations: List[Annotation],
-        **_,
     ):
         """
         Creates a prediction.
 
         Parameters
         ----------
         datum : Datum
-            The `Datum` associated with the `Prediction`.
+            The datum that the prediction is operating over.
         annotations : List[Annotation]
-            The list of `Annotations` associated with the `Prediction`.
+            The list of predicted annotations.
         """
-        return cls.definite(
-            datum=datum,
-            annotations=annotations,
-        )
+        super().__init__(datum=datum, annotations=annotations)
 
-    def __post_init__(self):
-        """
-        Validate the inputs of the `Prediction` based on task type.
-        """
+        # validation
         for annotation in self.annotations:
             task_type = annotation.task_type.get_value()
             if task_type in [
                 TaskType.CLASSIFICATION,
                 TaskType.OBJECT_DETECTION,
             ]:
                 for label in annotation.labels:
@@ -431,42 +418,58 @@
     """
 
     name: String = String.symbolic(owner="dataset", name="name")
     metadata: Dictionary = Dictionary.symbolic(
         owner="dataset", name="metadata"
     )
 
+    def __init__(
+        self,
+        *,
+        name: str,
+        metadata: Optional[dict] = None,
+        connection: Optional[ClientConnection] = None,
+    ):
+        """
+        Creates a local instance of a dataset.
+
+        Use 'Dataset.create' classmethod to create a dataset with persistence.
+
+        Parameters
+        ----------
+        name : str
+            The name of the dataset.
+        metadata : dict, optional
+            A dictionary of metadata that describes the dataset.
+        connection : ClientConnection, optional
+            An initialized client connection.
+        """
+        self.conn = connection
+        super().__init__(name=name, metadata=metadata if metadata else dict())
+
     @classmethod
     def create(
         cls,
         name: str,
-        metadata: Optional[dict] = None,
+        metadata: Optional[Dict[str, Any]] = None,
         connection: Optional[ClientConnection] = None,
-        **_,
     ) -> Dataset:
         """
         Creates a dataset that persists in the back end.
 
         Parameters
         ----------
         name : str
             The name of the dataset.
-        metadata : dict
+        metadata : dict, optional
             A dictionary of metadata that describes the dataset.
-
-        Returns
-        -------
-        valor.Dataset
-            The created dataset.
+        connection : ClientConnection, optional
+            An initialized client connection.
         """
-        dataset = cls.definite(
-            name=name,
-            metadata=metadata,
-        )
-        dataset.add_connection(connection)
+        dataset = cls(name=name, metadata=metadata, connection=connection)
         Client(dataset.conn).create_dataset(dataset)
         return dataset
 
     @classmethod
     def get(
         cls,
         name: str,
@@ -483,28 +486,14 @@
         Returns
         -------
         Union[valor.Dataset, None]
             The dataset or 'None' if it doesn't exist.
         """
         return Client(connection).get_dataset(name)
 
-    def add_connection(
-        self,
-        connection: Optional[ClientConnection],
-    ):
-        """
-        Stores a pre-existing connection.
-
-        Parameters
-        ----------
-        connection : ClientConnnetion, optional
-            An optional Valor client object for interacting with the API.
-        """
-        self.conn = connection
-
     def add_groundtruth(
         self,
         groundtruth: GroundTruth,
     ) -> None:
         """
         Add a ground truth to the dataset.
 
@@ -684,43 +673,61 @@
     >>> Model.create(name="model1", metadata={})
     >>> Model.create(name="model1", metadata={"foo": "bar", "pi": 3.14})
     """
 
     name: String = String.symbolic(owner="model", name="name")
     metadata: Dictionary = Dictionary.symbolic(owner="model", name="metadata")
 
+    def __init__(
+        self,
+        *,
+        name: str,
+        metadata: Optional[dict] = None,
+        connection: Optional[ClientConnection] = None,
+    ):
+        """
+        Creates a local instance of a model.
+
+        Use 'Model.create' classmethod to create a model with persistence.
+
+        Parameters
+        ----------
+        name : String
+            The name of the model.
+        metadata : Dictionary
+            A dictionary of metadata that describes the model.
+        connection : ClientConnection, optional
+            An initialized client connection.
+        symbol : Symbol, optional
+            Symbol to represent a model.
+        """
+        self.conn = connection
+        super().__init__(name=name, metadata=metadata if metadata else dict())
+
     @classmethod
     def create(
         cls,
         name: str,
-        metadata: Optional[dict] = None,
+        metadata: Optional[Dict[str, Any]] = None,
         connection: Optional[ClientConnection] = None,
         **_,
     ) -> Model:
         """
         Creates a model that persists in the back end.
 
         Parameters
         ----------
         name : str
             The name of the model.
-        metadata : dict
+        metadata : dict, optional
             A dictionary of metadata that describes the model.
-        connection : ClientConnnetion, optional
-            An optional Valor client object for interacting with the API.
-
-        Returns
-        -------
-        valor.Model
-            The created model.
+        connection : ClientConnection, optional
+            An initialized client connection.
         """
-        model = cls.definite(
-            name=name,
-            metadata=metadata,
-        )
+        model = cls(name=name, metadata=metadata, connection=connection)
         model.add_connection(connection)
         Client(connection).create_model(model)
         return model
 
     @classmethod
     def get(
         cls,
@@ -1233,18 +1240,14 @@
         for groundtruth in groundtruths:
             if not isinstance(groundtruth, GroundTruth):
                 raise TypeError(
                     f"Expected ground truth to be of type 'valor.GroundTruth' not '{type(groundtruth)}'."
                 )
             if not isinstance(groundtruth.annotations._value, list):
                 raise TypeError
-            if len(groundtruth.annotations._value) == 0:
-                warnings.warn(
-                    f"GroundTruth for datum with uid `{groundtruth.datum.uid}` contains no annotations."
-                )
             groundtruth_dict = encode_api_format(groundtruth)
             groundtruth_dict["datum"]["dataset_name"] = dataset.get_name()
             groundtruths_json.append(groundtruth_dict)
         self.conn.create_groundtruths(groundtruths_json)
 
     def get_groundtruth(
         self,
@@ -1312,16 +1315,16 @@
         Union[Dataset, None]
             A Dataset with a matching name, or 'None' if one doesn't exist.
         """
         try:
             resp = decode_api_format(self.conn.get_dataset(name))
             dataset = Dataset(
                 **resp,
+                connection=self.conn,
             )
-            dataset.add_connection(self.conn)
             return dataset
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_datasets(
@@ -1343,16 +1346,15 @@
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
         dataset_list = []
         for kwargs in self.conn.get_datasets(filter_):
             kwargs = decode_api_format(kwargs)
-            dataset = Dataset(**kwargs)
-            dataset.add_connection(self.conn)
+            dataset = Dataset(**kwargs, connection=self.conn)
             dataset_list.append(dataset)
         return dataset_list
 
     def get_datums(
         self,
         filter_by: Optional[FilterType] = None,
     ) -> List[Datum]:
@@ -1369,15 +1371,15 @@
         List[valor.Datum]
             A list datums.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
         return [
-            Datum.create(**decode_api_format(datum))
+            Datum(**decode_api_format(datum))
             for datum in self.conn.get_datums(filter_)
         ]
 
     def get_datum(
         self,
         dataset: Union[Dataset, str],
         uid: str,
@@ -1398,15 +1400,15 @@
         """
         dataset_name = (
             dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         try:
             resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)
             resp = decode_api_format(resp)
-            return Datum.create(**resp)
+            return Datum(**resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_dataset_status(
         self,
@@ -1509,18 +1511,14 @@
         for prediction in predictions:
             if not isinstance(prediction, Prediction):
                 raise TypeError(
                     f"Expected prediction to be of type 'valor.Prediction' not '{type(prediction)}'."
                 )
             if not isinstance(prediction.annotations._value, list):
                 raise TypeError
-            if len(prediction.annotations._value) == 0:
-                warnings.warn(
-                    f"Prediction for datum with uid `{prediction.datum.uid}` contains no annotations."
-                )
             prediction_dict = encode_api_format(prediction)
             prediction_dict["datum"]["dataset_name"] = dataset.get_name()
             prediction_dict["model_name"] = model.get_name()
             predictions_json.append(prediction_dict)
         self.conn.create_predictions(predictions_json)
 
     def get_prediction(
@@ -1554,15 +1552,15 @@
         try:
             resp = self.conn.get_prediction(
                 dataset_name=dataset_name,
                 model_name=model_name,
                 datum_uid=datum_uid,
             )
             resp = decode_api_format(resp)
-            return Prediction.create(**resp)
+            return Prediction(**resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def finalize_inferences(
         self, dataset: Union[Dataset, str], model: Union[Model, str]
```

### Comparing `valor-client-0.20.1/valor/enums.py` & `valor-client-0.20.2/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/exceptions.py` & `valor-client-0.20.2/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/metatypes.py` & `valor-client-0.20.2/valor/metatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ):
         if not isinstance(height, int) or not isinstance(width, int):
             raise TypeError("Height and width must be integers.")
         metadata = metadata if metadata else dict()
         metadata["height"] = height
         metadata["width"] = width
         return cls(
-            datum=Datum.definite(
+            datum=Datum(
                 uid=uid,
                 metadata=metadata,
             )
         )
 
     @classmethod
     def from_pil(cls, image: Image, uid: str):
@@ -142,15 +142,15 @@
         ):
             raise TypeError("Height, width and frame must be integers.")
         metadata = metadata if metadata else dict()
         metadata["height"] = height
         metadata["width"] = width
         metadata["frame"] = frame
         return cls(
-            Datum.definite(
+            Datum(
                 uid=uid,
                 metadata=metadata,
             )
         )
 
     @property
     def height(self) -> int:
```

### Comparing `valor-client-0.20.1/valor/schemas/compatibility.py` & `valor-client-0.20.2/valor/schemas/compatibility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from typing import Any, Optional, Union
 
-from valor.schemas.symbolic.collections import (
-    Dictionary,
-    _get_atomic_type_by_name,
-)
 from valor.schemas.symbolic.types import (
-    BoundingBox,
-    BoundingPolygon,
+    Box,
     Date,
     DateTime,
+    Dictionary,
     Duration,
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
     Raster,
     Time,
+    get_type_by_name,
 )
 
 
 def _encode_api_metadata_values(variable):
     if isinstance(
         variable,
         (
@@ -45,46 +42,41 @@
         return variable.encode_value()
 
 
 def _encode_api_metadata(metadata: Dictionary) -> dict:
     return {k: _encode_api_metadata_values(v) for k, v in metadata.items()}
 
 
-def _encode_api_geometry(
-    geometry: Union[
-        Polygon, MultiPolygon, BoundingPolygon, BoundingBox, Raster
-    ]
-):
-    value = geometry.get_value()
-    if value is None:
+def _encode_api_geometry(geometry: Union[Box, Polygon, MultiPolygon, Raster]):
+    if geometry.get_value() is None:
         return None
-    elif isinstance(geometry, BoundingBox):
+    elif isinstance(geometry, Box):
         return {
             "polygon": {
                 "points": [
-                    {"x": pt[0], "y": pt[1]} for pt in geometry.boundary
+                    {"x": pt[0], "y": pt[1]} for pt in geometry.boundary[:-1]
                 ]
             }
         }
-    elif isinstance(geometry, (BoundingPolygon, Polygon)):
+    elif isinstance(geometry, Polygon):
         return {
             "boundary": {
                 "points": [
-                    {"x": pt[0], "y": pt[1]} for pt in geometry.boundary
+                    {"x": pt[0], "y": pt[1]} for pt in geometry.boundary[:-1]
                 ]
             },
             "holes": [
-                {"points": [{"x": pt[0], "y": pt[1]} for pt in hole]}
+                {"points": [{"x": pt[0], "y": pt[1]} for pt in hole[:-1]]}
                 for hole in geometry.holes
             ],
         }
     elif isinstance(geometry, MultiPolygon):
         return {
             "polygons": [
-                _encode_api_geometry(poly) for poly in geometry.polygons
+                _encode_api_geometry(poly) for poly in geometry.to_polygons()
             ]
         }
     elif isinstance(geometry, Raster):
         value = geometry.encode_value()
         if value["geometry"] is not None:
             if Polygon.supports(value["geometry"]):
                 value["geometry"] = _encode_api_geometry(
@@ -126,19 +118,19 @@
     return json
 
 
 def _decode_api_metadata_values(value: Any):
     if not isinstance(value, dict):
         return value
     elif set(value.keys()) == {"geojson"}:
-        obj = _get_atomic_type_by_name(value["geojson"]["type"])
+        obj = get_type_by_name(value["geojson"]["type"])
         return obj.decode_value(value["geojson"]["coordinates"])
     elif len(value) == 1:
         k, v = list(value.items())[0]
-        obj = _get_atomic_type_by_name(k)
+        obj = get_type_by_name(k)
         return obj.decode_value(v)
     else:
         raise NotImplementedError(str(value))
 
 
 def _decode_api_metadata(metadata) -> dict:
     return {k: _decode_api_metadata_values(v) for k, v in metadata.items()}
@@ -176,15 +168,15 @@
             if value["holes"]
             else None
         )
         return [boundary, *holes] if holes else [boundary]
     elif set(value.keys()) == {"mask", "geometry"}:
         if value["geometry"] is not None:
             value["geometry"] = _decode_api_geometry(value["geometry"])
-        return Raster.decode_value(value).get_value()
+        return Raster.decode_value(value).get_value()  # type: ignore - none case already handled
 
 
 def decode_api_format(json: dict):
     """Decoded api format into client format."""
     # objects
     if "datum" in json:
         json["datum"] = decode_api_format(json["datum"])
```

### Comparing `valor-client-0.20.1/valor/schemas/evaluation.py` & `valor-client-0.20.2/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/schemas/filters.py` & `valor-client-0.20.2/valor/schemas/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         "dataset.metadata": "dataset_metadata",
         "model.name": "model_names",
         "model.metadata": "model_metadata",
         "datum.uid": "datum_uids",
         "datum.metadata": "datum_metadata",
         "annotation.task_type": "task_types",
         "annotation.metadata": "annotation_metadata",
-        "annotation.box": "require_bounding_box",
-        "annotation.box.area": "bounding_box_area",
+        "annotation.bounding_box": "require_bounding_box",
+        "annotation.bounding_box.area": "bounding_box_area",
         "annotation.polygon": "require_polygon",
         "annotation.polygon.area": "polygon_area",
         "annotation.raster": "require_raster",
         "annotation.raster.area": "raster_area",
         "annotation.labels": "labels",
         "label.id": "label_ids",
         "label.key": "label_keys",
```

### Comparing `valor-client-0.20.1/valor/schemas/symbolic/operators.py` & `valor-client-0.20.2/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/schemas/symbolic/types.py` & `valor-client-0.20.2/valor/schemas/symbolic/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import io
+import re
 import typing
 import warnings
 from base64 import b64decode, b64encode
-from typing import Any, List, Optional, Tuple, Union
+from collections.abc import MutableMapping
+from typing import Iterator
 
 import numpy as np
 import PIL.Image
 
 from valor.enums import TaskType
 from valor.schemas.symbolic.operators import (
     And,
@@ -36,17 +38,17 @@
     --------
     >>> Symbol(name="a")
     """
 
     def __init__(
         self,
         name: str,
-        key: Optional[str] = None,
-        attribute: Optional[str] = None,
-        owner: Optional[str] = None,
+        key: typing.Optional[str] = None,
+        attribute: typing.Optional[str] = None,
+        owner: typing.Optional[str] = None,
     ):
         self._owner = owner.lower() if owner else None
         self._name = name.lower()
         self._key = key.lower() if key else None
         self._attribute = attribute.lower() if attribute else None
 
     def __repr__(self):
@@ -106,68 +108,62 @@
 
     Contains either a value or a symbol.
 
     Examples
     --------
     Creating a valued variable.
     >>> Variable(value=...)
-    or
-    >>> Variable.definite(...)
+
+    Creating a optionally valued variable.
+    >>> Variable.nullable(value=...)
 
     Creating a symbolic variable.
-    >>> Variable(symbol=Symbol(...))
-    or
     >>> Variable.symbolic(name=...)
     """
 
     def __init__(
         self,
-        value: Optional[Any] = None,
-        symbol: Optional[Symbol] = None,
+        value: typing.Any,
     ):
-        if (value is not None) and (symbol is not None):
-            raise TypeError(
-                f"{type(self).__name__} cannot be symbolic and contain a value at the same time."
-            )
-        elif symbol is not None and not isinstance(symbol, Symbol):
-            raise TypeError(
-                f"{type(self).__name__} symbol should have type 'Symbol' or be set to 'None'"
-            )
-        elif symbol is None:
-            self.__validate__(value)
-        self._value = symbol if symbol else value
+        self.__validate__(value)
+        self._value = value
 
     def __repr__(self) -> str:
         return self._value.__repr__()
 
     def __str__(self) -> str:
         return str(self._value)
 
     @classmethod
-    def definite(
+    def nullable(
         cls,
-        value: Any,
+        value: typing.Optional[typing.Any],
     ):
         """
-        Initialize variable with a value.
+        Initialize variable with an optional.
 
         Parameters
         ----------
         value : Any
             The intended value of the variable.
         """
-        return cls(value=value)
+        if value is None:
+            obj = cls.__new__(cls)
+            obj._value = None
+            return obj
+        else:
+            return cls(value)
 
     @classmethod
     def symbolic(
         cls,
-        name: Optional[str] = None,
-        key: Optional[str] = None,
-        attribute: Optional[str] = None,
-        owner: Optional[str] = None,
+        name: typing.Optional[str] = None,
+        key: typing.Optional[str] = None,
+        attribute: typing.Optional[str] = None,
+        owner: typing.Optional[str] = None,
     ):
         """
         Initialize variable as a symbol.
 
         Parameters
         ----------
         name: str, optional
@@ -175,72 +171,78 @@
         key: str, optional
             An optional dictionary key.
         attribute: str, optional
             An optional attribute name.
         owner: str, optional
             An optional name describing the class that owns this symbol.
         """
-        name = cls.__name__ if not name else name
-        return cls(
-            symbol=Symbol(
-                name=name,
-                key=key,
-                attribute=attribute,
-                owner=owner,
-            )
+        name = cls.__name__.lower() if not name else name
+        symbol = Symbol(
+            name=name,
+            key=key,
+            attribute=attribute,
+            owner=owner,
         )
+        obj = cls.__new__(cls)
+        obj._value = symbol
+        return obj
 
     @classmethod
-    def preprocess(cls, value: Any):
+    def preprocess(cls, value: typing.Any):
         """
         This method converts any type to an instance of the variable class.
 
         It will raise an error if a value is unsupported.
 
         Parameters
         ----------
-        value : Any
+        value : typing.Any
             An instance of a variable, value, or symbol.
 
         Raises
         ------
         TypeError
             If a value or variable instance is of an incompatible type.
         """
         if isinstance(value, cls):
             return value
         elif isinstance(value, Symbol):
-            return cls(symbol=value)
+            return cls.symbolic(
+                name=value._name,
+                key=value._key,
+                attribute=value._attribute,
+                owner=value._owner,
+            )
         elif cls.supports(value):
             return cls(value=value)
         raise TypeError(
             f"{cls.__name__} does not support operations with value '{value}' of type '{type(value).__name__}'."
         )
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         """
         Validates typing.
 
         Parameters
         ----------
-        value : Any
+        value : typing.Any
             The value to validate.
 
         Raises
         ------
         NotImplementedError
             This function is not implemented in the base class.
         """
         raise NotImplementedError(
             f"Variable of type `{cls.__name__}` cannot be assigned a value."
         )
 
     @classmethod
-    def supports(cls, value: Any) -> bool:
+    def supports(cls, value: typing.Any) -> bool:
         """
         Checks if value is a supported type.
 
         Returns
         -------
         bool
         """
@@ -248,19 +250,21 @@
             cls.__validate__(value)
         except (TypeError, ValueError):
             return False
         else:
             return True
 
     @classmethod
-    def decode_value(cls, value: Any):
+    def decode_value(cls, value: typing.Any):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(value=value)
 
-    def encode_value(self) -> Any:
+    def encode_value(self) -> typing.Any:
         """Encode object to JSON compatible dictionary."""
         return self.get_value()
 
     @classmethod
     def from_dict(cls, value: dict):
         """Decode a JSON-compatible dictionary into an instance of the variable."""
         if set(value.keys()) != {"type", "value"}:
@@ -285,15 +289,15 @@
         return isinstance(self._value, Symbol)
 
     @property
     def is_value(self) -> bool:
         """Returns whether variable contains a value."""
         return not isinstance(self._value, Symbol)
 
-    def get_value(self) -> Any:
+    def get_value(self) -> typing.Any:
         """
         Retrieve value, if it exists.
 
         Raises
         ------
         TypeError
             If the variable is symbolic.
@@ -317,40 +321,52 @@
         -------
         Symbol
         """
         if not isinstance(self._value, Symbol):
             raise TypeError(f"{type(self).__name__} is a valued object.")
         return self._value
 
-    def __eq__(self, value: Any) -> Union["Bool", Eq]:  # type: ignore - overriding __eq__
+    def is_none(self) -> typing.Union["Bool", IsNull]:
+        """Conditional whether variable is 'None'"""
+        if self.is_value:
+            return Bool(self.get_value() is None)
+        return IsNull(self)
+
+    def is_not_none(self) -> typing.Union["Bool", IsNotNull]:
+        """Conditional whether variable is not 'None'"""
+        if self.is_value:
+            return Bool(self.get_value() is not None)
+        return IsNotNull(self)
+
+    def __eq__(self, value: typing.Any) -> typing.Union["Bool", Eq]:  # type: ignore - overriding __eq__
         raise AttributeError(
             f"'{type(self).__name__}' object has no attribute '__eq__'"
         )
 
-    def __ne__(self, value: Any) -> Union["Bool", Ne]:  # type: ignore - overriding __ne__
+    def __ne__(self, value: typing.Any) -> typing.Union["Bool", Ne]:  # type: ignore - overriding __ne__
         raise AttributeError(
             f"'{type(self).__name__}' object has no attribute '__ne__'"
         )
 
-    def __gt__(self, value: Any) -> Union["Bool", Gt]:
+    def __gt__(self, value: typing.Any) -> typing.Union["Bool", Gt]:
         raise AttributeError(
             f"'{type(self).__name__}' object has no attribute '__gt__'"
         )
 
-    def __ge__(self, value: Any) -> Union["Bool", Ge]:
+    def __ge__(self, value: typing.Any) -> typing.Union["Bool", Ge]:
         raise AttributeError(
             f"'{type(self).__name__}' object has no attribute '__ge__'"
         )
 
-    def __lt__(self, value: Any) -> Union["Bool", Lt]:
+    def __lt__(self, value: typing.Any) -> typing.Union["Bool", Lt]:
         raise AttributeError(
             f"'{type(self).__name__}' object has no attribute '__lt__'"
         )
 
-    def __le__(self, value: Any) -> Union["Bool", Le]:
+    def __le__(self, value: typing.Any) -> typing.Union["Bool", Le]:
         raise AttributeError(
             f"'{type(self).__name__}' object has no attribute '__le__'"
         )
 
 
 class Bool(Variable):
     """
@@ -364,177 +380,158 @@
         A symbolic representation.
 
     Examples
     --------
     >>> Bool(True)
     """
 
+    def __init__(self, value: bool):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         """
         Validates typing.
 
         Parameters
         ----------
-        value : Any
+        value : typing.Any
             The value to validate.
 
         Raises
         ------
         TypeError
             If the value type is not supported.
         """
         if not isinstance(value, bool):
             raise TypeError(
                 f"Expected type '{bool}' received type '{type(value)}'"
             )
 
-    def __eq__(self, value: Any) -> Union["Bool", Eq]:
+    def __eq__(self, value: typing.Any) -> typing.Union["Bool", Eq]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return type(self)(self.get_value() is other.get_value())
         return Eq(self, other)
 
-    def __ne__(self, value: Any) -> Union["Bool", Ne]:
+    def __ne__(self, value: typing.Any) -> typing.Union["Bool", Ne]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return type(self)(self.get_value() is not other.get_value())
         return Ne(self, other)
 
-    def __and__(self, value: Any) -> Union["Bool", And]:
+    def __and__(self, value: typing.Any) -> typing.Union["Bool", And]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return type(self)(self.get_value() and other.get_value())
         return And(self, other)
 
-    def __or__(self, value: Any) -> Union["Bool", Or]:
+    def __or__(self, value: typing.Any) -> typing.Union["Bool", Or]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return type(self)(self.get_value() or other.get_value())
         return Or(self, other)
 
-    def __xor__(self, value: Any) -> Union["Bool", Xor]:
+    def __xor__(self, value: typing.Any) -> typing.Union["Bool", Xor]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return self != value
         return Xor(self, other)
 
-    def __invert__(self) -> Union["Bool", Negate]:
+    def __invert__(self) -> typing.Union["Bool", Negate]:
         if self.is_value:
             return type(self)(not self.get_value())
         return Negate(self)
 
 
 class Equatable(Variable):
     """
     Variable modifier to handle equatable values.
     """
 
-    def __eq__(self, value: Any) -> Union["Bool", Eq]:
+    def __eq__(self, value: typing.Any) -> typing.Union["Bool", Eq]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             lhs = self.encode_value()
             rhs = other.encode_value()
             if lhs is None:
                 return Bool(rhs is None)
             elif rhs is None:
                 return Bool(lhs is None)
             else:
                 return Bool(lhs == rhs)
         return Eq(self, other)
 
-    def __ne__(self, value: Any) -> Union["Bool", Ne]:
+    def __ne__(self, value: typing.Any) -> typing.Union["Bool", Ne]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             lhs = self.encode_value()
             rhs = other.encode_value()
             if lhs is None:
                 return Bool(rhs is not None)
             elif rhs is None:
                 return Bool(lhs is not None)
             else:
                 return Bool(lhs != rhs)
         return Ne(self, other)
 
-    def in_(self, vlist: List[Any]) -> Or:
+    def in_(self, vlist: typing.List[typing.Any]) -> Or:
         """Returns Or(*[(self == v) for v in vlist])"""
         return Or(*[(self == v) for v in vlist])
 
     def __hash__(self):
         if self.is_symbolic:
             return hash(str(self))
         return hash(str(self.encode_value()))
 
 
 class Quantifiable(Equatable):
     """
     Variable modifier to handle quantifiable values.
     """
 
-    def __gt__(self, value: Any) -> Union["Bool", Gt]:
+    def __gt__(self, value: typing.Any) -> typing.Union["Bool", Gt]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return Bool(self.get_value() > other.get_value())
         return Gt(self, other)
 
-    def __ge__(self, value: Any) -> Union["Bool", Ge]:
+    def __ge__(self, value: typing.Any) -> typing.Union["Bool", Ge]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return Bool(self.get_value() >= other.get_value())
         return Ge(self, other)
 
-    def __lt__(self, value: Any) -> Union["Bool", Lt]:
+    def __lt__(self, value: typing.Any) -> typing.Union["Bool", Lt]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return Bool(self.get_value() < other.get_value())
         return Lt(self, other)
 
-    def __le__(self, value: Any) -> Union["Bool", Le]:
+    def __le__(self, value: typing.Any) -> typing.Union["Bool", Le]:
         other = self.preprocess(value)
         if self.is_value and other.is_value:
             return Bool(self.get_value() <= other.get_value())
         return Le(self, other)
 
 
-class Nullable(Variable):
-    """
-    Variable modifier to handle null values.
-    """
-
-    def is_none(self) -> Union["Bool", IsNull]:
-        """Conditional whether variable is 'None'"""
-        if self.is_value:
-            return Bool(self.get_value() is None)
-        return IsNull(self)
-
-    def is_not_none(self) -> Union["Bool", IsNotNull]:
-        """Conditional whether variable is not 'None'"""
-        if self.is_value:
-            return Bool(self.get_value() is not None)
-        return IsNotNull(self)
-
-    def get_value(self) -> Optional[Any]:
-        """Re-typed to output 'Optional[Any]'"""
-        return super().get_value()
-
-
 class Spatial(Variable):
     """
     Variable modifier to handle spatial values.
     """
 
-    def intersects(self, other: Any) -> Intersects:
+    def intersects(self, other: typing.Any) -> Intersects:
         """Conditional whether lhs intersects rhs."""
         return Intersects(self, self.preprocess(other))
 
-    def inside(self, other: Any) -> Inside:
+    def inside(self, other: typing.Any) -> Inside:
         """Conditional whether lhs is fully inside of rhs."""
         return Inside(self, self.preprocess(other))
 
-    def outside(self, other: Any) -> Outside:
+    def outside(self, other: typing.Any) -> Outside:
         """Conditional whether lhs is outside of rhs."""
         return Outside(self, self.preprocess(other))
 
 
 class Integer(Quantifiable):
     """
     Implementation of the built-in type 'int' as a Variable.
@@ -547,16 +544,19 @@
         A symbolic representation.
 
     Examples
     --------
     >>> Integer(123)
     """
 
+    def __init__(self, value: int):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, (int, np.integer)):
             raise TypeError(
                 f"Expected type '{int}' received type '{type(value)}'"
             )
 
 
 class Float(Quantifiable):
@@ -571,16 +571,19 @@
         A symbolic representation.
 
     Examples
     --------
     >>> Float(3.14)
     """
 
+    def __init__(self, value: float):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, (int, float, np.floating)):
             raise TypeError(
                 f"Expected type '{float}' received type '{type(value)}'"
             )
 
 
 class String(Equatable):
@@ -595,16 +598,19 @@
         A symbolic representation.
 
     Examples
     --------
     >>> String("hello world")
     """
 
+    def __init__(self, value: str):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, str):
             raise TypeError(
                 f"Expected type '{str}' received type '{type(value)}'"
             )
 
 
 class DateTime(Quantifiable):
@@ -620,29 +626,37 @@
 
     Examples
     --------
     >>> import datetime
     >>> DateTime(datetime.datetime(year=2024, month=1, day=1))
     """
 
+    def __init__(self, value: datetime.datetime):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, datetime.datetime):
             raise TypeError(
                 f"Expected type '{datetime.datetime}' received type '{type(value)}'"
             )
 
     @classmethod
-    def decode_value(cls, value: str):
+    def decode_value(cls, value: typing.Optional[str]):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(value=datetime.datetime.fromisoformat(value))
 
     def encode_value(self):
         """Encode object to JSON compatible dictionary."""
-        return self.get_value().isoformat()
+        value = self.get_value()
+        if value is None:
+            return None
+        return value.isoformat()
 
 
 class Date(Quantifiable):
     """
     Implementation of the type 'datetime.date' as a Variable.
 
     Parameters
@@ -654,29 +668,37 @@
 
     Examples
     --------
     >>> import datetime
     >>> Date(datetime.date(year=2024, month=1, day=1))
     """
 
+    def __init__(self, value: datetime.date):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, datetime.date):
             raise TypeError(
                 f"Expected type '{datetime.date}' received type '{type(value)}'"
             )
 
     @classmethod
-    def decode_value(cls, value: str):
+    def decode_value(cls, value: typing.Optional[str]):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(value=datetime.date.fromisoformat(value))
 
     def encode_value(self):
         """Encode object to JSON compatible dictionary."""
-        return self.get_value().isoformat()
+        value = self.get_value()
+        if value is None:
+            return None
+        return value.isoformat()
 
 
 class Time(Quantifiable):
     """
     Implementation of the type 'datetime.time' as a Variable.
 
     Parameters
@@ -688,29 +710,37 @@
 
     Examples
     --------
     >>> import datetime
     >>> Time(datetime.time(hour=1, minute=1))
     """
 
+    def __init__(self, value: datetime.time):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, datetime.time):
             raise TypeError(
                 f"Expected type '{datetime.time}' received type '{type(value)}'"
             )
 
     @classmethod
-    def decode_value(cls, value: str):
+    def decode_value(cls, value: typing.Optional[str]):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(value=datetime.time.fromisoformat(value))
 
     def encode_value(self):
         """Encode object to JSON compatible dictionary."""
-        return self.get_value().isoformat()
+        value = self.get_value()
+        if value is None:
+            return None
+        return value.isoformat()
 
 
 class Duration(Quantifiable):
     """
     Implementation of the type 'datetime.timedelta' as a Variable.
 
     Parameters
@@ -722,29 +752,37 @@
 
     Examples
     --------
     >>> import datetime
     >>> Duration(datetime.timedelta(seconds=100))
     """
 
+    def __init__(self, value: datetime.timedelta):
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, datetime.timedelta):
             raise TypeError(
                 f"Expected type '{datetime.timedelta}' received type '{type(value)}'"
             )
 
     @classmethod
-    def decode_value(cls, value: int):
+    def decode_value(cls, value: typing.Optional[int]):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(value=datetime.timedelta(seconds=value))
 
     def encode_value(self):
         """Encode object to JSON compatible dictionary."""
-        return self.get_value().total_seconds()
+        value = self.get_value()
+        if value is None:
+            return None
+        return value.total_seconds()
 
 
 class Point(Spatial, Equatable):
     """
     Represents a point in 2D space.
 
     Follows the GeoJSON specification (RFC 7946).
@@ -759,41 +797,44 @@
     Examples
     --------
     >>> Point((1,2))
     """
 
     def __init__(
         self,
-        value: Optional[Tuple[float, float]] = None,
-        symbol: Optional[Symbol] = None,
+        value: typing.Tuple[float, float],
     ):
-        super().__init__(value=value, symbol=symbol)
+        super().__init__(value=value)
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, tuple):
             raise TypeError(
-                f"Expected type 'Tuple[float, float]' received type '{type(value).__name__}'"
+                f"Expected type 'typing.Tuple[float, float]' received type '{type(value).__name__}'"
             )
         elif len(value) != 2:
             raise ValueError("")
         for item in value:
             if not isinstance(item, (int, float, np.floating)):
                 raise TypeError(
                     f"Expected type '{float.__name__}' received type '{type(item).__name__}'"
                 )
 
     @classmethod
-    def decode_value(cls, value: List[float]):
+    def decode_value(cls, value: typing.Optional[typing.List[float]]):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls((value[0], value[1]))
 
-    def encode_value(self) -> Any:
+    def encode_value(self) -> typing.Any:
         """Encode object to JSON compatible dictionary."""
         value = self.get_value()
+        if value is None:
+            return None
         return (float(value[0]), float(value[1]))
 
     def tuple(self):
         return self.get_value()
 
     def resize(
         self,
@@ -832,31 +873,34 @@
     Examples
     --------
     >>> MultiPoint([(0,0), (0,1), (1,1)])
     """
 
     def __init__(
         self,
-        value: Optional[List[Tuple[float, float]]] = None,
-        symbol: Optional[Symbol] = None,
+        value: typing.List[typing.Tuple[float, float]],
     ):
-        super().__init__(value=value, symbol=symbol)
+        super().__init__(value=value)
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, list):
             raise TypeError(
-                f"Expected 'List[Tuple[float, float]]' received type '{type(value).__name__}'"
+                f"Expected 'typing.List[typing.Tuple[float, float]]' received type '{type(value).__name__}'"
             )
         for point in value:
             Point.__validate__(point)
 
     @classmethod
-    def decode_value(cls, value: List[List[float]]):
+    def decode_value(
+        cls, value: typing.Optional[typing.List[typing.List[float]]]
+    ):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls([(point[0], point[1]) for point in value])
 
 
 class LineString(Spatial):
     """
     Represents a line.
 
@@ -878,32 +922,32 @@
 
     Examples
     --------
     Create a line.
     >>> LineString([(0,0), (0,1), (1,1)])
     """
 
-    def __init__(
-        self,
-        value: Optional[List[Tuple[float, float]]] = None,
-        symbol: Optional[Symbol] = None,
-    ):
-        super().__init__(value=value, symbol=symbol)
+    def __init__(self, value: typing.List[typing.Tuple[float, float]]):
+        super().__init__(value=value)
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         MultiPoint.__validate__(value)
         if len(value) < 2:
             raise ValueError(
                 "At least two points are required to make a line."
             )
 
     @classmethod
-    def decode_value(cls, value: List[List[float]]):
+    def decode_value(
+        cls, value: typing.Optional[typing.List[typing.List[float]]]
+    ):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls([(point[0], point[1]) for point in value])
 
 
 class MultiLineString(Spatial):
     """
     Represents a list of lines.
 
@@ -929,31 +973,35 @@
     ...         [(0.6, 0.6), (0.6, 0.7), (0.7, 0.7)],
     ...     ]
     ... )
     """
 
     def __init__(
         self,
-        value: Optional[List[List[Tuple[float, float]]]] = None,
-        symbol: Optional[Symbol] = None,
+        value: typing.List[typing.List[typing.Tuple[float, float]]],
     ):
-        super().__init__(value=value, symbol=symbol)
+        super().__init__(value=value)
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, list):
             raise TypeError(
                 f"Expected type 'List[List[Tuple[float, float]]]' received type '{type(value).__name__}'"
             )
         for line in value:
             LineString.__validate__(line)
 
     @classmethod
-    def decode_value(cls, value: List[List[List[float]]]):
+    def decode_value(
+        cls,
+        value: typing.Optional[typing.List[typing.List[typing.List[float]]]],
+    ):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(
             [[(point[0], point[1]) for point in line] for line in value]
         )
 
 
 class Polygon(Spatial):
     """
@@ -990,33 +1038,35 @@
     ...         [(0.1, 0.1), (0.1, 0.2), (0.2, 0.2), (0.1, 0.1)],
     ...         [(0.6, 0.6), (0.6, 0.7), (0.7, 0.7), (0.6, 0.6)],
     ...     ]
     ... )
     """
 
     def __init__(
-        self,
-        value: Optional[List[List[Tuple[float, float]]]] = None,
-        symbol: Optional[Symbol] = None,
+        self, value: typing.List[typing.List[typing.Tuple[float, float]]]
     ):
-        super().__init__(value=value, symbol=symbol)
+        super().__init__(value=value)
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         MultiLineString.__validate__(value)
         for line in value:
-            LineString.__validate__(line)
             if not (len(line) >= 4 and line[0] == line[-1]):
                 raise ValueError(
                     "Polygons are defined by at least 4 points with the first point being repeated at the end."
                 )
 
     @classmethod
-    def decode_value(cls, value: List[List[List[float]]]):
+    def decode_value(
+        cls,
+        value: typing.Optional[typing.List[typing.List[typing.List[float]]]],
+    ):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(
             [
                 [(point[0], point[1]) for point in subpolygon]
                 for subpolygon in value
             ]
         )
 
@@ -1031,32 +1081,32 @@
             owner=self._value._owner,
             name=self._value._name,
             key=self._value._key,
             attribute="area",
         )
 
     @property
-    def boundary(self) -> List[Tuple[float, float]]:
+    def boundary(self) -> typing.List[typing.Tuple[float, float]]:
         """
         The boundary of the polygon.
 
         Returns
         -------
         List[Tuple(float, float)]
             A list of points.
         """
         value = self.get_value()
         if value is None:
             raise ValueError("Polygon is 'None'")
         return value[0]
 
     @property
-    def holes(self) -> List[List[Tuple[float, float]]]:
+    def holes(self) -> typing.List[typing.List[typing.Tuple[float, float]]]:
         """
-        Any holes in the polygon.
+        typing.Any holes in the polygon.
 
         Returns
         -------
         List[List[Tuple(float, float)]]
             A list of holes.
         """
         value = self.get_value()
@@ -1105,14 +1155,135 @@
         Returns
         -------
         float
         """
         return max([p[1] for p in self.boundary])
 
 
+class Box(Polygon):
+    """
+    A Box is a polygon that is constrained to 4 unique points.
+
+    Note that this does not need to be axis-aligned.
+
+    Parameters
+    ----------
+    value : List[List[Tuple[float, float]]], optional
+        An polygon value representing a box.
+    symbol : Symbol, optional
+        A symbolic representation.
+
+    Attributes
+    ----------
+    area
+    polygon
+    boundary
+    holes
+    xmin
+    xmax
+    ymin
+    ymax
+
+    Examples
+    --------
+    >>> Box([[(0,0), (0,1), (1,1), (1,0), (0,0)]])
+
+    Create a Box using extrema.
+    >>> Box.from_extrema(
+    ...     xmin=0, xmax=1,
+    ...     ymin=0, ymax=1,
+    ... )
+    """
+
+    def __init__(
+        self, value: typing.List[typing.List[typing.Tuple[float, float]]]
+    ):
+        super().__init__(value=value)
+
+    @classmethod
+    def __validate__(cls, value: typing.Any):
+        """
+        Validates typing.
+
+        Parameters
+        ----------
+        value : typing.Any
+            The value to validate.
+
+        Raises
+        ------
+        TypeError
+            If the value type is not supported.
+        """
+        Polygon.__validate__(value)
+        if len(value) != 1:
+            raise ValueError("Box should not contain holes.")
+        elif len(value[0]) != 5:
+            raise ValueError("Box should consist of four unique points.")
+
+    @classmethod
+    def decode_value(
+        cls,
+        value: typing.Optional[typing.List[typing.List[typing.List[float]]]],
+    ):
+        """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
+        return super().decode_value(value)
+
+    @classmethod
+    def from_extrema(
+        cls,
+        xmin: float,
+        xmax: float,
+        ymin: float,
+        ymax: float,
+    ):
+        """
+        Create a Box from extrema values.
+
+        Parameters
+        ----------
+        xmin : float
+            Minimum x-coordinate of the bounding box.
+        xmax : float
+            Maximum x-coordinate of the bounding box.
+        ymin : float
+            Minimum y-coordinate of the bounding box.
+        ymax : float
+            Maximum y-coordinate of the bounding box.
+
+        Returns
+        -------
+        Box
+            A Box created from the provided extrema values.
+        """
+        points = [
+            [
+                (xmin, ymin),
+                (xmax, ymin),
+                (xmax, ymax),
+                (xmin, ymax),
+                (xmin, ymin),
+            ]
+        ]
+        return cls(value=points)
+
+    def to_polygon(self) -> Polygon:
+        """
+        Converts box to a generic polygon.
+
+        Returns
+        -------
+        Polygon
+            The box as a Polygon.
+        """
+        return Polygon(self.get_value())
+
+
 class MultiPolygon(Spatial):
     """
     Represents a collection of polygons.
 
     Follows the GeoJSON specification (RFC 7946).
 
     Parameters
@@ -1141,31 +1312,39 @@
     ...         ],
     ...     ]
     ... )
     """
 
     def __init__(
         self,
-        value: Optional[List[List[List[Tuple[float, float]]]]] = None,
-        symbol: Optional[Symbol] = None,
+        value: typing.List[
+            typing.List[typing.List[typing.Tuple[float, float]]]
+        ],
     ):
-        super().__init__(value=value, symbol=symbol)
+        super().__init__(value=value)
 
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         if not isinstance(value, list):
             raise TypeError(
                 f"Expected type 'List[List[List[Tuple[float, float]]]]' received type '{type(value).__name__}'"
             )
         for poly in value:
             Polygon.__validate__(poly)
 
     @classmethod
-    def decode_value(cls, value: List[List[List[List[float]]]]):
+    def decode_value(
+        cls,
+        value: typing.Optional[
+            typing.List[typing.List[typing.List[typing.List[float]]]]
+        ],
+    ):
         """Decode object from JSON compatible dictionary."""
+        if value is None:
+            return None
         return cls(
             [
                 [
                     [(point[0], point[1]) for point in subpolygon]
                     for subpolygon in polygon
                 ]
                 for polygon in value
@@ -1184,350 +1363,421 @@
         return Float.symbolic(
             owner=self._value._owner,
             name=self._value._name,
             key=self._value._key,
             attribute="area",
         )
 
-    @property
-    def polygons(self) -> List[Polygon]:
+    def to_polygons(self) -> typing.List[Polygon]:
         """
-        List of the component polygons.
+        Converts multipolygon to a list of Polygon instances.
 
         Returns
         -------
         List[Polygon]
         """
         return [Polygon(poly) for poly in self.get_value()]
 
 
-class Score(Float, Nullable):
+T = typing.TypeVar("T", bound=Variable)
+
+
+class List(typing.Generic[T], Equatable):
     """
-    Implements a score annotation as a nullable floating-point variable.
+    List is both a method of typing and a class-factory.
 
-    Parameters
-    ----------
-    value : float, optional
-        A score value between 0.0 and 1.0.
-    symbol : Symbol, optional
-        A symbolic representation.
+    The '__class_getitem__' classmethod produces strongly-typed VariableLists.
 
     Examples
     --------
-    >>> Score(0.9)
-    >>> Score(None)
+    >>> x = typing.List[String](["foo", "bar"])
     """
 
+    _registered_classes = dict()
+
     @classmethod
-    def __validate__(cls, value: Any):
-        """
-        Validates typing.
+    def __class_getitem__(cls, item_class: typing.Type[T]):
 
-        Parameters
-        ----------
-        value : Any
-            The value to validate.
+        if item_class in cls._registered_classes:
+            return cls._registered_classes[item_class]
 
-        Raises
-        ------
-        TypeError
-            If the value type is not supported.
-        """
-        if value is not None:
-            Float.__validate__(value)
-            if value < 0.0:
-                raise ValueError("score must be non-negative")
-            elif value > 1.0:
-                raise ValueError("score must not exceed 1.0")
+        class VariableList(Equatable):
+            """
+            Strongly-typed variable list.
 
-    @classmethod
-    def decode_value(cls, value: Optional[Union[float, np.floating]]):
-        """Decode object from JSON compatible dictionary."""
-        if value is None:
-            return cls(None)
-        return super().decode_value(value)
+            Parameters
+            ----------
+            value : typing.List[T], optional
+                A list of items with type T.
+            symbol : Symbol, optional
+                A symbolic representation.
+            """
 
+            def __init__(
+                self,
+                value: typing.List[typing.Any],
+            ):
+                if value is not None:
+                    if not isinstance(value, list):
+                        raise TypeError(
+                            f"Expected a value with type 'typing.List[{item_class.__name__}]' but received type '{type(value).__name__}'"
+                        )
+                    vlist = []
+                    for item in value:
+                        if isinstance(item, item_class):
+                            vlist.append(item)
+                        elif isinstance(item, dict) and set(item.keys()) != {
+                            "type",
+                            "value",
+                        }:
+                            vlist.append(item_class(**item))
+                        else:
+                            vlist.append(item_class(item))
+                    value = vlist
+                super().__init__(value=value)
+
+            @classmethod
+            def symbolic(
+                cls,
+                name: typing.Optional[str] = None,
+                key: typing.Optional[str] = None,
+                attribute: typing.Optional[str] = None,
+                owner: typing.Optional[str] = None,
+            ):
+                """Initialize variable as a symbol."""
+                if name is None:
+                    name = f"list[{item_class.__name__.lower()}]"
+                return super().symbolic(name, key, attribute, owner)
+
+            @classmethod
+            def __validate__(cls, value: list):
+                """Validate typing."""
+                if not isinstance(value, list):
+                    raise TypeError(
+                        f"Expected type '{list}' received type '{type(value)}'"
+                    )
+                for element in value:
+                    if not item_class.supports(element) and not issubclass(
+                        type(element), Variable
+                    ):
+                        raise TypeError(
+                            f"Expected list elements with type '{item_class}' received type '{type(element)}'"
+                        )
+
+            @classmethod
+            def decode_value(cls, value: typing.Any):
+                """Decode object from JSON compatible dictionary."""
+                if not value:
+                    return cls(value=[])
+                return cls(
+                    value=[
+                        item_class.decode_value(element) for element in value
+                    ]
+                )
 
-class TaskTypeEnum(String):
-    """
-    Variable wrapper for 'valor.enums.TaskType'.
+            def encode_value(self):
+                """Encode object to JSON compatible dictionary."""
+                value = self.get_value()
+                if value is None:
+                    return list()
+                return [element.encode_value() for element in self.get_value()]
 
-    Parameters
-    ----------
-    value : Union[str, valor.enums.TaskType], optional
-        A task type enum value.
-    symbol : Symbol, optional
-        A symbolic representation.
+            def to_dict(self) -> dict:
+                """Encode variable to a JSON-compatible dictionary."""
+                if isinstance(self._value, Symbol):
+                    return self._value.to_dict()
+                else:
+                    return {
+                        "type": f"list[{item_class.__name__.lower()}]",
+                        "value": self.encode_value(),
+                    }
 
-    Examples
-    --------
-    >>> from valor.enums import TaskType
-    >>> TaskTypeEnum(TaskType.CLASSIFICATION)
-    >>> TaskTypeEnum("classification")
-    """
+            def __getitem__(self, __key: int) -> T:
+                return self.get_value()[__key]
 
-    def __init__(
-        self,
-        value: Optional[Any] = None,
-        symbol: Optional[Symbol] = None,
-    ):
-        if isinstance(value, str):
-            value = TaskType(value)
-        super().__init__(value=value, symbol=symbol)
+            def __setitem__(self, __key: int, __value: typing.Any):
+                vlist = self.get_value()
+                vlist[__key] = item_class.preprocess(__value)
 
-    @classmethod
-    def __validate__(cls, value: Any):
-        """
-        Validates typing.
+            def __iter__(self) -> typing.Iterator[T]:
+                return iter([element for element in self.get_value()])
 
-        Parameters
-        ----------
-        value : Any
-            The value to validate.
+            def __len__(self):
+                return len(self.get_value())
 
-        Raises
-        ------
-        TypeError
-            If the value type is not supported.
-        """
-        if not isinstance(value, TaskType):
-            raise TypeError(
-                f"Expected value with type '{TaskType.__name__}' received type '{type(value).__name__}'"
+            @staticmethod
+            def get_element_type():
+                return item_class
+
+        cls._registered_classes[item_class] = VariableList
+        return VariableList
+
+    def __getitem__(self, __key: int) -> T:
+        raise NotImplementedError
+
+    def __setitem__(self, __key: int, __value: typing.Any):
+        raise NotImplementedError
+
+    def __iter__(self) -> typing.Iterator[T]:
+        raise NotImplementedError
+
+    def __len__(self) -> int:
+        raise NotImplementedError
+
+
+class DictionaryValue(Variable):
+    """Helper class for routing dictionary expressions."""
+
+    def __init__(self, symbol: Symbol):
+        if not isinstance(symbol, Symbol):
+            raise ValueError(
+                "DictionaryValue should only be initialized as a symbol."
             )
+        if symbol._attribute:
+            raise ValueError(
+                "DictionaryValue symbol should not contain attribute."
+            )
+        if not symbol._key:
+            raise ValueError("DictionaryValue symbol should contain key.")
+        super().symbolic(name=symbol._name, owner=symbol._owner)
 
     @classmethod
-    def decode_value(cls, value: str):
-        """Decode object from JSON compatible dictionary."""
-        return cls(TaskType(value))
+    def nullable(cls, value: typing.Any):
+        raise NotImplementedError("Dictionary values cannot be none.")
 
-    def encode_value(self) -> Any:
-        """Encode object to JSON compatible dictionary."""
-        return self.get_value().value
+    def __eq__(self, other: typing.Any):
+        return self._generate(fn="__eq__", other=other)
 
+    def __ne__(self, other: typing.Any):
+        return self._generate(fn="__ne__", other=other)
 
-class BoundingBox(Polygon, Nullable):
-    """
-    Bounding Box Annotation.
+    def __gt__(self, other: typing.Any):
+        return self._generate(fn="__gt__", other=other)
+
+    def __ge__(self, other: typing.Any):
+        return self._generate(fn="__ge__", other=other)
+
+    def __lt__(self, other: typing.Any):
+        return self._generate(fn="__lt__", other=other)
+
+    def __le__(self, other: typing.Any):
+        return self._generate(fn="__le__", other=other)
+
+    def intersects(self, other: typing.Any):
+        return self._generate(fn="intersects", other=other)
+
+    def inside(self, other: typing.Any):
+        return self._generate(fn="inside", other=other)
+
+    def outside(self, other: typing.Any):
+        return self._generate(fn="outside", other=other)
+
+    def is_none(self):
+        return IsNull(self)
+
+    def is_not_none(self):
+        return IsNotNull(self)
+
+    @property
+    def area(self):
+        """Returns area attribute."""
+        symbol = self.get_symbol()
+        return Float.symbolic(
+            owner=symbol._owner,
+            name=symbol._name,
+            key=symbol._key,
+            attribute="area",
+        )
+
+    def _generate(self, other: typing.Any, fn: str):
+        """Generate expression."""
+        if isinstance(other, Variable):
+            obj = type(other)
+        else:
+            obj = _get_type_by_value(other)
+        symbol = self.get_symbol()
+        sym = obj.symbolic(
+            owner=symbol._owner,
+            name=symbol._name,
+            attribute=symbol._attribute,
+            key=symbol._key,
+        )
+        return sym.__getattribute__(fn)(other)
 
-    Implements a nullable polygon with 4 unique points. Note that this does not need to be axis-aligned.
+
+class Dictionary(Equatable, MutableMapping):
+    """
+    Symbolic implementation of the built-in type 'dict'.
 
     Parameters
     ----------
-    value : List[List[Tuple[float, float]]], optional
-        An polygon value representing a box.
+    value : Dict[str, typing.Any], optional
+        A dictionary of items.
     symbol : Symbol, optional
         A symbolic representation.
 
-    Attributes
-    ----------
-    area
-    polygon
-    boundary
-    holes
-    xmin
-    xmax
-    ymin
-    ymax
-
     Examples
     --------
-    >>> BoundingBox([[(0,0), (0,1), (1,1), (1,0), (0,0)]])
+    >>> v = Dictionary({"k1": "v1", "k2": 3.14})
+    >>> s = Dictionary.symbolic(name="some_var")
 
-    Create a BoundingBox using extrema.
-    >>> BoundingBox.from_extrema(
-    ...     xmin=0, xmax=1,
-    ...     ymin=0, ymax=1,
-    ... )
+    # Create an equality expression.
+    >>> s["k1"] == v["k1"]
+    Eq(Symbol(name='some_var', key='k1'), 'v1')
     """
 
-    @classmethod
-    def __validate__(cls, value: Any):
-        """
-        Validates typing.
-
-        Parameters
-        ----------
-        value : Any
-            The value to validate.
-
-        Raises
-        ------
-        TypeError
-            If the value type is not supported.
-        """
-        if value is not None:
-            Polygon.__validate__(value)
-            if len(value) != 1:
-                raise ValueError("Bounding Box should not contain holes.")
-            elif len(value[0]) != 5:
+    def __init__(
+        self,
+        value: typing.Dict[str, typing.Any],
+    ):
+        self.__validate__(value)
+        _value = value.copy()
+        for k, v in value.items():
+            if v is None:
                 raise ValueError(
-                    "Bounding Box should consist of four unique points."
+                    "Dictionary does not accept 'None' as a value."
                 )
+            elif isinstance(v, Variable):
+                if v.is_symbolic:
+                    raise ValueError(
+                        "Dictionary does not accpet symbols as values."
+                    )
+                _value[k] = v
+            else:
+                _value[k] = _get_type_by_value(v)(v)
+        super().__init__(_value)
 
     @classmethod
-    def decode_value(cls, value: Optional[List[List[List[float]]]]):
-        """Decode object from JSON compatible dictionary."""
-        if value is None:
-            return cls(None)
-        return super().decode_value(value)
+    def __validate__(cls, value: typing.Any):
+        """Validate typing."""
+        if not isinstance(value, dict):
+            raise TypeError(
+                f"Expected type '{dict}' received type '{type(value)}'"
+            )
+        for k, v in value.items():
+            if not isinstance(k, str):
+                raise TypeError("Dictionary keys must be of type 'str'")
 
     @classmethod
-    def from_extrema(
-        cls,
-        xmin: float,
-        xmax: float,
-        ymin: float,
-        ymax: float,
-    ):
-        """
-        Create a BoundingBox from extrema values.
-
-        Parameters
-        ----------
-        xmin : float
-            Minimum x-coordinate of the bounding box.
-        xmax : float
-            Maximum x-coordinate of the bounding box.
-        ymin : float
-            Minimum y-coordinate of the bounding box.
-        ymax : float
-            Maximum y-coordinate of the bounding box.
+    def decode_value(cls, value: dict) -> typing.Any:
+        """Decode object from JSON compatible dictionary."""
+        return cls(
+            {
+                k: get_type_by_name(v["type"]).decode_value(v["value"])
+                for k, v in value.items()
+            }
+        )
 
-        Returns
-        -------
-        BoundingBox
-            A BoundingBox created from the provided extrema values.
-        """
-        points = [
-            [
-                (xmin, ymin),
-                (xmax, ymin),
-                (xmax, ymax),
-                (xmin, ymax),
-                (xmin, ymin),
-            ]
-        ]
-        return cls(value=points)
+    def encode_value(self) -> dict:
+        """Encode object to JSON compatible dictionary."""
+        value = self.get_value()
+        if value is None:
+            return dict()
+        return {k: v.to_dict() for k, v in self.items()}
 
-    @property
-    def polygon(self) -> Optional[Polygon]:
-        """
-        The box defined as a 'Polygon'.
+    def __getitem__(self, __key: str):
+        if self.is_symbolic:
+            symbol = self.get_symbol()
+            return DictionaryValue.symbolic(
+                owner=symbol._owner,
+                name=symbol._name,
+                attribute=None,
+                key=__key,
+            )
+        else:
+            value = self.get_value()
+            if not value:
+                raise KeyError(__key)
+            return value[__key]
+
+    def __setitem__(self, __key: str, __value: typing.Any):
+        if not isinstance(__value, Variable):
+            obj = _get_type_by_value(__value)
+            __value = obj(__value)
+        self.get_value()[__key] = __value
 
-        Returns
-        -------
-        Polygon | None
-            The component polygon or 'None' if it doesn't exist.
-        """
+    def __delitem__(self, __key: str) -> None:
         value = self.get_value()
-        return Polygon(value) if value else None
+        if not value:
+            value = dict()
+        return value.__delitem__(__key)
+
+    def __iter__(self) -> Iterator:
+        return self.get_value().__iter__()
+
+    def __len__(self) -> int:
+        return self.get_value().__len__()
 
 
-class BoundingPolygon(Polygon, Nullable):
+class TaskTypeEnum(String):
     """
-    Represents a polygon with a boundary and optional holes.
+    Variable wrapper for 'valor.enums.TaskType'.
 
     Parameters
     ----------
-    value : List[List[Tuple[float, float]]], optional
-        An polygon value.
+    value : typing.Union[str, valor.enums.TaskType], optional
+        A task type enum value.
     symbol : Symbol, optional
         A symbolic representation.
 
-    Attributes
-    ----------
-    area
-    polygon
-    boundary
-    holes
-    xmin
-    xmax
-    ymin
-    ymax
-
-    Raises
-    ------
-    TypeError
-        If `boundary` is not a `BasicPolygon` or cannot be converted to one.
-        If `holes` is not a list, or an element in `holes` is not a `BasicPolygon`.
-
     Examples
     --------
-    Create a polygon.
-    >>> polygon1 = Polygon(
-    ...     value = [[
-    ...         (0, 1),
-    ...         (1, 1),
-    ...         (1, 0),
-    ...         (0, 1),
-    ...     ]],
-    ... )
-
-    Create a polygon with holes.
-    >>> polygon2 = Polygon(
-    ...     value = [[
-    ...         (0, 1),
-    ...         (1, 1),
-    ...         (1, 0),
-    ...         (0, 1),
-    ...     ],[
-    ...         (0, 0.5),
-    ...         (0.5, 0.5),
-    ...         (0.5, 0),
-    ...         (0, 0.5),
-    ...     ]],
-    ... )
+    >>> from valor.enums import TaskType
+    >>> TaskTypeEnum(TaskType.CLASSIFICATION)
+    >>> TaskTypeEnum("classification")
     """
 
+    def __init__(
+        self,
+        value: typing.Union[str, TaskType],
+    ):
+        if isinstance(value, str):
+            value = TaskType(value)
+        super().__init__(value=value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         """
         Validates typing.
 
         Parameters
         ----------
-        value : Any
+        value : typing.Any
             The value to validate.
 
         Raises
         ------
         TypeError
             If the value type is not supported.
         """
-        if value is not None:
-            Polygon.__validate__(value)
+        if not isinstance(value, TaskType):
+            raise TypeError(
+                f"Expected value with type '{TaskType.__name__}' received type '{type(value).__name__}'"
+            )
 
     @classmethod
-    def decode_value(cls, value: Optional[List[List[List[float]]]]):
+    def decode_value(cls, value: str):
         """Decode object from JSON compatible dictionary."""
-        if value is None:
-            return cls(None)
-        return super().decode_value(value)
-
-    @property
-    def polygon(self) -> Optional[Polygon]:
-        """
-        The bounding polygon defined as a 'Polygon'.
+        return cls(TaskType(value))
 
-        Returns
-        -------
-        Polygon | None
-            The component polygon or 'None' if it doesn't exist.
-        """
+    def encode_value(self) -> typing.Any:
+        """Encode object to JSON compatible dictionary."""
         value = self.get_value()
-        return Polygon(value) if value else None
+        if value is None:
+            return None
+        return value.value
 
 
-class Raster(Spatial, Nullable):
+class Raster(Spatial):
     """
     Represents a binary mask.
 
     Parameters
     ----------
-    value : Dict[str, Union[np.ndarray, str, None]], optional
+    value : Dict[str, typing.Union[np.ndarray, str, None]], optional
         An raster value.
     symbol : Symbol, optional
         A symbolic representation.
 
     Parameters
     ----------
     area
@@ -1552,83 +1802,106 @@
     Convert to binary mask.
     >>> mask = (array > 0.5)
 
     Create Raster.
     >>> Raster.from_numpy(mask)
     """
 
+    def __init__(
+        self,
+        value: typing.Dict[
+            str, typing.Union[np.ndarray, Box, Polygon, MultiPolygon, None]
+        ],
+    ):
+        """
+        Initialize and instance of a raster.
+
+        Parameters
+        ----------
+        value : Dict[str, Union[np.ndarray, Box, Polygon, MultiPolygon, None]]
+            The raster in dictionary format {"mask": <np.ndarray>, "geometry": <geometry | None>}.
+        """
+        super().__init__(value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         """
         Validates typing.
 
         Parameters
         ----------
         value : Any
             The value to validate.
 
         Raises
         ------
         TypeError
             If the value type is not supported.
         """
-        if value is not None:
-            if not isinstance(value, dict):
-                raise TypeError(
-                    "Raster should contain a dictionary describing a mask and optionally a geometry."
-                )
-            elif set(value.keys()) != {"mask", "geometry"}:
-                raise ValueError(
-                    "Raster should be described by a dictionary with keys 'mask' and 'geometry'"
-                )
-            elif not isinstance(value["mask"], np.ndarray):
-                raise TypeError(
-                    f"Expected mask to have type '{np.ndarray}' receieved type '{value['mask']}'"
-                )
-            elif len(value["mask"].shape) != 2:
-                raise ValueError("raster only supports 2d arrays")
-            elif value["mask"].dtype != bool:
-                raise ValueError(
-                    f"Expecting a binary mask (i.e. of dtype bool) but got dtype {value['mask'].dtype}"
-                )
-            elif (
-                value["geometry"] is not None
-                and not Polygon.supports(value["geometry"])
-                and not MultiPolygon.supports(value["geometry"])
-            ):
-                raise TypeError(
-                    "Expected geometry to conform to either Polygon or MultiPolygon or be 'None'"
-                )
+        if not isinstance(value, dict):
+            raise TypeError(
+                "Raster should contain a dictionary describing a mask and optionally a geometry."
+            )
+        elif set(value.keys()) != {"mask", "geometry"}:
+            raise ValueError(
+                "Raster should be described by a dictionary with keys 'mask' and 'geometry'"
+            )
+        elif not isinstance(value["mask"], np.ndarray):
+            raise TypeError(
+                f"Expected mask to have type '{np.ndarray}' receieved type '{value['mask']}'"
+            )
+        elif len(value["mask"].shape) != 2:
+            raise ValueError("raster only supports 2d arrays")
+        elif value["mask"].dtype != bool:
+            raise ValueError(
+                f"Expecting a binary mask (i.e. of dtype bool) but got dtype {value['mask'].dtype}"
+            )
+        elif (
+            value["geometry"] is not None
+            and not Polygon.supports(value["geometry"])
+            and not MultiPolygon.supports(value["geometry"])
+        ):
+            raise TypeError(
+                "Expected geometry to conform to either Polygon or MultiPolygon or be 'None'"
+            )
 
-    def encode_value(self) -> Any:
+    def encode_value(self) -> typing.Any:
         """Encode object to JSON compatible dictionary."""
         value = self.get_value()
-        if value is not None:
-            f = io.BytesIO()
-            PIL.Image.fromarray(value["mask"]).save(f, format="PNG")
-            f.seek(0)
-            mask_bytes = f.read()
-            f.close()
-            value = {
-                "mask": b64encode(mask_bytes).decode(),
-                "geometry": value["geometry"],
-            }
-        return value
+        if value is None:
+            return None
+        f = io.BytesIO()
+        PIL.Image.fromarray(value["mask"]).save(f, format="PNG")
+        f.seek(0)
+        mask_bytes = f.read()
+        f.close()
+        return {
+            "mask": b64encode(mask_bytes).decode(),
+            "geometry": value["geometry"],
+        }
 
     @classmethod
-    def decode_value(cls, value: Any):
+    def decode_value(cls, value: typing.Any):
         """Decode object from JSON compatible dictionary."""
-        if value is not None:
-            mask_bytes = b64decode(value["mask"])
-            with io.BytesIO(mask_bytes) as f:
-                img = PIL.Image.open(f)
-                value = {
-                    "mask": np.array(img),
-                    "geometry": value["geometry"],
-                }
+        if value is None:
+            return None
+        if not (
+            isinstance(value, dict)
+            and set(value.keys()) == {"mask", "geometry"}
+        ):
+            raise ValueError(
+                f"Improperly formatted raster encoding. Received '{value}'"
+            )
+        mask_bytes = b64decode(value["mask"])
+        with io.BytesIO(mask_bytes) as f:
+            img = PIL.Image.open(f)
+            value = {
+                "mask": np.array(img),
+                "geometry": value["geometry"],
+            }
         return cls(value=value)
 
     @classmethod
     def from_numpy(cls, mask: np.ndarray):
         """
         Create a Raster object from a NumPy array.
 
@@ -1647,24 +1920,24 @@
             If the input array is not 2D or not of dtype bool.
         """
         return cls(value={"mask": mask, "geometry": None})
 
     @classmethod
     def from_geometry(
         cls,
-        geometry: Union[Polygon, MultiPolygon],
+        geometry: typing.Union[Box, Polygon, MultiPolygon],
         height: int,
         width: int,
     ):
         """
         Create a Raster object from a geometric mask.
 
         Parameters
         ----------
-        geometry : Union[Polygon, MultiPolygon]
+        geometry : Union[Box, Polygon, MultiPolygon]
             Defines the bitmask as a geometry. Overrides any existing mask.
         height : int
             The intended height of the binary mask.
         width : int
             The intended width of the binary mask.
 
         Returns
@@ -1685,103 +1958,192 @@
             owner=self._value._owner,
             name=self._value._name,
             key=self._value._key,
             attribute="area",
         )
 
     @property
-    def array(self) -> Optional[np.ndarray]:
+    def array(self) -> np.ndarray:
         """
         The bitmask as a numpy array.
 
         Returns
         -------
         Optional[np.ndarray]
             A 2D binary array representing the mask if it exists.
         """
         value = self.get_value()
-        if value is not None:
-            if value["geometry"] is not None:
-                warnings.warn(
-                    "array does not hold information as this is a geometry-based raster",
-                    RuntimeWarning,
-                )
-            return value["mask"]
-        warnings.warn("raster has no value", RuntimeWarning)
-        return None
+        if value["geometry"] is not None:
+            warnings.warn(
+                "Raster array does not contain bitmask as this is a geometry-defined raster.",
+                RuntimeWarning,
+            )
+        return value["mask"]
 
     @property
-    def geometry(self) -> Optional[Union[Polygon, MultiPolygon]]:
+    def geometry(self) -> typing.Union[Box, Polygon, MultiPolygon]:
         """
         The geometric mask if it exists.
 
         Returns
         -------
-        Polygon | MultiPolygon | None
+        Box | Polygon | MultiPolygon | None
             The geometry if it exists.
         """
-        value = self.get_value()
-        if value is not None:
-            return value["geometry"]
-        warnings.warn("raster has no value", RuntimeWarning)
-        return None
+        return self.get_value()["geometry"]
 
     @property
-    def height(self) -> Optional[int]:
+    def height(self) -> int:
         """Returns the height of the raster if it exists."""
-        array = self.array
-        if array is not None:
-            return array.shape[0]
-        return None
+        return self.array.shape[0]
 
     @property
-    def width(self) -> Optional[int]:
+    def width(self) -> int:
         """Returns the width of the raster if it exists."""
-        array = self.array
-        if array is not None:
-            return array.shape[1]
-        return None
+        return self.array.shape[1]
 
 
-class Embedding(Spatial, Nullable):
+class Embedding(Spatial):
     """
     Represents a model embedding.
 
     Parameters
     ----------
     value : List[float], optional
         An embedding value.
     symbol : Symbol, optional
         A symbolic representation.
     """
 
+    def __init__(
+        self, value: typing.Union[typing.List[int], typing.List[float]]
+    ):
+        """
+        Initializes an embedding.
+
+        Parameters
+        ----------
+        value : List[float]
+            A list of floating point numbers representing the embedding.
+        """
+        super().__init__(value)
+
     @classmethod
-    def __validate__(cls, value: Any):
+    def __validate__(cls, value: typing.Any):
         """
         Validates typing.
 
         Parameters
         ----------
         value : Any
             The value to validate.
 
         Raises
         ------
         TypeError
             If the value type is not supported.
         """
-        if value is not None:
-            if not isinstance(value, list):
-                raise TypeError(
-                    f"Expected type '{Optional[typing.List[float]]}' received type '{type(value)}'"
-                )
-            elif len(value) < 1:
-                raise ValueError(
-                    "embedding should have at least one dimension"
-                )
+        if not isinstance(value, list):
+            raise TypeError(
+                f"Expected type 'Optional[List[float]]' received type '{type(value)}'"
+            )
+        elif len(value) < 1:
+            raise ValueError("embedding should have at least one dimension")
 
     @classmethod
-    def decode_value(cls, value: Optional[List[float]]):
+    def decode_value(
+        cls, value: typing.Optional[typing.List[typing.Union[float, int]]]
+    ):
         """Decode object from JSON compatible dictionary."""
         if value is None:
-            return cls(None)
+            return None
         return super().decode_value(value)
+
+
+def _get_type_by_value(other: typing.Any):
+    """
+    Retrieves variable type using built-in type.
+
+    Order of checking is very important as certain types are subsets of others.
+    """
+    if Bool.supports(other):
+        return Bool
+    elif String.supports(other):
+        return String
+    elif Integer.supports(other):
+        return Integer
+    elif Float.supports(other):
+        return Float
+    elif DateTime.supports(other):
+        return DateTime
+    elif Date.supports(other):
+        return Date
+    elif Time.supports(other):
+        return Time
+    elif Duration.supports(other):
+        return Duration
+    elif MultiPolygon.supports(other):
+        return MultiPolygon
+    elif Polygon.supports(other):
+        return Polygon
+    elif Box.supports(other):
+        return Box
+    elif MultiLineString.supports(other):
+        return MultiLineString
+    elif LineString.supports(other):
+        return LineString
+    elif MultiPoint.supports(other):
+        return MultiPoint
+    elif Point.supports(other):
+        return Point
+    elif Raster.supports(other):
+        return Raster
+    elif Embedding.supports(other):
+        return Embedding
+    elif Dictionary.supports(other):
+        return Dictionary
+    else:
+        raise NotImplementedError(str(type(other).__name__))
+
+
+def get_type_by_name(
+    name: str, additional_types: typing.Optional[typing.Dict[str, type]] = None
+):
+    """Retrieves variable type by name."""
+    types_ = {
+        "bool": Bool,
+        "string": String,
+        "integer": Integer,
+        "float": Float,
+        "datetime": DateTime,
+        "date": Date,
+        "time": Time,
+        "duration": Duration,
+        "multipolygon": MultiPolygon,
+        "polygon": Polygon,
+        "multilinestring": MultiLineString,
+        "linestring": LineString,
+        "multipoint": MultiPoint,
+        "point": Point,
+        "raster": Raster,
+        "embedding": Embedding,
+        "dictionary": Dictionary,
+    }
+    if additional_types:
+        types_.update(additional_types)
+
+    parsed_name = name.lower().split(".")[-1]
+    type_ = types_.get(parsed_name, None)
+    if type_ is not None:
+        return type_
+
+    match = re.search(r"\[(.*?)\]", name.lower())
+    if not match:
+        raise NotImplementedError(name)
+
+    type_ = get_type_by_name(
+        name=match.group(1), additional_types=additional_types
+    )
+    if "list" in name.lower():
+        return List[type_]
+    else:
+        raise NotImplementedError(name)
```

### Comparing `valor-client-0.20.1/valor/type_checks.py` & `valor-client-0.20.2/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.20.1/valor/viz.py` & `valor-client-0.20.2/valor/viz.py`

 * *Files 18% similar despite different names*

```diff
@@ -90,23 +90,24 @@
     if len(annotated_datum.annotations) == 0:
         raise ValueError("annotations cannot be empty.")
 
     # validate raster size
     img_h = None
     img_w = None
     for annotation in annotated_datum.annotations:
+        raster = annotation.raster
+        if raster.get_value() is None:
+            raise ValueError("No raster exists.")
         if img_h is None:
-            img_h = annotation.raster.height
+            img_h = raster.height
         if img_w is None:
-            img_w = annotation.raster.width
-        if (img_h != annotation.raster.height) or (
-            img_w != annotation.raster.width
-        ):
+            img_w = raster.width
+        if (img_h != raster.height) or (img_w != raster.width):
             raise ValueError(
-                f"Size mismatch between rasters. {(img_h, img_w)} != {(annotation.raster.height, annotation.raster.width)}"
+                f"Size mismatch between rasters. {(img_h, img_w)} != {(raster.height, raster.width)}"
             )
     if img_h is None or img_w is None:
         raise ValueError(
             f"Segmentation bounds not properly defined. {(img_h, img_w)}"
         )
 
     # validate task type
@@ -150,26 +151,29 @@
         v: COLOR_MAP[i] for i, v in enumerate(unique_label_values)
     }
     seg_colors = [label_value_to_color[v] for v in label_values]
 
     # create mask
     combined_mask = np.zeros((img_h, img_w, 3), dtype=np.uint8)
     for annotation, color in zip(annotations, seg_colors):
-        if annotation.raster.array is not None:
-            if annotation.raster.geometry is None:
-                mask = annotation.raster.array
-            elif isinstance(annotation.raster.geometry, schemas.MultiPolygon):
+        raster = annotation.raster
+        if raster.get_value() is None:
+            raise ValueError("No raster exists.")
+        if raster.array is not None:
+            if raster.geometry is None:
+                mask = raster.array
+            elif isinstance(raster.geometry, schemas.MultiPolygon):
                 mask = _polygons_to_binary_mask(
-                    annotation.raster.geometry.polygons,
+                    raster.geometry.to_polygons(),
                     img_w=img_w,
                     img_h=img_h,
                 )
-            elif isinstance(annotation.raster.geometry, schemas.Polygon):
+            elif isinstance(raster.geometry, (schemas.Box, schemas.Polygon)):
                 mask = _polygons_to_binary_mask(
-                    [annotation.raster.geometry],
+                    [raster.geometry],
                     img_w=img_w,
                     img_h=img_h,
                 )
             else:
                 continue
             combined_mask[np.where(mask)] = color
         else:
@@ -211,15 +215,15 @@
     for i, detection in enumerate(annotations):
         if detection.task_type in [enums.TaskType.OBJECT_DETECTION]:
             img = _draw_detection_on_image(detection, img, inplace=i != 0)
     return img
 
 
 def draw_bounding_box_on_image(
-    bounding_box: schemas.BoundingBox,
+    bounding_box: schemas.Box,
     img: Image.Image,
     color: Tuple[int, int, int] = (255, 0, 0),
 ) -> Image.Image:
     """Draws a bounding polygon on an image. This operation is not done in place.
 
     Parameters
     ----------
@@ -246,24 +250,26 @@
 def _draw_detection_on_image(
     detection: Annotation, img: Image.Image, inplace: bool
 ) -> Image.Image:
     """Draw a detection on an image."""
     text = ", ".join(
         [f"{label.key}:{label.value}" for label in detection.labels]
     )
-    if detection.polygon is not None:
+    box = detection.bounding_box
+    polygon = detection.polygon
+    if polygon.get_value() is not None:
         img = _draw_bounding_polygon_on_image(
-            detection.polygon,
+            polygon,
             img,
             inplace=inplace,
             text=text,
         )
-    elif detection.bounding_box is not None:
+    elif box.get_value() is not None:
         img = _draw_bounding_polygon_on_image(
-            detection.bounding_box,
+            box,
             img,
             inplace=inplace,
             text=text,
         )
 
     return img
```

### Comparing `valor-client-0.20.1/valor_client.egg-info/PKG-INFO` & `valor-client-0.20.2/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.20.1
+Version: 0.20.2
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor-client-0.20.1/valor_client.egg-info/SOURCES.txt` & `valor-client-0.20.2/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

