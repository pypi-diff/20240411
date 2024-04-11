# Comparing `tmp/svc_toolkit-1.0.8.tar.gz` & `tmp/svc_toolkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svc_toolkit-1.0.8.tar", max compression
+gzip compressed data, was "svc_toolkit-1.0.9.tar", max compression
```

## Comparing `svc_toolkit-1.0.8.tar` & `svc_toolkit-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2024-04-11 02:25:59.064065 svc_toolkit-1.0.8/LICENSE
--rw-r--r--   0        0        0     2049 2024-04-11 02:25:59.064065 svc_toolkit-1.0.8/README.md
--rw-r--r--   0        0        0     1561 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/conversion/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/conversion/converter.py
--rw-r--r--   0        0        0     2443 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/conversion/converter_trainer.py
--rw-r--r--   0        0        0     1056 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/conversion/mixer.py
--rw-r--r--   0        0        0    12669 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/img/icon.png
--rw-r--r--   0        0        0    31498 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/img/loading.gif
--rw-r--r--   0        0        0     2377 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/main.py
--rw-r--r--   0        0        0      400 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/models/manifest.yml
--rw-r--r--   0        0        0        0 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/presenter/__init__.py
--rw-r--r--   0        0        0      293 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/presenter/common.py
--rw-r--r--   0        0        0      828 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/presenter/conversion.py
--rw-r--r--   0        0        0      613 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/presenter/mixing.py
--rw-r--r--   0        0        0     2595 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/presenter/separation.py
--rw-r--r--   0        0        0      675 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/presenter/training.py
--rw-r--r--   0        0        0        0 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/__init__.py
--rw-r--r--   0        0        0      987 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/audio.py
--rw-r--r--   0        0        0      196 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/constants.py
--rw-r--r--   0        0        0     7065 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/data.py
--rw-r--r--   0        0        0     2168 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/evaluator.py
--rw-r--r--   0        0        0     1985 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/logger.py
--rw-r--r--   0        0        0     7133 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/models.py
--rw-r--r--   0        0        0     3580 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/preprocess.py
--rw-r--r--   0        0        0     4697 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/separator.py
--rw-r--r--   0        0        0      752 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation/utility.py
--rw-r--r--   0        0        0     1471 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation_evaluation.py
--rw-r--r--   0        0        0     1214 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation_preprocess.py
--rw-r--r--   0        0        0     4146 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/separation_train.py
--rw-r--r--   0        0        0        0 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/utility/__init__.py
--rw-r--r--   0        0        0      239 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/utility/functions.py
--rw-r--r--   0        0        0        0 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/__init__.py
--rw-r--r--   0        0        0     7941 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/common.py
--rw-r--r--   0        0        0     7972 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/conversion.py
--rw-r--r--   0        0        0      760 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/loading_overlay.py
--rw-r--r--   0        0        0      993 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/loading_window.py
--rw-r--r--   0        0        0      578 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/main_window.py
--rw-r--r--   0        0        0     3326 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/mixing.py
--rw-r--r--   0        0        0     5075 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/separation.py
--rw-r--r--   0        0        0     5289 2024-04-11 02:25:59.080065 svc_toolkit-1.0.8/src/svc_toolkit/widget/training.py
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 svc_toolkit-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 02:58:35.715060 svc_toolkit-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2049 2024-04-11 02:58:35.715060 svc_toolkit-1.0.9/README.md
+-rw-r--r--   0        0        0     1561 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/conversion/__init__.py
+-rw-r--r--   0        0        0     1502 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/conversion/converter.py
+-rw-r--r--   0        0        0     2443 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/conversion/converter_trainer.py
+-rw-r--r--   0        0        0     1056 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/conversion/mixer.py
+-rw-r--r--   0        0        0    12669 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/img/icon.png
+-rw-r--r--   0        0        0    31498 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/img/loading.gif
+-rw-r--r--   0        0        0     2377 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/main.py
+-rw-r--r--   0        0        0      400 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/models/manifest.yml
+-rw-r--r--   0        0        0        0 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/presenter/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/presenter/common.py
+-rw-r--r--   0        0        0      828 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/presenter/conversion.py
+-rw-r--r--   0        0        0      613 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/presenter/mixing.py
+-rw-r--r--   0        0        0     2595 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/presenter/separation.py
+-rw-r--r--   0        0        0      675 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/presenter/training.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/audio.py
+-rw-r--r--   0        0        0      196 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/constants.py
+-rw-r--r--   0        0        0     7065 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/data.py
+-rw-r--r--   0        0        0     2168 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/evaluator.py
+-rw-r--r--   0        0        0     1985 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/logger.py
+-rw-r--r--   0        0        0     7133 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/models.py
+-rw-r--r--   0        0        0     3580 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/preprocess.py
+-rw-r--r--   0        0        0     4697 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/separator.py
+-rw-r--r--   0        0        0      752 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation/utility.py
+-rw-r--r--   0        0        0     1471 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation_evaluation.py
+-rw-r--r--   0        0        0     1214 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation_preprocess.py
+-rw-r--r--   0        0        0     4146 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/separation_train.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/utility/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/utility/functions.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/__init__.py
+-rw-r--r--   0        0        0     7941 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/common.py
+-rw-r--r--   0        0        0     7972 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/conversion.py
+-rw-r--r--   0        0        0      760 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/loading_overlay.py
+-rw-r--r--   0        0        0      993 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/loading_window.py
+-rw-r--r--   0        0        0      578 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/main_window.py
+-rw-r--r--   0        0        0     3326 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/mixing.py
+-rw-r--r--   0        0        0     5075 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/separation.py
+-rw-r--r--   0        0        0     5289 2024-04-11 02:58:35.731060 svc_toolkit-1.0.9/src/svc_toolkit/widget/training.py
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 svc_toolkit-1.0.9/PKG-INFO
```

### Comparing `svc_toolkit-1.0.8/LICENSE` & `svc_toolkit-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/README.md` & `svc_toolkit-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/pyproject.toml` & `svc_toolkit-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svc-toolkit"
-version = "1.0.8"
+version = "1.0.9"
 description = "A self-contained singing voice conversion application using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI."
 authors = ["jljl1337 <lckjack123@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jljl1337/svc-toolkit"
 documentation = "https://jljl1337.github.io/svc-toolkit/"
 classifiers = [
```

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/conversion/converter.py` & `svc_toolkit-1.0.9/src/svc_toolkit/conversion/converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,11 +37,11 @@
         output_wave, _output_sr = load(output_path, mono=False, sr=None)
 
         # Set a ndarray with zeros to the same shape as the input
         new_output_wave = np.zeros_like(input_wave)
 
         # Save the output file with the same number of channels
         for i in range(num_channels):
-            new_output_wave[i] = output_wave[i]
+            new_output_wave[i] = output_wave
 
         # Save the output file with the same number of channels
         sf.write(output_path, new_output_wave.T, _output_sr)
```

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/conversion/converter_trainer.py` & `svc_toolkit-1.0.9/src/svc_toolkit/conversion/converter_trainer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/conversion/mixer.py` & `svc_toolkit-1.0.9/src/svc_toolkit/conversion/mixer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/img/icon.png` & `svc_toolkit-1.0.9/src/svc_toolkit/img/icon.png`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/img/loading.gif` & `svc_toolkit-1.0.9/src/svc_toolkit/img/loading.gif`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/main.py` & `svc_toolkit-1.0.9/src/svc_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/presenter/conversion.py` & `svc_toolkit-1.0.9/src/svc_toolkit/presenter/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/presenter/mixing.py` & `svc_toolkit-1.0.9/src/svc_toolkit/presenter/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/presenter/separation.py` & `svc_toolkit-1.0.9/src/svc_toolkit/presenter/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/presenter/training.py` & `svc_toolkit-1.0.9/src/svc_toolkit/presenter/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/audio.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/audio.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/data.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/data.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/evaluator.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/evaluator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/logger.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/logger.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/models.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/models.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/preprocess.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/separator.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/separator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation/utility.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation/utility.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation_evaluation.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation_evaluation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation_preprocess.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation_preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/separation_train.py` & `svc_toolkit-1.0.9/src/svc_toolkit/separation_train.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/common.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/common.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/conversion.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/loading_overlay.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/loading_overlay.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/loading_window.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/loading_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/main_window.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/main_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/mixing.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/separation.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/src/svc_toolkit/widget/training.py` & `svc_toolkit-1.0.9/src/svc_toolkit/widget/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.8/PKG-INFO` & `svc_toolkit-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svc-toolkit
-Version: 1.0.8
+Version: 1.0.9
 Summary: A self-contained singing voice conversion application using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI.
 Home-page: https://github.com/jljl1337/svc-toolkit
 License: MIT
 Author: jljl1337
 Author-email: lckjack123@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

