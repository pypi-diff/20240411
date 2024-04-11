# Comparing `tmp/app_stle-0.0.2.tar.gz` & `tmp/app_stle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/app_stle-0.0.2.tar", last modified: Tue Nov 24 01:29:39 2020, max compression
+gzip compressed data, was "app_stle-0.0.3.tar", last modified: Thu Apr 11 14:19:30 2024, max compression
```

## Comparing `app_stle-0.0.2.tar` & `app_stle-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 greg      (1001) greg      (1001)        0 2020-11-24 01:29:39.000000 app_stle-0.0.2/
--rw-r--r--   0 greg      (1001) greg      (1001)     1452 2020-11-24 01:29:39.000000 app_stle-0.0.2/PKG-INFO
--rw-r--r--   0 greg      (1001) greg      (1001)      751 2020-11-24 00:40:00.000000 app_stle-0.0.2/README.md
-drwxr-xr-x   0 greg      (1001) greg      (1001)        0 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle/
--rwxr--r--   0 greg      (1001) greg      (1001)       28 2020-11-23 19:31:08.000000 app_stle-0.0.2/app_stle/__init__.py
--rw-r--r--   0 greg      (1001) greg      (1001)    10515 2020-11-24 01:26:28.000000 app_stle-0.0.2/app_stle/shockt.py
-drwxr-xr-x   0 greg      (1001) greg      (1001)        0 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle.egg-info/
--rw-r--r--   0 greg      (1001) greg      (1001)     1452 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1001) greg      (1001)      244 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1001) greg      (1001)        1 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1001) greg      (1001)       26 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle.egg-info/requires.txt
--rw-r--r--   0 greg      (1001) greg      (1001)        9 2020-11-24 01:29:39.000000 app_stle-0.0.2/app_stle.egg-info/top_level.txt
--rw-r--r--   0 greg      (1001) greg      (1001)        1 2020-11-23 19:31:31.000000 app_stle-0.0.2/app_stle.egg-info/zip-safe
--rw-r--r--   0 greg      (1001) greg      (1001)       38 2020-11-24 01:29:39.000000 app_stle-0.0.2/setup.cfg
--rwxr--r--   0 greg      (1001) greg      (1001)      896 2020-11-24 01:27:15.000000 app_stle-0.0.2/setup.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-04-11 14:19:30.133983 app_stle-0.0.3/
+-rw-rw-r--   0 greg      (1000) greg      (1000)     1451 2024-04-11 14:19:30.133983 app_stle-0.0.3/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)      750 2020-11-24 01:43:27.000000 app_stle-0.0.3/README.md
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-04-11 14:19:30.133983 app_stle-0.0.3/app_stle/
+-rwxr--r--   0 greg      (1000) greg      (1000)       28 2020-11-23 19:31:08.000000 app_stle-0.0.3/app_stle/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    10515 2024-04-11 14:15:29.000000 app_stle-0.0.3/app_stle/shockt.py
+drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2024-04-11 14:19:30.133983 app_stle-0.0.3/app_stle.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1451 2024-04-11 14:19:30.000000 app_stle-0.0.3/app_stle.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)      244 2024-04-11 14:19:30.000000 app_stle-0.0.3/app_stle.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2024-04-11 14:19:30.000000 app_stle-0.0.3/app_stle.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       31 2024-04-11 14:19:30.000000 app_stle-0.0.3/app_stle.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        9 2024-04-11 14:19:30.000000 app_stle-0.0.3/app_stle.egg-info/top_level.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2020-11-23 19:31:31.000000 app_stle-0.0.3/app_stle.egg-info/zip-safe
+-rw-rw-r--   0 greg      (1000) greg      (1000)       38 2024-04-11 14:19:30.133983 app_stle-0.0.3/setup.cfg
+-rwxr--r--   0 greg      (1000) greg      (1000)      901 2024-04-11 14:18:03.000000 app_stle-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `app_stle-0.0.2/PKG-INFO` & `app_stle-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app_stle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Adaptive pressure profile tracking of the shock-train leading edge.
 Home-page: https://gjhunt.github.io/app/
 Author: Gregory J. Hunt
 Author-email: ghunt@wm.edu
 License: GPL3
 Description: <img src="quartet.png" width="100%">
         
@@ -14,15 +14,15 @@
         
         ## Software
         
         The *python package* is available on pypi [here](https://pypi.org/project/app-stle/)
         
         ## Vignettes
         
-        A basic vignette of how to use APP is available [here](simple_example/simple_example.md) ([.py](simple_example/simple_example.py) | [.ipynb](simple_example/simple_example.ipynb))
+        A basic vignette of how to use APP is available [here](simple_example/simple_example.md) ([.py](simple_example/simple_example.py)  [.ipynb](simple_example/simple_example.ipynb))
         
         ## Papers
         
         ## 1. "Adaptive Pressure Profile Method to Locate the Isolator Shock Train Leading Edge Given Limited Pressure Information" AIAA 2020 P&E
         
         - Our *publication* in AIAA P&E is available [here](https://arc.aiaa.org/doi/abs/10.2514/6.2020-3715)
```

### Comparing `app_stle-0.0.2/README.md` & `app_stle-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Software
 
 The *python package* is available on pypi [here](https://pypi.org/project/app-stle/)
 
 ## Vignettes
 
-A basic vignette of how to use APP is available [here](simple_example/simple_example.md) ([.py](simple_example/simple_example.py) | [.ipynb](simple_example/simple_example.ipynb))
+A basic vignette of how to use APP is available [here](simple_example/simple_example.md) ([.py](simple_example/simple_example.py)  [.ipynb](simple_example/simple_example.ipynb))
 
 ## Papers
 
 ## 1. "Adaptive Pressure Profile Method to Locate the Isolator Shock Train Leading Edge Given Limited Pressure Information" AIAA 2020 P&E
 
 - Our *publication* in AIAA P&E is available [here](https://arc.aiaa.org/doi/abs/10.2514/6.2020-3715)
```

### Comparing `app_stle-0.0.2/app_stle/shockt.py` & `app_stle-0.0.3/app_stle/shockt.py`

 * *Files identical despite different names*

### Comparing `app_stle-0.0.2/app_stle.egg-info/PKG-INFO` & `app_stle-0.0.3/app_stle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-stle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Adaptive pressure profile tracking of the shock-train leading edge.
 Home-page: https://gjhunt.github.io/app/
 Author: Gregory J. Hunt
 Author-email: ghunt@wm.edu
 License: GPL3
 Description: <img src="quartet.png" width="100%">
         
@@ -14,15 +14,15 @@
         
         ## Software
         
         The *python package* is available on pypi [here](https://pypi.org/project/app-stle/)
         
         ## Vignettes
         
-        A basic vignette of how to use APP is available [here](simple_example/simple_example.md) ([.py](simple_example/simple_example.py) | [.ipynb](simple_example/simple_example.ipynb))
+        A basic vignette of how to use APP is available [here](simple_example/simple_example.md) ([.py](simple_example/simple_example.py)  [.ipynb](simple_example/simple_example.ipynb))
         
         ## Papers
         
         ## 1. "Adaptive Pressure Profile Method to Locate the Isolator Shock Train Leading Edge Given Limited Pressure Information" AIAA 2020 P&E
         
         - Our *publication* in AIAA P&E is available [here](https://arc.aiaa.org/doi/abs/10.2514/6.2020-3715)
```

### Comparing `app_stle-0.0.2/setup.py` & `app_stle-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='app_stle',
-      version='0.0.2',
+      version='0.0.3',
       url='https://gjhunt.github.io/app/',
       author='Gregory J. Hunt',
       author_email='ghunt@wm.edu',
       description='Adaptive pressure profile tracking of the shock-train leading edge.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='GPL3',
       packages=setuptools.find_packages(),
       install_requires=[
           'numpy',
           'scipy',
-          'sklearn',
+          'scikit-learn',
           'nlopt'
           ],
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
           "Operating System :: OS Independent",
           'Topic :: Scientific/Engineering',
```

