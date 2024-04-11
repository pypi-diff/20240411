# Comparing `tmp/arcor2_runtime-1.1.0.tar.gz` & `tmp/arcor2_runtime-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_runtime-1.1.0.tar", last modified: Wed Jan  3 13:06:59 2024, max compression
+gzip compressed data, was "arcor2_runtime-1.2.0.tar", last modified: Thu Apr 11 09:47:31 2024, max compression
```

## Comparing `arcor2_runtime-1.1.0.tar` & `arcor2_runtime-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-03 13:06:59.515022 arcor2_runtime-1.1.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2627 2024-01-03 13:06:59.515022 arcor2_runtime-1.1.0/PKG-INFO
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-03 13:06:59.515022 arcor2_runtime-1.1.0/arcor2_runtime/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/VERSION
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     8875 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/action.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      565 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/arguments.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      701 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/events.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      970 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/exceptions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1085 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/package.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/py.typed
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    11304 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime/resources.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-03 13:06:59.515022 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2627 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      507 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      112 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       15 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/arcor2_runtime.egg-info/top_level.txt
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      822 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/backend_shim.py
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-01-03 13:06:59.515022 arcor2_runtime-1.1.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3267 2024-01-03 13:06:59.000000 arcor2_runtime-1.1.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.993246 arcor2_runtime-1.2.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2715 2024-04-11 09:47:31.993246 arcor2_runtime-1.2.0/PKG-INFO
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.989246 arcor2_runtime-1.2.0/arcor2_runtime/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/VERSION
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     8875 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/action.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      565 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/arguments.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      701 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/events.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      970 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/exceptions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1085 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/package.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/py.typed
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    11304 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/arcor2_runtime/resources.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.993246 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     2715 2024-04-11 09:47:31.000000 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      507 2024-04-11 09:47:31.000000 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:31.000000 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:31.000000 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      102 2024-04-11 09:47:31.000000 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       15 2024-04-11 09:47:31.000000 arcor2_runtime-1.2.0/arcor2_runtime.egg-info/top_level.txt
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/backend_shim.py
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-11 09:47:31.993246 arcor2_runtime-1.2.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3345 2024-04-11 09:47:30.000000 arcor2_runtime-1.2.0/setup.py
```

### Comparing `arcor2_runtime-1.1.0/PKG-INFO` & `arcor2_runtime-1.2.0/arcor2_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
-Name: arcor2_runtime
-Version: 1.1.0
+Name: arcor2-runtime
+Version: 1.2.0
 Summary: ARCOR2 Runtime.
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
 
 # arcor2_runtime
 
 The stuff that is required by the main script.
 
 ## Environment variables
 
 - `ARCOR2_STREAMING_PERIOD=0.1` - controls the period of streaming a robot's EEF poses and joints.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.1.0] - 2024-01-03
+## [1.2.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
+## [1.1.0] - 2024-01-08
 
 ### Changed
 
 - Parameter `interact_with_scene_service` added to the `Resources` class.
 
 ## [1.0.0] - 2023-02-14
```

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime/action.py` & `arcor2_runtime-1.2.0/arcor2_runtime/action.py`

 * *Files identical despite different names*

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime/arguments.py` & `arcor2_runtime-1.2.0/arcor2_runtime/arguments.py`

 * *Files identical despite different names*

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime/events.py` & `arcor2_runtime-1.2.0/arcor2_runtime/events.py`

 * *Files identical despite different names*

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime/exceptions.py` & `arcor2_runtime-1.2.0/arcor2_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime/package.py` & `arcor2_runtime-1.2.0/arcor2_runtime/package.py`

 * *Files identical despite different names*

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime/resources.py` & `arcor2_runtime-1.2.0/arcor2_runtime/resources.py`

 * *Files identical despite different names*

### Comparing `arcor2_runtime-1.1.0/arcor2_runtime.egg-info/PKG-INFO` & `arcor2_runtime-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
-Name: arcor2-runtime
-Version: 1.1.0
+Name: arcor2_runtime
+Version: 1.2.0
 Summary: ARCOR2 Runtime.
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
 
 # arcor2_runtime
 
 The stuff that is required by the main script.
 
 ## Environment variables
 
 - `ARCOR2_STREAMING_PERIOD=0.1` - controls the period of streaming a robot's EEF poses and joints.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.1.0] - 2024-01-03
+## [1.2.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
+## [1.1.0] - 2024-01-08
 
 ### Changed
 
 - Parameter `interact_with_scene_service` added to the `Resources` class.
 
 ## [1.0.0] - 2023-02-14
```

### Comparing `arcor2_runtime-1.1.0/backend_shim.py` & `arcor2_runtime-1.2.0/backend_shim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
+import errno
 import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
 dist_dir = "dist/"
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
     '--global-option': [
         '--python-tag',
-        'py310',
+        'py311',
     ],
 }
 sdist_config_settings = {
 }
 
 # Python 2.7 doesn't have the exist_ok arg on os.makedirs().
 try:
```

### Comparing `arcor2_runtime-1.1.0/setup.py` & `arcor2_runtime-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,37 +8,43 @@
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
     'description': 'ARCOR2 Runtime.',
     'install_requires': (
-        'arcor2~=1.1.0',
-        'dataclasses-jsonschema[apispec,fast-dateparsing,fast-uuid,fast-validation]~=2.16.0',
+        'arcor2~=1.3.0',
+        'dataclasses-jsonschema[apispec,fast-dateparsing,fast-validation]~=2.16.0',
         'pyhumps==3.8.0',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_runtime
 
 The stuff that is required by the main script.
 
 ## Environment variables
 
 - `ARCOR2_STREAMING_PERIOD=0.1` - controls the period of streaming a robot's EEF poses and joints.
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
-## [1.1.0] - 2024-01-03
+## [1.2.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
+## [1.1.0] - 2024-01-08
 
 ### Changed
 
 - Parameter `interact_with_scene_service` added to the `Resources` class.
 
 ## [1.0.0] - 2023-02-14
 
@@ -112,10 +118,10 @@
             'VERSION',
             'py.typed',
         ),
     },
     'packages': (
         'arcor2_runtime',
     ),
-    'python_requires': '==3.10.*',
-    'version': '1.1.0',
+    'python_requires': '==3.11.*',
+    'version': '1.2.0',
 })
```

