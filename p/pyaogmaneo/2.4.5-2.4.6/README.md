# Comparing `tmp/pyaogmaneo-2.4.5.tar.gz` & `tmp/pyaogmaneo-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.4.5.tar", last modified: Wed Apr 10 17:08:48 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.4.6.tar", last modified: Thu Apr 11 18:48:56 2024, max compression
```

## Comparing `pyaogmaneo-2.4.5.tar` & `pyaogmaneo-2.4.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:08:48.779147 pyaogmaneo-2.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:08:48.779147 pyaogmaneo-2.4.5/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 17:08:48.779147 pyaogmaneo-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:08:48.779147 pyaogmaneo-2.4.5/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 17:08:48.000000 pyaogmaneo-2.4.5/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-10 17:08:48.000000 pyaogmaneo-2.4.5/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:08:48.000000 pyaogmaneo-2.4.5/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:08:48.000000 pyaogmaneo-2.4.5/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 17:08:48.000000 pyaogmaneo-2.4.5/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:08:48.779147 pyaogmaneo-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:08:48.775147 pyaogmaneo-2.4.5/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:08:48.779147 pyaogmaneo-2.4.5/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-04-10 17:08:37.000000 pyaogmaneo-2.4.5/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:48:56.237322 pyaogmaneo-2.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:48:56.237322 pyaogmaneo-2.4.6/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 18:48:56.237322 pyaogmaneo-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:48:56.237322 pyaogmaneo-2.4.6/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 18:48:56.000000 pyaogmaneo-2.4.6/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 18:48:56.000000 pyaogmaneo-2.4.6/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:48:56.000000 pyaogmaneo-2.4.6/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:48:56.000000 pyaogmaneo-2.4.6/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 18:48:56.000000 pyaogmaneo-2.4.6/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:48:56.237322 pyaogmaneo-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:48:56.233322 pyaogmaneo-2.4.6/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:48:56.237322 pyaogmaneo-2.4.6/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-04-11 18:48:45.000000 pyaogmaneo-2.4.6/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.4.5/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.4.6/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/CMakeLists.txt` & `pyaogmaneo-2.4.6/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG d1db5fba16909af8b43c171413775be95da117af
+        GIT_TAG afdb1bda080045b31bcad36e4ce3cdaee727e39c
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.4.5/LICENSE.md` & `pyaogmaneo-2.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/PKG-INFO` & `pyaogmaneo-2.4.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.4.5
+Version: 2.4.6
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.4.5/README.md` & `pyaogmaneo-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.4.6/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.4.5
+Version: 2.4.6
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.4.5/setup.py` & `pyaogmaneo-2.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.4.5",
+    version="2.4.6",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.5/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.4.6/source/pyaogmaneo/py_module.cpp`

 * *Files identical despite different names*

