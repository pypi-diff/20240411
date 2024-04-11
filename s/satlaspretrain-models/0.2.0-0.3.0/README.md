# Comparing `tmp/satlaspretrain_models-0.2.0.tar.gz` & `tmp/satlaspretrain_models-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/satlaspretrain_models-0.2.0.tar", last modified: Tue Feb  6 20:02:21 2024, max compression
+gzip compressed data, was "dist/satlaspretrain_models-0.3.0.tar", last modified: Thu Apr 11 17:32:45 2024, max compression
```

## Comparing `satlaspretrain_models-0.2.0.tar` & `satlaspretrain_models-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 piperw     (502) staff       (20)        0 2024-02-06 20:02:21.238825 satlaspretrain_models-0.2.0/
--rw-r--r--   0 piperw     (502) staff       (20)    11357 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/LICENSE
--rw-r--r--   0 piperw     (502) staff       (20)       34 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/MANIFEST.in
--rw-r--r--   0 piperw     (502) staff       (20)    12841 2024-02-06 20:02:21.238142 satlaspretrain_models-0.2.0/PKG-INFO
--rw-r--r--   0 piperw     (502) staff       (20)    12147 2024-02-06 19:53:43.000000 satlaspretrain_models-0.2.0/README.md
-drwxr-xr-x   0 piperw     (502) staff       (20)        0 2024-02-06 20:02:21.231547 satlaspretrain_models-0.2.0/satlaspretrain_models/
--rw-r--r--   0 piperw     (502) staff       (20)       68 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/__init__.py
--rw-r--r--   0 piperw     (502) staff       (20)    10268 2024-02-06 18:13:57.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/model.py
-drwxr-xr-x   0 piperw     (502) staff       (20)        0 2024-02-06 20:02:21.235834 satlaspretrain_models-0.2.0/satlaspretrain_models/models/
--rw-r--r--   0 piperw     (502) staff       (20)      135 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/models/__init__.py
--rw-r--r--   0 piperw     (502) staff       (20)     4959 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/models/backbones.py
--rw-r--r--   0 piperw     (502) staff       (20)      653 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/models/fpn.py
--rw-r--r--   0 piperw     (502) staff       (20)     9014 2024-02-06 19:53:43.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/models/heads.py
--rw-r--r--   0 piperw     (502) staff       (20)     5765 2024-02-06 04:56:24.000000 satlaspretrain_models-0.2.0/satlaspretrain_models/utils.py
-drwxr-xr-x   0 piperw     (502) staff       (20)        0 2024-02-06 20:02:21.233891 satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/
--rw-r--r--   0 piperw     (502) staff       (20)    12841 2024-02-06 20:02:21.000000 satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/PKG-INFO
--rw-r--r--   0 piperw     (502) staff       (20)      589 2024-02-06 20:02:21.000000 satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/SOURCES.txt
--rw-r--r--   0 piperw     (502) staff       (20)        1 2024-02-06 20:02:21.000000 satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/dependency_links.txt
--rw-r--r--   0 piperw     (502) staff       (20)       69 2024-02-06 20:02:21.000000 satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/requires.txt
--rw-r--r--   0 piperw     (502) staff       (20)       22 2024-02-06 20:02:21.000000 satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/top_level.txt
--rw-r--r--   0 piperw     (502) staff       (20)       38 2024-02-06 20:02:21.239015 satlaspretrain_models-0.2.0/setup.cfg
--rw-r--r--   0 piperw     (502) staff       (20)      859 2024-02-06 20:00:29.000000 satlaspretrain_models-0.2.0/setup.py
-drwxr-xr-x   0 piperw     (502) staff       (20)        0 2024-02-06 20:02:21.237333 satlaspretrain_models-0.2.0/tests/
--rw-r--r--   0 piperw     (502) staff       (20)     2286 2024-02-06 18:16:44.000000 satlaspretrain_models-0.2.0/tests/test_pretrained_models.py
--rw-r--r--   0 piperw     (502) staff       (20)     2037 2024-02-06 18:16:33.000000 satlaspretrain_models-0.2.0/tests/test_randomly_initialized_models.py
+drwxr-xr-x   0 piperw    (2623) users      (100)        0 2024-04-11 17:32:45.051701 satlaspretrain_models-0.3.0/
+-rw-r--r--   0 piperw    (2623) users      (100)    11357 2024-02-20 18:12:25.000000 satlaspretrain_models-0.3.0/LICENSE
+-rw-r--r--   0 piperw    (2623) users      (100)       34 2024-02-20 18:12:25.000000 satlaspretrain_models-0.3.0/MANIFEST.in
+-rw-r--r--   0 piperw    (2623) users      (100)    13891 2024-04-11 17:32:45.051701 satlaspretrain_models-0.3.0/PKG-INFO
+-rw-r--r--   0 piperw    (2623) users      (100)    13197 2024-03-15 18:36:22.000000 satlaspretrain_models-0.3.0/README.md
+drwxr-xr-x   0 piperw    (2623) users      (100)        0 2024-04-11 17:32:45.047701 satlaspretrain_models-0.3.0/satlaspretrain_models/
+-rw-r--r--   0 piperw    (2623) users      (100)       68 2024-02-20 18:12:25.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/__init__.py
+-rw-r--r--   0 piperw    (2623) users      (100)    10541 2024-04-11 17:29:57.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/model.py
+drwxr-xr-x   0 piperw    (2623) users      (100)        0 2024-04-11 17:32:45.047701 satlaspretrain_models-0.3.0/satlaspretrain_models/models/
+-rw-r--r--   0 piperw    (2623) users      (100)      145 2024-04-11 17:29:57.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/models/__init__.py
+-rw-r--r--   0 piperw    (2623) users      (100)     4951 2024-04-11 17:29:57.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/models/backbones.py
+-rw-r--r--   0 piperw    (2623) users      (100)     1818 2024-04-11 17:29:57.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/models/fpn.py
+-rw-r--r--   0 piperw    (2623) users      (100)     9046 2024-04-11 17:29:57.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/models/heads.py
+-rw-r--r--   0 piperw    (2623) users      (100)     6776 2024-03-15 18:36:22.000000 satlaspretrain_models-0.3.0/satlaspretrain_models/utils.py
+drwxr-xr-x   0 piperw    (2623) users      (100)        0 2024-04-11 17:32:45.047701 satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/
+-rw-r--r--   0 piperw    (2623) users      (100)    13891 2024-04-11 17:32:45.000000 satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/PKG-INFO
+-rw-r--r--   0 piperw    (2623) users      (100)      589 2024-04-11 17:32:45.000000 satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/SOURCES.txt
+-rw-r--r--   0 piperw    (2623) users      (100)        1 2024-04-11 17:32:45.000000 satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/dependency_links.txt
+-rw-r--r--   0 piperw    (2623) users      (100)       69 2024-04-11 17:32:45.000000 satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/requires.txt
+-rw-r--r--   0 piperw    (2623) users      (100)       22 2024-04-11 17:32:45.000000 satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/top_level.txt
+-rw-r--r--   0 piperw    (2623) users      (100)       38 2024-04-11 17:32:45.051701 satlaspretrain_models-0.3.0/setup.cfg
+-rw-r--r--   0 piperw    (2623) users      (100)      859 2024-04-11 17:31:27.000000 satlaspretrain_models-0.3.0/setup.py
+drwxr-xr-x   0 piperw    (2623) users      (100)        0 2024-04-11 17:32:45.051701 satlaspretrain_models-0.3.0/tests/
+-rw-r--r--   0 piperw    (2623) users      (100)     2705 2024-02-20 18:12:25.000000 satlaspretrain_models-0.3.0/tests/test_pretrained_models.py
+-rw-r--r--   0 piperw    (2623) users      (100)     2461 2024-02-20 18:12:25.000000 satlaspretrain_models-0.3.0/tests/test_randomly_initialized_models.py
```

### Comparing `satlaspretrain_models-0.2.0/LICENSE` & `satlaspretrain_models-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satlaspretrain_models-0.2.0/PKG-INFO` & `satlaspretrain_models-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satlaspretrain_models
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple package that makes it easy to load remote sensing foundation models for downstream use cases.
 Home-page: https://github.com/allenai/satlaspretrain_models
 Author: Satlas @ AI2
 Author-email: satlas@allenai.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -70,23 +70,24 @@
 Checkpoints are released under [ODC-BY](https://github.com/allenai/satlas/blob/main/DataLicense).
 This package will download model checkpoints automatically, but you can download them directly using the links below if desired.
 
 #### Sentinel-2 Pretrained Models
 |  | Single-image, RGB | Multi-image, RGB |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel2_SwinB_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_si_rgb.pth?download=true) | [Sentinel2_SwinB_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_mi_rgb.pth?download=true) |
-| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_rgb.pth?download=true) | |
+| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_rgb.pth?download=true) | [Sentinel2_SwinT_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_rgb.pth?download=true) |
 | **Resnet50** | [Sentinel2_Resnet50_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_si_rgb.pth?download=true) | [Sentinel2_Resnet50_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_rgb.pth?download=true) |
 | **Resnet152** | [Sentinel2_Resnet152_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_rgb.pth?download=true) | [Sentinel2_Resnet152_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_rgb.pth?download=true) |
 
 |  | Single-image, MS | Multi-image, MS |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel2_SwinB_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_si_ms.pth?download=true) | [Sentinel2_SwinB_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_mi_ms.pth?download=true) |
-| **Resnet50** | [Sentinel2_Resnet50_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | |
-| **Resnet152** | [Sentinel2_Resnet152_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_ms.pth?download=true) | |
+| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | [Sentinel2_SwinT_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_ms.pth?download=true) |
+| **Resnet50** | [Sentinel2_Resnet50_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | [Sentinel2_Resnet50_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_ms.pth?download=true) |
+| **Resnet152** | [Sentinel2_Resnet152_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_ms.pth?download=true) | [Sentinel2_Resnet152_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_ms.pth?download=true) |
 
 #### Sentinel-1 Pretrained Models
 |  | Single-image, VH+VV | Multi-image, VH+VV |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel1_SwinB_SI](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel1_swinb_si.pth?download=true) | [Sentinel1_SwinB_MI](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel1_swinb_mi.pth?download=true) |
 
 #### Landsat 8/9 Pretrained Models
@@ -212,14 +213,19 @@
 ```
 
 Demos
 -----
 We provide a [demo](https://github.com/allenai/satlaspretrain_models/blob/main/demo.ipynb) showing how to finetune a 
 SatlasPretrain Sentinel-2 model on the EuroSAT classification task.
 
+We also provide a [torchgeo demo](https://github.com/allenai/satlaspretrain_models/blob/main/torchgeo_demo.ipynb), 
+showing how to load SatlasPretrain weights into a model, download a dataset, initialize a trainer, and finetune the model on the UCMerced classification task. 
+*Note*: a separate conda environment must be initialized to run this demo, see details in the notebook. 
+ 
+
 Tests
 -----
 There are tests to test loading pretrained models and one to test randomly initialized models.
 
 To run the tests, run the following command from the root directory:
 `pytest tests/`
```

### Comparing `satlaspretrain_models-0.2.0/README.md` & `satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: satlaspretrain-models
+Version: 0.3.0
+Summary: A simple package that makes it easy to load remote sensing foundation models for downstream use cases.
+Home-page: https://github.com/allenai/satlaspretrain_models
+Author: Satlas @ AI2
+Author-email: satlas@allenai.org
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch>=2.1.0
+Requires-Dist: torchvision>=0.16.0
+Requires-Dist: requests
+Requires-Dist: matplotlib
+Requires-Dist: pytest
+Requires-Dist: notebook
+
 SatlasPretrain Models: Foundation models for satellite and aerial imagery.
 --------------------------------------------------------------------------
 
 **SatlasPretrain** is a large-scale pre-training dataset for remote sensing image understanding. This work
 was published at ICCV 2023. Details and download links for the dataset can be found
 [here](https://github.com/allenai/satlas/blob/main/SatlasPretrain.md).
 
@@ -50,23 +70,24 @@
 Checkpoints are released under [ODC-BY](https://github.com/allenai/satlas/blob/main/DataLicense).
 This package will download model checkpoints automatically, but you can download them directly using the links below if desired.
 
 #### Sentinel-2 Pretrained Models
 |  | Single-image, RGB | Multi-image, RGB |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel2_SwinB_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_si_rgb.pth?download=true) | [Sentinel2_SwinB_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_mi_rgb.pth?download=true) |
-| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_rgb.pth?download=true) | |
+| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_rgb.pth?download=true) | [Sentinel2_SwinT_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_rgb.pth?download=true) |
 | **Resnet50** | [Sentinel2_Resnet50_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_si_rgb.pth?download=true) | [Sentinel2_Resnet50_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_rgb.pth?download=true) |
 | **Resnet152** | [Sentinel2_Resnet152_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_rgb.pth?download=true) | [Sentinel2_Resnet152_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_rgb.pth?download=true) |
 
 |  | Single-image, MS | Multi-image, MS |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel2_SwinB_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_si_ms.pth?download=true) | [Sentinel2_SwinB_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_mi_ms.pth?download=true) |
-| **Resnet50** | [Sentinel2_Resnet50_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | |
-| **Resnet152** | [Sentinel2_Resnet152_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_ms.pth?download=true) | |
+| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | [Sentinel2_SwinT_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_ms.pth?download=true) |
+| **Resnet50** | [Sentinel2_Resnet50_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | [Sentinel2_Resnet50_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_ms.pth?download=true) |
+| **Resnet152** | [Sentinel2_Resnet152_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_ms.pth?download=true) | [Sentinel2_Resnet152_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_ms.pth?download=true) |
 
 #### Sentinel-1 Pretrained Models
 |  | Single-image, VH+VV | Multi-image, VH+VV |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel1_SwinB_SI](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel1_swinb_si.pth?download=true) | [Sentinel1_SwinB_MI](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel1_swinb_mi.pth?download=true) |
 
 #### Landsat 8/9 Pretrained Models
@@ -192,14 +213,19 @@
 ```
 
 Demos
 -----
 We provide a [demo](https://github.com/allenai/satlaspretrain_models/blob/main/demo.ipynb) showing how to finetune a 
 SatlasPretrain Sentinel-2 model on the EuroSAT classification task.
 
+We also provide a [torchgeo demo](https://github.com/allenai/satlaspretrain_models/blob/main/torchgeo_demo.ipynb), 
+showing how to load SatlasPretrain weights into a model, download a dataset, initialize a trainer, and finetune the model on the UCMerced classification task. 
+*Note*: a separate conda environment must be initialized to run this demo, see details in the notebook. 
+ 
+
 Tests
 -----
 There are tests to test loading pretrained models and one to test randomly initialized models.
 
 To run the tests, run the following command from the root directory:
 `pytest tests/`
```

### Comparing `satlaspretrain_models-0.2.0/satlaspretrain_models/model.py` & `satlaspretrain_models-0.3.0/satlaspretrain_models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,21 @@
             raise ValueError("Invalid backbone.")
         if head and not isinstance(head, Head):
             raise ValueError("Invalid head.")
         if head and (num_categories is None):
             raise ValueError("Must specify num_categories if head is desired.")
 
         self.backbone = self._initialize_backbone(num_channels, backbone, multi_image, weights)
-        self.fpn = self._initialize_fpn(self.backbone.out_channels, weights) if fpn else None
+
+        if fpn:
+            self.fpn = self._initialize_fpn(self.backbone.out_channels, weights)
+            self.upsample = Upsample(self.fpn.out_channels)
+        else:
+            self.fpn = None
+
         if head:
             self.head = self._initialize_head(head, self.fpn.out_channels, num_categories) if fpn else self._initialize_head(head, self.backbone.out_channels, num_categories)
         else:
             self.head = None
 
     def _initialize_backbone(self, num_channels, backbone_arch, multi_image, weights):
         # Load backbone model according to specified architecture.
@@ -145,14 +151,15 @@
         return None
 
     def forward(self, imgs, targets=None):
         # Define forward pass
         x = self.backbone(imgs)
         if self.fpn:
             x = self.fpn(x)
+            x = self.upsample(x)
         if self.head:
             x, loss = self.head(imgs, x, targets)
             return x, loss
         return x
 
 
 if __name__ == "__main__":
@@ -195,9 +202,12 @@
                     }]
             elif head == Head.INSTANCE:
                 rand_targets = [{
                         'boxes': torch.tensor([[100, 100, 110, 110], [30, 30, 40, 40]], dtype=torch.float32),
                         'labels': torch.tensor([0,1], dtype=torch.int64),
                         'masks': torch.zeros_like(rand_img)
                     }]
+            elif head in [Head.SEGMENT, Head.BINSEGMENT, Head.REGRESS]:
+                rand_targets = torch.zeros_like((rand_img))
+
             output, loss = model(rand_img, rand_targets)
             print("Successfully initialized the pretrained model with ID:", model_id, " with FPN and randomly initialized ", head, " Head.")
```

### Comparing `satlaspretrain_models-0.2.0/satlaspretrain_models/models/backbones.py` & `satlaspretrain_models-0.3.0/satlaspretrain_models/models/backbones.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch.nn
 import torchvision
 
 class SwinBackbone(torch.nn.Module):
-    def __init__(self, num_channels, arch='swinb'):
+    def __init__(self, num_channels, arch):
         super(SwinBackbone, self).__init__()
 
         if arch == 'swinb':
             self.backbone = torchvision.models.swin_v2_b()
             self.out_channels = [
                 [4, 128],
                 [8, 256],
```

### Comparing `satlaspretrain_models-0.2.0/satlaspretrain_models/models/heads.py` & `satlaspretrain_models-0.3.0/satlaspretrain_models/models/heads.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,50 +172,50 @@
         raw_outputs = self.layers(raw_features[0])
         loss = None
 
         if self.task_type == 'segment':
             outputs = torch.nn.functional.softmax(raw_outputs, dim=1)
 
             if targets is not None:
-                task_targets = torch.stack([target for target in targets], dim=0)
-                loss = self.loss_func(raw_outputs, task_targets.long())
+                task_targets = torch.stack([target for target in targets], dim=0).long()
+                loss = self.loss_func(raw_outputs, task_targets)
                 loss = loss.mean()
 
         elif self.task_type == 'bin_segment':
             outputs = torch.nn.functional.softmax(raw_outputs, dim=1)
 
             if targets is not None:
-                task_targets = torch.stack([target for target in targets], dim=0)
-                loss = self.loss_func(raw_outputs, task_targets.float())
+                task_targets = torch.stack([target for target in targets], dim=0).long()
+                loss = self.loss_func(raw_outputs, task_targets)
                 loss = loss.mean()
 
         elif self.task_type == 'regress':
             raw_outputs = raw_outputs[:, 0, :, :]
             outputs = 255*raw_outputs
 
             if targets is not None:
-                task_targets = torch.stack([target for target in targets], dim=0)
+                task_targets = torch.stack([target for target in targets], dim=0).long()
                 loss = self.loss_func(raw_outputs, task_targets.float()/255)
                 loss = loss.mean()
 
         elif self.task_type == 'classification':
             features = torch.amax(raw_outputs, dim=(2,3))
             logits = self.extra(features)
             outputs = torch.nn.functional.softmax(logits, dim=1)
 
             if targets is not None:
-                task_targets = targets.to(torch.long)
+                task_targets = torch.stack([target for target in targets], dim=0).long()
                 loss = self.loss_func(logits, task_targets)
                 loss = loss.mean()
 
         elif self.task_type == 'multi-label-classification':
             features = torch.amax(raw_outputs, dim=(2,3))
             logits = self.extra(features)
             outputs = torch.sigmoid(logits)
 
             if targets is not None:
-                task_targets = torch.cat([target for target in targets], dim=0).to(torch.float32)
+                task_targets = torch.stack([target for target in targets], dim=0).long()
                 loss = self.loss_func(logits, task_targets)
                 loss = loss.mean()
 
         return outputs, loss
```

### Comparing `satlaspretrain_models-0.2.0/satlaspretrain_models/utils.py` & `satlaspretrain_models-0.3.0/satlaspretrain_models/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,14 +85,26 @@
     },
     'Sentinel2_SwinT_SI_MS': {
         'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true',
         'backbone': Backbone.SWINT,
         'num_channels': 9,
         'multi_image': False
     },
+    'Sentinel2_SwinT_MI_RGB': {
+        'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_rgb.pth?download=true',
+        'backbone': Backbone.SWINT,
+        'num_channels': 3,
+        'multi_image': True
+    },
+    'Sentinel2_SwinT_MI_MS': {
+        'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_ms.pth?download=true',
+        'backbone': Backbone.SWINT,
+        'num_channels': 9,
+        'multi_image': True
+    },
     'Sentinel2_Resnet50_SI_RGB': {
         'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_si_rgb.pth?download=true',
         'backbone': Backbone.RESNET50,
         'num_channels': 3,
         'multi_image': False
     },
     'Sentinel2_Resnet50_SI_MS': {
@@ -103,14 +115,20 @@
     },
     'Sentinel2_Resnet50_MI_RGB': {
         'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_rgb.pth?download=true',
         'backbone': Backbone.RESNET50,
         'num_channels': 3,
         'multi_image': True
     },
+    'Sentinel2_Resnet50_MI_MS': {
+        'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_ms.pth?download=true',
+        'backbone': Backbone.RESNET50,
+        'num_channels': 9,
+        'multi_image': True
+    },
     'Sentinel2_Resnet152_SI_RGB': {
         'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_rgb.pth?download=true',
         'backbone': Backbone.RESNET152,
         'num_channels': 3,
         'multi_image': False
     },
     'Sentinel2_Resnet152_SI_MS': {
@@ -121,14 +139,20 @@
     },
     'Sentinel2_Resnet152_MI_RGB': {
         'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_rgb.pth?download=true',
         'backbone': Backbone.RESNET152,
         'num_channels': 3,
         'multi_image': True
     },
+    'Sentinel2_Resnet152_MI_MS': {
+        'url': 'https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_ms.pth?download=true',
+        'backbone': Backbone.RESNET152,
+        'num_channels': 9,
+        'multi_image': True
+    },
 }
 
 
 def adjust_state_dict_prefix(state_dict, needed, prefix=None, prefix_allowed_count=None):
     """
     Adjusts the keys in the state dictionary by replacing 'backbone.backbone' prefix with 'backbone'.
```

### Comparing `satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/PKG-INFO` & `satlaspretrain_models-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: satlaspretrain-models
-Version: 0.2.0
-Summary: A simple package that makes it easy to load remote sensing foundation models for downstream use cases.
-Home-page: https://github.com/allenai/satlaspretrain_models
-Author: Satlas @ AI2
-Author-email: satlas@allenai.org
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=2.1.0
-Requires-Dist: torchvision>=0.16.0
-Requires-Dist: requests
-Requires-Dist: matplotlib
-Requires-Dist: pytest
-Requires-Dist: notebook
-
 SatlasPretrain Models: Foundation models for satellite and aerial imagery.
 --------------------------------------------------------------------------
 
 **SatlasPretrain** is a large-scale pre-training dataset for remote sensing image understanding. This work
 was published at ICCV 2023. Details and download links for the dataset can be found
 [here](https://github.com/allenai/satlas/blob/main/SatlasPretrain.md).
 
@@ -70,23 +50,24 @@
 Checkpoints are released under [ODC-BY](https://github.com/allenai/satlas/blob/main/DataLicense).
 This package will download model checkpoints automatically, but you can download them directly using the links below if desired.
 
 #### Sentinel-2 Pretrained Models
 |  | Single-image, RGB | Multi-image, RGB |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel2_SwinB_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_si_rgb.pth?download=true) | [Sentinel2_SwinB_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_mi_rgb.pth?download=true) |
-| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_rgb.pth?download=true) | |
+| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_rgb.pth?download=true) | [Sentinel2_SwinT_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_rgb.pth?download=true) |
 | **Resnet50** | [Sentinel2_Resnet50_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_si_rgb.pth?download=true) | [Sentinel2_Resnet50_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_rgb.pth?download=true) |
 | **Resnet152** | [Sentinel2_Resnet152_SI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_rgb.pth?download=true) | [Sentinel2_Resnet152_MI_RGB](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_rgb.pth?download=true) |
 
 |  | Single-image, MS | Multi-image, MS |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel2_SwinB_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_si_ms.pth?download=true) | [Sentinel2_SwinB_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swinb_mi_ms.pth?download=true) |
-| **Resnet50** | [Sentinel2_Resnet50_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | |
-| **Resnet152** | [Sentinel2_Resnet152_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_ms.pth?download=true) | |
+| **Swin-v2-Tiny** | [Sentinel2_SwinT_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | [Sentinel2_SwinT_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_mi_ms.pth?download=true) |
+| **Resnet50** | [Sentinel2_Resnet50_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_swint_si_ms.pth?download=true) | [Sentinel2_Resnet50_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet50_mi_ms.pth?download=true) |
+| **Resnet152** | [Sentinel2_Resnet152_SI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_si_ms.pth?download=true) | [Sentinel2_Resnet152_MI_MS](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel2_resnet152_mi_ms.pth?download=true) |
 
 #### Sentinel-1 Pretrained Models
 |  | Single-image, VH+VV | Multi-image, VH+VV |
 | ---------- | ------------ | ------------ |
 | **Swin-v2-Base** | [Sentinel1_SwinB_SI](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel1_swinb_si.pth?download=true) | [Sentinel1_SwinB_MI](https://huggingface.co/allenai/satlas-pretrain/resolve/main/sentinel1_swinb_mi.pth?download=true) |
 
 #### Landsat 8/9 Pretrained Models
@@ -212,14 +193,19 @@
 ```
 
 Demos
 -----
 We provide a [demo](https://github.com/allenai/satlaspretrain_models/blob/main/demo.ipynb) showing how to finetune a 
 SatlasPretrain Sentinel-2 model on the EuroSAT classification task.
 
+We also provide a [torchgeo demo](https://github.com/allenai/satlaspretrain_models/blob/main/torchgeo_demo.ipynb), 
+showing how to load SatlasPretrain weights into a model, download a dataset, initialize a trainer, and finetune the model on the UCMerced classification task. 
+*Note*: a separate conda environment must be initialized to run this demo, see details in the notebook. 
+ 
+
 Tests
 -----
 There are tests to test loading pretrained models and one to test randomly initialized models.
 
 To run the tests, run the following command from the root directory:
 `pytest tests/`
```

### Comparing `satlaspretrain_models-0.2.0/satlaspretrain_models.egg-info/SOURCES.txt` & `satlaspretrain_models-0.3.0/satlaspretrain_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satlaspretrain_models-0.2.0/setup.py` & `satlaspretrain_models-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="satlaspretrain_models",
-    version="0.2.0",
+    version="0.3.0",
     author="Satlas @ AI2",
     author_email="satlas@allenai.org",
     description="A simple package that makes it easy to load remote sensing foundation models for downstream use cases.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/allenai/satlaspretrain_models",
     packages=find_packages(),
```

### Comparing `satlaspretrain_models-0.2.0/tests/test_pretrained_models.py` & `satlaspretrain_models-0.3.0/tests/test_pretrained_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,43 +10,55 @@
     return Weights()
 
 # Test loading pretrained backbone models without FPN or Head
 @pytest.mark.parametrize("model_id", SatlasPretrain_weights.keys())
 def test_pretrained_backbone(weights_manager, model_id):
     model_info = SatlasPretrain_weights[model_id]
     model = weights_manager.get_pretrained_model(model_id)
-    rand_img = torch.rand((8, model_info['num_channels'], 128, 128))
+    rand_img = torch.rand((8, model_info['num_channels'], 128, 128)).float()
     output = model(rand_img)
     assert output is not None
 
 # Test loading pretrained backbone models with FPN, without Head
 @pytest.mark.parametrize("model_id", SatlasPretrain_weights.keys())
 def test_pretrained_backbone_with_fpn(weights_manager, model_id):
     model_info = SatlasPretrain_weights[model_id]
     model = weights_manager.get_pretrained_model(model_id, fpn=True)
-    rand_img = torch.rand((8, model_info['num_channels'], 128, 128))
+    rand_img = torch.rand((8, model_info['num_channels'], 128, 128)).float()
     output = model(rand_img)
     assert output is not None
 
 # Test loading pretrained backbones with FPN and every possible Head
 @pytest.mark.parametrize("model_id,head", [(model_id, head) for model_id in SatlasPretrain_weights.keys() for head in Head])
 def test_pretrained_backbone_with_fpn_and_head(weights_manager, model_id, head):
     model_info = SatlasPretrain_weights[model_id]
     model = weights_manager.get_pretrained_model(model_id, fpn=True, head=head, num_categories=2)
-    rand_img = torch.rand((1, model_info['num_channels'], 128, 128))
+    rand_img = torch.rand((1, model_info['num_channels'], 128, 128)).float()
 
     rand_targets = None
     if head == Head.DETECT:
         rand_targets = [{
             'boxes': torch.tensor([[100, 100, 110, 110], [30, 30, 40, 40]], dtype=torch.float32),
             'labels': torch.tensor([0,1], dtype=torch.int64)
         }]
     elif head == Head.INSTANCE:
         rand_targets = [{
             'boxes': torch.tensor([[100, 100, 110, 110], [30, 30, 40, 40]], dtype=torch.float32),
             'labels': torch.tensor([0,1], dtype=torch.int64),
             'masks': torch.zeros_like(rand_img)
         }]
-    
-    output, loss = model(rand_img, rand_targets) if rand_targets else model(rand_img)
-    assert output is not None and loss is not None
+    elif head == Head.BINSEGMENT:
+        rand_targets = torch.zeros((1, 2, 32, 32))
+    elif head == Head.REGRESS:
+        rand_targets = torch.zeros((1, 2, 32, 32)).float()
+    elif head == Head.CLASSIFY:
+        rand_targets = torch.tensor([1])
 
+    # TODO: add rand_targets for SEGMENT and MULTICLASSIFY
+
+    if rand_targets is not None:
+        output, loss = model(rand_img, rand_targets)
+        assert output is not None
+        assert loss is not None
+    else:
+        output = model(rand_img)
+        assert output is not None
```

### Comparing `satlaspretrain_models-0.2.0/tests/test_randomly_initialized_models.py` & `satlaspretrain_models-0.3.0/tests/test_randomly_initialized_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,40 +4,53 @@
 from satlaspretrain_models.model import Model
 from satlaspretrain_models.utils import Backbone, Head
 
 # Test loading randomly initialized backbone models without FPN or Head
 @pytest.mark.parametrize("backbone", [backbone for backbone in Backbone])
 def test_random_backbone(backbone):
     model = Model(num_channels=3, multi_image=False, backbone=backbone, fpn=False, head=None, num_categories=None, weights=None)
-    rand_img = torch.rand((8, 3, 128, 128))
+    rand_img = torch.rand((8, 3, 128, 128)).float()
     output = model(rand_img)
     assert output is not None
 
 # Test loading randomly initialized backbone models with FPN, without Head
 @pytest.mark.parametrize("backbone", [backbone for backbone in Backbone])
 def test_random_backbone_with_fpn(backbone):
     model = Model(num_channels=3, multi_image=False, backbone=backbone, fpn=True, head=None, num_categories=None, weights=None)
-    rand_img = torch.rand((8, 3, 128, 128))
+    rand_img = torch.rand((8, 3, 128, 128)).float()
     output = model(rand_img)
     assert output is not None
 
 # Test loading pretrained backbones with FPN and every possible Head
 @pytest.mark.parametrize("backbone,head", [(backbone, head) for backbone in Backbone for head in Head])
 def test_random_backbone_with_fpn_and_head(backbone, head):
     model = Model(num_channels=3, multi_image=False, backbone=backbone, fpn=True, head=head, num_categories=2, weights=None)
-    rand_img = torch.rand((1, 3, 128, 128))
+    rand_img = torch.rand((1, 3, 128, 128)).float()
 
     rand_targets = None
     if head == Head.DETECT:
         rand_targets = [{
             'boxes': torch.tensor([[100, 100, 110, 110], [30, 30, 40, 40]], dtype=torch.float32),
             'labels': torch.tensor([0,1], dtype=torch.int64)
         }]
     elif head == Head.INSTANCE:
         rand_targets = [{
             'boxes': torch.tensor([[100, 100, 110, 110], [30, 30, 40, 40]], dtype=torch.float32),
             'labels': torch.tensor([0,1], dtype=torch.int64),
             'masks': torch.zeros_like(rand_img)
         }]
+    elif head == Head.BINSEGMENT:
+        rand_targets = torch.zeros((1, 2, 32, 32))
+    elif head == Head.REGRESS:
+        rand_targets = torch.zeros((1, 2, 32, 32)).float()
+    elif head == Head.CLASSIFY:
+        rand_targets = torch.tensor([1])
 
-    output, loss = model(rand_img, rand_targets) if rand_targets else model(rand_img)
-    assert output is not None and loss is not None
+    # TODO: add rand_targets for SEGMENT and MULTICLASSIFY
+
+    if rand_targets is not None:
+        output, loss = model(rand_img, rand_targets)
+        assert output is not None
+        assert loss is not None
+    else:
+        output = model(rand_img)
+        assert output is not None
```

