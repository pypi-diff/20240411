# Comparing `tmp/obpcreator-0.0.8.tar.gz` & `tmp/obpcreator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obpcreator-0.0.8.tar", last modified: Fri Feb  2 08:51:19 2024, max compression
+gzip compressed data, was "obpcreator-0.0.9.tar", last modified: Fri Feb  2 13:25:20 2024, max compression
```

## Comparing `obpcreator-0.0.8.tar` & `obpcreator-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-02-02 08:51:19.724094 obpcreator-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpcreator-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3646 2024-02-02 08:51:19.722101 obpcreator-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2024-02-02 08:47:51.000000 obpcreator-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-02 08:51:19.673557 obpcreator-0.0.8/obpcreator/
--rw-rw-rw-   0        0        0        0 2024-02-01 14:31:14.000000 obpcreator-0.0.8/obpcreator/__init__.py
--rw-rw-rw-   0        0        0     6257 2024-02-01 11:25:22.000000 obpcreator-0.0.8/obpcreator/data_model.py
--rw-rw-rw-   0        0        0     1297 2023-11-27 10:40:53.000000 obpcreator-0.0.8/obpcreator/generate_BSE_scan_pattern.py
--rw-rw-rw-   0        0        0     5938 2024-02-01 21:02:36.000000 obpcreator-0.0.8/obpcreator/generate_build.py
--rw-rw-rw-   0        0        0     4617 2024-01-23 08:19:44.000000 obpcreator-0.0.8/obpcreator/point_infill_creation.py
-drwxrwxrwx   0        0        0        0 2024-02-02 08:51:19.710995 obpcreator-0.0.8/obpcreator/scanning_strategies/
--rw-rw-rw-   0        0        0        0 2023-11-08 09:54:03.000000 obpcreator-0.0.8/obpcreator/scanning_strategies/__init__.py
--rw-rw-rw-   0        0        0     2574 2024-02-01 21:25:42.000000 obpcreator-0.0.8/obpcreator/scanning_strategies/contour_strategies.py
--rw-rw-rw-   0        0        0    10401 2024-02-01 21:25:39.000000 obpcreator-0.0.8/obpcreator/scanning_strategies/infill_strategies.py
--rw-rw-rw-   0        0        0     5226 2024-02-02 08:49:30.000000 obpcreator-0.0.8/obpcreator/simple_input.py
-drwxrwxrwx   0        0        0        0 2024-02-02 08:51:19.713526 obpcreator-0.0.8/obpcreator/support_functions/
--rw-rw-rw-   0        0        0        0 2023-10-05 13:27:36.000000 obpcreator-0.0.8/obpcreator/support_functions/__init__.py
--rw-rw-rw-   0        0        0      518 2024-01-17 15:08:05.000000 obpcreator-0.0.8/obpcreator/support_functions/pv_mesh_manipulation.py
-drwxrwxrwx   0        0        0        0 2024-02-02 08:51:19.719101 obpcreator-0.0.8/obpcreator/visualisation/
--rw-rw-rw-   0        0        0        0 2023-10-05 13:27:36.000000 obpcreator-0.0.8/obpcreator/visualisation/__init__.py
--rw-rw-rw-   0        0        0      730 2024-01-31 15:45:33.000000 obpcreator-0.0.8/obpcreator/visualisation/layer_vis.py
--rw-rw-rw-   0        0        0     1327 2024-01-25 19:52:25.000000 obpcreator-0.0.8/obpcreator/visualisation/pv_mesh_vis.py
-drwxrwxrwx   0        0        0        0 2024-02-02 08:51:19.721093 obpcreator-0.0.8/obpcreator.egg-info/
--rw-rw-rw-   0        0        0     3646 2024-02-02 08:51:19.000000 obpcreator-0.0.8/obpcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      738 2024-02-02 08:51:19.000000 obpcreator-0.0.8/obpcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-02 08:51:19.000000 obpcreator-0.0.8/obpcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-02-02 08:51:19.000000 obpcreator-0.0.8/obpcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-02 08:51:19.000000 obpcreator-0.0.8/obpcreator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      764 2024-02-02 08:47:47.000000 obpcreator-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-02 08:51:19.724094 obpcreator-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-02 13:25:20.468847 obpcreator-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpcreator-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3646 2024-02-02 13:25:20.468343 obpcreator-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1703 2024-02-02 08:47:51.000000 obpcreator-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-02 13:25:20.410916 obpcreator-0.0.9/obpcreator/
+-rw-rw-rw-   0        0        0        0 2024-02-01 14:31:14.000000 obpcreator-0.0.9/obpcreator/__init__.py
+-rw-rw-rw-   0        0        0     6257 2024-02-01 11:25:22.000000 obpcreator-0.0.9/obpcreator/data_model.py
+-rw-rw-rw-   0        0        0     1297 2023-11-27 10:40:53.000000 obpcreator-0.0.9/obpcreator/generate_BSE_scan_pattern.py
+-rw-rw-rw-   0        0        0     6045 2024-02-02 13:22:31.000000 obpcreator-0.0.9/obpcreator/generate_build.py
+-rw-rw-rw-   0        0        0     4617 2024-01-23 08:19:44.000000 obpcreator-0.0.9/obpcreator/point_infill_creation.py
+drwxrwxrwx   0        0        0        0 2024-02-02 13:25:20.444580 obpcreator-0.0.9/obpcreator/scanning_strategies/
+-rw-rw-rw-   0        0        0        0 2023-11-08 09:54:03.000000 obpcreator-0.0.9/obpcreator/scanning_strategies/__init__.py
+-rw-rw-rw-   0        0        0     2574 2024-02-01 21:25:42.000000 obpcreator-0.0.9/obpcreator/scanning_strategies/contour_strategies.py
+-rw-rw-rw-   0        0        0    10401 2024-02-01 21:25:39.000000 obpcreator-0.0.9/obpcreator/scanning_strategies/infill_strategies.py
+-rw-rw-rw-   0        0        0     5226 2024-02-02 08:49:30.000000 obpcreator-0.0.9/obpcreator/simple_input.py
+drwxrwxrwx   0        0        0        0 2024-02-02 13:25:20.457649 obpcreator-0.0.9/obpcreator/support_functions/
+-rw-rw-rw-   0        0        0        0 2023-10-05 13:27:36.000000 obpcreator-0.0.9/obpcreator/support_functions/__init__.py
+-rw-rw-rw-   0        0        0      518 2024-01-17 15:08:05.000000 obpcreator-0.0.9/obpcreator/support_functions/pv_mesh_manipulation.py
+drwxrwxrwx   0        0        0        0 2024-02-02 13:25:20.464148 obpcreator-0.0.9/obpcreator/visualisation/
+-rw-rw-rw-   0        0        0        0 2023-10-05 13:27:36.000000 obpcreator-0.0.9/obpcreator/visualisation/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-01-31 15:45:33.000000 obpcreator-0.0.9/obpcreator/visualisation/layer_vis.py
+-rw-rw-rw-   0        0        0     1327 2024-01-25 19:52:25.000000 obpcreator-0.0.9/obpcreator/visualisation/pv_mesh_vis.py
+drwxrwxrwx   0        0        0        0 2024-02-02 13:25:20.466770 obpcreator-0.0.9/obpcreator.egg-info/
+-rw-rw-rw-   0        0        0     3646 2024-02-02 13:25:20.000000 obpcreator-0.0.9/obpcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2024-02-02 13:25:20.000000 obpcreator-0.0.9/obpcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-02 13:25:20.000000 obpcreator-0.0.9/obpcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2024-02-02 13:25:20.000000 obpcreator-0.0.9/obpcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-02-02 13:25:20.000000 obpcreator-0.0.9/obpcreator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      764 2024-02-02 13:24:05.000000 obpcreator-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-02 13:25:20.468847 obpcreator-0.0.9/setup.cfg
```

### Comparing `obpcreator-0.0.8/LICENSE` & `obpcreator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/PKG-INFO` & `obpcreator-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpcreator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generation of open beam path files based on different strategies
 Author-email: Anton Wiberg <wiberg.anton@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `obpcreator-0.0.8/README.md` & `obpcreator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/data_model.py` & `obpcreator-0.0.9/obpcreator/data_model.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/generate_BSE_scan_pattern.py` & `obpcreator-0.0.9/obpcreator/generate_BSE_scan_pattern.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/generate_build.py` & `obpcreator-0.0.9/obpcreator/generate_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,30 +88,34 @@
     lines_to_write.append(f"    triggered_start: {build.layerfeed.triggered_start}")
     lines_with_newlines = [line + '\n' for line in lines_to_write]
     f = open(path, "w")
     f.writelines(lines_with_newlines)
     f.close()
 
 def generate_contour(part, layer):
+    if part.contour_setting.scan_strategy == "":
+        return []
     strategy_func = getattr(contour_strategies, part.contour_setting.scan_strategy, None)
     if strategy_func:
         return strategy_func(part, layer)
         #return strategy_func(paths, scan_settings)
     else:
         print(f"No function named {part.contour_setting.scan_strategy} exists")
+        return []
 
 def generate_infill(part, layer):
     if part.infill_setting.scan_strategy == "":
         return []
     strategy_func = getattr(infill_strategies, part.infill_setting.scan_strategy, None)
     if strategy_func:
         return strategy_func(part, layer)
         #return strategy_func(point_infill, scan_settings)
     else:
         print(f"No function named {part.infill_setting.scan_strategy,} exists")
+        return []
 
 def get_max_layers(build):
     max_layers = 0
     for part in build.parts:
         layers = part.point_geometry.keep_matrix.shape[2]
         max_layers = max(max_layers,layers)
     return max_layers
```

### Comparing `obpcreator-0.0.8/obpcreator/point_infill_creation.py` & `obpcreator-0.0.9/obpcreator/point_infill_creation.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/scanning_strategies/contour_strategies.py` & `obpcreator-0.0.9/obpcreator/scanning_strategies/contour_strategies.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/scanning_strategies/infill_strategies.py` & `obpcreator-0.0.9/obpcreator/scanning_strategies/infill_strategies.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/simple_input.py` & `obpcreator-0.0.9/obpcreator/simple_input.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/support_functions/pv_mesh_manipulation.py` & `obpcreator-0.0.9/obpcreator/support_functions/pv_mesh_manipulation.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/visualisation/layer_vis.py` & `obpcreator-0.0.9/obpcreator/visualisation/layer_vis.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator/visualisation/pv_mesh_vis.py` & `obpcreator-0.0.9/obpcreator/visualisation/pv_mesh_vis.py`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/obpcreator.egg-info/PKG-INFO` & `obpcreator-0.0.9/obpcreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpcreator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generation of open beam path files based on different strategies
 Author-email: Anton Wiberg <wiberg.anton@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `obpcreator-0.0.8/obpcreator.egg-info/SOURCES.txt` & `obpcreator-0.0.9/obpcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obpcreator-0.0.8/pyproject.toml` & `obpcreator-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "obpcreator"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Anton Wiberg", email = "wiberg.anton@gmail.com" }
 ]
 description = "Generation of open beam path files based on different strategies"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
```

