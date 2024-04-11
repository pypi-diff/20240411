# Comparing `tmp/tenetan-0.1.0.tar.gz` & `tmp/tenetan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenetan-0.1.0.tar", last modified: Tue Apr  9 16:53:58 2024, max compression
+gzip compressed data, was "tenetan-0.1.1.tar", last modified: Thu Apr 11 15:31:21 2024, max compression
```

## Comparing `tenetan-0.1.0.tar` & `tenetan-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-09 16:53:58.887681 tenetan-0.1.0/
--rw-r--r--   0 abakhtin22   (503) staff       (20)    35149 2023-10-06 11:48:01.000000 tenetan-0.1.0/LICENSE
--rw-r--r--   0 abakhtin22   (503) staff       (20)    41679 2024-04-09 16:53:58.887415 tenetan-0.1.0/PKG-INFO
--rw-r--r--   0 abakhtin22   (503) staff       (20)      271 2024-04-09 16:52:01.000000 tenetan-0.1.0/README.md
--rw-r--r--   0 abakhtin22   (503) staff       (20)      962 2024-04-09 16:52:01.000000 tenetan-0.1.0/pyproject.toml
--rw-r--r--   0 abakhtin22   (503) staff       (20)       38 2024-04-09 16:53:58.887749 tenetan-0.1.0/setup.cfg
-drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-09 16:53:58.884766 tenetan-0.1.0/tenetan/
--rw-r--r--   0 abakhtin22   (503) staff       (20)       72 2024-04-09 14:45:50.000000 tenetan-0.1.0/tenetan/__init__.py
-drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-09 16:53:58.886034 tenetan-0.1.0/tenetan/community/
--rw-r--r--   0 abakhtin22   (503) staff       (20)       85 2024-04-09 14:45:34.000000 tenetan-0.1.0/tenetan/community/__init__.py
--rw-r--r--   0 abakhtin22   (503) staff       (20)     4110 2024-04-09 14:45:34.000000 tenetan-0.1.0/tenetan/community/parafac.py
-drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-09 16:53:58.886322 tenetan-0.1.0/tenetan/networks/
--rw-r--r--   0 abakhtin22   (503) staff       (20)       64 2023-10-06 12:06:12.000000 tenetan-0.1.0/tenetan/networks/__init__.py
--rw-r--r--   0 abakhtin22   (503) staff       (20)      805 2024-04-04 16:05:10.000000 tenetan-0.1.0/tenetan/networks/snapshot.py
-drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-09 16:53:58.886758 tenetan-0.1.0/tenetan/preprocess/
--rw-r--r--   0 abakhtin22   (503) staff       (20)      118 2024-04-09 14:45:50.000000 tenetan-0.1.0/tenetan/preprocess/__init__.py
--rw-r--r--   0 abakhtin22   (503) staff       (20)     4006 2024-04-09 14:45:50.000000 tenetan-0.1.0/tenetan/preprocess/__main__.py
--rw-r--r--   0 abakhtin22   (503) staff       (20)     2773 2024-04-09 14:45:50.000000 tenetan-0.1.0/tenetan/preprocess/preprocess.py
-drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-09 16:53:58.886967 tenetan-0.1.0/tenetan.egg-info/
--rw-r--r--   0 abakhtin22   (503) staff       (20)    41679 2024-04-09 16:53:58.000000 tenetan-0.1.0/tenetan.egg-info/PKG-INFO
--rw-r--r--   0 abakhtin22   (503) staff       (20)      418 2024-04-09 16:53:58.000000 tenetan-0.1.0/tenetan.egg-info/SOURCES.txt
--rw-r--r--   0 abakhtin22   (503) staff       (20)        1 2024-04-09 16:53:58.000000 tenetan-0.1.0/tenetan.egg-info/dependency_links.txt
--rw-r--r--   0 abakhtin22   (503) staff       (20)       45 2024-04-09 16:53:58.000000 tenetan-0.1.0/tenetan.egg-info/requires.txt
--rw-r--r--   0 abakhtin22   (503) staff       (20)        8 2024-04-09 16:53:58.000000 tenetan-0.1.0/tenetan.egg-info/top_level.txt
+drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-11 15:31:21.885211 tenetan-0.1.1/
+-rw-r--r--   0 abakhtin22   (503) staff       (20)    35149 2023-10-06 11:48:01.000000 tenetan-0.1.1/LICENSE
+-rw-r--r--   0 abakhtin22   (503) staff       (20)    41679 2024-04-11 15:31:21.884969 tenetan-0.1.1/PKG-INFO
+-rw-r--r--   0 abakhtin22   (503) staff       (20)      271 2024-04-09 16:52:01.000000 tenetan-0.1.1/README.md
+-rw-r--r--   0 abakhtin22   (503) staff       (20)      962 2024-04-11 15:30:44.000000 tenetan-0.1.1/pyproject.toml
+-rw-r--r--   0 abakhtin22   (503) staff       (20)       38 2024-04-11 15:31:21.885263 tenetan-0.1.1/setup.cfg
+drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-11 15:31:21.881229 tenetan-0.1.1/tenetan/
+-rw-r--r--   0 abakhtin22   (503) staff       (20)       72 2024-04-09 14:45:50.000000 tenetan-0.1.1/tenetan/__init__.py
+drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-11 15:31:21.882905 tenetan-0.1.1/tenetan/community/
+-rw-r--r--   0 abakhtin22   (503) staff       (20)       85 2024-04-09 14:45:34.000000 tenetan-0.1.1/tenetan/community/__init__.py
+-rw-r--r--   0 abakhtin22   (503) staff       (20)     4111 2024-04-11 15:30:19.000000 tenetan-0.1.1/tenetan/community/parafac.py
+drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-11 15:31:21.883418 tenetan-0.1.1/tenetan/networks/
+-rw-r--r--   0 abakhtin22   (503) staff       (20)       64 2023-10-06 12:06:12.000000 tenetan-0.1.1/tenetan/networks/__init__.py
+-rw-r--r--   0 abakhtin22   (503) staff       (20)      805 2024-04-04 16:05:10.000000 tenetan-0.1.1/tenetan/networks/snapshot.py
+drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-11 15:31:21.884274 tenetan-0.1.1/tenetan/preprocess/
+-rw-r--r--   0 abakhtin22   (503) staff       (20)      118 2024-04-09 14:45:50.000000 tenetan-0.1.1/tenetan/preprocess/__init__.py
+-rw-r--r--   0 abakhtin22   (503) staff       (20)     4006 2024-04-09 14:45:50.000000 tenetan-0.1.1/tenetan/preprocess/__main__.py
+-rw-r--r--   0 abakhtin22   (503) staff       (20)     2773 2024-04-09 14:45:50.000000 tenetan-0.1.1/tenetan/preprocess/preprocess.py
+drwxr-xr-x   0 abakhtin22   (503) staff       (20)        0 2024-04-11 15:31:21.884531 tenetan-0.1.1/tenetan.egg-info/
+-rw-r--r--   0 abakhtin22   (503) staff       (20)    41679 2024-04-11 15:31:21.000000 tenetan-0.1.1/tenetan.egg-info/PKG-INFO
+-rw-r--r--   0 abakhtin22   (503) staff       (20)      418 2024-04-11 15:31:21.000000 tenetan-0.1.1/tenetan.egg-info/SOURCES.txt
+-rw-r--r--   0 abakhtin22   (503) staff       (20)        1 2024-04-11 15:31:21.000000 tenetan-0.1.1/tenetan.egg-info/dependency_links.txt
+-rw-r--r--   0 abakhtin22   (503) staff       (20)       45 2024-04-11 15:31:21.000000 tenetan-0.1.1/tenetan.egg-info/requires.txt
+-rw-r--r--   0 abakhtin22   (503) staff       (20)        8 2024-04-11 15:31:21.000000 tenetan-0.1.1/tenetan.egg-info/top_level.txt
```

### Comparing `tenetan-0.1.0/LICENSE` & `tenetan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tenetan-0.1.0/PKG-INFO` & `tenetan-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenetan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Temporal Network Analysis Library
 Author-email: Alexander Bakhtin <alexander.bakhtin@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tenetan-0.1.0/pyproject.toml` & `tenetan-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Topic :: Scientific/Engineering :: Mathematics"]
 
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.6"
 dependencies = [
     "tensorly==0.8.1",
     "TLViz==0.1.1"]
 
 [project.optional-dependencies]
 prepr = ["pandas"]
```

### Comparing `tenetan-0.1.0/tenetan/community/parafac.py` & `tenetan-0.1.1/tenetan/community/parafac.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             in_temporal_activity = tl.zeros_like(raw_temporal_activity)
             for i in range(tl.shape(in_temporal_activity)[0]):
                 for j in range(tl.shape(in_temporal_activity)[1]):
                     in_temporal_activity = tl.index_update(in_temporal_activity, tl.index[i, j],
                                                            raw_temporal_activity[i, j] * weights[j])
             return_dict[data] = in_temporal_activity
         elif data == "out_temporal_activity":
-            weights = tl.sum(in_communities, axis=0)
+            weights = tl.sum(out_communities, axis=0)
             out_temporal_activity = tl.zeros_like(raw_temporal_activity)
             for i in range(tl.shape(out_temporal_activity)[0]):
                 for j in range(tl.shape(out_temporal_activity)[1]):
                     out_temporal_activity = tl.index_update(out_temporal_activity, tl.index[i, j],
                                                             raw_temporal_activity[i, j]*weights[j])
             return_dict[data] = out_temporal_activity
         elif data == 'core_consistency':
```

### Comparing `tenetan-0.1.0/tenetan/networks/snapshot.py` & `tenetan-0.1.1/tenetan/networks/snapshot.py`

 * *Files identical despite different names*

### Comparing `tenetan-0.1.0/tenetan/preprocess/__main__.py` & `tenetan-0.1.1/tenetan/preprocess/__main__.py`

 * *Files identical despite different names*

### Comparing `tenetan-0.1.0/tenetan/preprocess/preprocess.py` & `tenetan-0.1.1/tenetan/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `tenetan-0.1.0/tenetan.egg-info/PKG-INFO` & `tenetan-0.1.1/tenetan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenetan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Temporal Network Analysis Library
 Author-email: Alexander Bakhtin <alexander.bakhtin@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

