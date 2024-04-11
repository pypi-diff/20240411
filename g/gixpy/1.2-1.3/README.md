# Comparing `tmp/gixpy-1.2.tar.gz` & `tmp/gixpy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gixpy-1.2.tar", last modified: Thu Apr 11 03:17:38 2024, max compression
+gzip compressed data, was "gixpy-1.3.tar", last modified: Thu Apr 11 03:20:01 2024, max compression
```

## Comparing `gixpy-1.2.tar` & `gixpy-1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 03:17:38.907012 gixpy-1.2/
--rw-rw-rw-   0        0        0      395 2024-04-11 03:17:38.907012 gixpy-1.2/PKG-INFO
--rw-rw-rw-   0        0        0    21235 2024-04-11 03:16:54.000000 gixpy-1.2/gixpy.c
-drwxrwxrwx   0        0        0        0 2024-04-11 03:17:38.907012 gixpy-1.2/gixpy.egg-info/
--rw-rw-rw-   0        0        0      395 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 03:17:38.000000 gixpy-1.2/gixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      572 2024-04-11 03:16:46.000000 gixpy-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 03:17:38.907012 gixpy-1.2/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-04-11 03:16:56.000000 gixpy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:01.971228 gixpy-1.3/
+-rw-rw-rw-   0        0        0      433 2024-04-11 03:20:01.969230 gixpy-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    21235 2024-04-11 03:19:30.000000 gixpy-1.3/gixpy.c
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:01.965226 gixpy-1.3/gixpy.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2024-04-11 03:19:20.000000 gixpy-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 03:20:01.972227 gixpy-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-04-11 03:19:24.000000 gixpy-1.3/setup.py
```

### Comparing `gixpy-1.2/gixpy.c` & `gixpy-1.3/gixpy.c`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
  * Initialize gixpy. May be called multiple times, so avoid
  * using static state.
  */
 int exec_gixpy(PyObject *module) {
     PyModule_AddFunctions(module, gixpy_functions);
 
     PyModule_AddStringConstant(module, "__author__", "Teddy Tortorici");
-    PyModule_AddStringConstant(module, "__version__", "1.2");
+    PyModule_AddStringConstant(module, "__version__", "1.3");
     PyModule_AddIntConstant(module, "year", 2024);
 
     return 0; /* success */
 }
 
 /*
  * Documentation for gixpy.
```

### Comparing `gixpy-1.2/setup.py` & `gixpy-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         'C:\\Users\\Teddy\\AppData\\Roaming\\Python\\Python39\\site-packages\\numpy\\core\\include'],
     library_dirs=["\\root\\project"],
     language="c",
 )
 
 setup(
     name='gixpy',
-    version="1.2",
+    version="1.3",
     description="Python package to quickly transform GIWAXS images using C",
     long_description="Visit github.com/etortorici/gixpy for details",
     author_email='edward.tortorici@colorado.edu',
     license='GPL',
     ext_modules=[gp_module],
     install_requires=["numpy"],
 )
```

