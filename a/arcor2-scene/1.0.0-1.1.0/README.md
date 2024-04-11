# Comparing `tmp/arcor2_scene-1.0.0.tar.gz` & `tmp/arcor2_scene-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_scene-1.0.0.tar", last modified: Tue Feb 14 12:55:50 2023, max compression
+gzip compressed data, was "arcor2_scene-1.1.0.tar", last modified: Thu Apr 11 09:47:28 2024, max compression
```

## Comparing `arcor2_scene-1.0.0.tar` & `arcor2_scene-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.043362 arcor2_scene-1.0.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     1837 2023-02-14 12:55:50.043362 arcor2_scene-1.0.0/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.043362 arcor2_scene-1.0.0/arcor2_scene/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/arcor2_scene/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      215 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/arcor2_scene/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      437 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/arcor2_scene/exceptions.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/arcor2_scene/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.043362 arcor2_scene-1.0.0/arcor2_scene/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/arcor2_scene/scripts/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    16963 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/arcor2_scene/scripts/scene.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.043362 arcor2_scene-1.0.0/arcor2_scene.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     1837 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      457 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       65 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      111 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       13 2023-02-14 12:55:50.000000 arcor2_scene-1.0.0/arcor2_scene.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      698 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-02-14 12:55:50.043362 arcor2_scene-1.0.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2664 2023-02-14 12:55:49.000000 arcor2_scene-1.0.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.449385 arcor2_scene-1.1.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     1925 2024-04-11 09:47:28.449385 arcor2_scene-1.1.0/PKG-INFO
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.441386 arcor2_scene-1.1.0/arcor2_scene/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/arcor2_scene/VERSION
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      215 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/arcor2_scene/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      437 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/arcor2_scene/exceptions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/arcor2_scene/py.typed
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.445386 arcor2_scene-1.1.0/arcor2_scene/scripts/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/arcor2_scene/scripts/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    16959 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/arcor2_scene/scripts/scene.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:28.445386 arcor2_scene-1.1.0/arcor2_scene.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     1925 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      457 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       65 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      111 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       13 2024-04-11 09:47:28.000000 arcor2_scene-1.1.0/arcor2_scene.egg-info/top_level.txt
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/backend_shim.py
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-11 09:47:28.449385 arcor2_scene-1.1.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2752 2024-04-11 09:47:27.000000 arcor2_scene-1.1.0/setup.py
```

### Comparing `arcor2_scene-1.0.0/PKG-INFO` & `arcor2_scene-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: arcor2_scene
-Version: 1.0.0
+Version: 1.1.0
 Summary: ARCOR2 Scene Service
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.10.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2_scene
 
 ARCOR2 Scene service has similar functionality to Kinali's Scene service (in version 0.8.0), but not all endpoints are implemented, and on the other hand, there are some additional, specific ones.
 
 ## Environment variables
@@ -27,14 +27,20 @@
 - `ARCOR2_SCENE_DEBUG=1` - turns on debug logging.
 - `ARCOR2_SCENE_INFLATION=0.01` - controls how much in meters are collision models inflated (for simple collision checking).
 - `ARCOR2_SCENE_DELAY_MEAN=0` and `ARCOR2_SCENE_DELAY_SIGMA=0` can be used to simulate long-lasting startup of the scene (with some randomness). May be useful for debugging.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 - Health check end-point changed to `/healthz/ready`.
```

### Comparing `arcor2_scene-1.0.0/arcor2_scene/scripts/scene.py` & `arcor2_scene-1.1.0/arcor2_scene/scripts/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 app = create_app(__name__)
 logger = get_logger(__name__)
 logger.propagate = False
 
 
 class CollisionObject(NamedTuple):
-
     model: object_type.Models
     pose: common.Pose
 
 
 collision_objects: dict[str, CollisionObject] = {}
 started: bool = False
 inflation = 0.01
@@ -417,17 +416,15 @@
     o3d uses different coordinates, but in this case it should not matter
 
     o3d        x right,   y down, z forward
     arcor2/ros x forward, y left, z up
     unity      x Right,   y Up,   z Forward
     """
     for obj_id, (model, pose) in collision_objects.items():
-
         if isinstance(model, object_type.Box):
-
             # The left bottom corner on the front will be placed at (0, 0, 0)
             sx = model.size_x + inflation
             sy = model.size_y + inflation
             sz = model.size_z + inflation
 
             tm = o3d.geometry.TriangleMesh.create_box(sx, sy, sz)
 
@@ -545,15 +542,14 @@
                     $ref: WebApiError
     """
 
     return jsonify(started)
 
 
 def main() -> None:
-
     global inflation
 
     parser = argparse.ArgumentParser(description=SCENE_SERVICE_NAME)
     parser.add_argument("-s", "--swagger", action="store_true", default=False)
 
     parser.add_argument(
         "-d",
```

### Comparing `arcor2_scene-1.0.0/arcor2_scene.egg-info/PKG-INFO` & `arcor2_scene-1.1.0/arcor2_scene.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: arcor2-scene
-Version: 1.0.0
+Version: 1.1.0
 Summary: ARCOR2 Scene Service
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.10.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2_scene
 
 ARCOR2 Scene service has similar functionality to Kinali's Scene service (in version 0.8.0), but not all endpoints are implemented, and on the other hand, there are some additional, specific ones.
 
 ## Environment variables
@@ -27,14 +27,20 @@
 - `ARCOR2_SCENE_DEBUG=1` - turns on debug logging.
 - `ARCOR2_SCENE_INFLATION=0.01` - controls how much in meters are collision models inflated (for simple collision checking).
 - `ARCOR2_SCENE_DELAY_MEAN=0` and `ARCOR2_SCENE_DELAY_SIGMA=0` can be used to simulate long-lasting startup of the scene (with some randomness). May be useful for debugging.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 - Health check end-point changed to `/healthz/ready`.
```

### Comparing `arcor2_scene-1.0.0/setup.py` & `arcor2_scene-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     'author': 'Robo@FIT',
     'author_email': 'imaterna@fit.vut.cz',
     'classifiers': [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering',
     ],
     'description': 'ARCOR2 Scene Service',
     'entry_points': {
         'console_scripts': [
             'arcor2_scene = arcor2_scene.scripts.scene:main',
         ],
     },
     'install_requires': (
-        'Flask~=2.2.2',
-        'arcor2~=1.0.0',
-        'numpy-quaternion[numba,scipy]~=2022.4.2',
-        'numpy~=1.23.5',
-        'open3d==0.16.0',
+        'Flask~=3.0.2',
+        'arcor2~=1.3.0',
+        'numpy-quaternion[numba,scipy]~=2023.0.3',
+        'numpy~=1.26.4',
+        'open3d==0.18.0',
         'pyhumps==3.8.0',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_scene
 
 ARCOR2 Scene service has similar functionality to Kinali's Scene service (in version 0.8.0), but not all endpoints are implemented, and on the other hand, there are some additional, specific ones.
 
@@ -43,14 +43,20 @@
 - `ARCOR2_SCENE_DEBUG=1` - turns on debug logging.
 - `ARCOR2_SCENE_INFLATION=0.01` - controls how much in meters are collision models inflated (for simple collision checking).
 - `ARCOR2_SCENE_DELAY_MEAN=0` and `ARCOR2_SCENE_DELAY_SIGMA=0` can be used to simulate long-lasting startup of the scene (with some randomness). May be useful for debugging.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 - Health check end-point changed to `/healthz/ready`.
 
@@ -81,10 +87,10 @@
             'py.typed',
         ),
     },
     'packages': (
         'arcor2_scene',
         'arcor2_scene.scripts',
     ),
-    'python_requires': '==3.10.*',
-    'version': '1.0.0',
+    'python_requires': '==3.11.*',
+    'version': '1.1.0',
 })
```

