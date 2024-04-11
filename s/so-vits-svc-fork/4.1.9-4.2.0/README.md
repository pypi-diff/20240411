# Comparing `tmp/so_vits_svc_fork-4.1.9.tar.gz` & `tmp/so_vits_svc_fork-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.1.9.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.2.0.tar", max compression
```

## Comparing `so_vits_svc_fork-4.1.9.tar` & `so_vits_svc_fork-4.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2023-09-16 02:51:22.483109 so_vits_svc_fork-4.1.9/LICENSE
--rw-r--r--   0        0        0    30142 2023-09-16 02:51:22.483109 so_vits_svc_fork-4.1.9/README.md
--rw-r--r--   0        0        0     3094 2023-09-16 02:51:23.559106 so_vits_svc_fork-4.1.9/pyproject.toml
--rw-r--r--   0        0        0       70 2023-09-16 02:51:23.511106 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24947 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     4914 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    30617 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24749 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9418 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     2206 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    15617 2023-09-16 02:51:22.487109 so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    31951 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.1.9/PKG-INFO
+-rw-r--r--   0        0        0    12463 2024-04-11 03:10:27.152538 so_vits_svc_fork-4.2.0/LICENSE
+-rw-r--r--   0        0        0    33321 2024-04-11 03:10:27.152538 so_vits_svc_fork-4.2.0/README.md
+-rw-r--r--   0        0        0     3121 2024-04-11 03:10:27.952539 so_vits_svc_fork-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-04-11 03:10:27.916539 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24947 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     4914 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30617 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      872 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24749 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9418 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4733 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     3004 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2206 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    15617 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    35235 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.2.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.1.9/LICENSE` & `so_vits_svc_fork-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/README.md` & `so_vits_svc_fork-4.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SoftVC VITS Singing Voice Conversion Fork
 
 [简体中文](README_zh_CN.md)
 
 <p align="center">
-  <a href="https://github.com/34j/so-vits-svc-fork/actions/workflows/ci.yml?query=branch%3Amain">
-    <img src="https://img.shields.io/github/actions/workflow/status/34j/so-vits-svc-fork/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  <a href="https://github.com/voicepaw/so-vits-svc-fork/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/voicepaw/so-vits-svc-fork/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://so-vits-svc-fork.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/so-vits-svc-fork.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
   </a>
-  <a href="https://codecov.io/gh/34j/so-vits-svc-fork">
-    <img src="https://img.shields.io/codecov/c/github/34j/so-vits-svc-fork.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  <a href="https://codecov.io/gh/voicepaw/so-vits-svc-fork">
+    <img src="https://img.shields.io/codecov/c/github/voicepaw/so-vits-svc-fork.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
     <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
   </a>
   <a href="https://github.com/ambv/black">
@@ -30,33 +30,37 @@
   </a>
   <img src="https://img.shields.io/pypi/pyversions/so-vits-svc-fork.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/so-vits-svc-fork.svg?style=flat-square" alt="License">
 </p>
 
 A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with **realtime support** and **greatly improved interface**. Based on branch `4.0` (v1) (or `4.1`) and the models are compatible.
 
+> Updates to this repository have been limited to maintenance since Spring 2023.
+> It is difficult to narrow the list of alternatives here, but please consider trying other projects if you are looking for a voice changer with even better performance (especially in terms of latency other than quality).
+> However, this project may be ideal for those who want to try out voice conversion for the moment (because it is easy to install).
+
 ## Features not available in the original repo
 
 - **Realtime voice conversion** (enhanced in v1.1.0)
 - Integrates [`QuickVC`](https://github.com/quickvc/QuickVC-VoiceConversion)
 - Fixed misuse of [`ContentVec`](https://github.com/auspicious3000/contentvec) in the original repository.[^c]
 - More accurate pitch estimation using [`CREPE`](https://github.com/marl/crepe/).
 - GUI and unified CLI available
 - ~2x faster training
 - Ready to use just by installing with `pip`.
 - Automatically download pretrained models. No need to install `fairseq`.
 - Code completely formatted with black, isort, autoflake etc.
 
-[^c]: [#206](https://github.com/34j/so-vits-svc-fork/issues/206)
+[^c]: [#206](https://github.com/voicepaw/so-vits-svc-fork/issues/206)
 
 ## Installation
 
 ### Option 1. One click easy installation
 
-<a href="https://github.com/34j/so-vits-svc-fork/releases/download/v1.3.2/install.bat" download>
+<a href="https://github.com/voicepaw/so-vits-svc-fork/releases/download/v1.3.2/install.bat" download>
   <img src="https://img.shields.io/badge/.bat-download-blue?style=flat-square&logo=windows" alt="Download .bat">
 </a>
 
 This BAT file will automatically perform the steps described below.
 
 ### Option 2. Manual installation (using pipx, experimental)
 
@@ -76,15 +80,15 @@
 python -m pipx ensurepath
 ```
 
 #### 2. Installing so-vits-svc-fork
 
 ```shell
 pipx install so-vits-svc-fork --python=3.10
-pipx inject so-vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://download.pytorch.org/whl/cu118 # https://download.pytorch.org/whl/nightly/cu121
+pipx inject so-vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 ```
 
 ### Option 3. Manual installation
 
 <details>
   <summary>Creating a virtual environment</summary>
 
@@ -113,23 +117,23 @@
 
 </details>
 
 Install this via pip (or your favourite package manager that uses pip):
 
 ```shell
 python -m pip install -U pip setuptools wheel
-pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118 # https://download.pytorch.org/whl/nightly/cu121
+pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 pip install -U so-vits-svc-fork
 ```
 
 <details>
   <summary>Notes</summary>
 
-- If no GPU is available or using MacOS, simply remove `pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118`. MPS is probably supported.
-- If you are using an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/cu118` with `--index-url https://download.pytorch.org/whl/nightly/rocm5.6`. AMD GPUs are not supported on Windows ([#120](https://github.com/34j/so-vits-svc-fork/issues/120)).
+- If no GPU is available or using MacOS, simply remove `pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu121`. MPS is probably supported.
+- If you are using an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/cu121` with `--index-url https://download.pytorch.org/whl/nightly/rocm5.7`. AMD GPUs are not supported on Windows ([#120](https://github.com/voicepaw/so-vits-svc-fork/issues/120)).
   </details>
 
 ### Update
 
 Please update this package regularly to get the latest features and bug fixes.
 
 ```shell
@@ -139,15 +143,15 @@
 
 ## Usage
 
 ### Inference
 
 #### GUI
 
-![GUI](https://raw.githubusercontent.com/34j/so-vits-svc-fork/main/docs/_static/gui.png)
+![GUI](https://raw.githubusercontent.com/voicepaw/so-vits-svc-fork/main/docs/_static/gui.png)
 
 GUI launches with the following command:
 
 ```shell
 svcg
 ```
 
@@ -185,16 +189,16 @@
 - If your dataset is a long audio file with multiple speakers, use `svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
 - To manually classify audio files, `svc pre-classify` is available. Up and down arrow keys can be used to change the playback speed.
 
 [^1]: https://ytpmv.info/how-to-use-uvr/
 
 #### Cloud
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
-[![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/voicepaw/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
+[![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/voicepaw/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
 [![Paperspace Referral](<https://img.shields.io/badge/Referral%20($10)-9VJN74I-blue?style=flat-square&logo=paperspace>)](https://www.paperspace.com/?r=9VJN74I)[^p]
 
 If you do not have access to a GPU with more than 10 GB of VRAM, the free plan of Google Colab is recommended for light users and the Pro/Growth plan of Paperspace is recommended for heavy users. Conversely, if you have access to a high-end GPU, the use of cloud services is not recommended.
 
 [^p]: If you register a referral code and then add a payment method, you may save about $5 on your first month's monthly billing. Note that both referral rewards are Paperspace credits and not cash. It was a tough decision but inserted because debugging and training the initial model requires a large amount of computing power and the developer is a student.
 
 #### Local
@@ -214,15 +218,15 @@
 - Need at least 4GB of VRAM. [^r-training]
 - It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity. Setting `batch_size` to `auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically increase `batch_size` until OOM error occurs, but may not be useful in some cases.
 - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm crepe`.
 - To use `ContentVec` correctly, replace `svc pre-config` with `-t so-vits-svc-4.0v1`. Training may take slightly longer because some weights are reset due to reusing legacy initial generator weights.
 - To use `MS-iSTFT Decoder`, replace `svc pre-config` with `svc pre-config -t quickvc`.
 - Silence removal and volume normalization are automatically performed (as in the upstream repo) and are not required.
 - If you have trained on a large, copyright-free dataset, consider releasing it as an initial model.
-- For further details (e.g. parameters, etc.), you can see the [Wiki](https://github.com/34j/so-vits-svc-fork/wiki) or [Discussions](https://github.com/34j/so-vits-svc-fork/discussions).
+- For further details (e.g. parameters, etc.), you can see the [Wiki](https://github.com/voicepaw/so-vits-svc-fork/wiki) or [Discussions](https://github.com/voicepaw/so-vits-svc-fork/discussions).
 
 [^r-training]: [#456](https://github.com/voicepaw/so-vits-svc-fork/issues/456)
 
 ### Further help
 
 For more details, run `svc -h` or `svc <subcommand> -h`.
 
@@ -318,14 +322,23 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ph0rk0z"><img src="https://avatars.githubusercontent.com/u/59298527?v=4?s=80" width="80px;" alt="Forkoz"/><br /><sub><b>Forkoz</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3APh0rk0z" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Ph0rk0z" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zerui18"><img src="https://avatars.githubusercontent.com/u/34794550?v=4?s=80" width="80px;" alt="Zerui Chen"/><br /><sub><b>Zerui Chen</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Zerui18" title="Code">💻</a> <a href="#ideas-Zerui18" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.meimadix.com"><img src="https://avatars.githubusercontent.com/u/653972?v=4?s=80" width="80px;" alt="Roee Shenberg"/><br /><sub><b>Roee Shenberg</b></sub></a><br /><a href="#userTesting-shenberg" title="User Testing">📓</a> <a href="#ideas-shenberg" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=shenberg" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ShinyJustyZ"><img src="https://avatars.githubusercontent.com/u/65282440?v=4?s=80" width="80px;" alt="Justas"/><br /><sub><b>Justas</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AShinyJustyZ" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=ShinyJustyZ" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://onako2.github.io/"><img src="https://avatars.githubusercontent.com/u/79749977?v=4?s=80" width="80px;" alt="Onako2"/><br /><sub><b>Onako2</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Onako2" title="Documentation">📖</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/4ll0w3v1l"><img src="https://avatars.githubusercontent.com/u/53517147?v=4?s=80" width="80px;" alt="4ll0w3v1l"/><br /><sub><b>4ll0w3v1l</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=4ll0w3v1l" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/SamuelSwartzberg"><img src="https://avatars.githubusercontent.com/u/16353439?v=4?s=80" width="80px;" alt="j5y0V6b"/><br /><sub><b>j5y0V6b</b></sub></a><br /><a href="#security-SamuelSwartzberg" title="Security">🛡️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/marcellocirelli"><img src="https://avatars.githubusercontent.com/u/51972090?v=4?s=80" width="80px;" alt="marcellocirelli"/><br /><sub><b>marcellocirelli</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Amarcellocirelli" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Priyanshu-hawk"><img src="https://avatars.githubusercontent.com/u/76026651?v=4?s=80" width="80px;" alt="Priyanshu Patel"/><br /><sub><b>Priyanshu Patel</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Priyanshu-hawk" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/annagorshunova"><img src="https://avatars.githubusercontent.com/u/5199204?v=4?s=80" width="80px;" alt="Anna Gorshunova"/><br /><sub><b>Anna Gorshunova</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aannagorshunova" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=annagorshunova" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,84 +1,90 @@
 # SoftVC VITS Singing Voice Conversion Fork [ç®ä½ä¸­æ](README_zh_CN.md)
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with
 **realtime support** and **greatly improved interface**. Based on branch `4.0`
-(v1) (or `4.1`) and the models are compatible. ## Features not available in the
-original repo - **Realtime voice conversion** (enhanced in v1.1.0) - Integrates
-[`QuickVC`](https://github.com/quickvc/QuickVC-VoiceConversion) - Fixed misuse
-of [`ContentVec`](https://github.com/auspicious3000/contentvec) in the original
-repository.[^c] - More accurate pitch estimation using [`CREPE`](https://
-github.com/marl/crepe/). - GUI and unified CLI available - ~2x faster training
-- Ready to use just by installing with `pip`. - Automatically download
-pretrained models. No need to install `fairseq`. - Code completely formatted
-with black, isort, autoflake etc. [^c]: [#206](https://github.com/34j/so-vits-
-svc-fork/issues/206) ## Installation ### Option 1. One click easy installation
-_[_D_o_w_n_l_o_a_d_ _._b_a_t_]This BAT file will automatically perform the steps described
-below. ### Option 2. Manual installation (using pipx, experimental) #### 1.
-Installing pipx Windows (development version required due to [pypa/pipx#940]
-(https://github.com/pypa/pipx/issues/940)): ```shell py -3 -m pip install --
-user git+https://github.com/pypa/pipx.git py -3 -m pipx ensurepath ``` Linux/
-MacOS: ```shell python -m pip install --user pipx python -m pipx ensurepath ```
-#### 2. Installing so-vits-svc-fork ```shell pipx install so-vits-svc-fork --
-python=3.10 pipx inject so-vits-svc-fork torch torchaudio --pip-args="--
-upgrade" --index-url=https://download.pytorch.org/whl/cu118 # https://
-download.pytorch.org/whl/nightly/cu121 ``` ### Option 3. Manual installation
-Creating a virtual environment Windows: ```shell py -3.10 -m venv venv
-venv\Scripts\activate ``` Linux/MacOS: ```shell python3.10 -m venv venv source
-venv/bin/activate ``` Anaconda: ```shell conda create -n so-vits-svc-fork
-python=3.10 pip conda activate so-vits-svc-fork ``` Installing without creating
-a virtual environment may cause a `PermissionError` if Python is installed in
-Program Files, etc. Install this via pip (or your favourite package manager
-that uses pip): ```shell python -m pip install -U pip setuptools wheel pip
-install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118
-# https://download.pytorch.org/whl/nightly/cu121 pip install -U so-vits-svc-
-fork ``` Notes - If no GPU is available or using MacOS, simply remove `pip
-install -U torch torchaudio --index-url https://download.pytorch.org/whl/
-cu118`. MPS is probably supported. - If you are using an AMD GPU on Linux,
-replace `--index-url https://download.pytorch.org/whl/cu118` with `--index-url
-https://download.pytorch.org/whl/nightly/rocm5.6`. AMD GPUs are not supported
-on Windows ([#120](https://github.com/34j/so-vits-svc-fork/issues/120)). ###
-Update Please update this package regularly to get the latest features and bug
-fixes. ```shell pip install -U so-vits-svc-fork # pipx upgrade so-vits-svc-fork
-``` ## Usage ### Inference #### GUI ![GUI](https://raw.githubusercontent.com/
-34j/so-vits-svc-fork/main/docs/_static/gui.png) GUI launches with the following
-command: ```shell svcg ``` #### CLI - Realtime (from microphone) ```shell svc
-vc ``` - File ```shell svc infer source.wav ``` Pretrained models are available
-on [Hugging Face](https://huggingface.co/models?search=so-vits-svc) or
-[CIVITAI](https://civitai.com/?query=so-vits-svc). #### Notes - If using WSL,
-please note that WSL requires additional setup to handle audio and the GUI will
-not work without finding an audio device. - In real-time inference, if there is
-noise on the inputs, the HuBERT model will react to those as well. Consider
-using realtime noise reduction applications such as [RTX Voice](https://
-www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) in this
-case. - Models other than for 4.0v1 or this repository are not supported. - GPU
-inference requires at least 4 GB of VRAM. If it does not work, try CPU
-inference as it is fast enough. [^r-inference] [^r-inference]: [#469](https://
-github.com/voicepaw/so-vits-svc-fork/issues/469) ### Training #### Before
-training - If your dataset has BGM, please remove the BGM using software such
-as [Ultimate Vocal Remover](https://ultimatevocalremover.com/). `3_HP-Vocal-
-UVR.pth` or `UVR-MDX-NET Main` is recommended. [^1] - If your dataset is a long
-audio file with a single speaker, use `svc pre-split` to split the dataset into
-multiple files (using `librosa`). - If your dataset is a long audio file with
-multiple speakers, use `svc pre-sd` to split the dataset into multiple files
-(using `pyannote.audio`). Further manual classification may be necessary due to
-accuracy issues. If speakers speak with a variety of speech styles, set --min-
-speakers larger than the actual number of speakers. Due to unresolved
-dependencies, please install `pyannote.audio` manually: `pip install pyannote-
-audio`. - To manually classify audio files, `svc pre-classify` is available. Up
-and down arrow keys can be used to change the playback speed. [^1]: https://
-ytpmv.info/how-to-use-uvr/ #### Cloud [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-
-vits-svc-fork-4.0.ipynb) [![Open In Paperspace](https://img.shields.io/badge/
-Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://
-console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-
-vits-svc-fork-4.0-paperspace.ipynb) [![Paperspace Referral](
+(v1) (or `4.1`) and the models are compatible. > Updates to this repository
+have been limited to maintenance since Spring 2023. > It is difficult to narrow
+the list of alternatives here, but please consider trying other projects if you
+are looking for a voice changer with even better performance (especially in
+terms of latency other than quality). > However, this project may be ideal for
+those who want to try out voice conversion for the moment (because it is easy
+to install). ## Features not available in the original repo - **Realtime voice
+conversion** (enhanced in v1.1.0) - Integrates [`QuickVC`](https://github.com/
+quickvc/QuickVC-VoiceConversion) - Fixed misuse of [`ContentVec`](https://
+github.com/auspicious3000/contentvec) in the original repository.[^c] - More
+accurate pitch estimation using [`CREPE`](https://github.com/marl/crepe/). -
+GUI and unified CLI available - ~2x faster training - Ready to use just by
+installing with `pip`. - Automatically download pretrained models. No need to
+install `fairseq`. - Code completely formatted with black, isort, autoflake
+etc. [^c]: [#206](https://github.com/voicepaw/so-vits-svc-fork/issues/206) ##
+Installation ### Option 1. One click easy installation _[_D_o_w_n_l_o_a_d_ _._b_a_t_]This BAT
+file will automatically perform the steps described below. ### Option 2. Manual
+installation (using pipx, experimental) #### 1. Installing pipx Windows
+(development version required due to [pypa/pipx#940](https://github.com/pypa/
+pipx/issues/940)): ```shell py -3 -m pip install --user git+https://github.com/
+pypa/pipx.git py -3 -m pipx ensurepath ``` Linux/MacOS: ```shell python -m pip
+install --user pipx python -m pipx ensurepath ``` #### 2. Installing so-vits-
+svc-fork ```shell pipx install so-vits-svc-fork --python=3.10 pipx inject so-
+vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://
+download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
+``` ### Option 3. Manual installation Creating a virtual environment Windows:
+```shell py -3.10 -m venv venv venv\Scripts\activate ``` Linux/MacOS: ```shell
+python3.10 -m venv venv source venv/bin/activate ``` Anaconda: ```shell conda
+create -n so-vits-svc-fork python=3.10 pip conda activate so-vits-svc-fork ```
+Installing without creating a virtual environment may cause a `PermissionError`
+if Python is installed in Program Files, etc. Install this via pip (or your
+favourite package manager that uses pip): ```shell python -m pip install -U pip
+setuptools wheel pip install -U torch torchaudio --index-url https://
+download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
+pip install -U so-vits-svc-fork ``` Notes - If no GPU is available or using
+MacOS, simply remove `pip install -U torch torchaudio --index-url https://
+download.pytorch.org/whl/cu121`. MPS is probably supported. - If you are using
+an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/
+cu121` with `--index-url https://download.pytorch.org/whl/nightly/rocm5.7`. AMD
+GPUs are not supported on Windows ([#120](https://github.com/voicepaw/so-vits-
+svc-fork/issues/120)). ### Update Please update this package regularly to get
+the latest features and bug fixes. ```shell pip install -U so-vits-svc-fork #
+pipx upgrade so-vits-svc-fork ``` ## Usage ### Inference #### GUI ![GUI](https:
+//raw.githubusercontent.com/voicepaw/so-vits-svc-fork/main/docs/_static/
+gui.png) GUI launches with the following command: ```shell svcg ``` #### CLI -
+Realtime (from microphone) ```shell svc vc ``` - File ```shell svc infer
+source.wav ``` Pretrained models are available on [Hugging Face](https://
+huggingface.co/models?search=so-vits-svc) or [CIVITAI](https://civitai.com/
+?query=so-vits-svc). #### Notes - If using WSL, please note that WSL requires
+additional setup to handle audio and the GUI will not work without finding an
+audio device. - In real-time inference, if there is noise on the inputs, the
+HuBERT model will react to those as well. Consider using realtime noise
+reduction applications such as [RTX Voice](https://www.nvidia.com/en-us/
+geforce/guides/nvidia-rtx-voice-setup-guide/) in this case. - Models other than
+for 4.0v1 or this repository are not supported. - GPU inference requires at
+least 4 GB of VRAM. If it does not work, try CPU inference as it is fast
+enough. [^r-inference] [^r-inference]: [#469](https://github.com/voicepaw/so-
+vits-svc-fork/issues/469) ### Training #### Before training - If your dataset
+has BGM, please remove the BGM using software such as [Ultimate Vocal Remover]
+(https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main`
+is recommended. [^1] - If your dataset is a long audio file with a single
+speaker, use `svc pre-split` to split the dataset into multiple files (using
+`librosa`). - If your dataset is a long audio file with multiple speakers, use
+`svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`).
+Further manual classification may be necessary due to accuracy issues. If
+speakers speak with a variety of speech styles, set --min-speakers larger than
+the actual number of speakers. Due to unresolved dependencies, please install
+`pyannote.audio` manually: `pip install pyannote-audio`. - To manually classify
+audio files, `svc pre-classify` is available. Up and down arrow keys can be
+used to change the playback speed. [^1]: https://ytpmv.info/how-to-use-uvr/
+#### Cloud [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/github/voicepaw/so-vits-svc-fork/
+blob/main/notebooks/so-vits-svc-fork-4.0.ipynb) [![Open In Paperspace](https://
+img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-
+square&logo=paperspace)](https://console.paperspace.com/github/voicepaw/so-
+vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb) [!
+[Paperspace Referral](
 img.shields.io/badge/Referral%20($10)-9VJN74I-blue?style=flat-
 square&logo=paperspace>)](https://www.paperspace.com/?r=9VJN74I)[^p] If you do
 not have access to a GPU with more than 10 GB of VRAM, the free plan of Google
 Colab is recommended for light users and the Pro/Growth plan of Paperspace is
 recommended for heavy users. Conversely, if you have access to a high-end GPU,
 the use of cloud services is not recommended. [^p]: If you register a referral
 code and then add a payment method, you may save about $5 on your first month's
@@ -98,20 +104,20 @@
 correctly, replace `svc pre-config` with `-t so-vits-svc-4.0v1`. Training may
 take slightly longer because some weights are reset due to reusing legacy
 initial generator weights. - To use `MS-iSTFT Decoder`, replace `svc pre-
 config` with `svc pre-config -t quickvc`. - Silence removal and volume
 normalization are automatically performed (as in the upstream repo) and are not
 required. - If you have trained on a large, copyright-free dataset, consider
 releasing it as an initial model. - For further details (e.g. parameters,
-etc.), you can see the [Wiki](https://github.com/34j/so-vits-svc-fork/wiki) or
-[Discussions](https://github.com/34j/so-vits-svc-fork/discussions). [^r-
-training]: [#456](https://github.com/voicepaw/so-vits-svc-fork/issues/456) ###
-Further help For more details, run `svc -h` or `svc -h`. ```shell > svc -
-h Usage: svc [OPTIONS] COMMAND [ARGS]... so-vits-svc allows any folder
-structure for training data. However, the following folder structure is
+etc.), you can see the [Wiki](https://github.com/voicepaw/so-vits-svc-fork/
+wiki) or [Discussions](https://github.com/voicepaw/so-vits-svc-fork/
+discussions). [^r-training]: [#456](https://github.com/voicepaw/so-vits-svc-
+fork/issues/456) ### Further help For more details, run `svc -h` or `svc -h`.
+```shell > svc -h Usage: svc [OPTIONS] COMMAND [ARGS]... so-vits-svc allows any
+folder structure for training data. However, the following folder structure is
 recommended. When training: dataset_raw/{speaker_name}/**/{wav_name}.
 {any_format} When inference: configs/44k/config.json, logs/44k/G_XXXX.pth If
 the folder structure is followed, you DO NOT NEED TO SPECIFY model path, config
 path, etc. (The latest model will be automatically loaded.) To train a model,
 run pre-resample, pre-config, pre-hubert, train. To infer a model, run infer.
 Options: -h, --help Show this message and exit. Commands: clean Clean up files,
 only useful if you are using the default file structure infer Inference onnx
@@ -121,45 +127,50 @@
 be... pre-resample Preprocessing part 1: resample pre-sd Speech diarization
 using pyannote.audio pre-split Split audio files into multiple files train
 Train model If D_0.pth or G_0.pth not found, automatically download from hub.
 train-cluster Train k-means clustering vc Realtime inference from microphone
 ``` #### External Links [Video Tutorial](https://www.youtube.com/
 watch?v=tZn0lcGO5OQ) ## Contributors â¨ Thanks goes to these wonderful people
 ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-   _[_3_4_j_]     _[_G_a_r_r_e_t_t_C_o_n_w_a_y_]   _[_B_l_u_e_A_m_u_l_e_t_]   _[_T_h_r_o_w_a_w_a_y_A_c_c_o_u_n_t_0_1_]    _[_ç_·__]        _[_L_o_r_d_m_a_u_5_]         _[_D_L_9_0_9_]
-    _33_44_jj       _GG_aa_rr_rr_ee_tt_tt_CC_oo_nn_ww_aa_yy     _BB_ll_uu_ee_AA_mm_uu_ll_ee_tt     _TT_hh_rr_oo_ww_aa_ww_aa_yy_AA_cc_cc_oo_uu_nn_tt_00_11      _?ç_?·_?          _LL_oo_rr_dd_mm_aa_uu_55           _DD_LL_99_00_99
- _ð___» _ð__¤_   _ð___» _ð___ _ð___   _ð__¤_ _ð___¬ _ð___»          _ð___          _ð___ _ð___  _ð___ _ð___» _ð__¤_ _ð___§      _ð___
- _ð___ _ð___¡        _ð___             _ð___§                                             _ð___¬ _ð___
+   _[_3_4_j_]     _[_G_a_r_r_e_t_t_C_o_n_w_a_y_]    _[_B_l_u_e_A_m_u_l_e_t_]   _[_T_h_r_o_w_a_w_a_y_A_c_c_o_u_n_t_0_1_]    _[_ç_·__]        _[_L_o_r_d_m_a_u_5_]         _[_D_L_9_0_9_]
+    _33_44_jj       _GG_aa_rr_rr_ee_tt_tt_CC_oo_nn_ww_aa_yy      _BB_ll_uu_ee_AA_mm_uu_ll_ee_tt     _TT_hh_rr_oo_ww_aa_ww_aa_yy_AA_cc_cc_oo_uu_nn_tt_00_11      _?ç_?·_?          _LL_oo_rr_dd_mm_aa_uu_55           _DD_LL_99_00_99
+ _ð___» _ð__¤_   _ð___» _ð___ _ð___    _ð__¤_ _ð___¬ _ð___»          _ð___          _ð___ _ð___  _ð___ _ð___» _ð__¤_ _ð___§      _ð___
+ _ð___ _ð___¡        _ð___              _ð___§                                             _ð___¬ _ð___
  _ð___ _ð___§
 _ð___ _â__ _ï_¸_
   _â__ _ð___£
     _ð___
-_[_S_a_t_i_s_f_y_2_5_6_]    _[_P_i_e_r_l_u_i_g_i   _[_r_u_c_k_u_s_m_a_t_t_s_t_e_r_]       _[_D_e_s_u_k_a_-_a_r_t_]   _[_h_e_y_f_i_x_i_t_]     _[_N_e_r_d_y_ _R_o_d_e_n_t_]      _[_è_°_¢_å_®__]
- _SS_aa_tt_ii_ss_ff_yy_22_55_66      _Z_a_g_a_r_i_a_]     _rr_uu_cc_kk_uu_ss_mm_aa_tt_tt_ss_tt_ee_rr         _DD_ee_ss_uu_kk_aa_--_aa_rr_tt     _hh_ee_yy_ff_ii_xx_ii_tt       _NN_ee_rr_dd_yy_ _RR_oo_dd_ee_nn_tt        _?è_?°_?¢_?å_?®_?
-    _ð___         _PP_ii_ee_rr_ll_uu_ii_gg_ii         _ð___                 _ð___          _ð___             _ð___¹             _ð___
+_[_S_a_t_i_s_f_y_2_5_6_]    _[_P_i_e_r_l_u_i_g_i   _[_r_u_c_k_u_s_m_a_t_t_s_t_e_r_]        _[_D_e_s_u_k_a_-_a_r_t_]   _[_h_e_y_f_i_x_i_t_]     _[_N_e_r_d_y_ _R_o_d_e_n_t_]      _[_è_°_¢_å_®__]
+ _SS_aa_tt_ii_ss_ff_yy_22_55_66      _Z_a_g_a_r_i_a_]     _rr_uu_cc_kk_uu_ss_mm_aa_tt_tt_ss_tt_ee_rr          _DD_ee_ss_uu_kk_aa_--_aa_rr_tt     _hh_ee_yy_ff_ii_xx_ii_tt       _NN_ee_rr_dd_yy_ _RR_oo_dd_ee_nn_tt        _?è_?°_?¢_?å_?®_?
+    _ð___         _PP_ii_ee_rr_ll_uu_ii_gg_ii         _ð___                  _ð___          _ð___             _ð___¹             _ð___
                   _ZZ_aa_gg_aa_rr_ii_aa
                    _ð___
-_[_C_o_l_d_C_a_w_f_e_e_]   _[_s_b_e_r_s_i_e_r_]       _[_M_e_l_d_o_n_e_r_]          _[_m_m_o_d_e_u_s_h_e_r_]    _[_A_l_o_n_D_a_n_]         _[_L_i_k_k_k_e_z_]     _[_D_u_c_t_ _T_a_p_e
- _CC_oo_ll_dd_CC_aa_ww_ff_ee_ee     _ss_bb_ee_rr_ss_ii_ee_rr         _MM_ee_ll_dd_oo_nn_ee_rr            _mm_mm_oo_dd_ee_uu_ss_hh_ee_rr      _AA_ll_oo_nn_DD_aa_nn           _LL_ii_kk_kk_kk_ee_zz        _G_a_m_e_s_]
-    _ð___     _ð__¤_ _ð___ _ð___   _ð___ _ð__¤_ _ð___»            _ð___          _ð___              _ð___        _DD_uu_cc_tt_ _TT_aa_pp_ee
-                                                                                                      _GG_aa_mm_ee_ss
-                                                                                                       _ð___
- _[_X_i_a_n_g_l_o_n_g       _[_7_5_a_o_s_u_]       _[_t_o_n_y_c_o_8_2_]            _[_y_x_l_l_l_c_]    _[_o_u_t_h_i_p_p_e_d_] _[_e_s_c_o_o_l_i_o_i_n_g_l_e_s_i_a_s_] _[_B_l_a_c_k_s_i_n_g_h_]
-    _H_e_]            _77_55_aa_oo_ss_uu         _tt_oo_nn_yy_cc_oo_88_22              _yy_xx_ll_ll_ll_cc      _oo_uu_tt_hh_ii_pp_pp_ee_dd   _ee_ss_cc_oo_oo_ll_ii_oo_ii_nn_gg_ll_ee_ss_ii_aa_ss   _BB_ll_aa_cc_kk_ss_ii_nn_gg_hh
-_XX_ii_aa_nn_gg_ll_oo_nn_gg_ _HH_ee        _ð___            _ð___              _ð__¤_ _ð___»       _ð___       _ð___ _ð___ _ð___¹        _ð___
+_[_C_o_l_d_C_a_w_f_e_e_]   _[_s_b_e_r_s_i_e_r_]        _[_M_e_l_d_o_n_e_r_]          _[_m_m_o_d_e_u_s_h_e_r_]    _[_A_l_o_n_D_a_n_]         _[_L_i_k_k_k_e_z_]     _[_D_u_c_t_ _T_a_p_e
+ _CC_oo_ll_dd_CC_aa_ww_ff_ee_ee     _ss_bb_ee_rr_ss_ii_ee_rr          _MM_ee_ll_dd_oo_nn_ee_rr            _mm_mm_oo_dd_ee_uu_ss_hh_ee_rr      _AA_ll_oo_nn_DD_aa_nn           _LL_ii_kk_kk_kk_ee_zz        _G_a_m_e_s_]
+    _ð___     _ð__¤_ _ð___ _ð___    _ð___ _ð__¤_ _ð___»            _ð___          _ð___              _ð___        _DD_uu_cc_tt_ _TT_aa_pp_ee
+                                                                                                       _GG_aa_mm_ee_ss
+                                                                                                        _ð___
+ _[_X_i_a_n_g_l_o_n_g       _[_7_5_a_o_s_u_]        _[_t_o_n_y_c_o_8_2_]            _[_y_x_l_l_l_c_]    _[_o_u_t_h_i_p_p_e_d_] _[_e_s_c_o_o_l_i_o_i_n_g_l_e_s_i_a_s_] _[_B_l_a_c_k_s_i_n_g_h_]
+    _H_e_]            _77_55_aa_oo_ss_uu          _tt_oo_nn_yy_cc_oo_88_22              _yy_xx_ll_ll_ll_cc      _oo_uu_tt_hh_ii_pp_pp_ee_dd   _ee_ss_cc_oo_oo_ll_ii_oo_ii_nn_gg_ll_ee_ss_ii_aa_ss   _BB_ll_aa_cc_kk_ss_ii_nn_gg_hh
+_XX_ii_aa_nn_gg_ll_oo_nn_gg_ _HH_ee        _ð___             _ð___              _ð__¤_ _ð___»       _ð___       _ð___ _ð___ _ð___¹        _ð___
     _ð___
-  _[_M_g_s_._ _M_.      _[_E_x_o_s_f_e_e_r_]      _[_g_u_r_a_n_o_n_]      _[_A_l_e_x_a_n_d_e_r_ _K_o_u_m_i_s_]  _[_a_c_e_k_a_g_a_m_i_]       _[_H_i_g_h_u_p_e_c_h_]      _[_S_c_o_r_p_i_]
-   _T_h_o_y_i_b        _EE_xx_oo_ss_ff_ee_ee_rr        _gg_uu_rr_aa_nn_oo_nn        _AA_ll_ee_xx_aa_nn_dd_ee_rr_ _KK_oo_uu_mm_ii_ss    _aa_cc_ee_kk_aa_gg_aa_mm_ii         _HH_ii_gg_hh_uu_pp_ee_cc_hh        _SS_cc_oo_rr_pp_ii
- _A_n_t_a_r_n_u_s_a_]      _ð___ _ð___»    _ð___ _ð__¤_ _ð___»          _ð___»            _ð___              _ð___            _ð___»
+  _[_M_g_s_._ _M_.      _[_E_x_o_s_f_e_e_r_]        _[_g_u_r_a_n_o_n_]     _[_A_l_e_x_a_n_d_e_r_ _K_o_u_m_i_s_]  _[_a_c_e_k_a_g_a_m_i_]       _[_H_i_g_h_u_p_e_c_h_]      _[_S_c_o_r_p_i_]
+   _T_h_o_y_i_b        _EE_xx_oo_ss_ff_ee_ee_rr          _gg_uu_rr_aa_nn_oo_nn       _AA_ll_ee_xx_aa_nn_dd_ee_rr_ _KK_oo_uu_mm_ii_ss    _aa_cc_ee_kk_aa_gg_aa_mm_ii         _HH_ii_gg_hh_uu_pp_ee_cc_hh        _SS_cc_oo_rr_pp_ii
+ _A_n_t_a_r_n_u_s_a_]      _ð___ _ð___»     _ð___ _ð__¤_ _ð___»          _ð___»            _ð___              _ð___            _ð___»
   _MM_gg_ss_.._ _MM_..
    _TT_hh_oo_yy_ii_bb
  _AA_nn_tt_aa_rr_nn_uu_ss_aa
     _ð___
- _[_M_a_x_i_m_x_l_s_]     _[_S_t_a_r_3_L_o_r_d_]        _[_F_o_r_k_o_z_]         _[_Z_e_r_u_i_ _C_h_e_n_]      _[_R_o_e_e
-  _MM_aa_xx_ii_mm_xx_ll_ss       _SS_tt_aa_rr_33_LL_oo_rr_dd          _FF_oo_rr_kk_oo_zz           _ZZ_ee_rr_uu_ii_ _CC_hh_ee_nn     _S_h_e_n_b_e_r_g_]
-    _ð___»         _ð___ _ð___»        _ð___ _ð___»          _ð___» _ð__¤_        _RR_oo_ee_ee
-                                                                    _SS_hh_ee_nn_bb_ee_rr_gg
-                                                                    _ð___ _ð__¤_
-                                                                      _ð___»
+ _[_M_a_x_i_m_x_l_s_]     _[_S_t_a_r_3_L_o_r_d_]        _[_F_o_r_k_o_z_]          _[_Z_e_r_u_i_ _C_h_e_n_]      _[_R_o_e_e           _[_J_u_s_t_a_s_]        _[_O_n_a_k_o_2_]
+  _MM_aa_xx_ii_mm_xx_ll_ss       _SS_tt_aa_rr_33_LL_oo_rr_dd          _FF_oo_rr_kk_oo_zz            _ZZ_ee_rr_uu_ii_ _CC_hh_ee_nn     _S_h_e_n_b_e_r_g_]          _JJ_uu_ss_tt_aa_ss          _OO_nn_aa_kk_oo_22
+    _ð___»         _ð___ _ð___»         _ð___ _ð___»          _ð___» _ð__¤_        _RR_oo_ee_ee            _ð___ _ð___»         _ð___
+                                                                     _SS_hh_ee_nn_bb_ee_rr_gg
+                                                                     _ð___ _ð__¤_
+                                                                       _ð___»
+_[_4_l_l_0_w_3_v_1_l_]      _[_j_5_y_0_V_6_b_]   _[_m_a_r_c_e_l_l_o_c_i_r_e_l_l_i_]   _[_P_r_i_y_a_n_s_h_u_ _P_a_t_e_l_]     _[_A_n_n_a
+ _44_ll_ll_00_ww_33_vv_11_ll        _jj_55_yy_00_VV_66_bb     _mm_aa_rr_cc_ee_ll_ll_oo_cc_ii_rr_ee_ll_ll_ii     _PP_rr_ii_yy_aa_nn_ss_hh_uu_ _PP_aa_tt_ee_ll   _G_o_r_s_h_u_n_o_v_a_]
+    _ð___»          _ð___¡_ï_¸_          _ð___                 _ð___»           _AA_nn_nn_aa
+                                                                    _GG_oo_rr_ss_hh_uu_nn_oo_vv_aa
+                                                                     _ð___ _ð___»
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `so_vits_svc_fork-4.1.9/pyproject.toml` & `so_vits_svc_fork-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.1.9"
+version = "4.2.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -27,15 +27,15 @@
 svcf-gui = "so_vits_svc_fork.gui:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/34j/so-vits-svc-fork/issues"
 "Changelog" = "https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.13"
 librosa = "*"
 numpy = "^1.23"
 pyworld = "*"
 requests = "*"
 scipy = "*"
 sounddevice = "*"
 SoundFile = "*"
@@ -47,30 +47,28 @@
 torch = "*"
 torchaudio = "*"
 tensorboard = "*"
 rich = "*"
 tqdm-joblib = "*"
 tensorboardx = "*"
 cm-time = ">=0.1.2"
-pysimplegui = ">=4.6"
+pysimplegui = ">=4.6,<5" # never update this, advertising popup window will be shown
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
 lightning = "^2.0.1"
-fastapi = "==0.103.1"
+fastapi = "==0.110.1"
 transformers = "^4.28.1"
 matplotlib = "^3.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
-poetry = "^1.4.2"
 pipdeptree = "^2.7.0"
 pip-licenses = "^4.3.1"
-black = "^23.3.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/hparams.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any
 
 
 class HParams:
     def __init__(self, **kwargs: Any) -> None:
         for k, v in kwargs.items():
-            if type(v) == dict:
+            if type(v) == dict:  # noqa
                 v = HParams(**v)
             self[k] = v
 
     def keys(self):
         return self.__dict__.keys()
 
     def items(self):
```

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  MIT License (https://opensource.org/licenses/MIT)
 
 """Pseudo QMF modules."""
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-from scipy.signal import kaiser
+from scipy.signal.windows import kaiser
 
 
 def design_prototype_filter(taps=62, cutoff_ratio=0.15, beta=9.0):
     """Design prototype filter for PQMF.
     This method is based on `A Kaiser window approach for the design of prototype
     filters of cosine modulated filterbanks`_.
     Args:
```

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 ) -> None:
     try:
         audio, sr = librosa.load(input_path, sr=sr, mono=True)
     except Exception as e:
         LOG.warning(f"Failed to read {input_path}: {e}")
         return
     pipeline = Pipeline.from_pretrained(
-        "pyannote/speaker-diarization", use_auth_token=huggingface_token
+        "pyannote/speaker-diarization-3.1", use_auth_token=huggingface_token
     )
     if pipeline is None:
         raise ValueError("Failed to load pipeline")
-
+    pipeline = pipeline.to(torch.device("cuda"))
     LOG.info(f"Processing {input_path}. This may take a while...")
     diarization = pipeline(
         input_path, min_speakers=min_speakers, max_speakers=max_speakers
     )
 
     LOG.info(f"Found {len(diarization)} tracks, writing to {output_dir}")
     speaker_count = defaultdict(int)
@@ -48,15 +48,15 @@
         list(diarization.itertracks(yield_label=True)), desc=f"Writing {input_path}"
     ):
         if segment.end - segment.start < 1:
             continue
         speaker_count[speaker] += 1
         audio_cut = audio[int(segment.start * sr) : int(segment.end * sr)]
         sf.write(
-            (output_dir / f"{speaker}_{speaker_count[speaker]}.wav"),
+            (output_dir / f"{speaker}_{speaker_count[speaker]:04d}.wav"),
             audio_cut,
             sr,
         )
 
     LOG.info(f"Speaker count: {speaker_count}")
```

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.9/PKG-INFO` & `so_vits_svc_fork-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.1.9
+Version: 4.2.0
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: SoundFile
 Requires-Dist: cm-time (>=0.1.2)
-Requires-Dist: fastapi (==0.103.1)
+Requires-Dist: fastapi (==0.110.1)
 Requires-Dist: librosa
 Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: onnx
 Requires-Dist: onnxoptimizer
 Requires-Dist: onnxsim
 Requires-Dist: pebble (>=5.0)
 Requires-Dist: praat-parselmouth
-Requires-Dist: pysimplegui (>=4.6)
+Requires-Dist: pysimplegui (>=4.6,<5)
 Requires-Dist: pyworld
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: scipy
 Requires-Dist: sounddevice
 Requires-Dist: tensorboard
 Requires-Dist: tensorboardx
@@ -50,22 +52,22 @@
 Description-Content-Type: text/markdown
 
 # SoftVC VITS Singing Voice Conversion Fork
 
 [简体中文](README_zh_CN.md)
 
 <p align="center">
-  <a href="https://github.com/34j/so-vits-svc-fork/actions/workflows/ci.yml?query=branch%3Amain">
-    <img src="https://img.shields.io/github/actions/workflow/status/34j/so-vits-svc-fork/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
+  <a href="https://github.com/voicepaw/so-vits-svc-fork/actions/workflows/ci.yml?query=branch%3Amain">
+    <img src="https://img.shields.io/github/actions/workflow/status/voicepaw/so-vits-svc-fork/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >
   </a>
   <a href="https://so-vits-svc-fork.readthedocs.io">
     <img src="https://img.shields.io/readthedocs/so-vits-svc-fork.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
   </a>
-  <a href="https://codecov.io/gh/34j/so-vits-svc-fork">
-    <img src="https://img.shields.io/codecov/c/github/34j/so-vits-svc-fork.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  <a href="https://codecov.io/gh/voicepaw/so-vits-svc-fork">
+    <img src="https://img.shields.io/codecov/c/github/voicepaw/so-vits-svc-fork.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
     <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
   </a>
   <a href="https://github.com/ambv/black">
@@ -81,33 +83,37 @@
   </a>
   <img src="https://img.shields.io/pypi/pyversions/so-vits-svc-fork.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/so-vits-svc-fork.svg?style=flat-square" alt="License">
 </p>
 
 A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with **realtime support** and **greatly improved interface**. Based on branch `4.0` (v1) (or `4.1`) and the models are compatible.
 
+> Updates to this repository have been limited to maintenance since Spring 2023.
+> It is difficult to narrow the list of alternatives here, but please consider trying other projects if you are looking for a voice changer with even better performance (especially in terms of latency other than quality).
+> However, this project may be ideal for those who want to try out voice conversion for the moment (because it is easy to install).
+
 ## Features not available in the original repo
 
 - **Realtime voice conversion** (enhanced in v1.1.0)
 - Integrates [`QuickVC`](https://github.com/quickvc/QuickVC-VoiceConversion)
 - Fixed misuse of [`ContentVec`](https://github.com/auspicious3000/contentvec) in the original repository.[^c]
 - More accurate pitch estimation using [`CREPE`](https://github.com/marl/crepe/).
 - GUI and unified CLI available
 - ~2x faster training
 - Ready to use just by installing with `pip`.
 - Automatically download pretrained models. No need to install `fairseq`.
 - Code completely formatted with black, isort, autoflake etc.
 
-[^c]: [#206](https://github.com/34j/so-vits-svc-fork/issues/206)
+[^c]: [#206](https://github.com/voicepaw/so-vits-svc-fork/issues/206)
 
 ## Installation
 
 ### Option 1. One click easy installation
 
-<a href="https://github.com/34j/so-vits-svc-fork/releases/download/v1.3.2/install.bat" download>
+<a href="https://github.com/voicepaw/so-vits-svc-fork/releases/download/v1.3.2/install.bat" download>
   <img src="https://img.shields.io/badge/.bat-download-blue?style=flat-square&logo=windows" alt="Download .bat">
 </a>
 
 This BAT file will automatically perform the steps described below.
 
 ### Option 2. Manual installation (using pipx, experimental)
 
@@ -127,15 +133,15 @@
 python -m pipx ensurepath
 ```
 
 #### 2. Installing so-vits-svc-fork
 
 ```shell
 pipx install so-vits-svc-fork --python=3.10
-pipx inject so-vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://download.pytorch.org/whl/cu118 # https://download.pytorch.org/whl/nightly/cu121
+pipx inject so-vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 ```
 
 ### Option 3. Manual installation
 
 <details>
   <summary>Creating a virtual environment</summary>
 
@@ -164,23 +170,23 @@
 
 </details>
 
 Install this via pip (or your favourite package manager that uses pip):
 
 ```shell
 python -m pip install -U pip setuptools wheel
-pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118 # https://download.pytorch.org/whl/nightly/cu121
+pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 pip install -U so-vits-svc-fork
 ```
 
 <details>
   <summary>Notes</summary>
 
-- If no GPU is available or using MacOS, simply remove `pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118`. MPS is probably supported.
-- If you are using an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/cu118` with `--index-url https://download.pytorch.org/whl/nightly/rocm5.6`. AMD GPUs are not supported on Windows ([#120](https://github.com/34j/so-vits-svc-fork/issues/120)).
+- If no GPU is available or using MacOS, simply remove `pip install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu121`. MPS is probably supported.
+- If you are using an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/cu121` with `--index-url https://download.pytorch.org/whl/nightly/rocm5.7`. AMD GPUs are not supported on Windows ([#120](https://github.com/voicepaw/so-vits-svc-fork/issues/120)).
   </details>
 
 ### Update
 
 Please update this package regularly to get the latest features and bug fixes.
 
 ```shell
@@ -190,15 +196,15 @@
 
 ## Usage
 
 ### Inference
 
 #### GUI
 
-![GUI](https://raw.githubusercontent.com/34j/so-vits-svc-fork/main/docs/_static/gui.png)
+![GUI](https://raw.githubusercontent.com/voicepaw/so-vits-svc-fork/main/docs/_static/gui.png)
 
 GUI launches with the following command:
 
 ```shell
 svcg
 ```
 
@@ -236,16 +242,16 @@
 - If your dataset is a long audio file with multiple speakers, use `svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`). Further manual classification may be necessary due to accuracy issues. If speakers speak with a variety of speech styles, set --min-speakers larger than the actual number of speakers. Due to unresolved dependencies, please install `pyannote.audio` manually: `pip install pyannote-audio`.
 - To manually classify audio files, `svc pre-classify` is available. Up and down arrow keys can be used to change the playback speed.
 
 [^1]: https://ytpmv.info/how-to-use-uvr/
 
 #### Cloud
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
-[![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/voicepaw/so-vits-svc-fork/blob/main/notebooks/so-vits-svc-fork-4.0.ipynb)
+[![Open In Paperspace](https://img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://console.paperspace.com/github/voicepaw/so-vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb)
 [![Paperspace Referral](<https://img.shields.io/badge/Referral%20($10)-9VJN74I-blue?style=flat-square&logo=paperspace>)](https://www.paperspace.com/?r=9VJN74I)[^p]
 
 If you do not have access to a GPU with more than 10 GB of VRAM, the free plan of Google Colab is recommended for light users and the Pro/Growth plan of Paperspace is recommended for heavy users. Conversely, if you have access to a high-end GPU, the use of cloud services is not recommended.
 
 [^p]: If you register a referral code and then add a payment method, you may save about $5 on your first month's monthly billing. Note that both referral rewards are Paperspace credits and not cash. It was a tough decision but inserted because debugging and training the initial model requires a large amount of computing power and the developer is a student.
 
 #### Local
@@ -265,15 +271,15 @@
 - Need at least 4GB of VRAM. [^r-training]
 - It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity. Setting `batch_size` to `auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically increase `batch_size` until OOM error occurs, but may not be useful in some cases.
 - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm crepe`.
 - To use `ContentVec` correctly, replace `svc pre-config` with `-t so-vits-svc-4.0v1`. Training may take slightly longer because some weights are reset due to reusing legacy initial generator weights.
 - To use `MS-iSTFT Decoder`, replace `svc pre-config` with `svc pre-config -t quickvc`.
 - Silence removal and volume normalization are automatically performed (as in the upstream repo) and are not required.
 - If you have trained on a large, copyright-free dataset, consider releasing it as an initial model.
-- For further details (e.g. parameters, etc.), you can see the [Wiki](https://github.com/34j/so-vits-svc-fork/wiki) or [Discussions](https://github.com/34j/so-vits-svc-fork/discussions).
+- For further details (e.g. parameters, etc.), you can see the [Wiki](https://github.com/voicepaw/so-vits-svc-fork/wiki) or [Discussions](https://github.com/voicepaw/so-vits-svc-fork/discussions).
 
 [^r-training]: [#456](https://github.com/voicepaw/so-vits-svc-fork/issues/456)
 
 ### Further help
 
 For more details, run `svc -h` or `svc <subcommand> -h`.
 
@@ -369,14 +375,23 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ph0rk0z"><img src="https://avatars.githubusercontent.com/u/59298527?v=4?s=80" width="80px;" alt="Forkoz"/><br /><sub><b>Forkoz</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3APh0rk0z" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Ph0rk0z" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zerui18"><img src="https://avatars.githubusercontent.com/u/34794550?v=4?s=80" width="80px;" alt="Zerui Chen"/><br /><sub><b>Zerui Chen</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Zerui18" title="Code">💻</a> <a href="#ideas-Zerui18" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.meimadix.com"><img src="https://avatars.githubusercontent.com/u/653972?v=4?s=80" width="80px;" alt="Roee Shenberg"/><br /><sub><b>Roee Shenberg</b></sub></a><br /><a href="#userTesting-shenberg" title="User Testing">📓</a> <a href="#ideas-shenberg" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=shenberg" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ShinyJustyZ"><img src="https://avatars.githubusercontent.com/u/65282440?v=4?s=80" width="80px;" alt="Justas"/><br /><sub><b>Justas</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AShinyJustyZ" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=ShinyJustyZ" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://onako2.github.io/"><img src="https://avatars.githubusercontent.com/u/79749977?v=4?s=80" width="80px;" alt="Onako2"/><br /><sub><b>Onako2</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Onako2" title="Documentation">📖</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/4ll0w3v1l"><img src="https://avatars.githubusercontent.com/u/53517147?v=4?s=80" width="80px;" alt="4ll0w3v1l"/><br /><sub><b>4ll0w3v1l</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=4ll0w3v1l" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/SamuelSwartzberg"><img src="https://avatars.githubusercontent.com/u/16353439?v=4?s=80" width="80px;" alt="j5y0V6b"/><br /><sub><b>j5y0V6b</b></sub></a><br /><a href="#security-SamuelSwartzberg" title="Security">🛡️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/marcellocirelli"><img src="https://avatars.githubusercontent.com/u/51972090?v=4?s=80" width="80px;" alt="marcellocirelli"/><br /><sub><b>marcellocirelli</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Amarcellocirelli" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Priyanshu-hawk"><img src="https://avatars.githubusercontent.com/u/76026651?v=4?s=80" width="80px;" alt="Priyanshu Patel"/><br /><sub><b>Priyanshu Patel</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Priyanshu-hawk" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/annagorshunova"><img src="https://avatars.githubusercontent.com/u/5199204?v=4?s=80" width="80px;" alt="Anna Gorshunova"/><br /><sub><b>Anna Gorshunova</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3Aannagorshunova" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=annagorshunova" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,108 +1,116 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.1.9 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.2.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
->=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+>=3.8,<3.13 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: SoundFile Requires-
-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi (==0.103.1) Requires-Dist:
-librosa Requires-Dist: lightning (>=2.0.1,<3.0.0) Requires-Dist: matplotlib
-(>=3.7.1,<4.0.0) Requires-Dist: numpy (>=1.23,<2.0) Requires-Dist: onnx
-Requires-Dist: onnxoptimizer Requires-Dist: onnxsim Requires-Dist: pebble
-(>=5.0) Requires-Dist: praat-parselmouth Requires-Dist: pysimplegui (>=4.6)
-Requires-Dist: pyworld Requires-Dist: requests Requires-Dist: rich Requires-
-Dist: scipy Requires-Dist: sounddevice Requires-Dist: tensorboard Requires-
-Dist: tensorboardx Requires-Dist: torch Requires-Dist: torchaudio Requires-
-Dist: torchcrepe (>=0.0.17) Requires-Dist: tqdm Requires-Dist: tqdm-joblib
-Requires-Dist: transformers (>=4.28.1,<5.0.0) Project-URL: Bug Tracker, https:/
-/github.com/34j/so-vits-svc-fork/issues Project-URL: Changelog, https://
-github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://so-vits-svc-fork.readthedocs.io Project-URL: Repository,
-https://github.com/34j/so-vits-svc-fork Description-Content-Type: text/markdown
-# SoftVC VITS Singing Voice Conversion Fork [ç®ä½ä¸­æ](README_zh_CN.md)
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: SoundFile Requires-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi
+(==0.110.1) Requires-Dist: librosa Requires-Dist: lightning (>=2.0.1,<3.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: onnx Requires-Dist: onnxoptimizer Requires-Dist: onnxsim
+Requires-Dist: pebble (>=5.0) Requires-Dist: praat-parselmouth Requires-Dist:
+pysimplegui (>=4.6,<5) Requires-Dist: pyworld Requires-Dist: requests Requires-
+Dist: rich Requires-Dist: scipy Requires-Dist: sounddevice Requires-Dist:
+tensorboard Requires-Dist: tensorboardx Requires-Dist: torch Requires-Dist:
+torchaudio Requires-Dist: torchcrepe (>=0.0.17) Requires-Dist: tqdm Requires-
+Dist: tqdm-joblib Requires-Dist: transformers (>=4.28.1,<5.0.0) Project-URL:
+Bug Tracker, https://github.com/34j/so-vits-svc-fork/issues Project-URL:
+Changelog, https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://so-vits-svc-fork.readthedocs.io Project-
+URL: Repository, https://github.com/34j/so-vits-svc-fork Description-Content-
+Type: text/markdown # SoftVC VITS Singing Voice Conversion Fork [ç®ä½ä¸­æ]
+(README_zh_CN.md)
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with
 **realtime support** and **greatly improved interface**. Based on branch `4.0`
-(v1) (or `4.1`) and the models are compatible. ## Features not available in the
-original repo - **Realtime voice conversion** (enhanced in v1.1.0) - Integrates
-[`QuickVC`](https://github.com/quickvc/QuickVC-VoiceConversion) - Fixed misuse
-of [`ContentVec`](https://github.com/auspicious3000/contentvec) in the original
-repository.[^c] - More accurate pitch estimation using [`CREPE`](https://
-github.com/marl/crepe/). - GUI and unified CLI available - ~2x faster training
-- Ready to use just by installing with `pip`. - Automatically download
-pretrained models. No need to install `fairseq`. - Code completely formatted
-with black, isort, autoflake etc. [^c]: [#206](https://github.com/34j/so-vits-
-svc-fork/issues/206) ## Installation ### Option 1. One click easy installation
-_[_D_o_w_n_l_o_a_d_ _._b_a_t_]This BAT file will automatically perform the steps described
-below. ### Option 2. Manual installation (using pipx, experimental) #### 1.
-Installing pipx Windows (development version required due to [pypa/pipx#940]
-(https://github.com/pypa/pipx/issues/940)): ```shell py -3 -m pip install --
-user git+https://github.com/pypa/pipx.git py -3 -m pipx ensurepath ``` Linux/
-MacOS: ```shell python -m pip install --user pipx python -m pipx ensurepath ```
-#### 2. Installing so-vits-svc-fork ```shell pipx install so-vits-svc-fork --
-python=3.10 pipx inject so-vits-svc-fork torch torchaudio --pip-args="--
-upgrade" --index-url=https://download.pytorch.org/whl/cu118 # https://
-download.pytorch.org/whl/nightly/cu121 ``` ### Option 3. Manual installation
-Creating a virtual environment Windows: ```shell py -3.10 -m venv venv
-venv\Scripts\activate ``` Linux/MacOS: ```shell python3.10 -m venv venv source
-venv/bin/activate ``` Anaconda: ```shell conda create -n so-vits-svc-fork
-python=3.10 pip conda activate so-vits-svc-fork ``` Installing without creating
-a virtual environment may cause a `PermissionError` if Python is installed in
-Program Files, etc. Install this via pip (or your favourite package manager
-that uses pip): ```shell python -m pip install -U pip setuptools wheel pip
-install -U torch torchaudio --index-url https://download.pytorch.org/whl/cu118
-# https://download.pytorch.org/whl/nightly/cu121 pip install -U so-vits-svc-
-fork ``` Notes - If no GPU is available or using MacOS, simply remove `pip
-install -U torch torchaudio --index-url https://download.pytorch.org/whl/
-cu118`. MPS is probably supported. - If you are using an AMD GPU on Linux,
-replace `--index-url https://download.pytorch.org/whl/cu118` with `--index-url
-https://download.pytorch.org/whl/nightly/rocm5.6`. AMD GPUs are not supported
-on Windows ([#120](https://github.com/34j/so-vits-svc-fork/issues/120)). ###
-Update Please update this package regularly to get the latest features and bug
-fixes. ```shell pip install -U so-vits-svc-fork # pipx upgrade so-vits-svc-fork
-``` ## Usage ### Inference #### GUI ![GUI](https://raw.githubusercontent.com/
-34j/so-vits-svc-fork/main/docs/_static/gui.png) GUI launches with the following
-command: ```shell svcg ``` #### CLI - Realtime (from microphone) ```shell svc
-vc ``` - File ```shell svc infer source.wav ``` Pretrained models are available
-on [Hugging Face](https://huggingface.co/models?search=so-vits-svc) or
-[CIVITAI](https://civitai.com/?query=so-vits-svc). #### Notes - If using WSL,
-please note that WSL requires additional setup to handle audio and the GUI will
-not work without finding an audio device. - In real-time inference, if there is
-noise on the inputs, the HuBERT model will react to those as well. Consider
-using realtime noise reduction applications such as [RTX Voice](https://
-www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) in this
-case. - Models other than for 4.0v1 or this repository are not supported. - GPU
-inference requires at least 4 GB of VRAM. If it does not work, try CPU
-inference as it is fast enough. [^r-inference] [^r-inference]: [#469](https://
-github.com/voicepaw/so-vits-svc-fork/issues/469) ### Training #### Before
-training - If your dataset has BGM, please remove the BGM using software such
-as [Ultimate Vocal Remover](https://ultimatevocalremover.com/). `3_HP-Vocal-
-UVR.pth` or `UVR-MDX-NET Main` is recommended. [^1] - If your dataset is a long
-audio file with a single speaker, use `svc pre-split` to split the dataset into
-multiple files (using `librosa`). - If your dataset is a long audio file with
-multiple speakers, use `svc pre-sd` to split the dataset into multiple files
-(using `pyannote.audio`). Further manual classification may be necessary due to
-accuracy issues. If speakers speak with a variety of speech styles, set --min-
-speakers larger than the actual number of speakers. Due to unresolved
-dependencies, please install `pyannote.audio` manually: `pip install pyannote-
-audio`. - To manually classify audio files, `svc pre-classify` is available. Up
-and down arrow keys can be used to change the playback speed. [^1]: https://
-ytpmv.info/how-to-use-uvr/ #### Cloud [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/34j/so-vits-svc-fork/blob/main/notebooks/so-
-vits-svc-fork-4.0.ipynb) [![Open In Paperspace](https://img.shields.io/badge/
-Open%20in-Paperspace-blue?style=flat-square&logo=paperspace)](https://
-console.paperspace.com/github/34j/so-vits-svc-fork-paperspace/blob/main/so-
-vits-svc-fork-4.0-paperspace.ipynb) [![Paperspace Referral](
+(v1) (or `4.1`) and the models are compatible. > Updates to this repository
+have been limited to maintenance since Spring 2023. > It is difficult to narrow
+the list of alternatives here, but please consider trying other projects if you
+are looking for a voice changer with even better performance (especially in
+terms of latency other than quality). > However, this project may be ideal for
+those who want to try out voice conversion for the moment (because it is easy
+to install). ## Features not available in the original repo - **Realtime voice
+conversion** (enhanced in v1.1.0) - Integrates [`QuickVC`](https://github.com/
+quickvc/QuickVC-VoiceConversion) - Fixed misuse of [`ContentVec`](https://
+github.com/auspicious3000/contentvec) in the original repository.[^c] - More
+accurate pitch estimation using [`CREPE`](https://github.com/marl/crepe/). -
+GUI and unified CLI available - ~2x faster training - Ready to use just by
+installing with `pip`. - Automatically download pretrained models. No need to
+install `fairseq`. - Code completely formatted with black, isort, autoflake
+etc. [^c]: [#206](https://github.com/voicepaw/so-vits-svc-fork/issues/206) ##
+Installation ### Option 1. One click easy installation _[_D_o_w_n_l_o_a_d_ _._b_a_t_]This BAT
+file will automatically perform the steps described below. ### Option 2. Manual
+installation (using pipx, experimental) #### 1. Installing pipx Windows
+(development version required due to [pypa/pipx#940](https://github.com/pypa/
+pipx/issues/940)): ```shell py -3 -m pip install --user git+https://github.com/
+pypa/pipx.git py -3 -m pipx ensurepath ``` Linux/MacOS: ```shell python -m pip
+install --user pipx python -m pipx ensurepath ``` #### 2. Installing so-vits-
+svc-fork ```shell pipx install so-vits-svc-fork --python=3.10 pipx inject so-
+vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://
+download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
+``` ### Option 3. Manual installation Creating a virtual environment Windows:
+```shell py -3.10 -m venv venv venv\Scripts\activate ``` Linux/MacOS: ```shell
+python3.10 -m venv venv source venv/bin/activate ``` Anaconda: ```shell conda
+create -n so-vits-svc-fork python=3.10 pip conda activate so-vits-svc-fork ```
+Installing without creating a virtual environment may cause a `PermissionError`
+if Python is installed in Program Files, etc. Install this via pip (or your
+favourite package manager that uses pip): ```shell python -m pip install -U pip
+setuptools wheel pip install -U torch torchaudio --index-url https://
+download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
+pip install -U so-vits-svc-fork ``` Notes - If no GPU is available or using
+MacOS, simply remove `pip install -U torch torchaudio --index-url https://
+download.pytorch.org/whl/cu121`. MPS is probably supported. - If you are using
+an AMD GPU on Linux, replace `--index-url https://download.pytorch.org/whl/
+cu121` with `--index-url https://download.pytorch.org/whl/nightly/rocm5.7`. AMD
+GPUs are not supported on Windows ([#120](https://github.com/voicepaw/so-vits-
+svc-fork/issues/120)). ### Update Please update this package regularly to get
+the latest features and bug fixes. ```shell pip install -U so-vits-svc-fork #
+pipx upgrade so-vits-svc-fork ``` ## Usage ### Inference #### GUI ![GUI](https:
+//raw.githubusercontent.com/voicepaw/so-vits-svc-fork/main/docs/_static/
+gui.png) GUI launches with the following command: ```shell svcg ``` #### CLI -
+Realtime (from microphone) ```shell svc vc ``` - File ```shell svc infer
+source.wav ``` Pretrained models are available on [Hugging Face](https://
+huggingface.co/models?search=so-vits-svc) or [CIVITAI](https://civitai.com/
+?query=so-vits-svc). #### Notes - If using WSL, please note that WSL requires
+additional setup to handle audio and the GUI will not work without finding an
+audio device. - In real-time inference, if there is noise on the inputs, the
+HuBERT model will react to those as well. Consider using realtime noise
+reduction applications such as [RTX Voice](https://www.nvidia.com/en-us/
+geforce/guides/nvidia-rtx-voice-setup-guide/) in this case. - Models other than
+for 4.0v1 or this repository are not supported. - GPU inference requires at
+least 4 GB of VRAM. If it does not work, try CPU inference as it is fast
+enough. [^r-inference] [^r-inference]: [#469](https://github.com/voicepaw/so-
+vits-svc-fork/issues/469) ### Training #### Before training - If your dataset
+has BGM, please remove the BGM using software such as [Ultimate Vocal Remover]
+(https://ultimatevocalremover.com/). `3_HP-Vocal-UVR.pth` or `UVR-MDX-NET Main`
+is recommended. [^1] - If your dataset is a long audio file with a single
+speaker, use `svc pre-split` to split the dataset into multiple files (using
+`librosa`). - If your dataset is a long audio file with multiple speakers, use
+`svc pre-sd` to split the dataset into multiple files (using `pyannote.audio`).
+Further manual classification may be necessary due to accuracy issues. If
+speakers speak with a variety of speech styles, set --min-speakers larger than
+the actual number of speakers. Due to unresolved dependencies, please install
+`pyannote.audio` manually: `pip install pyannote-audio`. - To manually classify
+audio files, `svc pre-classify` is available. Up and down arrow keys can be
+used to change the playback speed. [^1]: https://ytpmv.info/how-to-use-uvr/
+#### Cloud [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/github/voicepaw/so-vits-svc-fork/
+blob/main/notebooks/so-vits-svc-fork-4.0.ipynb) [![Open In Paperspace](https://
+img.shields.io/badge/Open%20in-Paperspace-blue?style=flat-
+square&logo=paperspace)](https://console.paperspace.com/github/voicepaw/so-
+vits-svc-fork-paperspace/blob/main/so-vits-svc-fork-4.0-paperspace.ipynb) [!
+[Paperspace Referral](
 img.shields.io/badge/Referral%20($10)-9VJN74I-blue?style=flat-
 square&logo=paperspace>)](https://www.paperspace.com/?r=9VJN74I)[^p] If you do
 not have access to a GPU with more than 10 GB of VRAM, the free plan of Google
 Colab is recommended for light users and the Pro/Growth plan of Paperspace is
 recommended for heavy users. Conversely, if you have access to a high-end GPU,
 the use of cloud services is not recommended. [^p]: If you register a referral
 code and then add a payment method, you may save about $5 on your first month's
@@ -122,20 +130,20 @@
 correctly, replace `svc pre-config` with `-t so-vits-svc-4.0v1`. Training may
 take slightly longer because some weights are reset due to reusing legacy
 initial generator weights. - To use `MS-iSTFT Decoder`, replace `svc pre-
 config` with `svc pre-config -t quickvc`. - Silence removal and volume
 normalization are automatically performed (as in the upstream repo) and are not
 required. - If you have trained on a large, copyright-free dataset, consider
 releasing it as an initial model. - For further details (e.g. parameters,
-etc.), you can see the [Wiki](https://github.com/34j/so-vits-svc-fork/wiki) or
-[Discussions](https://github.com/34j/so-vits-svc-fork/discussions). [^r-
-training]: [#456](https://github.com/voicepaw/so-vits-svc-fork/issues/456) ###
-Further help For more details, run `svc -h` or `svc -h`. ```shell > svc -
-h Usage: svc [OPTIONS] COMMAND [ARGS]... so-vits-svc allows any folder
-structure for training data. However, the following folder structure is
+etc.), you can see the [Wiki](https://github.com/voicepaw/so-vits-svc-fork/
+wiki) or [Discussions](https://github.com/voicepaw/so-vits-svc-fork/
+discussions). [^r-training]: [#456](https://github.com/voicepaw/so-vits-svc-
+fork/issues/456) ### Further help For more details, run `svc -h` or `svc -h`.
+```shell > svc -h Usage: svc [OPTIONS] COMMAND [ARGS]... so-vits-svc allows any
+folder structure for training data. However, the following folder structure is
 recommended. When training: dataset_raw/{speaker_name}/**/{wav_name}.
 {any_format} When inference: configs/44k/config.json, logs/44k/G_XXXX.pth If
 the folder structure is followed, you DO NOT NEED TO SPECIFY model path, config
 path, etc. (The latest model will be automatically loaded.) To train a model,
 run pre-resample, pre-config, pre-hubert, train. To infer a model, run infer.
 Options: -h, --help Show this message and exit. Commands: clean Clean up files,
 only useful if you are using the default file structure infer Inference onnx
@@ -145,45 +153,50 @@
 be... pre-resample Preprocessing part 1: resample pre-sd Speech diarization
 using pyannote.audio pre-split Split audio files into multiple files train
 Train model If D_0.pth or G_0.pth not found, automatically download from hub.
 train-cluster Train k-means clustering vc Realtime inference from microphone
 ``` #### External Links [Video Tutorial](https://www.youtube.com/
 watch?v=tZn0lcGO5OQ) ## Contributors â¨ Thanks goes to these wonderful people
 ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-   _[_3_4_j_]     _[_G_a_r_r_e_t_t_C_o_n_w_a_y_]   _[_B_l_u_e_A_m_u_l_e_t_]   _[_T_h_r_o_w_a_w_a_y_A_c_c_o_u_n_t_0_1_]    _[_ç_·__]        _[_L_o_r_d_m_a_u_5_]         _[_D_L_9_0_9_]
-    _33_44_jj       _GG_aa_rr_rr_ee_tt_tt_CC_oo_nn_ww_aa_yy     _BB_ll_uu_ee_AA_mm_uu_ll_ee_tt     _TT_hh_rr_oo_ww_aa_ww_aa_yy_AA_cc_cc_oo_uu_nn_tt_00_11      _?ç_?·_?          _LL_oo_rr_dd_mm_aa_uu_55           _DD_LL_99_00_99
- _ð___» _ð__¤_   _ð___» _ð___ _ð___   _ð__¤_ _ð___¬ _ð___»          _ð___          _ð___ _ð___  _ð___ _ð___» _ð__¤_ _ð___§      _ð___
- _ð___ _ð___¡        _ð___             _ð___§                                             _ð___¬ _ð___
+   _[_3_4_j_]     _[_G_a_r_r_e_t_t_C_o_n_w_a_y_]    _[_B_l_u_e_A_m_u_l_e_t_]   _[_T_h_r_o_w_a_w_a_y_A_c_c_o_u_n_t_0_1_]    _[_ç_·__]        _[_L_o_r_d_m_a_u_5_]         _[_D_L_9_0_9_]
+    _33_44_jj       _GG_aa_rr_rr_ee_tt_tt_CC_oo_nn_ww_aa_yy      _BB_ll_uu_ee_AA_mm_uu_ll_ee_tt     _TT_hh_rr_oo_ww_aa_ww_aa_yy_AA_cc_cc_oo_uu_nn_tt_00_11      _?ç_?·_?          _LL_oo_rr_dd_mm_aa_uu_55           _DD_LL_99_00_99
+ _ð___» _ð__¤_   _ð___» _ð___ _ð___    _ð__¤_ _ð___¬ _ð___»          _ð___          _ð___ _ð___  _ð___ _ð___» _ð__¤_ _ð___§      _ð___
+ _ð___ _ð___¡        _ð___              _ð___§                                             _ð___¬ _ð___
  _ð___ _ð___§
 _ð___ _â__ _ï_¸_
   _â__ _ð___£
     _ð___
-_[_S_a_t_i_s_f_y_2_5_6_]    _[_P_i_e_r_l_u_i_g_i   _[_r_u_c_k_u_s_m_a_t_t_s_t_e_r_]       _[_D_e_s_u_k_a_-_a_r_t_]   _[_h_e_y_f_i_x_i_t_]     _[_N_e_r_d_y_ _R_o_d_e_n_t_]      _[_è_°_¢_å_®__]
- _SS_aa_tt_ii_ss_ff_yy_22_55_66      _Z_a_g_a_r_i_a_]     _rr_uu_cc_kk_uu_ss_mm_aa_tt_tt_ss_tt_ee_rr         _DD_ee_ss_uu_kk_aa_--_aa_rr_tt     _hh_ee_yy_ff_ii_xx_ii_tt       _NN_ee_rr_dd_yy_ _RR_oo_dd_ee_nn_tt        _?è_?°_?¢_?å_?®_?
-    _ð___         _PP_ii_ee_rr_ll_uu_ii_gg_ii         _ð___                 _ð___          _ð___             _ð___¹             _ð___
+_[_S_a_t_i_s_f_y_2_5_6_]    _[_P_i_e_r_l_u_i_g_i   _[_r_u_c_k_u_s_m_a_t_t_s_t_e_r_]        _[_D_e_s_u_k_a_-_a_r_t_]   _[_h_e_y_f_i_x_i_t_]     _[_N_e_r_d_y_ _R_o_d_e_n_t_]      _[_è_°_¢_å_®__]
+ _SS_aa_tt_ii_ss_ff_yy_22_55_66      _Z_a_g_a_r_i_a_]     _rr_uu_cc_kk_uu_ss_mm_aa_tt_tt_ss_tt_ee_rr          _DD_ee_ss_uu_kk_aa_--_aa_rr_tt     _hh_ee_yy_ff_ii_xx_ii_tt       _NN_ee_rr_dd_yy_ _RR_oo_dd_ee_nn_tt        _?è_?°_?¢_?å_?®_?
+    _ð___         _PP_ii_ee_rr_ll_uu_ii_gg_ii         _ð___                  _ð___          _ð___             _ð___¹             _ð___
                   _ZZ_aa_gg_aa_rr_ii_aa
                    _ð___
-_[_C_o_l_d_C_a_w_f_e_e_]   _[_s_b_e_r_s_i_e_r_]       _[_M_e_l_d_o_n_e_r_]          _[_m_m_o_d_e_u_s_h_e_r_]    _[_A_l_o_n_D_a_n_]         _[_L_i_k_k_k_e_z_]     _[_D_u_c_t_ _T_a_p_e
- _CC_oo_ll_dd_CC_aa_ww_ff_ee_ee     _ss_bb_ee_rr_ss_ii_ee_rr         _MM_ee_ll_dd_oo_nn_ee_rr            _mm_mm_oo_dd_ee_uu_ss_hh_ee_rr      _AA_ll_oo_nn_DD_aa_nn           _LL_ii_kk_kk_kk_ee_zz        _G_a_m_e_s_]
-    _ð___     _ð__¤_ _ð___ _ð___   _ð___ _ð__¤_ _ð___»            _ð___          _ð___              _ð___        _DD_uu_cc_tt_ _TT_aa_pp_ee
-                                                                                                      _GG_aa_mm_ee_ss
-                                                                                                       _ð___
- _[_X_i_a_n_g_l_o_n_g       _[_7_5_a_o_s_u_]       _[_t_o_n_y_c_o_8_2_]            _[_y_x_l_l_l_c_]    _[_o_u_t_h_i_p_p_e_d_] _[_e_s_c_o_o_l_i_o_i_n_g_l_e_s_i_a_s_] _[_B_l_a_c_k_s_i_n_g_h_]
-    _H_e_]            _77_55_aa_oo_ss_uu         _tt_oo_nn_yy_cc_oo_88_22              _yy_xx_ll_ll_ll_cc      _oo_uu_tt_hh_ii_pp_pp_ee_dd   _ee_ss_cc_oo_oo_ll_ii_oo_ii_nn_gg_ll_ee_ss_ii_aa_ss   _BB_ll_aa_cc_kk_ss_ii_nn_gg_hh
-_XX_ii_aa_nn_gg_ll_oo_nn_gg_ _HH_ee        _ð___            _ð___              _ð__¤_ _ð___»       _ð___       _ð___ _ð___ _ð___¹        _ð___
+_[_C_o_l_d_C_a_w_f_e_e_]   _[_s_b_e_r_s_i_e_r_]        _[_M_e_l_d_o_n_e_r_]          _[_m_m_o_d_e_u_s_h_e_r_]    _[_A_l_o_n_D_a_n_]         _[_L_i_k_k_k_e_z_]     _[_D_u_c_t_ _T_a_p_e
+ _CC_oo_ll_dd_CC_aa_ww_ff_ee_ee     _ss_bb_ee_rr_ss_ii_ee_rr          _MM_ee_ll_dd_oo_nn_ee_rr            _mm_mm_oo_dd_ee_uu_ss_hh_ee_rr      _AA_ll_oo_nn_DD_aa_nn           _LL_ii_kk_kk_kk_ee_zz        _G_a_m_e_s_]
+    _ð___     _ð__¤_ _ð___ _ð___    _ð___ _ð__¤_ _ð___»            _ð___          _ð___              _ð___        _DD_uu_cc_tt_ _TT_aa_pp_ee
+                                                                                                       _GG_aa_mm_ee_ss
+                                                                                                        _ð___
+ _[_X_i_a_n_g_l_o_n_g       _[_7_5_a_o_s_u_]        _[_t_o_n_y_c_o_8_2_]            _[_y_x_l_l_l_c_]    _[_o_u_t_h_i_p_p_e_d_] _[_e_s_c_o_o_l_i_o_i_n_g_l_e_s_i_a_s_] _[_B_l_a_c_k_s_i_n_g_h_]
+    _H_e_]            _77_55_aa_oo_ss_uu          _tt_oo_nn_yy_cc_oo_88_22              _yy_xx_ll_ll_ll_cc      _oo_uu_tt_hh_ii_pp_pp_ee_dd   _ee_ss_cc_oo_oo_ll_ii_oo_ii_nn_gg_ll_ee_ss_ii_aa_ss   _BB_ll_aa_cc_kk_ss_ii_nn_gg_hh
+_XX_ii_aa_nn_gg_ll_oo_nn_gg_ _HH_ee        _ð___             _ð___              _ð__¤_ _ð___»       _ð___       _ð___ _ð___ _ð___¹        _ð___
     _ð___
-  _[_M_g_s_._ _M_.      _[_E_x_o_s_f_e_e_r_]      _[_g_u_r_a_n_o_n_]      _[_A_l_e_x_a_n_d_e_r_ _K_o_u_m_i_s_]  _[_a_c_e_k_a_g_a_m_i_]       _[_H_i_g_h_u_p_e_c_h_]      _[_S_c_o_r_p_i_]
-   _T_h_o_y_i_b        _EE_xx_oo_ss_ff_ee_ee_rr        _gg_uu_rr_aa_nn_oo_nn        _AA_ll_ee_xx_aa_nn_dd_ee_rr_ _KK_oo_uu_mm_ii_ss    _aa_cc_ee_kk_aa_gg_aa_mm_ii         _HH_ii_gg_hh_uu_pp_ee_cc_hh        _SS_cc_oo_rr_pp_ii
- _A_n_t_a_r_n_u_s_a_]      _ð___ _ð___»    _ð___ _ð__¤_ _ð___»          _ð___»            _ð___              _ð___            _ð___»
+  _[_M_g_s_._ _M_.      _[_E_x_o_s_f_e_e_r_]        _[_g_u_r_a_n_o_n_]     _[_A_l_e_x_a_n_d_e_r_ _K_o_u_m_i_s_]  _[_a_c_e_k_a_g_a_m_i_]       _[_H_i_g_h_u_p_e_c_h_]      _[_S_c_o_r_p_i_]
+   _T_h_o_y_i_b        _EE_xx_oo_ss_ff_ee_ee_rr          _gg_uu_rr_aa_nn_oo_nn       _AA_ll_ee_xx_aa_nn_dd_ee_rr_ _KK_oo_uu_mm_ii_ss    _aa_cc_ee_kk_aa_gg_aa_mm_ii         _HH_ii_gg_hh_uu_pp_ee_cc_hh        _SS_cc_oo_rr_pp_ii
+ _A_n_t_a_r_n_u_s_a_]      _ð___ _ð___»     _ð___ _ð__¤_ _ð___»          _ð___»            _ð___              _ð___            _ð___»
   _MM_gg_ss_.._ _MM_..
    _TT_hh_oo_yy_ii_bb
  _AA_nn_tt_aa_rr_nn_uu_ss_aa
     _ð___
- _[_M_a_x_i_m_x_l_s_]     _[_S_t_a_r_3_L_o_r_d_]        _[_F_o_r_k_o_z_]         _[_Z_e_r_u_i_ _C_h_e_n_]      _[_R_o_e_e
-  _MM_aa_xx_ii_mm_xx_ll_ss       _SS_tt_aa_rr_33_LL_oo_rr_dd          _FF_oo_rr_kk_oo_zz           _ZZ_ee_rr_uu_ii_ _CC_hh_ee_nn     _S_h_e_n_b_e_r_g_]
-    _ð___»         _ð___ _ð___»        _ð___ _ð___»          _ð___» _ð__¤_        _RR_oo_ee_ee
-                                                                    _SS_hh_ee_nn_bb_ee_rr_gg
-                                                                    _ð___ _ð__¤_
-                                                                      _ð___»
+ _[_M_a_x_i_m_x_l_s_]     _[_S_t_a_r_3_L_o_r_d_]        _[_F_o_r_k_o_z_]          _[_Z_e_r_u_i_ _C_h_e_n_]      _[_R_o_e_e           _[_J_u_s_t_a_s_]        _[_O_n_a_k_o_2_]
+  _MM_aa_xx_ii_mm_xx_ll_ss       _SS_tt_aa_rr_33_LL_oo_rr_dd          _FF_oo_rr_kk_oo_zz            _ZZ_ee_rr_uu_ii_ _CC_hh_ee_nn     _S_h_e_n_b_e_r_g_]          _JJ_uu_ss_tt_aa_ss          _OO_nn_aa_kk_oo_22
+    _ð___»         _ð___ _ð___»         _ð___ _ð___»          _ð___» _ð__¤_        _RR_oo_ee_ee            _ð___ _ð___»         _ð___
+                                                                     _SS_hh_ee_nn_bb_ee_rr_gg
+                                                                     _ð___ _ð__¤_
+                                                                       _ð___»
+_[_4_l_l_0_w_3_v_1_l_]      _[_j_5_y_0_V_6_b_]   _[_m_a_r_c_e_l_l_o_c_i_r_e_l_l_i_]   _[_P_r_i_y_a_n_s_h_u_ _P_a_t_e_l_]     _[_A_n_n_a
+ _44_ll_ll_00_ww_33_vv_11_ll        _jj_55_yy_00_VV_66_bb     _mm_aa_rr_cc_ee_ll_ll_oo_cc_ii_rr_ee_ll_ll_ii     _PP_rr_ii_yy_aa_nn_ss_hh_uu_ _PP_aa_tt_ee_ll   _G_o_r_s_h_u_n_o_v_a_]
+    _ð___»          _ð___¡_ï_¸_          _ð___                 _ð___»           _AA_nn_nn_aa
+                                                                    _GG_oo_rr_ss_hh_uu_nn_oo_vv_aa
+                                                                     _ð___ _ð___»
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

