# Comparing `tmp/dstool-0.1.0b0.tar.gz` & `tmp/dstool-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstool-0.1.0b0.tar", last modified: Sat Apr  6 18:21:54 2024, max compression
+gzip compressed data, was "dstool-0.1.0rc0.tar", last modified: Thu Apr 11 15:38:47 2024, max compression
```

## Comparing `dstool-0.1.0b0.tar` & `dstool-0.1.0rc0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.028596 dstool-0.1.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 18:21:45.000000 dstool-0.1.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-06 18:21:45.000000 dstool-0.1.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-06 18:21:54.028596 dstool-0.1.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-06 18:21:45.000000 dstool-0.1.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.020596 dstool-0.1.0b0/dstool/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.024596 dstool-0.1.0b0/dstool/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/decorators/class_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/decorators/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/decorators/measure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.024596 dstool-0.1.0b0/dstool/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/parallel/parallel_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.024596 dstool-0.1.0b0/dstool/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.024596 dstool-0.1.0b0/dstool/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 18:21:45.000000 dstool-0.1.0b0/dstool/tensors/safetensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.028596 dstool-0.1.0b0/dstool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-06 18:21:53.000000 dstool-0.1.0b0/dstool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 18:21:53.000000 dstool-0.1.0b0/dstool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:21:53.000000 dstool-0.1.0b0/dstool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 18:21:53.000000 dstool-0.1.0b0/dstool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 18:21:53.000000 dstool-0.1.0b0/dstool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 18:21:53.000000 dstool-0.1.0b0/dstool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:21:54.028596 dstool-0.1.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-06 18:21:45.000000 dstool-0.1.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:54.024596 dstool-0.1.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:21:45.000000 dstool-0.1.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-06 18:21:45.000000 dstool-0.1.0b0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 18:21:45.000000 dstool-0.1.0b0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.176751 dstool-0.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-11 15:38:47.176751 dstool-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.172751 dstool-0.1.0rc0/dstool/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.172751 dstool-0.1.0rc0/dstool/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/decorators/class_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/decorators/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/decorators/measure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.172751 dstool-0.1.0rc0/dstool/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/parallel/parallel_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.172751 dstool-0.1.0rc0/dstool/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.176751 dstool-0.1.0rc0/dstool/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/tensors/lossless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/dstool/tensors/safetensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.176751 dstool-0.1.0rc0/dstool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-11 15:38:47.000000 dstool-0.1.0rc0/dstool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 15:38:47.000000 dstool-0.1.0rc0/dstool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:38:47.000000 dstool-0.1.0rc0/dstool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 15:38:47.000000 dstool-0.1.0rc0/dstool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 15:38:47.000000 dstool-0.1.0rc0/dstool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 15:38:47.000000 dstool-0.1.0rc0/dstool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:38:47.176751 dstool-0.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:47.176751 dstool-0.1.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 15:38:34.000000 dstool-0.1.0rc0/tests/test_base.py
```

### Comparing `dstool-0.1.0b0/LICENSE` & `dstool-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0b0/PKG-INFO` & `dstool-0.1.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: dstool
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: Awesome dstool created by xzyaoi
 Home-page: https://github.com/xzyaoi/dstool/
 Author: xzyaoi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: plotly
 Requires-Dist: rich
 Requires-Dist: safetensors
 Requires-Dist: typer
+Requires-Dist: py7zr
+Requires-Dist: zarr
+Requires-Dist: cupy-cuda12x
+Requires-Dist: cchardet
+Requires-Dist: scikit-build
+Requires-Dist: pytest
+Requires-Dist: numcodecs
+Requires-Dist: gekko
+Requires-Dist: ninja
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `dstool-0.1.0b0/README.md` & `dstool-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0b0/dstool/decorators/debugger.py` & `dstool-0.1.0rc0/dstool/decorators/debugger.py`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0b0/dstool/decorators/measure.py` & `dstool-0.1.0rc0/dstool/decorators/measure.py`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0b0/dstool/parallel/parallel_func.py` & `dstool-0.1.0rc0/dstool/parallel/parallel_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from multiprocessing import cpu_count
 from typing import Callable
+
 from joblib import Parallel, delayed
 
 
 def parallel(
     func=None, args=(), merge_func=lambda x: x, parallelism=cpu_count()
 ):
```

### Comparing `dstool-0.1.0b0/dstool/plot/style.py` & `dstool-0.1.0rc0/dstool/plot/style.py`

 * *Files identical despite different names*

### Comparing `dstool-0.1.0b0/dstool.egg-info/PKG-INFO` & `dstool-0.1.0rc0/dstool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: dstool
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: Awesome dstool created by xzyaoi
 Home-page: https://github.com/xzyaoi/dstool/
 Author: xzyaoi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: plotly
 Requires-Dist: rich
 Requires-Dist: safetensors
 Requires-Dist: typer
+Requires-Dist: py7zr
+Requires-Dist: zarr
+Requires-Dist: cupy-cuda12x
+Requires-Dist: cchardet
+Requires-Dist: scikit-build
+Requires-Dist: pytest
+Requires-Dist: numcodecs
+Requires-Dist: gekko
+Requires-Dist: ninja
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `dstool-0.1.0b0/dstool.egg-info/SOURCES.txt` & `dstool-0.1.0rc0/dstool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 dstool/decorators/debugger.py
 dstool/decorators/measure.py
 dstool/parallel/__init__.py
 dstool/parallel/parallel_func.py
 dstool/plot/__init__.py
 dstool/plot/style.py
 dstool/tensors/__init__.py
+dstool/tensors/lossless.py
 dstool/tensors/safetensors.py
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
```

### Comparing `dstool-0.1.0b0/setup.py` & `dstool-0.1.0rc0/setup.py`

 * *Files identical despite different names*

