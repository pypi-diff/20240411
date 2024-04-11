# Comparing `tmp/svc_toolkit-1.0.5.tar.gz` & `tmp/svc_toolkit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svc_toolkit-1.0.5.tar", max compression
+gzip compressed data, was "svc_toolkit-1.0.6.tar", max compression
```

## Comparing `svc_toolkit-1.0.5.tar` & `svc_toolkit-1.0.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      897 2024-04-05 01:40:24.743965 svc_toolkit-1.0.5/README.md
--rw-r--r--   0        0        0     1634 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/__init__.py
--rw-r--r--   0        0        0      787 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter.py
--rw-r--r--   0        0        0     2443 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter_trainer.py
--rw-r--r--   0        0        0     1056 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/conversion/mixer.py
--rw-r--r--   0        0        0    12669 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/img/icon.png
--rw-r--r--   0        0        0    31498 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/img/loading.gif
--rw-r--r--   0        0        0     2377 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/main.py
--rw-r--r--   0        0        0      197 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/models/manifest.yml
--rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/__init__.py
--rw-r--r--   0        0        0      293 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/common.py
--rw-r--r--   0        0        0      828 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/conversion.py
--rw-r--r--   0        0        0      613 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/mixing.py
--rw-r--r--   0        0        0     2595 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/separation.py
--rw-r--r--   0        0        0      675 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/presenter/training.py
--rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/__init__.py
--rw-r--r--   0        0        0      987 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/audio.py
--rw-r--r--   0        0        0      196 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/constants.py
--rw-r--r--   0        0        0     7065 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/data.py
--rw-r--r--   0        0        0     2168 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/evaluator.py
--rw-r--r--   0        0        0     1985 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/logger.py
--rw-r--r--   0        0        0     7133 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/models.py
--rw-r--r--   0        0        0     3580 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/preprocess.py
--rw-r--r--   0        0        0     4697 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/separator.py
--rw-r--r--   0        0        0      752 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation/utility.py
--rw-r--r--   0        0        0     1290 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation_evaluation.py
--rw-r--r--   0        0        0      978 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation_preprocess.py
--rw-r--r--   0        0        0     3922 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/separation_train.py
--rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/utility/__init__.py
--rw-r--r--   0        0        0      239 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/utility/functions.py
--rw-r--r--   0        0        0        0 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/__init__.py
--rw-r--r--   0        0        0     7941 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/common.py
--rw-r--r--   0        0        0     7972 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/conversion.py
--rw-r--r--   0        0        0      760 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_overlay.py
--rw-r--r--   0        0        0      993 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_window.py
--rw-r--r--   0        0        0      578 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/main_window.py
--rw-r--r--   0        0        0     3325 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/mixing.py
--rw-r--r--   0        0        0     4679 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/separation.py
--rw-r--r--   0        0        0     5279 2024-04-05 01:40:24.747965 svc_toolkit-1.0.5/src/svc_toolkit/widget/training.py
--rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 svc_toolkit-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-10 23:59:17.258379 svc_toolkit-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2049 2024-04-10 23:59:17.258379 svc_toolkit-1.0.6/README.md
+-rw-r--r--   0        0        0     1548 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter.py
+-rw-r--r--   0        0        0     2443 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter_trainer.py
+-rw-r--r--   0        0        0     1056 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/conversion/mixer.py
+-rw-r--r--   0        0        0    12669 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/img/icon.png
+-rw-r--r--   0        0        0    31498 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/img/loading.gif
+-rw-r--r--   0        0        0     2377 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/main.py
+-rw-r--r--   0        0        0      400 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/models/manifest.yml
+-rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/common.py
+-rw-r--r--   0        0        0      828 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/conversion.py
+-rw-r--r--   0        0        0      613 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/mixing.py
+-rw-r--r--   0        0        0     2595 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/separation.py
+-rw-r--r--   0        0        0      675 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/presenter/training.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/audio.py
+-rw-r--r--   0        0        0      196 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/constants.py
+-rw-r--r--   0        0        0     7065 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/data.py
+-rw-r--r--   0        0        0     2168 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/evaluator.py
+-rw-r--r--   0        0        0     1985 2024-04-10 23:59:17.274379 svc_toolkit-1.0.6/src/svc_toolkit/separation/logger.py
+-rw-r--r--   0        0        0     7133 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/models.py
+-rw-r--r--   0        0        0     3580 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/preprocess.py
+-rw-r--r--   0        0        0     4697 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/separator.py
+-rw-r--r--   0        0        0      752 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation/utility.py
+-rw-r--r--   0        0        0     1471 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation_evaluation.py
+-rw-r--r--   0        0        0     1214 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation_preprocess.py
+-rw-r--r--   0        0        0     4146 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/separation_train.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/utility/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/utility/functions.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/__init__.py
+-rw-r--r--   0        0        0     7941 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/common.py
+-rw-r--r--   0        0        0     7972 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/conversion.py
+-rw-r--r--   0        0        0      760 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_overlay.py
+-rw-r--r--   0        0        0      993 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_window.py
+-rw-r--r--   0        0        0      578 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/main_window.py
+-rw-r--r--   0        0        0     3326 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/mixing.py
+-rw-r--r--   0        0        0     5075 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/separation.py
+-rw-r--r--   0        0        0     5289 2024-04-10 23:59:17.278379 svc_toolkit-1.0.6/src/svc_toolkit/widget/training.py
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 svc_toolkit-1.0.6/PKG-INFO
```

### Comparing `svc_toolkit-1.0.5/pyproject.toml` & `svc_toolkit-1.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "svc-toolkit"
-version = "1.0.5"
-description = "A self-contained singing voice conversion using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI."
+version = "1.0.6"
+description = "A self-contained singing voice conversion application using the so-vits-svc architecture, with Deep U-Net model for vocal separation feature and easy to use GUI."
 authors = ["jljl1337 <lckjack123@gmail.com>"]
-license = ""
+license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jljl1337/svc-toolkit"
 documentation = "https://jljl1337.github.io/svc-toolkit/"
 classifiers = [
     "Operating System :: OS Independent",
 ]
 packages = [
@@ -35,27 +35,21 @@
 librosa = "0.10.1"
 so-vits-svc-fork = "4.1.40"
 pyside6 = "6.6.1"
 pyside6-utils = "1.2.2"
 huggingface-hub = "0.20.3"
 
 [tool.poetry.group.dev.dependencies]
-poetry = "^1.8"
-setuptools = "^69.2"
+ipykernel = "^6.26"
 pytest = "8.0.0"
 pytest-qt = "^4.4"
 pytest-cov = "^4.1"
 pytest-xvfb = "^3.0.0"
 mkdocs-material = "^9.5"
 moises-db = { git = "https://github.com/moises-ai/moises-db.git", branch = "main" }
 
 [tool.pytest.ini_options]
-addopts = "--cov=src/ --cov-config=.coveragerc --cov-report=html --cov-report=xml -W ignore::DeprecationWarning "
-pythonpath = ["src"]
+addopts = "--cov=src/ --cov-report=html --cov-report=xml -W ignore::DeprecationWarning "
+testpaths = ["tests"]
 
 [tool.coverage.run]
-branch = true
-
-[tool.coverage.report]
-exclude_lines = [
-    'if __name__ == "__main__":',
-]
+omit = ["src/svc_toolkit/*.py"]
```

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter.py` & `svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/conversion/converter_trainer.py` & `svc_toolkit-1.0.6/src/svc_toolkit/conversion/converter_trainer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/conversion/mixer.py` & `svc_toolkit-1.0.6/src/svc_toolkit/conversion/mixer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/img/icon.png` & `svc_toolkit-1.0.6/src/svc_toolkit/img/icon.png`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/img/loading.gif` & `svc_toolkit-1.0.6/src/svc_toolkit/img/loading.gif`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/main.py` & `svc_toolkit-1.0.6/src/svc_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/presenter/conversion.py` & `svc_toolkit-1.0.6/src/svc_toolkit/presenter/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/presenter/mixing.py` & `svc_toolkit-1.0.6/src/svc_toolkit/presenter/mixing.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/presenter/separation.py` & `svc_toolkit-1.0.6/src/svc_toolkit/presenter/separation.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/presenter/training.py` & `svc_toolkit-1.0.6/src/svc_toolkit/presenter/training.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/audio.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/audio.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/data.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/data.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/evaluator.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/evaluator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/logger.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/logger.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/models.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/models.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/preprocess.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/preprocess.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/separator.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/separator.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation/utility.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation/utility.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation_evaluation.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation_evaluation.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import torch
 import matplotlib.pyplot as plt
 
 from svc_toolkit.separation.evaluator import Evaluator
 
 def main():
-    parser = ArgumentParser()
-    parser.add_argument('-m', '--model_dir', type=str, required=True)
-    parser.add_argument('-t', '--test_csv', type=str, required=True)
-    parser.add_argument('-p', '--precision', type=str, default='bf16')
-    parser.add_argument('-l', '--last', default=False, action=argparse.BooleanOptionalAction)
+    parser = ArgumentParser(description='Evaluate a separation model.')
+    parser.add_argument('-m', '--model_dir', type=str, required=True, help='Path to the model directory')
+    parser.add_argument('-t', '--test_csv', type=str, required=True, help='Path to the test csv file')
+    parser.add_argument('-p', '--precision', type=str, default='bf16', choices=['bf16', '32'], help='Precision')
+    parser.add_argument('-l', '--last', default=False, action=argparse.BooleanOptionalAction, help='Use the last model')
     args = parser.parse_args()
 
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
     evaluator = Evaluator(args.model_dir, device, args.precision, args.last)
     df_result = evaluator.evaluate(args.test_csv)
```

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/separation_train.py` & `svc_toolkit-1.0.6/src/svc_toolkit/separation_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from svc_toolkit.separation import constants
 from svc_toolkit.separation import utility
 from svc_toolkit.separation.data import MagnitudeDataModule
 from svc_toolkit.separation.logger import MyLogger
 from svc_toolkit.separation.models import UNetLightning
 
 def main():
-    parser = ArgumentParser()
-    parser.add_argument('-t', '--train_csv', type=str, required=True)
-    parser.add_argument('-v', '--val_csv', type=str, required=True)
-    parser.add_argument('-e', '--experiment', type=str, default='exp')
-    parser.add_argument('-m', '--model_dir', type=str, default='./model/')
-    parser.add_argument('-c', '--config', type=str, default='./config.yml')
+    parser = ArgumentParser(description='Train a separation model.')
+    parser.add_argument('-t', '--train_csv', type=str, required=True, help='Path to the training csv file')
+    parser.add_argument('-v', '--val_csv', type=str, required=True, help='Path to the validation csv file')
+    parser.add_argument('-e', '--experiment', type=str, default='exp', help='Name of the experiment')
+    parser.add_argument('-m', '--model_dir', type=str, default='./model_log/', help='Path to the model log directory')
+    parser.add_argument('-c', '--config', type=str, default='./config.yml', help='Path to the config file')
     args = parser.parse_args()
 
     config = load_yaml(args.config)
 
     # If resuming, use the old config
     resume_path = config['resume_path']
     if resume_path != '':
```

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/common.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/common.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/conversion.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/conversion.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_overlay.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_overlay.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/loading_window.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/loading_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/main_window.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/main_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/mixing.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/mixing.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.start_button.setEnabled(True)
 
         error_message = self.mixing_thread.error_message
 
         if error_message:
             error_message_box(error_message)
         else:
-            info_message_box('Mixing completed')
+            info_message_box('Mixing completed.')
 
     def start_mixing(self):
         error_message = ''
 
         if not self.source_1_file_widget.get_file():
             error_message += 'Source 1 file is not selected.\n'
         if not self.source_2_file_widget.get_file():
```

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/separation.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/separation.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,20 @@
         try:
             self.error_message = None
             self.separation_function(self.progress_signal.emit, **self.kwargs)
 
         except Exception as e:
             self.error_message = str(e)
 
+            if 'autocast' in self.error_message:
+                new_error_message = 'Your device may not be compatible with the current precision. '
+                new_error_message += 'please choose another device or precision. '
+                new_error_message += 'This is prompted due to the following error:\n' + self.error_message
+                self.error_message = new_error_message
+
 class SeparationWidget(QWidget):
     def __init__(self):
         super().__init__()
 
         layout = QVBoxLayout(self)
 
         self.file_group_box = QGroupBox('Files')
```

### Comparing `svc_toolkit-1.0.5/src/svc_toolkit/widget/training.py` & `svc_toolkit-1.0.6/src/svc_toolkit/widget/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,32 +27,32 @@
         self.train_function = train_function
         self.config_file = config_file
         self.model_output_dir = model_output_dir
 
     def run(self):
         try:
             self.error_message = None
-            self.train_function(self.model_output_dir, self.config_file)
+            self.train_function(self.config_file, self.model_output_dir)
 
         except Exception as e:
             self.error_message = str(e)
 
 class TrainingWidget(OverlayWidget):
     def __init__(self):
         super().__init__(parent=None)
 
         layout = QVBoxLayout(self)
 
-        self.preprocess_group_box = QGroupBox('Preprocess')
+        self.preprocess_group_box = QGroupBox('Preprocessing')
         self.preprocess_layout = QVBoxLayout(self.preprocess_group_box)
 
         self.dataset_dir_widget = DirectoryWidget('Dataset Directory')
         self.Output_dir_widget = DirectoryWidget('Output Directory')
-        self.split_checkbox = CheckboxWidget('Split Dataset')
-        self.start_preprocess_button = QPushButton('Start Preprocess')
+        self.split_checkbox = CheckboxWidget('Split Audio Files')
+        self.start_preprocess_button = QPushButton('Start Preprocessing')
         self.start_preprocess_button.clicked.connect(self._start_preprocess)
 
         self.preprocess_layout.addWidget(self.dataset_dir_widget)
         self.preprocess_layout.addWidget(self.Output_dir_widget)
         self.preprocess_layout.addWidget(self.split_checkbox)
         self.preprocess_layout.addWidget(self.start_preprocess_button)
```

