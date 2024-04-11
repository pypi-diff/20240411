# Comparing `tmp/svc_toolkit-1.0.6.tar.gz` & `tmp/svc_toolkit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svc_toolkit-1.0.6.tar", max compression
+gzip compressed data, was "svc_toolkit-1.0.7.tar", max compression
```

## Comparing `svc_toolkit-1.0.6.tar` & `svc_toolkit-1.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2024-04-10 23:59:17.258379 svc_toolkit-1.0.6/LICENSE
--rw-r--r--   0        0        0     2049 2024-04-10 23:59:17.258379 svc_toolkit-1.0.6/README.md
--rw-r--r--   0        0        0     1548 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/__init__.py
--rw-r--r--   0        0        0      787 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter.py
--rw-r--r--   0        0        0     2443 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter_trainer.py
--rw-r--r--   0        0        0     1056 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/mixer.py
--rw-r--r--   0        0        0    12669 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/img/icon.png
--rw-r--r--   0        0        0    31498 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/img/loading.gif
--rw-r--r--   0        0        0     2377 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/main.py
--rw-r--r--   0        0        0      400 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/models/manifest.yml
--rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/__init__.py
--rw-r--r--   0        0        0      293 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/common.py
--rw-r--r--   0        0        0      828 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/conversion.py
--rw-r--r--   0        0        0      613 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/mixing.py
--rw-r--r--   0        0        0     2595 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/separation.py
--rw-r--r--   0        0        0      675 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/training.py
--rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/__init__.py
--rw-r--r--   0        0        0      987 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/audio.py
--rw-r--r--   0        0        0      196 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/constants.py
--rw-r--r--   0        0        0     7065 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/data.py
--rw-r--r--   0        0        0     2168 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/evaluator.py
--rw-r--r--   0        0        0     1985 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/logger.py
--rw-r--r--   0        0        0     7133 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/models.py
--rw-r--r--   0        0        0     3580 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/preprocess.py
--rw-r--r--   0        0        0     4697 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/separator.py
--rw-r--r--   0        0        0      752 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/utility.py
--rw-r--r--   0        0        0     1471 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation_evaluation.py
--rw-r--r--   0        0        0     1214 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation_preprocess.py
--rw-r--r--   0        0        0     4146 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation_train.py
--rw-r--r--   0        0        0        0 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/utility/__init__.py
--rw-r--r--   0        0        0      239 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/utility/functions.py
--rw-r--r--   0        0        0        0 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/__init__.py
--rw-r--r--   0        0        0     7941 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/common.py
--rw-r--r--   0        0        0     7972 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/conversion.py
--rw-r--r--   0        0        0      760 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_overlay.py
--rw-r--r--   0        0        0      993 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_window.py
--rw-r--r--   0        0        0      578 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/main_window.py
--rw-r--r--   0        0        0     3326 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/mixing.py
--rw-r--r--   0        0        0     5075 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/separation.py
--rw-r--r--   0        0        0     5289 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/training.py
--rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 svc_toolkit-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 01:30:09.204032 svc_toolkit-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2049 2024-04-11 01:30:09.204032 svc_toolkit-1.0.7/README.md
+-rw-r--r--   0        0        0     1561 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/conversion/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/conversion/converter.py
+-rw-r--r--   0        0        0     2443 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/conversion/converter_trainer.py
+-rw-r--r--   0        0        0     1056 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/conversion/mixer.py
+-rw-r--r--   0        0        0    12669 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/img/icon.png
+-rw-r--r--   0        0        0    31498 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/img/loading.gif
+-rw-r--r--   0        0        0     2377 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/main.py
+-rw-r--r--   0        0        0      400 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/models/manifest.yml
+-rw-r--r--   0        0        0        0 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/presenter/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/presenter/common.py
+-rw-r--r--   0        0        0      828 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/presenter/conversion.py
+-rw-r--r--   0        0        0      613 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/presenter/mixing.py
+-rw-r--r--   0        0        0     2595 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/presenter/separation.py
+-rw-r--r--   0        0        0      675 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/presenter/training.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/audio.py
+-rw-r--r--   0        0        0      196 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/constants.py
+-rw-r--r--   0        0        0     7065 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/data.py
+-rw-r--r--   0        0        0     2168 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/evaluator.py
+-rw-r--r--   0        0        0     1985 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/logger.py
+-rw-r--r--   0        0        0     7133 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/models.py
+-rw-r--r--   0        0        0     3580 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/preprocess.py
+-rw-r--r--   0        0        0     4697 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/separator.py
+-rw-r--r--   0        0        0      752 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation/utility.py
+-rw-r--r--   0        0        0     1471 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation_evaluation.py
+-rw-r--r--   0        0        0     1214 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation_preprocess.py
+-rw-r--r--   0        0        0     4146 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/separation_train.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/utility/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/utility/functions.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/__init__.py
+-rw-r--r--   0        0        0     7941 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/common.py
+-rw-r--r--   0        0        0     7972 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/conversion.py
+-rw-r--r--   0        0        0      760 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/loading_overlay.py
+-rw-r--r--   0        0        0      993 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/loading_window.py
+-rw-r--r--   0        0        0      578 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/main_window.py
+-rw-r--r--   0        0        0     3326 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/mixing.py
+-rw-r--r--   0        0        0     5075 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/separation.py
+-rw-r--r--   0        0        0     5289 2024-04-11 01:30:09.220032 svc_toolkit-1.0.7/src/svc_toolkit/widget/training.py
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 svc_toolkit-1.0.7/PKG-INFO
```

### Comparing `svc_toolkit-1.0.6/LICENSE` & `svc_toolkit-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/README.md` & `svc_toolkit-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/pyproject.toml` & `svc_toolkit-1.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svc-toolkit"
-version = "1.0.6"
+version = "1.0.7"
 description = "A self-contained singing voice conversion application using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI."
 authors = ["jljl1337 <lckjack123@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jljl1337/svc-toolkit"
 documentation = "https://jljl1337.github.io/svc-toolkit/"
 classifiers = [
@@ -18,14 +18,15 @@
 svct = "svc_toolkit.main:main"
 vs-preprocess = "svc_toolkit.separation_preprocess:main"
 vs-train = "svc_toolkit.separation_train:main"
 vs-eval = "svc_toolkit.separation_train:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
+pip = "24.0"
 numpy = "1.26.3"
 scipy = "1.12.0"
 pyyaml = "6.0.1"
 torch = "2.1.1"
 torchaudio = "2.1.1"
 lightning = "2.1.3"
 torchmetrics = "1.2.0"
```

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter.py` & `svc_toolkit-1.0.7/src/svc_toolkit/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter_trainer.py` & `svc_toolkit-1.0.7/src/svc_toolkit/conversion/converter_trainer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/conversion/mixer.py` & `svc_toolkit-1.0.7/src/svc_toolkit/conversion/mixer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/img/icon.png` & `svc_toolkit-1.0.7/src/svc_toolkit/img/icon.png`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/img/loading.gif` & `svc_toolkit-1.0.7/src/svc_toolkit/img/loading.gif`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/main.py` & `svc_toolkit-1.0.7/src/svc_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/presenter/conversion.py` & `svc_toolkit-1.0.7/src/svc_toolkit/presenter/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/presenter/mixing.py` & `svc_toolkit-1.0.7/src/svc_toolkit/presenter/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/presenter/separation.py` & `svc_toolkit-1.0.7/src/svc_toolkit/presenter/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/presenter/training.py` & `svc_toolkit-1.0.7/src/svc_toolkit/presenter/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/audio.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/audio.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/data.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/data.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/evaluator.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/evaluator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/logger.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/logger.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/models.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/models.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/preprocess.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/separator.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/separator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation/utility.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation/utility.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation_evaluation.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation_evaluation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation_preprocess.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation_preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/separation_train.py` & `svc_toolkit-1.0.7/src/svc_toolkit/separation_train.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/common.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/common.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/conversion.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_overlay.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/loading_overlay.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_window.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/loading_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/main_window.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/main_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/mixing.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/separation.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/src/svc_toolkit/widget/training.py` & `svc_toolkit-1.0.7/src/svc_toolkit/widget/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.6/PKG-INFO` & `svc_toolkit-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svc-toolkit
-Version: 1.0.6
+Version: 1.0.7
 Summary: A self-contained singing voice conversion application using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI.
 Home-page: https://github.com/jljl1337/svc-toolkit
 License: MIT
 Author: jljl1337
 Author-email: lckjack123@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: huggingface-hub (==0.20.3)
 Requires-Dist: librosa (==0.10.1)
 Requires-Dist: lightning (==2.1.3)
 Requires-Dist: matplotlib (==3.8.1)
 Requires-Dist: numpy (==1.26.3)
 Requires-Dist: pandas (==2.1.3)
+Requires-Dist: pip (==24.0)
 Requires-Dist: pyside6 (==6.6.1)
 Requires-Dist: pyside6-utils (==1.2.2)
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: scikit-learn (==1.4.0)
 Requires-Dist: scipy (==1.12.0)
 Requires-Dist: so-vits-svc-fork (==4.1.40)
 Requires-Dist: torch (==2.1.1)
```

