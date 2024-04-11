# Comparing `tmp/skanym-0.0.3.tar.gz` & `tmp/skanym-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skanym-0.0.3.tar", last modified: Thu Nov  9 14:04:53 2023, max compression
+gzip compressed data, was "skanym-0.1.0.tar", last modified: Thu Apr 11 09:18:07 2024, max compression
```

## Comparing `skanym-0.0.3.tar` & `skanym-0.1.0.tar`

### file list

```diff
@@ -1,64 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:53.008139 skanym-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-11-07 12:29:13.000000 skanym-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2756 2023-11-09 14:04:53.006133 skanym-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-10-25 14:14:50.000000 skanym-0.0.3/README.md
--rw-rw-rw-   0        0        0     1077 2023-11-09 13:48:58.000000 skanym-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-09 14:04:53.008139 skanym-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.621340 skanym-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.631595 skanym-0.0.3/src/skanym/
--rw-rw-rw-   0        0        0       87 2023-11-08 13:10:28.000000 skanym-0.0.3/src/skanym/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.664133 skanym-0.0.3/src/skanym/algo/
--rw-rw-rw-   0        0        0       53 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/algo/__init__.py
--rw-rw-rw-   0        0        0     7173 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/algo/motionblending.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.666123 skanym-0.0.3/src/skanym/core/
--rw-rw-rw-   0        0        0       32 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.701604 skanym-0.0.3/src/skanym/core/animate/
--rw-rw-rw-   0        0        0      231 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/__init__.py
--rw-rw-rw-   0        0        0     3226 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/animation.py
--rw-rw-rw-   0        0        0    20645 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/animator.py
--rw-rw-rw-   0        0        0    18953 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/curve.py
--rw-rw-rw-   0        0        0    10792 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/jointanimation.py
--rw-rw-rw-   0        0        0     2319 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/key.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.717426 skanym-0.0.3/src/skanym/core/animate/tests/
--rw-rw-rw-   0        0        0        0 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/tests/__init__.py
--rw-rw-rw-   0        0        0    11297 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/tests/test_curve.py
--rw-rw-rw-   0        0        0    12600 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/animate/tests/test_joint_animation.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.734351 skanym-0.0.3/src/skanym/core/math/
--rw-rw-rw-   0        0        0      236 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/math/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/math/constants.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.748066 skanym-0.0.3/src/skanym/core/math/tests/
--rw-rw-rw-   0        0        0        0 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/math/tests/__init__.py
--rw-rw-rw-   0        0        0    11903 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/math/tests/test_transform.py
--rw-rw-rw-   0        0        0    13088 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/math/transform.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.770678 skanym-0.0.3/src/skanym/core/model/
--rw-rw-rw-   0        0        0       93 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/model/__init__.py
--rw-rw-rw-   0        0        0    10485 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/model/joint.py
--rw-rw-rw-   0        0        0     3148 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/model/skeleton.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.780110 skanym-0.0.3/src/skanym/core/model/tests/
--rw-rw-rw-   0        0        0        0 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/model/tests/__init__.py
--rw-rw-rw-   0        0        0    17190 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/core/model/tests/test_joint.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.800603 skanym-0.0.3/src/skanym/examples/
--rw-rw-rw-   0        0        0     3587 2023-11-07 15:50:54.000000 skanym-0.0.3/src/skanym/examples/demo_features.py
--rw-rw-rw-   0        0        0     4614 2023-11-07 15:50:59.000000 skanym-0.0.3/src/skanym/examples/demo_hello_world.py
--rw-rw-rw-   0        0        0      760 2023-11-07 15:59:33.000000 skanym-0.0.3/src/skanym/examples/demo_load_fbx.py
--rw-rw-rw-   0        0        0      625 2023-11-07 15:51:06.000000 skanym-0.0.3/src/skanym/examples/demo_load_gltf.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.841533 skanym-0.0.3/src/skanym/examples/input/
--rw-rw-rw-   0        0        0   556256 2023-10-25 12:32:29.000000 skanym-0.0.3/src/skanym/examples/input/death.fbx
--rw-rw-rw-   0        0        0   329504 2023-10-25 12:32:29.000000 skanym-0.0.3/src/skanym/examples/input/run.fbx
--rw-rw-rw-   0        0        0   386416 2023-10-25 12:32:29.000000 skanym-0.0.3/src/skanym/examples/input/walk.fbx
--rw-rw-rw-   0        0        0   158864 2023-10-25 12:32:29.000000 skanym-0.0.3/src/skanym/examples/input/walk_glb.glb
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.863804 skanym-0.0.3/src/skanym/utils/
--rw-rw-rw-   0        0        0        0 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.989710 skanym-0.0.3/src/skanym/utils/fbx_bindings/
--rw-rw-rw-   0        0        0     3075 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/utils/fbx_bindings/FbxCommon.py
--rw-rw-rw-   0        0        0        0 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/utils/fbx_bindings/__init__.py
--rw-rw-rw-   0        0        0  9286144 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/utils/fbx_bindings/fbx.pyd
--rw-rw-rw-   0        0        0   105472 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/utils/fbx_bindings/sip.pyd
--rw-rw-rw-   0        0        0    19825 2023-11-07 15:31:50.000000 skanym-0.0.3/src/skanym/utils/loader.py
--rw-rw-rw-   0        0        0     3432 2023-11-07 11:28:47.000000 skanym-0.0.3/src/skanym/utils/other.py
-drwxrwxrwx   0        0        0        0 2023-11-09 14:04:52.654178 skanym-0.0.3/src/skanym.egg-info/
--rw-rw-rw-   0        0        0     2756 2023-11-09 14:04:52.000000 skanym-0.0.3/src/skanym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1578 2023-11-09 14:04:52.000000 skanym-0.0.3/src/skanym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 14:04:52.000000 skanym-0.0.3/src/skanym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-11-09 14:04:52.000000 skanym-0.0.3/src/skanym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-11-09 14:04:52.000000 skanym-0.0.3/src/skanym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.836931 skanym-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 12:29:13.000000 skanym-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2425 2024-04-11 09:18:07.832898 skanym-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-11-21 09:04:08.000000 skanym-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1077 2024-04-08 11:54:24.000000 skanym-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:18:07.837942 skanym-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:06.925871 skanym-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:06.961786 skanym-0.1.0/src/skanym/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.118103 skanym-0.1.0/src/skanym/animators/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/animators/__init__.py
+-rw-rw-rw-   0        0        0     2315 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/baseAnimator.py
+-rw-rw-rw-   0        0        0    10365 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/baseFkAnimator.py
+-rw-rw-rw-   0        0        0     2019 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/globalFkAnimator.py
+-rw-rw-rw-   0        0        0     1391 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/localFkAnimator.py
+-rw-rw-rw-   0        0        0     9316 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/pcaAnimator.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.180815 skanym-0.1.0/src/skanym/loaders/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/__init__.py
+-rw-rw-rw-   0        0        0    10632 2024-04-11 09:17:24.000000 skanym-0.1.0/src/skanym/loaders/fbxLoader.py
+-rw-rw-rw-   0        0        0     7899 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/glbLoader.py
+-rw-rw-rw-   0        0        0      655 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/iFileLoader.py
+-rw-rw-rw-   0        0        0      423 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/objectLoader.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.185338 skanym-0.1.0/src/skanym/structures/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.328876 skanym-0.1.0/src/skanym/structures/animation/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/__init__.py
+-rw-rw-rw-   0        0        0     1644 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/animation/animation.py
+-rw-rw-rw-   0        0        0      547 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/animationCurve.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/iCurve.py
+-rw-rw-rw-   0        0        0      890 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/key.py
+-rw-rw-rw-   0        0        0     1146 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/animation/positionCurve.py
+-rw-rw-rw-   0        0        0     1208 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/animation/quaternionCurve.py
+-rw-rw-rw-   0        0        0      784 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/scalarCurve.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.375085 skanym-0.1.0/src/skanym/structures/character/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/character/__init__.py
+-rw-rw-rw-   0        0        0     5439 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/character/joint.py
+-rw-rw-rw-   0        0        0     4233 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/character/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.451118 skanym-0.1.0/src/skanym/structures/data/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/iTransform.py
+-rw-rw-rw-   0        0        0     1305 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/transform.py
+-rw-rw-rw-   0        0        0     1179 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/transformMatrix.py
+-rw-rw-rw-   0        0        0     2305 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/vectorizedArray.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.478515 skanym-0.1.0/src/skanym/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 13:33:29.000000 skanym-0.1.0/src/skanym/utils/__init__.py
+-rw-rw-rw-   0        0        0    10909 2024-04-09 13:24:52.000000 skanym-0.1.0/src/skanym/utils/conversion.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.818353 skanym-0.1.0/src/skanym/utils/fbx_bindings/
+-rw-rw-rw-   0        0        0     3075 2023-11-07 11:28:47.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/FbxCommon.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 18:17:16.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/__init__.py
+-rw-rw-rw-   0        0        0  9286144 2023-11-07 11:28:47.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/fbx.pyd
+-rw-rw-rw-   0        0        0   105472 2023-11-07 11:28:47.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/sip.pyd
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.827807 skanym-0.1.0/src/skanym.egg-info/
+-rw-rw-rw-   0        0        0     2425 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/top_level.txt
```

### Comparing `skanym-0.0.3/LICENSE.txt` & `skanym-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skanym-0.0.3/PKG-INFO` & `skanym-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skanym
-Version: 0.0.3
+Version: 0.1.0
 Summary: Standalone package for skeletal animation
 Author-email: Dimitri Kohler <dimitri.kohler@he-arc.ch>
 License: MIT License
         
         Copyright (c) 2022 Dimitri Kohler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,22 +37,22 @@
 Requires-Dist: numpy-quaternion>=2022.0.0
 Requires-Dist: numpy
 Requires-Dist: pygltflib>=1.15.0
 Requires-Dist: bpy>=3.4.0
 Provides-Extra: gui
 Requires-Dist: skanym_gui; extra == "gui"
 
-# Skanym Core
+# Skanym
+
 This repository contains The core fonctionalities to create, edit and export 3D animations using the skeletal animation principle.
 
 ## Wikis
-(Motion Machine)[Link to the wiki]
-(Skanym)[Link to the wiki]
 
-## Historical context
-The skeletal-animation package was originally developed as part of a bachelor thesis in 2021-2022 ([link]() to the original repository [access required]). It was then maintained/extended for future use ([link]() to the latest version [access required]).
-This repository contains a fork of the core modules of the skeletal-animation package. The goal is to improve upon those modules
-to better fit the requirements for the Motion Machine project.
+- [Motion Machine](https://gitlab-etu.ing.he-arc.ch/groups/isc/general/motion-machine/-/wikis/home)
+
+- [Skanym](https://gitlab-etu.ing.he-arc.ch/isc/general/motion-machine/skanym-package/-/wikis/home)
+
+
```

### Comparing `skanym-0.0.3/pyproject.toml` & `skanym-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skanym"
-version = "0.0.3"
+version = "0.1.0"
 description = "Standalone package for skeletal animation"
 readme = "README.md"
 requires-python = "==3.10.*"
 license = {file = "LICENSE.txt"} 
 authors = [
     {name = "Dimitri Kohler", email = "dimitri.kohler@he-arc.ch"},
 ]
```

### Comparing `skanym-0.0.3/src/skanym/utils/fbx_bindings/FbxCommon.py` & `skanym-0.1.0/src/skanym/utils/fbx_bindings/FbxCommon.py`

 * *Files identical despite different names*

### Comparing `skanym-0.0.3/src/skanym.egg-info/PKG-INFO` & `skanym-0.1.0/src/skanym.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skanym
-Version: 0.0.3
+Version: 0.1.0
 Summary: Standalone package for skeletal animation
 Author-email: Dimitri Kohler <dimitri.kohler@he-arc.ch>
 License: MIT License
         
         Copyright (c) 2022 Dimitri Kohler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,22 +37,22 @@
 Requires-Dist: numpy-quaternion>=2022.0.0
 Requires-Dist: numpy
 Requires-Dist: pygltflib>=1.15.0
 Requires-Dist: bpy>=3.4.0
 Provides-Extra: gui
 Requires-Dist: skanym_gui; extra == "gui"
 
-# Skanym Core
+# Skanym
+
 This repository contains The core fonctionalities to create, edit and export 3D animations using the skeletal animation principle.
 
 ## Wikis
-(Motion Machine)[Link to the wiki]
-(Skanym)[Link to the wiki]
 
-## Historical context
-The skeletal-animation package was originally developed as part of a bachelor thesis in 2021-2022 ([link]() to the original repository [access required]). It was then maintained/extended for future use ([link]() to the latest version [access required]).
-This repository contains a fork of the core modules of the skeletal-animation package. The goal is to improve upon those modules
-to better fit the requirements for the Motion Machine project.
+- [Motion Machine](https://gitlab-etu.ing.he-arc.ch/groups/isc/general/motion-machine/-/wikis/home)
+
+- [Skanym](https://gitlab-etu.ing.he-arc.ch/isc/general/motion-machine/skanym-package/-/wikis/home)
+
+
```

