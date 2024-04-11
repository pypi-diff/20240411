# Comparing `tmp/gixpy-1.1.tar.gz` & `tmp/gixpy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gixpy-1.1.tar", last modified: Thu Apr 11 03:12:46 2024, max compression
+gzip compressed data, was "gixpy-1.2.tar", last modified: Thu Apr 11 03:17:38 2024, max compression
```

## Comparing `gixpy-1.1.tar` & `gixpy-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 03:12:46.162092 gixpy-1.1/
--rw-rw-rw-   0        0        0      436 2024-04-11 03:12:46.162092 gixpy-1.1/PKG-INFO
--rw-rw-rw-   0        0        0    21235 2024-04-11 03:09:51.000000 gixpy-1.1/gixpy.c
-drwxrwxrwx   0        0        0        0 2024-04-11 03:12:46.158801 gixpy-1.1/gixpy.egg-info/
--rw-rw-rw-   0        0        0      436 2024-04-11 03:12:46.000000 gixpy-1.1/gixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-04-11 03:12:46.000000 gixpy-1.1/gixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 03:12:46.000000 gixpy-1.1/gixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 03:12:46.000000 gixpy-1.1/gixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      575 2024-04-11 03:10:44.000000 gixpy-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 03:12:46.168546 gixpy-1.1/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-04-11 03:09:36.000000 gixpy-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:17:38.907012 gixpy-1.2/
+-rw-rw-rw-   0        0        0      395 2024-04-11 03:17:38.907012 gixpy-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    21235 2024-04-11 03:16:54.000000 gixpy-1.2/gixpy.c
+drwxrwxrwx   0        0        0        0 2024-04-11 03:17:38.907012 gixpy-1.2/gixpy.egg-info/
+-rw-rw-rw-   0        0        0      395 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2024-04-11 03:16:46.000000 gixpy-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 03:17:38.907012 gixpy-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-04-11 03:16:56.000000 gixpy-1.2/setup.py
```

### Comparing `gixpy-1.1/gixpy.c` & `gixpy-1.2/gixpy.c`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
  * Initialize gixpy. May be called multiple times, so avoid
  * using static state.
  */
 int exec_gixpy(PyObject *module) {
     PyModule_AddFunctions(module, gixpy_functions);
 
     PyModule_AddStringConstant(module, "__author__", "Teddy Tortorici");
-    PyModule_AddStringConstant(module, "__version__", "1.1");
+    PyModule_AddStringConstant(module, "__version__", "1.2");
     PyModule_AddIntConstant(module, "year", 2024);
 
     return 0; /* success */
 }
 
 /*
  * Documentation for gixpy.
```

### Comparing `gixpy-1.1/pyproject.toml` & `gixpy-1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gixpy"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Teddy Tortorici", email="edward.tortorici@colorado.edu" },
 ]
 description = "Transform GIWAXS images"
-readme = "README.md"
+readme = "README"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `gixpy-1.1/setup.py` & `gixpy-1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         'C:\\Users\\Teddy\\AppData\\Roaming\\Python\\Python39\\site-packages\\numpy\\core\\include'],
     library_dirs=["\\root\\project"],
     language="c",
 )
 
 setup(
     name='gixpy',
-    version="1.1",
+    version="1.2",
     description="Python package to quickly transform GIWAXS images using C",
     long_description="Visit github.com/etortorici/gixpy for details",
     author_email='edward.tortorici@colorado.edu',
     license='GPL',
     ext_modules=[gp_module],
     install_requires=["numpy"],
 )
```

