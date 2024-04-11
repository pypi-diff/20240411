# Comparing `tmp/LATSourceModel-1.10.8.tar.gz` & `tmp/LATSourceModel-1.10.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LATSourceModel-1.10.8.tar", last modified: Thu Aug 10 13:02:04 2023, max compression
+gzip compressed data, was "LATSourceModel-1.10.9.tar", last modified: Mon Aug 28 10:14:41 2023, max compression
```

## Comparing `LATSourceModel-1.10.8.tar` & `LATSourceModel-1.10.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-10 13:02:04.826020 LATSourceModel-1.10.8/
--rw-r--r--   0 tyrelj     (501) staff       (20)    35129 2023-07-10 15:27:39.000000 LATSourceModel-1.10.8/LICENSE
--rw-r--r--   0 tyrelj     (501) staff       (20)     1731 2023-08-10 13:02:04.825910 LATSourceModel-1.10.8/PKG-INFO
--rw-r--r--   0 tyrelj     (501) staff       (20)     1078 2023-07-10 18:10:29.000000 LATSourceModel-1.10.8/README.md
--rw-r--r--   0 tyrelj     (501) staff       (20)      912 2023-08-10 12:58:03.000000 LATSourceModel-1.10.8/pyproject.toml
--rw-r--r--   0 tyrelj     (501) staff       (20)       38 2023-08-10 13:02:04.826053 LATSourceModel-1.10.8/setup.cfg
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-10 13:02:04.824001 LATSourceModel-1.10.8/src/
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-10 13:02:04.825040 LATSourceModel-1.10.8/src/LATSourceModel/
--rw-r--r--   0 tyrelj     (501) staff       (20)    49082 2023-08-10 12:42:19.000000 LATSourceModel-1.10.8/src/LATSourceModel/SourceList.py
--rw-r--r--   0 tyrelj     (501) staff       (20)      116 2023-07-16 19:02:17.000000 LATSourceModel-1.10.8/src/LATSourceModel/__init__.py
--rw-r--r--   0 tyrelj     (501) staff       (20)    10547 2023-07-24 12:30:24.000000 LATSourceModel-1.10.8/src/LATSourceModel/make4FGLxml.py
--rw-r--r--   0 tyrelj     (501) staff       (20)    74177 2023-07-18 17:10:18.000000 LATSourceModel-1.10.8/src/LATSourceModel/model_components.py
--rw-r--r--   0 tyrelj     (501) staff       (20)    11927 2023-07-18 17:10:18.000000 LATSourceModel-1.10.8/src/LATSourceModel/utilities.py
-drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-10 13:02:04.825752 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/
--rw-r--r--   0 tyrelj     (501) staff       (20)     1731 2023-08-10 13:02:04.000000 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/PKG-INFO
--rw-r--r--   0 tyrelj     (501) staff       (20)      455 2023-08-10 13:02:04.000000 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/SOURCES.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)        1 2023-08-10 13:02:04.000000 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/dependency_links.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)       63 2023-08-10 13:02:04.000000 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/entry_points.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)       21 2023-08-10 13:02:04.000000 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/requires.txt
--rw-r--r--   0 tyrelj     (501) staff       (20)       15 2023-08-10 13:02:04.000000 LATSourceModel-1.10.8/src/LATSourceModel.egg-info/top_level.txt
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-28 10:14:41.706164 LATSourceModel-1.10.9/
+-rw-r--r--   0 tyrelj     (501) staff       (20)    35129 2023-07-10 15:27:39.000000 LATSourceModel-1.10.9/LICENSE
+-rw-r--r--   0 tyrelj     (501) staff       (20)     1731 2023-08-28 10:14:41.706051 LATSourceModel-1.10.9/PKG-INFO
+-rw-r--r--   0 tyrelj     (501) staff       (20)     1078 2023-07-10 18:10:29.000000 LATSourceModel-1.10.9/README.md
+-rw-r--r--   0 tyrelj     (501) staff       (20)      912 2023-08-28 10:11:24.000000 LATSourceModel-1.10.9/pyproject.toml
+-rw-r--r--   0 tyrelj     (501) staff       (20)       38 2023-08-28 10:14:41.706200 LATSourceModel-1.10.9/setup.cfg
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-28 10:14:41.703010 LATSourceModel-1.10.9/src/
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-28 10:14:41.704991 LATSourceModel-1.10.9/src/LATSourceModel/
+-rw-r--r--   0 tyrelj     (501) staff       (20)    49082 2023-08-10 12:42:19.000000 LATSourceModel-1.10.9/src/LATSourceModel/SourceList.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)      116 2023-07-16 19:02:17.000000 LATSourceModel-1.10.9/src/LATSourceModel/__init__.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)    10549 2023-08-28 10:04:01.000000 LATSourceModel-1.10.9/src/LATSourceModel/make4FGLxml.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)    74177 2023-07-18 17:10:18.000000 LATSourceModel-1.10.9/src/LATSourceModel/model_components.py
+-rw-r--r--   0 tyrelj     (501) staff       (20)    11927 2023-07-18 17:10:18.000000 LATSourceModel-1.10.9/src/LATSourceModel/utilities.py
+drwxr-xr-x   0 tyrelj     (501) staff       (20)        0 2023-08-28 10:14:41.705770 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/
+-rw-r--r--   0 tyrelj     (501) staff       (20)     1731 2023-08-28 10:14:41.000000 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/PKG-INFO
+-rw-r--r--   0 tyrelj     (501) staff       (20)      455 2023-08-28 10:14:41.000000 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/SOURCES.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)        1 2023-08-28 10:14:41.000000 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/dependency_links.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)       63 2023-08-28 10:14:41.000000 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/entry_points.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)       21 2023-08-28 10:14:41.000000 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/requires.txt
+-rw-r--r--   0 tyrelj     (501) staff       (20)       15 2023-08-28 10:14:41.000000 LATSourceModel-1.10.9/src/LATSourceModel.egg-info/top_level.txt
```

### Comparing `LATSourceModel-1.10.8/LICENSE` & `LATSourceModel-1.10.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.8/PKG-INFO` & `LATSourceModel-1.10.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LATSourceModel
-Version: 1.10.8
+Version: 1.10.9
 Summary: A set of functions and classes to build spatial-spectral models for analysis of Fermi LAT gamma-ray data.
 Author-email: Tyrel Johnson <tyrel.j.johnson@gmail.com>
 License: GPL-3.0
 Project-URL: Home, https://github.com/physicsranger/make4FGLxml
 Project-URL: Issues, https://github.com/physicsranger/make4FGLxml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `LATSourceModel-1.10.8/README.md` & `LATSourceModel-1.10.9/README.md`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.8/pyproject.toml` & `LATSourceModel-1.10.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LATSourceModel"
 authors = [
     {name = "Tyrel Johnson", email = "tyrel.j.johnson@gmail.com"},
 ]
-version = "1.10.8"
+version = "1.10.9"
 description = "A set of functions and classes to build spatial-spectral models for analysis of Fermi LAT gamma-ray data."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.4" #for pathlib
 license = {text = "GPL-3.0"}
 classifiers = [
 "Programming Language :: Python :: 3",
 "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `LATSourceModel-1.10.8/src/LATSourceModel/SourceList.py` & `LATSourceModel-1.10.9/src/LATSourceModel/SourceList.py`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.8/src/LATSourceModel/make4FGLxml.py` & `LATSourceModel-1.10.9/src/LATSourceModel/make4FGLxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     
     parser.add_argument("-ON","--use_old_names",type=mybool,default=False,
                 help="Flag to use the make2FLGxml style naming convention, underscore before name and no spaces,\
  default is False.",nargs="?",const=True,
                 choices=['True','False','T','F','t','f','TRUE','FALSE','true','false',1,0])
     
     parser.add_argument('-DR',type=int,default=3,help='Choice of data release, 3 for 4FGL-DR3, 2 for 4FGL-DR2, and 1 for 4FGL.',
-                choices=[1,2,3])
+                choices=[1,2,3,4])
 
     parser.add_argument('--new',type=str,default=None,help='RA, DEC, source_name, and model for a non-4FGL point source to be\
  added to the model.  Must be a string contained within single quotes with keys in double quotes.')
     
     args=parser.parse_args()
 
     #determine how the ROI information will be derived,
```

### Comparing `LATSourceModel-1.10.8/src/LATSourceModel/model_components.py` & `LATSourceModel-1.10.9/src/LATSourceModel/model_components.py`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.8/src/LATSourceModel/utilities.py` & `LATSourceModel-1.10.9/src/LATSourceModel/utilities.py`

 * *Files identical despite different names*

### Comparing `LATSourceModel-1.10.8/src/LATSourceModel.egg-info/PKG-INFO` & `LATSourceModel-1.10.9/src/LATSourceModel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LATSourceModel
-Version: 1.10.8
+Version: 1.10.9
 Summary: A set of functions and classes to build spatial-spectral models for analysis of Fermi LAT gamma-ray data.
 Author-email: Tyrel Johnson <tyrel.j.johnson@gmail.com>
 License: GPL-3.0
 Project-URL: Home, https://github.com/physicsranger/make4FGLxml
 Project-URL: Issues, https://github.com/physicsranger/make4FGLxml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

