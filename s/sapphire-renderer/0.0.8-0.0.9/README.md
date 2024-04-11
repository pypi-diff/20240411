# Comparing `tmp/sapphire-renderer-0.0.8.tar.gz` & `tmp/sapphire-renderer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapphire-renderer-0.0.8.tar", last modified: Tue Mar 19 02:58:22 2024, max compression
+gzip compressed data, was "sapphire-renderer-0.0.9.tar", last modified: Tue Mar 19 03:03:03 2024, max compression
```

## Comparing `sapphire-renderer-0.0.8.tar` & `sapphire-renderer-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.689768 sapphire-renderer-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 02:58:22.689768 sapphire-renderer-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-19 02:58:22.000000 sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-19 02:58:22.000000 sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 02:58:22.000000 sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-19 02:58:22.000000 sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/sapphirerenderer/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/sapphirerenderer/object_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/object_classes/base_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/object_classes/vert_line_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/stl_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/objects/torus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/sapphirerenderer/point_math/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/point_math/matricies.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/point_math/project_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:58:22.685768 sapphire-renderer-0.0.8/src/sapphirerenderer/utility_objects/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-19 02:58:18.000000 sapphire-renderer-0.0.8/src/sapphirerenderer/utility_objects/camera.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.260582 sapphire-renderer-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-19 03:03:03.000000 sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-19 03:03:03.000000 sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 03:03:03.000000 sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-19 03:03:03.000000 sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/src/sapphirerenderer/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/src/sapphirerenderer/object_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/object_classes/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/object_classes/vert_line_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/stl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/objects/torus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/src/sapphirerenderer/point_math/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/point_math/matricies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/point_math/project_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 03:03:03.264582 sapphire-renderer-0.0.9/src/sapphirerenderer/utility_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-19 03:02:57.000000 sapphire-renderer-0.0.9/src/sapphirerenderer/utility_objects/camera.py
```

### Comparing `sapphire-renderer-0.0.8/PKG-INFO` & `sapphire-renderer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire-renderer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to easely render simple 3d scenes
 Author-email: Dark_Eden <darkedenc9@gmail.com>
 Project-URL: Homepage, https://github.com/DarkEden-coding/Sapphire-Renderer
 Project-URL: Bug Tracker, https://github.com/DarkEden-coding/Sapphire-Renderer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sapphire-renderer-0.0.8/pyproject.toml` & `sapphire-renderer-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sapphire-renderer"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Dark_Eden", email="darkedenc9@gmail.com" },
 ]
 description = "A package to easely render simple 3d scenes"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/PKG-INFO` & `sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire-renderer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to easely render simple 3d scenes
 Author-email: Dark_Eden <darkedenc9@gmail.com>
 Project-URL: Homepage, https://github.com/DarkEden-coding/Sapphire-Renderer
 Project-URL: Bug Tracker, https://github.com/DarkEden-coding/Sapphire-Renderer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sapphire-renderer-0.0.8/src/sapphire_renderer.egg-info/SOURCES.txt` & `sapphire-renderer-0.0.9/src/sapphire_renderer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/main.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/main.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/object_classes/base_object.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/object_classes/base_object.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/object_classes/vert_line_object.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/object_classes/vert_line_object.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/axes.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/axes.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/cube.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/cube.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/line.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/line.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/pyramid.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/pyramid.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/sphere.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/sphere.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/stl_.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/stl_.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/objects/torus.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/objects/torus.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/point_math/matricies.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/point_math/matricies.py`

 * *Files identical despite different names*

### Comparing `sapphire-renderer-0.0.8/src/sapphirerenderer/utility_objects/camera.py` & `sapphire-renderer-0.0.9/src/sapphirerenderer/utility_objects/camera.py`

 * *Files identical despite different names*

