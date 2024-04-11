# Comparing `tmp/pyosv-0.0.8.tar.gz` & `tmp/pyosv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosv-0.0.8.tar", last modified: Thu Jan 25 14:16:51 2024, max compression
+gzip compressed data, was "pyosv-0.0.9.tar", last modified: Thu Jan 25 14:32:14 2024, max compression
```

## Comparing `pyosv-0.0.8.tar` & `pyosv-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.935372 pyosv-0.0.8/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1072 2023-10-23 13:06:27.000000 pyosv-0.0.8/LICENSE
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3277 2024-01-25 14:16:51.934828 pyosv-0.0.8/PKG-INFO
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1167 2024-01-25 14:12:07.000000 pyosv-0.0.8/README.md
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.902963 pyosv-0.0.8/pyosv/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      173 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/__init__.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.921538 pyosv-0.0.8/pyosv/ai/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      120 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/ai/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1662 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/ai/clustering.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     2197 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/ai/data_reduction.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.923271 pyosv-0.0.8/pyosv/freq/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      105 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/freq/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1813 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/freq/fft.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3705 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/freq/filters.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.925702 pyosv-0.0.8/pyosv/io/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      129 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/io/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     4052 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/io/batch_reader.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3390 2024-01-25 13:35:25.000000 pyosv-0.0.8/pyosv/io/reader.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     2443 2024-01-25 13:36:01.000000 pyosv-0.0.8/pyosv/io/writer.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.928753 pyosv-0.0.8/pyosv/plot/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      113 2024-01-25 14:16:20.000000 pyosv-0.0.8/pyosv/plot/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3793 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/plot/cube.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1715 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/plot/geo.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3533 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/plot/plot.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.930284 pyosv-0.0.8/pyosv/post/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      128 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/post/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1600 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/post/normalized_difference.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     5888 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/post/patch_extractor.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.932071 pyosv-0.0.8/pyosv/pre/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      191 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/pre/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     2857 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/pre/hist_normalizer.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     6158 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/pre/normalizer.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     7312 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/pre/normalizer_bands.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.933754 pyosv-0.0.8/pyosv/utils/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      116 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/utils/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     1695 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/utils/mapper.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      685 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/utils/paths.py
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3244 2023-10-23 13:06:27.000000 pyosv-0.0.8/pyosv/utils/printer.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.918765 pyosv-0.0.8/pyosv.egg-info/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     3277 2024-01-25 14:16:51.000000 pyosv-0.0.8/pyosv.egg-info/PKG-INFO
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      802 2024-01-25 14:16:51.000000 pyosv-0.0.8/pyosv.egg-info/SOURCES.txt
--rw-r--r--   0 asebastianelli (1445502215) 1276952531        1 2024-01-25 14:16:51.000000 pyosv-0.0.8/pyosv.egg-info/dependency_links.txt
--rw-r--r--   0 asebastianelli (1445502215) 1276952531       71 2024-01-25 14:16:51.000000 pyosv-0.0.8/pyosv.egg-info/requires.txt
--rw-r--r--   0 asebastianelli (1445502215) 1276952531       12 2024-01-25 14:16:51.000000 pyosv-0.0.8/pyosv.egg-info/top_level.txt
--rw-r--r--   0 asebastianelli (1445502215) 1276952531      809 2024-01-25 14:16:35.000000 pyosv-0.0.8/pyproject.toml
--rw-r--r--   0 asebastianelli (1445502215) 1276952531       38 2024-01-25 14:16:51.935501 pyosv-0.0.8/setup.cfg
--rw-r--r--   0 asebastianelli (1445502215) 1276952531     2420 2024-01-25 14:16:46.000000 pyosv-0.0.8/setup.py
-drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:16:51.934232 pyosv-0.0.8/tests/
--rw-r--r--   0 asebastianelli (1445502215) 1276952531        0 2023-10-23 13:06:27.000000 pyosv-0.0.8/tests/__init__.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.100805 pyosv-0.0.9/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1072 2023-10-23 13:06:27.000000 pyosv-0.0.9/LICENSE
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3600 2024-01-25 14:32:14.099175 pyosv-0.0.9/PKG-INFO
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1490 2024-01-25 14:29:32.000000 pyosv-0.0.9/README.md
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.056958 pyosv-0.0.9/pyosv/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      173 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/__init__.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.080565 pyosv-0.0.9/pyosv/ai/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      120 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/ai/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1662 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/ai/clustering.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     2197 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/ai/data_reduction.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.082387 pyosv-0.0.9/pyosv/freq/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      105 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/freq/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1813 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/freq/fft.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3705 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/freq/filters.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.085352 pyosv-0.0.9/pyosv/io/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      129 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/io/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     4052 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/io/batch_reader.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3390 2024-01-25 13:35:25.000000 pyosv-0.0.9/pyosv/io/reader.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     2443 2024-01-25 13:36:01.000000 pyosv-0.0.9/pyosv/io/writer.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.089349 pyosv-0.0.9/pyosv/plot/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      112 2024-01-25 14:22:01.000000 pyosv-0.0.9/pyosv/plot/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3793 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/plot/cube.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1715 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/plot/geo.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3533 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/plot/plot.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.091649 pyosv-0.0.9/pyosv/post/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      128 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/post/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1600 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/post/normalized_difference.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     5888 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/post/patch_extractor.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.094658 pyosv-0.0.9/pyosv/pre/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      191 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/pre/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     2857 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/pre/hist_normalizer.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     6158 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/pre/normalizer.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     7312 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/pre/normalizer_bands.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.098060 pyosv-0.0.9/pyosv/utils/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      116 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/utils/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     1695 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/utils/mapper.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      685 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/utils/paths.py
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3244 2023-10-23 13:06:27.000000 pyosv-0.0.9/pyosv/utils/printer.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.078543 pyosv-0.0.9/pyosv.egg-info/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     3600 2024-01-25 14:32:13.000000 pyosv-0.0.9/pyosv.egg-info/PKG-INFO
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      802 2024-01-25 14:32:13.000000 pyosv-0.0.9/pyosv.egg-info/SOURCES.txt
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531        1 2024-01-25 14:32:13.000000 pyosv-0.0.9/pyosv.egg-info/dependency_links.txt
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531       71 2024-01-25 14:32:13.000000 pyosv-0.0.9/pyosv.egg-info/requires.txt
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531       12 2024-01-25 14:32:13.000000 pyosv-0.0.9/pyosv.egg-info/top_level.txt
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531      809 2024-01-25 14:31:38.000000 pyosv-0.0.9/pyproject.toml
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531       38 2024-01-25 14:32:14.100912 pyosv-0.0.9/setup.cfg
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531     2420 2024-01-25 14:31:45.000000 pyosv-0.0.9/setup.py
+drwxr-xr-x   0 asebastianelli (1445502215) 1276952531        0 2024-01-25 14:32:14.098507 pyosv-0.0.9/tests/
+-rw-r--r--   0 asebastianelli (1445502215) 1276952531        0 2023-10-23 13:06:27.000000 pyosv-0.0.9/tests/__init__.py
```

### Comparing `pyosv-0.0.8/LICENSE` & `pyosv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/PKG-INFO` & `pyosv-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Open Satellite Vision
 Home-page: https://github.com/alessandrosebastianelli/opensv.git
 Author: Alessandro Sebastianelli
 Author-email: Alessandro Sebastianelli <alessandro.sebastianelli1995@gmail.com>
 License: Copyright (c) 2023-2023 Alessandro Sebastianelli
         
         Permission is hereby granted, free of charge, to any person
@@ -54,19 +54,37 @@
 
 This library comprises a collection of functions and classes tailored to manage satellite based data.
 
 <a class="btn btn-success" href="https://alessandrosebastianelli.github.io/opensv/pyosv.html" target="_blank">Click here to access the documentation</a>
 
 ## Installation
 
+You need to create a virtual environment
+
+```bash
+conda create -n osv python=3.10 -y
+conda activate osv
+conda install pip -y
+```
+
 This package is stored on [PyPi](https://pypi.org/project/pyosv/), you can easily install it using pip
 
 ```bash
 pip install --upgrade pyosv
 ```
 
-Although certain elements of this library draw from Mayavi, these package is not included in the library's prerequisites, and therefore, it will not be automatically installed. 
+Although certain elements of this library draw from Mayavi, these package is not included in the library's prerequisites, and therefore, it will not be automatically installed. To install it run the following command, once your virtual environment is active
+
+```bash
+pip install mayavi
+```
+
+or 
 
+```bash
+conda install mayavi
+```
+if there are issue with the first command.
 
 ## How to contribute
 
 [Click here](https://github.com/alessandrosebastianelli/opensv/issues/2)
```

### Comparing `pyosv-0.0.8/README.md` & `pyosv-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,37 @@
 
 This library comprises a collection of functions and classes tailored to manage satellite based data.
 
 <a class="btn btn-success" href="https://alessandrosebastianelli.github.io/opensv/pyosv.html" target="_blank">Click here to access the documentation</a>
 
 ## Installation
 
+You need to create a virtual environment
+
+```bash
+conda create -n osv python=3.10 -y
+conda activate osv
+conda install pip -y
+```
+
 This package is stored on [PyPi](https://pypi.org/project/pyosv/), you can easily install it using pip
 
 ```bash
 pip install --upgrade pyosv
 ```
 
-Although certain elements of this library draw from Mayavi, these package is not included in the library's prerequisites, and therefore, it will not be automatically installed. 
+Although certain elements of this library draw from Mayavi, these package is not included in the library's prerequisites, and therefore, it will not be automatically installed. To install it run the following command, once your virtual environment is active
+
+```bash
+pip install mayavi
+```
+
+or 
 
+```bash
+conda install mayavi
+```
+if there are issue with the first command.
 
 ## How to contribute
 
 [Click here](https://github.com/alessandrosebastianelli/opensv/issues/2)
```

### Comparing `pyosv-0.0.8/pyosv/ai/clustering.py` & `pyosv-0.0.9/pyosv/ai/clustering.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/ai/data_reduction.py` & `pyosv-0.0.9/pyosv/ai/data_reduction.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/freq/fft.py` & `pyosv-0.0.9/pyosv/freq/fft.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/freq/filters.py` & `pyosv-0.0.9/pyosv/freq/filters.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/io/batch_reader.py` & `pyosv-0.0.9/pyosv/io/batch_reader.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/io/reader.py` & `pyosv-0.0.9/pyosv/io/reader.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/io/writer.py` & `pyosv-0.0.9/pyosv/io/writer.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/plot/cube.py` & `pyosv-0.0.9/pyosv/plot/cube.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/plot/geo.py` & `pyosv-0.0.9/pyosv/plot/geo.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/plot/plot.py` & `pyosv-0.0.9/pyosv/plot/plot.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/post/normalized_difference.py` & `pyosv-0.0.9/pyosv/post/normalized_difference.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/post/patch_extractor.py` & `pyosv-0.0.9/pyosv/post/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/pre/hist_normalizer.py` & `pyosv-0.0.9/pyosv/pre/hist_normalizer.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/pre/normalizer.py` & `pyosv-0.0.9/pyosv/pre/normalizer.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/pre/normalizer_bands.py` & `pyosv-0.0.9/pyosv/pre/normalizer_bands.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/utils/mapper.py` & `pyosv-0.0.9/pyosv/utils/mapper.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/utils/paths.py` & `pyosv-0.0.9/pyosv/utils/paths.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv/utils/printer.py` & `pyosv-0.0.9/pyosv/utils/printer.py`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyosv.egg-info/PKG-INFO` & `pyosv-0.0.9/pyosv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Open Satellite Vision
 Home-page: https://github.com/alessandrosebastianelli/opensv.git
 Author: Alessandro Sebastianelli
 Author-email: Alessandro Sebastianelli <alessandro.sebastianelli1995@gmail.com>
 License: Copyright (c) 2023-2023 Alessandro Sebastianelli
         
         Permission is hereby granted, free of charge, to any person
@@ -54,19 +54,37 @@
 
 This library comprises a collection of functions and classes tailored to manage satellite based data.
 
 <a class="btn btn-success" href="https://alessandrosebastianelli.github.io/opensv/pyosv.html" target="_blank">Click here to access the documentation</a>
 
 ## Installation
 
+You need to create a virtual environment
+
+```bash
+conda create -n osv python=3.10 -y
+conda activate osv
+conda install pip -y
+```
+
 This package is stored on [PyPi](https://pypi.org/project/pyosv/), you can easily install it using pip
 
 ```bash
 pip install --upgrade pyosv
 ```
 
-Although certain elements of this library draw from Mayavi, these package is not included in the library's prerequisites, and therefore, it will not be automatically installed. 
+Although certain elements of this library draw from Mayavi, these package is not included in the library's prerequisites, and therefore, it will not be automatically installed. To install it run the following command, once your virtual environment is active
+
+```bash
+pip install mayavi
+```
+
+or 
 
+```bash
+conda install mayavi
+```
+if there are issue with the first command.
 
 ## How to contribute
 
 [Click here](https://github.com/alessandrosebastianelli/opensv/issues/2)
```

### Comparing `pyosv-0.0.8/pyosv.egg-info/SOURCES.txt` & `pyosv-0.0.9/pyosv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyosv-0.0.8/pyproject.toml` & `pyosv-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["numpy", "rasterio", "scikit-learn", "tqdm", "matplotlib", "scipy", "cartopy", "pyproj", "pyqt5"]
 
 [project]
 name = "pyosv"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Alessandro Sebastianelli", email="alessandro.sebastianelli1995@gmail.com" },
 ]
 description = "Python Open Satellite Vision"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pyosv-0.0.8/setup.py` & `pyosv-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             return file.read()
     except IOError:
         return ""
 
 # Package 
 HERE = pathlib.Path(__file__).parent
 PACKAGE_NAME  = 'pyosv'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 AUTHOR = 'Alessandro Sebastianelli'
 AUTHOR_EMAIL = 'alessandro.sebastianelli1995@gmail.com'
 URL = 'https://github.com/alessandrosebastianelli/opensv.git'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'OpenSV - Open Satellite Vision'
 LONG_DESCRIPTION = readme()
```

