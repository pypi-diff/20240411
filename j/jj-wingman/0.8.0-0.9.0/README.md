# Comparing `tmp/jj_wingman-0.8.0.tar.gz` & `tmp/jj_wingman-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.8.0.tar", last modified: Wed Apr 10 14:36:54 2024, max compression
+gzip compressed data, was "jj_wingman-0.9.0.tar", last modified: Thu Apr 11 20:50:41 2024, max compression
```

## Comparing `jj_wingman-0.8.0.tar` & `jj_wingman-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/jj_wingman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/test/test_replay_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/wingman/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/cli_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/neural_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/print_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/replay_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/wingman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:50:41.317119 jj_wingman-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-04-11 20:50:41.317119 jj_wingman-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:50:41.317119 jj_wingman-0.9.0/jj_wingman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-04-11 20:50:41.000000 jj_wingman-0.9.0/jj_wingman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 20:50:41.000000 jj_wingman-0.9.0/jj_wingman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:50:41.000000 jj_wingman-0.9.0/jj_wingman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 20:50:41.000000 jj_wingman-0.9.0/jj_wingman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 20:50:41.000000 jj_wingman-0.9.0/jj_wingman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 20:50:41.000000 jj_wingman-0.9.0/jj_wingman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:50:41.317119 jj_wingman-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:50:41.313120 jj_wingman-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/test/test_replay_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:50:41.317119 jj_wingman-0.9.0/wingman/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/cli_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/neural_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/print_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/replay_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15968 2024-04-11 20:50:36.000000 jj_wingman-0.9.0/wingman/wingman.py
```

### Comparing `jj_wingman-0.8.0/LICENSE.txt` & `jj_wingman-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.8.0/PKG-INFO` & `jj_wingman-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.8.0
+Version: 0.9.0
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -24,15 +24,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjshoots/Wingman
 Keywords: Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: wandb
 Requires-Dist: pyyaml
 
 <p align="center">
@@ -96,15 +96,15 @@
 wandb_project: 'my_new_project'
 ```
 
 The parameters described are as follows:
 - `debug`: Whether to set the model to debug mode
 - `save_directory`: Where should Wingman point to for model weight saving
 - `model_id`: Wingman records the model under this ID, if this is left as null, Wingman automatically chooses a number.
-- `model_num`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
+- `ckpt_number`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
 - `log_status`: Whether to save a `.txt` log file of Wingman's outputs.
 - `increment`: Whether to increment checkpoint number, if this is set to false, Wingman won't save multiple variations of the same model.
 - `logging_interval`: During training, pass the training step to wingman, and after `logging_interval` steps has passed, Wingman will record the training. If Wingman has found a new lowest point, the model weights will be saved to a new file.
 - `max_skips`: How many logging steps skipped without finding a new lowest point (specified using the `logging_interval` argument) before Wingman will save an intermediary checkpoint of the model.
 - `greater_than`: You can tell Wingman to only checkpoint the model when the previous checkpointed loss is more than the current loss by this value.
 - `wandb`: Whether to log things to WandB.
 - `wandb_name`: The name of the run to be displayed in WandB. If left blank, Wingman automatically assigns one depending on the model version number.
```

### Comparing `jj_wingman-0.8.0/README.md` & `jj_wingman-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 wandb_project: 'my_new_project'
 ```
 
 The parameters described are as follows:
 - `debug`: Whether to set the model to debug mode
 - `save_directory`: Where should Wingman point to for model weight saving
 - `model_id`: Wingman records the model under this ID, if this is left as null, Wingman automatically chooses a number.
-- `model_num`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
+- `ckpt_number`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
 - `log_status`: Whether to save a `.txt` log file of Wingman's outputs.
 - `increment`: Whether to increment checkpoint number, if this is set to false, Wingman won't save multiple variations of the same model.
 - `logging_interval`: During training, pass the training step to wingman, and after `logging_interval` steps has passed, Wingman will record the training. If Wingman has found a new lowest point, the model weights will be saved to a new file.
 - `max_skips`: How many logging steps skipped without finding a new lowest point (specified using the `logging_interval` argument) before Wingman will save an intermediary checkpoint of the model.
 - `greater_than`: You can tell Wingman to only checkpoint the model when the previous checkpointed loss is more than the current loss by this value.
 - `wandb`: Whether to log things to WandB.
 - `wandb_name`: The name of the run to be displayed in WandB. If left blank, Wingman automatically assigns one depending on the model version number.
```

### Comparing `jj_wingman-0.8.0/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.9.0/jj_wingman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.8.0
+Version: 0.9.0
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -24,15 +24,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/jjshoots/Wingman
 Keywords: Machine Learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: wandb
 Requires-Dist: pyyaml
 
 <p align="center">
@@ -96,15 +96,15 @@
 wandb_project: 'my_new_project'
 ```
 
 The parameters described are as follows:
 - `debug`: Whether to set the model to debug mode
 - `save_directory`: Where should Wingman point to for model weight saving
 - `model_id`: Wingman records the model under this ID, if this is left as null, Wingman automatically chooses a number.
-- `model_num`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
+- `ckpt_number`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
 - `log_status`: Whether to save a `.txt` log file of Wingman's outputs.
 - `increment`: Whether to increment checkpoint number, if this is set to false, Wingman won't save multiple variations of the same model.
 - `logging_interval`: During training, pass the training step to wingman, and after `logging_interval` steps has passed, Wingman will record the training. If Wingman has found a new lowest point, the model weights will be saved to a new file.
 - `max_skips`: How many logging steps skipped without finding a new lowest point (specified using the `logging_interval` argument) before Wingman will save an intermediary checkpoint of the model.
 - `greater_than`: You can tell Wingman to only checkpoint the model when the previous checkpointed loss is more than the current loss by this value.
 - `wandb`: Whether to log things to WandB.
 - `wandb_name`: The name of the run to be displayed in WandB. If left blank, Wingman automatically assigns one depending on the model version number.
```

### Comparing `jj_wingman-0.8.0/pyproject.toml` & `jj_wingman-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["numpy", "wandb", "pyyaml"]
 keywords = ["Machine Learning"]
```

### Comparing `jj_wingman-0.8.0/test/test_replay_buffer.py` & `jj_wingman-0.9.0/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.8.0/wingman/cli_scripts.py` & `jj_wingman-0.9.0/wingman/cli_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """CLI functionality of Wingman."""
 import glob
 import os
 import shutil
 import sys
 
-from .print_utils import cstr, wm_print
+from wingman.print_utils import cstr, wm_print
 
 
 def _get_dir_size(path):
     total = 0
     with os.scandir(path) as it:
         for entry in it:
             if entry.is_file():
```

### Comparing `jj_wingman-0.8.0/wingman/neural_blocks.py` & `jj_wingman-0.9.0/wingman/neural_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Easy creation of neural networks."""
 from typing import List, Optional
 
+from wingman.exceptions import NeuralBlocksException
+
 try:
     import torch.nn as nn
 except ImportError as e:
     raise ImportError(
         "Could not import torch, this is not bundled as part of Wingman and has to be installed manually."
     ) from e
 
@@ -242,19 +244,22 @@
             norm:
 
         Returns:
             nn.Sequential:
         """
         network_depth = len(channels_description) - 1
 
-        assert (
-            network_depth == len(kernels_description)
-            and network_depth == len(activation_description)
-            and network_depth == len(pooling_description)
-        ), "All network descriptions must be of the same size"
+        if (
+            network_depth != len(kernels_description)
+            or network_depth != len(activation_description)
+            or network_depth != len(pooling_description)
+        ):
+            raise NeuralBlocksException(
+                "All network descriptions must be of the same size"
+            )
 
         module_list = []
         for i in range(network_depth):
             module_list.append(
                 cls.conv_module(
                     channels_description[i],
                     channels_description[i + 1],
@@ -289,20 +294,23 @@
             norm (str): norm
 
         Returns:
             nn.Sequential:
         """
         network_depth = len(channels_description) - 1
 
-        assert (
-            network_depth == len(kernels_description)
-            and network_depth == len(activation_description)
-            and network_depth == len(padding_description)
-            and network_depth == len(stride_description)
-        ), "All network descriptions must be of the same size"
+        if (
+            network_depth != len(kernels_description)
+            or network_depth != len(activation_description)
+            or network_depth != len(padding_description)
+            or network_depth != len(stride_description)
+        ):
+            raise NeuralBlocksException(
+                "All network descriptions must be of the same size"
+            )
 
         module_list = []
         for i in range(network_depth):
             module_list.append(
                 cls.deconv_module(
                     channels_description[i],
                     channels_description[i + 1],
@@ -333,17 +341,18 @@
             bias (bool): bias
 
         Returns:
             nn.Sequential:
         """
         network_depth = len(features_description) - 1
 
-        assert network_depth == len(
-            activation_description
-        ), "All network descriptions must be of the same size"
+        if network_depth != len(activation_description):
+            raise NeuralBlocksException(
+                f"All network descriptions must be of the same size, got {network_depth} for `network_depth` and {activation_description} for `activation_description`."
+            )
 
         module_list = []
         for i in range(network_depth):
             module_list.append(
                 cls.linear_module(
                     features_description[i],
                     features_description[i + 1],
```

### Comparing `jj_wingman-0.8.0/wingman/print_utils.py` & `jj_wingman-0.9.0/wingman/print_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """For fancy printing in Wingman."""
 from __future__ import annotations
 
 import re
 from pathlib import Path
-from typing import Any
+from typing import Any, Literal
 
 # colour list
 c_colors = {
     "HEADER": "\033[95m",
     "OKBLUE": "\033[94m",
     "OKCYAN": "\033[96m",
     "OKGREEN": "\033[92m",
@@ -15,15 +15,20 @@
     "FAIL": "\033[91m",
     "BOLD": "\033[1m",
     "UNDERLINE": "\033[4m",
 }
 end_c = "\033[0m"
 
 
-def cstr(x: Any, ctype: str) -> str:
+def cstr(
+    x: Any,
+    ctype: Literal[
+        "HEADER", "OKBLUE", "OKCYAN", "OKGREEN", "WARNING", "FAIL", "BOLD", "UNDERLINE"
+    ],
+) -> str:
     """Makes a string colourful.
 
     Args:
         x (Any): the string
         ctype (str): the colour
 
     Returns:
```

### Comparing `jj_wingman-0.8.0/wingman/replay_buffer.py` & `jj_wingman-0.9.0/wingman/replay_buffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Replay buffer implementation with push, automatic overflow, and automatic torch dataset functionality."""
 from __future__ import annotations
 
 from typing import Any, Sequence
 
 import numpy as np
 
+from wingman.exceptions import ReplayBufferException
+
 try:
     from torch.utils.data import Dataset
 except ImportError as e:
     raise ImportError(
         "Could not import torch, this is not bundled as part of Wingman and has to be installed manually."
     ) from e
 
@@ -79,30 +81,35 @@
             data (Sequence[np.ndarray | float | int | bool]): data
             bulk (bool): whether to bulk add stuff into the replay buffer
             random_rollover (bool): whether to rollover the data in the replay buffer once full or to randomly insert
         """
         # check if we are bulk adding things in and assert lengths
         bulk_size = 1
         if bulk:
-            assert all([isinstance(d, np.ndarray) for d in data]), cstr(
-                "All things must be np.ndarray for bulk data.", "FAIL"
-            )
+            # assert all things are numpy array
+            if not all([isinstance(d, np.ndarray) for d in data]):
+                raise ReplayBufferException(
+                    "All things must be np.ndarray for bulk data. "
+                    f"Got {[type(d) for d in data]}."
+                )
 
             bulk_size = data[0].shape[0]  # pyright: ignore
 
-            assert all([len(d) == bulk_size for d in data]), cstr(  # pyright: ignore
-                f"All things in data must have same len for the first dimension for bulk data. Received data with {[len(d) for d in data]} items respectively.",  # pyright: ignore
-                "FAIL",
-            )
+            # assert all items have same length
+            if not all([len(d) == bulk_size for d in data]):  # pyright: ignore[reportArgumentType]
+                raise ReplayBufferException(
+                    "All things in data must have same len for the first dimension for bulk data. "
+                    f"Received data with {[len(d) for d in data]} items respectively.",  # pyright: ignore[reportArgumentType]
+                )
 
             # assert on memory lengths
-            assert self.mem_size >= bulk_size, cstr(
-                f"Bulk size ({bulk_size}) should be less than or equal to memory size ({self.mem_size}).",
-                "FAIL",
-            )
+            if self.mem_size < bulk_size:
+                raise ReplayBufferException(
+                    f"Bulk size ({bulk_size}) should be less than or equal to memory size ({self.mem_size}).",
+                )
 
         np_data = list(map(lambda x: self.__ensure_dims(x, bulk), data))
 
         # instantiate the memory if it does not exist
         if self.count == 0:
             self.memory = []
             for thing in np_data:
@@ -117,18 +124,19 @@
 
             mem_size_bytes = sum([d.nbytes for d in self.memory])
             wm_print(
                 cstr(f"Replay Buffer Size: {mem_size_bytes / 1e9} gigabytes.", "OKCYAN")
             )
 
         # assert that the number of lists in memory is same as data to push
-        assert len(np_data) == len(self.memory), cstr(
-            f"Data length not similar to memory buffer length. Replay buffer has {len(self.memory)} items, but received {len(np_data)} items.",
-            "FAIL",
-        )
+        if len(np_data) != len(self.memory):
+            raise ReplayBufferException(
+                f"Data length not similar to memory buffer length. Replay buffer has {len(self.memory)} items. "
+                f"But received {len(np_data)} items.",
+            )
 
         # indexing for memory positions
         start = self.count % self.mem_size
         stop = min(start + bulk_size, self.mem_size)
         rollover = -(self.mem_size - start - bulk_size)
         if random_rollover:
             if not self.is_full:
```

### Comparing `jj_wingman-0.8.0/wingman/utils.py` & `jj_wingman-0.9.0/wingman/utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.8.0/wingman/wingman.py` & `jj_wingman-0.9.0/wingman/wingman.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from pathlib import Path
 from typing import Tuple
 
 import numpy as np
 import wandb
 import yaml
 
-from .print_utils import cstr, wm_print
+from wingman.exceptions import WingmanException
+from wingman.print_utils import cstr, wm_print
 
 
 class Wingman:
     """Wingman.
 
     Class to handle checkpointing of loss and handling of weights files.
     Minimal example:
@@ -62,17 +63,21 @@
         """
         # save our experiment description
         self.config_yaml: Path = Path(config_yaml)
         self.experiment_description = experiment_description
         self.cfg = self.__yaml_to_args()
 
         # make sure that logging_interval is positive
-        assert (
-            self.cfg.logging_interval > 0
-        ), f"logging_interval must be a positive number, got {self.cfg.logging_interval}."
+        if self.cfg.logging_interval <= 0:
+            raise WingmanException(
+                cstr(
+                    f"logging_interval must be a positive number, got {self.cfg.logging_interval}.",
+                    "FAIL",
+                )
+            )
 
         # the logger
         self.log = dict()
 
         # runtime variables
         self.num_losses = 0
         self.cumulative_loss = 0
@@ -162,17 +167,18 @@
                 "wandb",
                 "wandb_name",
                 "wandb_notes",
                 "wandb_id",
                 "wandb_entity",
                 "wandb_project",
             ]
-            for item in assertion_list:
-                assert item in config, cstr(
-                    f"Missing parameter {item} in config file.", "FAIL"
+            missing_set = set(assertion_list) - set(config.keys())
+            if missing_set:
+                raise WingmanException(
+                    cstr(f"Missing parameters {missing_set} in config file.", "FAIL")
                 )
 
             # override model_id if needed
             if config["model_id"] is None:
                 config["model_id"] = np.random.randint(999999)
 
             # make a logging file if required
@@ -243,18 +249,21 @@
             Tuple[bool, Path, Path]: to_update, weights_file, optim_file
         """
         # if step is None, we automatically increment
         if step is None:
             step = self.previous_checkpoint_step + 1
 
         # check that our step didn't go in reverse
-        assert step >= self.previous_checkpoint_step, cstr(
-            f"We can't step backwards! Got step {step} but the previous logging step was {self.previous_checkpoint_step}.",
-            "FAIL",
-        )
+        if step < self.previous_checkpoint_step:
+            raise WingmanException(
+                cstr(
+                    f"We can't step backwards! Got step {step} but the previous logging step was {self.previous_checkpoint_step}.",
+                    "FAIL",
+                )
+            )
         self.previous_checkpoint_step = step
 
         """ACCUMULATE LOSS"""
         self.cumulative_loss += loss
         self.num_losses += 1.0
 
         # if we haven't passed the required number of steps
@@ -341,17 +350,18 @@
         ```
         wm.log["foo"] = "bar"
         ```
 
         Returns:
             None:
         """
-        assert isinstance(self.log, dict), cstr(
-            f"log must be dictionary, currently it is {self.log}.", "FAIL"
-        )
+        if not isinstance(self.log, dict):
+            raise WingmanException(
+                cstr(f"log must be dictionary, currently it is {self.log}.", "FAIL")
+            )
         if self.cfg.wandb:
             wandb.log(self.log)
 
     def write_auxiliary(
         self, data: np.ndarray, variable_name: str, precision: str = "%1.3f"
     ) -> None:
         """write_auxiliary.
@@ -360,15 +370,18 @@
             data (np.ndarray): data
             variable_name (str): variable_name
             precision (str): precision
 
         Returns:
             None:
         """
-        assert len(data.shape) == 1, "Data must be only 1 dimensional ndarray"
+        if not len(data.shape) == 1:
+            raise WingmanException(
+                cstr("Data must be only 1 dimensional ndarray", "FAIL")
+            )
         filename = self.model_directory / f"{variable_name}.csv"
         with open(filename, "ab") as f:
             np.savetxt(f, [data], delimiter=",", fmt=precision)
 
     def get_weight_files(self, latest: bool = True) -> Tuple[bool, Path, Path]:
         """get_weight_files.
```

