# Comparing `tmp/prpy-0.2.2.tar.gz` & `tmp/prpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prpy-0.2.2.tar", last modified: Wed Apr 10 16:25:37 2024, max compression
+gzip compressed data, was "prpy-0.2.3.tar", last modified: Thu Apr 11 10:36:57 2024, max compression
```

## Comparing `prpy-0.2.2.tar` & `prpy-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.726260 prpy-0.2.2/
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.677487 prpy-0.2.2/.github/
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.681896 prpy-0.2.2/.github/workflows/
--rw-r--r--   0 prouast    (501) staff       (20)     1028 2024-04-10 16:12:37.000000 prpy-0.2.2/.github/workflows/main.yml
--rw-r--r--   0 prouast    (501) staff       (20)     1830 2024-04-10 16:03:39.000000 prpy-0.2.2/.gitignore
--rw-r--r--   0 prouast    (501) staff       (20)     1058 2024-04-10 16:03:39.000000 prpy-0.2.2/LICENSE
--rw-r--r--   0 prouast    (501) staff       (20)      196 2024-04-10 16:06:46.000000 prpy-0.2.2/MANIFEST.in
--rw-r--r--   0 prouast    (501) staff       (20)     2448 2024-04-10 16:25:37.725185 prpy-0.2.2/PKG-INFO
--rw-r--r--   0 prouast    (501) staff       (20)     1015 2024-04-10 16:07:49.000000 prpy-0.2.2/README.md
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.683387 prpy-0.2.2/prpy/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     1209 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/constants.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.690039 prpy-0.2.2/prpy/ffmpeg/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/ffmpeg/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     3126 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/ffmpeg/probe.py
--rw-r--r--   0 prouast    (501) staff       (20)    16971 2024-04-10 16:08:01.000000 prpy-0.2.2/prpy/ffmpeg/readwrite.py
--rw-r--r--   0 prouast    (501) staff       (20)     3195 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/ffmpeg/utils.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.695544 prpy-0.2.2/prpy/numpy/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/numpy/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     8314 2024-04-10 16:08:09.000000 prpy-0.2.2/prpy/numpy/face.py
--rw-r--r--   0 prouast    (501) staff       (20)     7064 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/numpy/image.py
--rw-r--r--   0 prouast    (501) staff       (20)     6395 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/numpy/metric.py
--rw-r--r--   0 prouast    (501) staff       (20)    21767 2024-04-10 16:08:15.000000 prpy-0.2.2/prpy/numpy/signal.py
--rw-r--r--   0 prouast    (501) staff       (20)     7764 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/numpy/stride_tricks.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.703443 prpy-0.2.2/prpy/tensorflow/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     7554 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/image.py
--rw-r--r--   0 prouast    (501) staff       (20)     4248 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/loss.py
--rw-r--r--   0 prouast    (501) staff       (20)     3384 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/lr_schedule.py
--rw-r--r--   0 prouast    (501) staff       (20)     7660 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/model_saver.py
--rw-r--r--   0 prouast    (501) staff       (20)     8525 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/nan.py
--rw-r--r--   0 prouast    (501) staff       (20)     9844 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/optimizer.py
--rw-r--r--   0 prouast    (501) staff       (20)     3326 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/tensorflow/signal.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.705526 prpy-0.2.2/prpy/torch/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/torch/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     7582 2024-04-10 16:03:39.000000 prpy-0.2.2/prpy/torch/model_saver.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.718993 prpy-0.2.2/prpy.egg-info/
--rw-r--r--   0 prouast    (501) staff       (20)     2448 2024-04-10 16:25:37.000000 prpy-0.2.2/prpy.egg-info/PKG-INFO
--rw-r--r--   0 prouast    (501) staff       (20)      977 2024-04-10 16:25:37.000000 prpy-0.2.2/prpy.egg-info/SOURCES.txt
--rw-r--r--   0 prouast    (501) staff       (20)        1 2024-04-10 16:25:37.000000 prpy-0.2.2/prpy.egg-info/dependency_links.txt
--rw-r--r--   0 prouast    (501) staff       (20)      200 2024-04-10 16:25:37.000000 prpy-0.2.2/prpy.egg-info/requires.txt
--rw-r--r--   0 prouast    (501) staff       (20)        5 2024-04-10 16:25:37.000000 prpy-0.2.2/prpy.egg-info/top_level.txt
--rw-r--r--   0 prouast    (501) staff       (20)     1076 2024-04-10 16:07:11.000000 prpy-0.2.2/pyproject.toml
--rw-r--r--   0 prouast    (501) staff       (20)       38 2024-04-10 16:25:37.726459 prpy-0.2.2/setup.cfg
--rw-r--r--   0 prouast    (501) staff       (20)       38 2024-04-10 16:03:39.000000 prpy-0.2.2/setup.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-10 16:25:37.716883 prpy-0.2.2/tests/
--rw-r--r--   0 prouast    (501) staff       (20)     2101 2024-04-10 16:08:25.000000 prpy-0.2.2/tests/conftest.py
--rw-r--r--   0 prouast    (501) staff       (20)     4210 2024-04-10 16:08:34.000000 prpy-0.2.2/tests/test_ffmpeg.py
--rw-r--r--   0 prouast    (501) staff       (20)     3886 2024-04-10 16:08:54.000000 prpy-0.2.2/tests/test_numpy_face.py
--rw-r--r--   0 prouast    (501) staff       (20)     3860 2024-04-10 16:09:05.000000 prpy-0.2.2/tests/test_numpy_image.py
--rw-r--r--   0 prouast    (501) staff       (20)     2499 2024-04-10 16:09:14.000000 prpy-0.2.2/tests/test_numpy_metric.py
--rw-r--r--   0 prouast    (501) staff       (20)    13187 2024-04-10 16:09:26.000000 prpy-0.2.2/tests/test_numpy_signal.py
--rw-r--r--   0 prouast    (501) staff       (20)     2943 2024-04-10 16:10:54.000000 prpy-0.2.2/tests/test_numpy_stride_tricks.py
--rw-r--r--   0 prouast    (501) staff       (20)    29110 2024-04-10 16:09:37.000000 prpy-0.2.2/tests/test_tensorflow.py
--rw-r--r--   0 prouast    (501) staff       (20)     4434 2024-04-10 16:09:41.000000 prpy-0.2.2/tests/test_torch.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.581313 prpy-0.2.3/
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.557300 prpy-0.2.3/.github/
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.560738 prpy-0.2.3/.github/workflows/
+-rw-r--r--   0 prouast    (501) staff       (20)     1028 2024-04-10 16:29:37.000000 prpy-0.2.3/.github/workflows/main.yml
+-rw-r--r--   0 prouast    (501) staff       (20)     1830 2024-04-10 16:03:39.000000 prpy-0.2.3/.gitignore
+-rw-r--r--   0 prouast    (501) staff       (20)     1058 2024-04-10 16:03:39.000000 prpy-0.2.3/LICENSE
+-rw-r--r--   0 prouast    (501) staff       (20)      196 2024-04-10 16:06:46.000000 prpy-0.2.3/MANIFEST.in
+-rw-r--r--   0 prouast    (501) staff       (20)     2448 2024-04-11 10:36:57.580673 prpy-0.2.3/PKG-INFO
+-rw-r--r--   0 prouast    (501) staff       (20)     1015 2024-04-10 16:07:49.000000 prpy-0.2.3/README.md
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.561434 prpy-0.2.3/prpy/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     1209 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/constants.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.565359 prpy-0.2.3/prpy/ffmpeg/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/ffmpeg/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3126 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/ffmpeg/probe.py
+-rw-r--r--   0 prouast    (501) staff       (20)    16979 2024-04-11 10:30:32.000000 prpy-0.2.3/prpy/ffmpeg/readwrite.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3195 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/ffmpeg/utils.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.568086 prpy-0.2.3/prpy/numpy/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/numpy/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     8359 2024-04-11 10:23:49.000000 prpy-0.2.3/prpy/numpy/face.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7074 2024-04-11 10:28:22.000000 prpy-0.2.3/prpy/numpy/image.py
+-rw-r--r--   0 prouast    (501) staff       (20)     6395 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/numpy/metric.py
+-rw-r--r--   0 prouast    (501) staff       (20)    21767 2024-04-10 16:08:15.000000 prpy-0.2.3/prpy/numpy/signal.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7764 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/numpy/stride_tricks.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.571314 prpy-0.2.3/prpy/tensorflow/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7554 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/image.py
+-rw-r--r--   0 prouast    (501) staff       (20)     4248 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/loss.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3384 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/lr_schedule.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7660 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/model_saver.py
+-rw-r--r--   0 prouast    (501) staff       (20)     8525 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/nan.py
+-rw-r--r--   0 prouast    (501) staff       (20)     9844 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/optimizer.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3326 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/tensorflow/signal.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.571954 prpy-0.2.3/prpy/torch/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/torch/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7582 2024-04-10 16:03:39.000000 prpy-0.2.3/prpy/torch/model_saver.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.577224 prpy-0.2.3/prpy.egg-info/
+-rw-r--r--   0 prouast    (501) staff       (20)     2448 2024-04-11 10:36:57.000000 prpy-0.2.3/prpy.egg-info/PKG-INFO
+-rw-r--r--   0 prouast    (501) staff       (20)      977 2024-04-11 10:36:57.000000 prpy-0.2.3/prpy.egg-info/SOURCES.txt
+-rw-r--r--   0 prouast    (501) staff       (20)        1 2024-04-11 10:36:57.000000 prpy-0.2.3/prpy.egg-info/dependency_links.txt
+-rw-r--r--   0 prouast    (501) staff       (20)      200 2024-04-11 10:36:57.000000 prpy-0.2.3/prpy.egg-info/requires.txt
+-rw-r--r--   0 prouast    (501) staff       (20)        5 2024-04-11 10:36:57.000000 prpy-0.2.3/prpy.egg-info/top_level.txt
+-rw-r--r--   0 prouast    (501) staff       (20)     1076 2024-04-10 16:07:11.000000 prpy-0.2.3/pyproject.toml
+-rw-r--r--   0 prouast    (501) staff       (20)       38 2024-04-11 10:36:57.581435 prpy-0.2.3/setup.cfg
+-rw-r--r--   0 prouast    (501) staff       (20)       38 2024-04-10 16:03:39.000000 prpy-0.2.3/setup.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 10:36:57.575741 prpy-0.2.3/tests/
+-rw-r--r--   0 prouast    (501) staff       (20)     2101 2024-04-10 16:08:25.000000 prpy-0.2.3/tests/conftest.py
+-rw-r--r--   0 prouast    (501) staff       (20)     4210 2024-04-10 16:08:34.000000 prpy-0.2.3/tests/test_ffmpeg.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3886 2024-04-10 16:08:54.000000 prpy-0.2.3/tests/test_numpy_face.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3860 2024-04-10 16:09:05.000000 prpy-0.2.3/tests/test_numpy_image.py
+-rw-r--r--   0 prouast    (501) staff       (20)     2499 2024-04-10 16:09:14.000000 prpy-0.2.3/tests/test_numpy_metric.py
+-rw-r--r--   0 prouast    (501) staff       (20)    13187 2024-04-10 16:09:26.000000 prpy-0.2.3/tests/test_numpy_signal.py
+-rw-r--r--   0 prouast    (501) staff       (20)     2943 2024-04-10 16:10:54.000000 prpy-0.2.3/tests/test_numpy_stride_tricks.py
+-rw-r--r--   0 prouast    (501) staff       (20)    29110 2024-04-10 16:09:37.000000 prpy-0.2.3/tests/test_tensorflow.py
+-rw-r--r--   0 prouast    (501) staff       (20)     4434 2024-04-10 16:09:41.000000 prpy-0.2.3/tests/test_torch.py
```

### Comparing `prpy-0.2.2/.github/workflows/main.yml` & `prpy-0.2.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/.gitignore` & `prpy-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/LICENSE` & `prpy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/PKG-INFO` & `prpy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collection of Python utils for signal, image, and video processing
 Author-email: Philipp Rouast <philipp@rouast.com>
 License: MIT License
 Project-URL: Repository, https://github.com/prouast/prpy.git
 Project-URL: Issues, https://github.com/prouast/prpy/issues
 Keywords: python,numpy,ffmpeg,tensorflow,torch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prpy-0.2.2/README.md` & `prpy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/__init__.py` & `prpy-0.2.3/prpy/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/constants.py` & `prpy-0.2.3/prpy/constants.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/ffmpeg/__init__.py` & `prpy-0.2.3/prpy/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/ffmpeg/probe.py` & `prpy-0.2.3/prpy/ffmpeg/probe.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/ffmpeg/readwrite.py` & `prpy-0.2.3/prpy/ffmpeg/readwrite.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
   Args:
     stream: The ffmpeg stream
     fps: The existing frame rate
     n: The existing number of frames
     w: The existing width
     h: The existing height
-    target_fps: Try to downsample frames to achieve this framerate (optional)
+    target_fps: Downsample frames to approximate this framerate (optional)
     crop: Coords and sizes for spatial cropping (x, y, width, height) (optional)
     scale: Size(s) for spatial scaling. Scalar or (width, height) (optional)
     trim: Frame numbers for temporal trimming (start, end) (optional)
     preserve_aspect_ratio: Preserve the aspect ratio if scaling
     scale_algorithm: The algorithm used for scaling.
       Supported: bicubic, bilinear, area, lanczos. Default: bicubic
   Returns:
@@ -121,22 +121,22 @@
   """
   assert isinstance(stream, ffmpeg.nodes.FilterableStream)
   assert isinstance(fps, (float, int))
   assert isinstance(n, int)
   assert isinstance(w, int)
   assert isinstance(h, int)
   assert target_fps is None or isinstance(target_fps, (float, int))
-  assert crop is None or (isinstance(crop, tuple) and len(crop) == 4 and all(isinstance(i, int) for i in crop))
+  assert crop is None or (isinstance(crop, tuple) and len(crop) == 4 and all(isinstance(i, int, np.int64) for i in crop))
   assert scale is None or isinstance(scale, int) or (isinstance(scale, tuple) and len(scale) == 2 and all(isinstance(i, int) for i in scale))
   assert trim is None or (isinstance(trim, tuple) and len(trim) == 2 and all(isinstance(i, int) for i in trim))
   assert isinstance(preserve_aspect_ratio, bool)
   assert isinstance(scale_algorithm, str)
   ds_factor = 1
   if target_fps is not None and target_fps > fps: logging.warn("target_fps should not be greater than fps. Ignoring.")
-  elif target_fps is not None: ds_factor = int(fps // target_fps)
+  elif target_fps is not None: ds_factor = round(fps / target_fps)
   # Target number of frames
   target_n = trim[1] - trim[0] if trim is not None else n
   target_n = int(target_n / ds_factor)
   # Target size after taking into account cropping
   target_w = crop[2] if crop is not None else w
   target_h = crop[3] if crop is not None else h
   # Target size after taking into account scaling
```

### Comparing `prpy-0.2.2/prpy/ffmpeg/utils.py` & `prpy-0.2.3/prpy/ffmpeg/utils.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/numpy/__init__.py` & `prpy-0.2.3/prpy/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/numpy/face.py` & `prpy-0.2.3/prpy/numpy/face.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 # SOFTWARE.
 
 import numpy as np
 from prpy.numpy.image import crop_slice_resize
 from typing import Tuple, Union
 
 def _get_roi_from_det(
-    det: tuple,
+    det: Union[tuple, np.ndarray],
     rel_change: tuple,
     clip_dims: Union[tuple, None] = None
   ) -> Tuple[int, int, int, int]:
   """Convert face detection to roi by relative add/reduce.
 
   Args:
     det: The face detection [0, H/W] in format (x0, y0, x1, y1).
     rel_change: The relative change to make in format (left, top, right, bottom).
     clip_dims: tuple (frame_w, frame_h) to clip the result to (optional).
   Returns:
     out: The roi [0, H/W] in format (x0, y0, x1, y1)
   """
-  assert isinstance(det, tuple) and len(det) == 4 and all(isinstance(i, int) for i in det)
+  assert isinstance(det, (tuple, np.ndarray)) and len(det) == 4 and all(isinstance(i, (int, np.int64)) for i in det)
   assert det[2] > det[0]
   assert det[3] > det[1]
   assert isinstance(rel_change, tuple) and len(rel_change) == 4 and all(isinstance(i, float) for i in rel_change)
   assert clip_dims is None or (isinstance(clip_dims, tuple) and len(clip_dims) == 2 and all(isinstance(i, int) for i in clip_dims))
   def _clip_dims(val, min_dim, max_dim):
     return min(max(val, min_dim), max_dim)
   det_w = det[2]-det[0]
```

### Comparing `prpy-0.2.2/prpy/numpy/image.py` & `prpy-0.2.3/prpy/numpy/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     scale_algorithm: The algorithm used for scaling.
       Supports: bicubic, bilinear, area (not for PIL!), lanczos. Default: bicubic
   Returns:
     result: The processed frame(s) as float32 shape (h, w, 3) or (n_frames, h, w, 3)
   """
   assert isinstance(inputs, np.ndarray) and (len(inputs.shape) == 3 or len(inputs.shape) == 4)
   assert isinstance(target_size, int) or (isinstance(target_size, (tuple, list)) and len(target_size) == 2 and all(isinstance(i, int) for i in target_size))
-  assert roi is None or (isinstance(roi, (tuple, list)) and len(roi) == 4 and all(isinstance(i, int) for i in roi) and roi[2] > roi[0] and roi[3] > roi[1])
+  assert roi is None or (isinstance(roi, (tuple, list)) and len(roi) == 4 and all(isinstance(i, int, np.int64) for i in roi) and roi[2] > roi[0] and roi[3] > roi[1])
   assert target_idxs is None or isinstance(target_idxs, np.ndarray) or (isinstance(target_idxs, (tuple, list)) and all(isinstance(i, int) for i in target_idxs))
   assert isinstance(preserve_aspect_ratio, bool)
   assert isinstance(keepdims, bool)
   assert isinstance(library, str)
   assert isinstance(scale_algorithm, str)
   unpack_target_size = lambda x: (x[0], x[1]) if isinstance(x, (list, tuple)) else (x, x)
   target_height, target_width = unpack_target_size(target_size)
```

### Comparing `prpy-0.2.2/prpy/numpy/metric.py` & `prpy-0.2.3/prpy/numpy/metric.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/numpy/signal.py` & `prpy-0.2.3/prpy/numpy/signal.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/numpy/stride_tricks.py` & `prpy-0.2.3/prpy/numpy/stride_tricks.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/__init__.py` & `prpy-0.2.3/prpy/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/image.py` & `prpy-0.2.3/prpy/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/loss.py` & `prpy-0.2.3/prpy/tensorflow/loss.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/lr_schedule.py` & `prpy-0.2.3/prpy/tensorflow/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/model_saver.py` & `prpy-0.2.3/prpy/tensorflow/model_saver.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/nan.py` & `prpy-0.2.3/prpy/tensorflow/nan.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/optimizer.py` & `prpy-0.2.3/prpy/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/tensorflow/signal.py` & `prpy-0.2.3/prpy/tensorflow/signal.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/torch/__init__.py` & `prpy-0.2.3/prpy/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy/torch/model_saver.py` & `prpy-0.2.3/prpy/torch/model_saver.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/prpy.egg-info/PKG-INFO` & `prpy-0.2.3/prpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collection of Python utils for signal, image, and video processing
 Author-email: Philipp Rouast <philipp@rouast.com>
 License: MIT License
 Project-URL: Repository, https://github.com/prouast/prpy.git
 Project-URL: Issues, https://github.com/prouast/prpy/issues
 Keywords: python,numpy,ffmpeg,tensorflow,torch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prpy-0.2.2/prpy.egg-info/SOURCES.txt` & `prpy-0.2.3/prpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/pyproject.toml` & `prpy-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/conftest.py` & `prpy-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_ffmpeg.py` & `prpy-0.2.3/tests/test_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_numpy_face.py` & `prpy-0.2.3/tests/test_numpy_face.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_numpy_image.py` & `prpy-0.2.3/tests/test_numpy_image.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_numpy_metric.py` & `prpy-0.2.3/tests/test_numpy_metric.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_numpy_signal.py` & `prpy-0.2.3/tests/test_numpy_signal.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_numpy_stride_tricks.py` & `prpy-0.2.3/tests/test_numpy_stride_tricks.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_tensorflow.py` & `prpy-0.2.3/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.2/tests/test_torch.py` & `prpy-0.2.3/tests/test_torch.py`

 * *Files identical despite different names*

