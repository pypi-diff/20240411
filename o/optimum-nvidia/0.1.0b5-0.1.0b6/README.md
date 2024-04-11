# Comparing `tmp/optimum-nvidia-0.1.0b5.tar.gz` & `tmp/optimum-nvidia-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-nvidia-0.1.0b5.tar", last modified: Mon Apr  8 21:25:08 2024, max compression
+gzip compressed data, was "optimum-nvidia-0.1.0b6.tar", last modified: Thu Apr 11 21:09:44 2024, max compression
```

## Comparing `optimum-nvidia-0.1.0b5.tar` & `optimum-nvidia-0.1.0b6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.223185 optimum-nvidia-0.1.0b5/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    11357 2023-12-05 19:15:32.000000 optimum-nvidia-0.1.0b5/LICENSE
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7404 2024-04-08 21:25:08.223185 optimum-nvidia-0.1.0b5/PKG-INFO
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5099 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/README.md
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2795 2024-04-08 21:01:57.000000 optimum-nvidia-0.1.0b5/pyproject.toml
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      584 2024-04-08 21:25:08.223185 optimum-nvidia-0.1.0b5/setup.cfg
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3344 2024-04-08 21:02:05.000000 optimum-nvidia-0.1.0b5/setup.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.217185 optimum-nvidia-0.1.0b5/src/
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.218185 optimum-nvidia-0.1.0b5/src/optimum/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      646 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/__init__.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.218185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      853 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/__init__.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.219185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      686 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9713 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5180 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/local.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7297 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1855 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/errors.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.219185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/generation/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1448 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/generation/logits_process.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    20093 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/hub.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.219185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/lang/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3808 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/lang/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      987 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/logging.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.219185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      728 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2612 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/auto.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1365 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/base.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4404 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/gemma.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4426 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/llama.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4440 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/mistral.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    50724 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/whisper.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.219185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4968 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      792 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/base.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9520 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/text_generation.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.220185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      779 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/__init__.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.220185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/ammo/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      171 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/ammo/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5810 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/ammo/config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4907 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/ammo/quantizer.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    10814 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/datasets.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     8277 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/runtime.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.220185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1422 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4131 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/cli.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1040 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/constants.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1337 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/env.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2655 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/hub.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3098 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/nvml.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2023 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/offload.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2798 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/onnx.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1438 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/patching.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.220185 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/tests/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      694 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/tests/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1972 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/tests/utils.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      754 2024-04-08 21:12:44.000000 optimum-nvidia-0.1.0b5/src/optimum/nvidia/version.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.221185 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7404 2024-04-08 21:25:08.000000 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/PKG-INFO
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1815 2024-04-08 21:25:08.000000 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/SOURCES.txt
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)       24 2024-04-08 21:25:08.000000 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/dependency_links.txt
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        1 2024-04-08 21:15:11.000000 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/not-zip-safe
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      392 2024-04-08 21:25:08.000000 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/requires.txt
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        8 2024-04-08 21:25:08.000000 optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/top_level.txt
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-08 21:25:08.221185 optimum-nvidia-0.1.0b5/tests/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2295 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/tests/test_config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1729 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/tests/test_dtype.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2235 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b5/tests/test_hub.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1331 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b5/tests/test_quantization.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.170442 optimum-nvidia-0.1.0b6/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    11357 2023-12-05 19:15:32.000000 optimum-nvidia-0.1.0b6/LICENSE
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7404 2024-04-11 21:09:44.170442 optimum-nvidia-0.1.0b6/PKG-INFO
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5099 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/README.md
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2795 2024-04-08 21:01:57.000000 optimum-nvidia-0.1.0b6/pyproject.toml
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      584 2024-04-11 21:09:44.170442 optimum-nvidia-0.1.0b6/setup.cfg
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3344 2024-04-08 21:02:05.000000 optimum-nvidia-0.1.0b6/setup.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.165442 optimum-nvidia-0.1.0b6/src/
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.165442 optimum-nvidia-0.1.0b6/src/optimum/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      646 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/__init__.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      853 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/__init__.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      686 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9713 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5180 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/local.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7297 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1855 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/errors.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/generation/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1448 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/generation/logits_process.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    19797 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/hub.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/lang/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3808 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/lang/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      987 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/logging.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      728 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2612 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/auto.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1365 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/base.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4447 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/gemma.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4426 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/llama.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4483 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/mistral.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    50629 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/whisper.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.167442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4968 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      792 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/base.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9226 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/text_generation.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.167442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      779 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/__init__.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.167442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      171 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5810 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4907 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/quantizer.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    10814 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/datasets.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    13945 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/runtime.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1422 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4131 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/cli.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1040 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/constants.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1337 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/env.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2655 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/hub.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3098 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/nvml.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2023 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/offload.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2798 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/onnx.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1438 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/patching.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      694 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1972 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/utils.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      754 2024-04-11 21:09:31.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/version.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7404 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/PKG-INFO
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1815 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/SOURCES.txt
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)       24 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/dependency_links.txt
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        1 2024-04-08 21:15:11.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/not-zip-safe
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      392 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/requires.txt
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        8 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/top_level.txt
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/tests/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2295 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/tests/test_config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1729 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/tests/test_dtype.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2235 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/tests/test_hub.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1331 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/tests/test_quantization.py
```

### Comparing `optimum-nvidia-0.1.0b5/LICENSE` & `optimum-nvidia-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/PKG-INFO` & `optimum-nvidia-0.1.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-nvidia
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Optimum Nvidia is the interface between the Hugging Face Transformers and NVIDIA GPUs. "
 Home-page: https://huggingface.co/hardware/nvidia
 Author: HuggingFace Inc. Machine Learning Optimization Team
 Author-email: "HuggingFace Inc. Machine Learning Optimization Team" <hardware@huggingface.co>
 License: Apache/2.0
 Project-URL: Homepage, https://huggingface.co/hardware/nvidia
 Project-URL: Repository, https://github.com/huggingface/optimum-nvidia
```

### Comparing `optimum-nvidia-0.1.0b5/README.md` & `optimum-nvidia-0.1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/pyproject.toml` & `optimum-nvidia-0.1.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/setup.cfg` & `optimum-nvidia-0.1.0b6/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/setup.py` & `optimum-nvidia-0.1.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/config.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/builder/local.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/local.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/config.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/errors.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/errors.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/generation/logits_process.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/generation/logits_process.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/hub.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,25 +379,15 @@
                 resume_download=resume_download,
                 local_files_only=local_files_only,
                 token=token,
             )
         except OSError:
             generation_config = None
 
-        transformers_config = AutoConfig.from_pretrained(
-            model_id,
-            revision=revision,
-            cache_dir=cache_dir,
-            force_download=force_download,
-            proxies=proxies,
-            resume_download=resume_download,
-            local_files_only=local_files_only,
-            token=token,
-        )
-
+        transformers_config = AutoConfig.for_model(**config)
         model = cls(
             engines_folders,
             gpus_per_node=model_kwargs.pop("gpus_per_node", 1),
             use_cuda_graph=model_kwargs.pop("use_cuda_graph", False),
             generation_config=generation_config,
             transformers_config=transformers_config,
         )
@@ -409,15 +399,15 @@
     def _save_pretrained(self, save_directory: Path) -> None:
         if not hasattr(self, ATTR_TRTLLM_ENGINE_FOLDER):
             raise ValueError(
                 "Unable to determine the root folder containing TensorRT-LLM engines. "
                 "Please open-up an issue at https://github.com/huggingface/optimum-nvidia"
             )
 
-        self.transformers_config.save_pretrained(save_directory)
+        self.config.save_pretrained(save_directory)
         if self.generation_config is not None:
             self.generation_config.save_pretrained(save_directory)
 
         # Retrieve the folder
         engines_folders = getattr(self, ATTR_TRTLLM_ENGINE_FOLDER)
         for i in range(len(engines_folders)):
             engine_folder = Path(engines_folders[i])
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/lang/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/logging.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/auto.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/auto.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/base.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/gemma.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/gemma.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             pp_size=1,
             use_prompt_tuning=False,
             use_parallel_embedding=False,
             embedding_sharding_dim=0,
             share_embedding_table=False,
             max_lora_rank=64,
             quantization=qconfig,
+            rotary_base=config.rope_theta,
         )
 
         trt_config.mapping.gpus_per_node = min(trt_config.mapping.world_size, 8)
 
         return trt_config
 
     def get_plugins_config(self) -> PluginConfig:
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/llama.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/llama.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/mistral.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             use_prompt_tuning=False,
             use_parallel_embedding=False,
             embedding_sharding_dim=0,
             share_embedding_table=False,
             max_lora_rank=64,
             head_size=config.hidden_size / config.num_attention_heads,
             quantization=qconfig,
+            rotary_base=config.rope_theta,
         )
 
         trt_config.mapping.gpus_per_node = min(trt_config.mapping.world_size, 8)
 
         return trt_config
 
     def get_plugins_config(self) -> PluginConfig:
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/models/whisper.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/whisper.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,15 +685,15 @@
             generation_config=generation_config,
         )
 
         if generation_config is None:
             generation_config = GenerationConfig()
         self.generation_config = generation_config
 
-        self.transformers_config = transformers_config
+        self.config = transformers_config
 
         # Encoder.
         serialize_path = engines_folders[0] / "rank0.engine"
         with open(serialize_path, "rb") as f:
             encoder_session = Session.from_serialized_engine(f.read())
 
         self.encoder_session = encoder_session
@@ -1074,15 +1074,15 @@
             raise ValueError(
                 f"TensorRT-LLM only supports inputs on CUDA device. Got: inputs.device = {inputs.device}"
             )
 
         def raise_unsupported(value: Any, name: str, default: Any = None):
             if value != default:
                 raise ValueError(
-                    f"TensorRTForSpeechSeq2Seq.generate does not support {name} (got {value}). Please open an issue at https://github.com/huggingface/optimum-nvidia/issues."
+                    f"TensorRTForSpeechSeq2Seq.generate does not support the argument {name} (got {name}={value}). Please open an issue at https://github.com/huggingface/optimum-nvidia/issues."
                 )
 
         raise_unsupported(stopping_criteria, name="stopping_criteria")
         raise_unsupported(prefix_allowed_tokens_fn, name="prefix_allowed_tokens_fn")
         raise_unsupported(synced_gpus, name="synced_gpus", default=False)
         raise_unsupported(return_timestamps, name="return_timestamps")
         raise_unsupported(task, name="task")
@@ -1105,15 +1105,15 @@
             language=language,
             task=task,
             is_multilingual=is_multilingual,
             generation_config=generation_config,
         )
         self._set_token_ids(
             generation_config=generation_config,
-            config=self.transformers_config,
+            config=self.config,
             kwargs=kwargs,
         )
         self._set_thresholds_and_condition(
             generation_config=generation_config,
             logprob_threshold=logprob_threshold,
             compression_ratio_threshold=compression_ratio_threshold,
             no_speech_threshold=no_speech_threshold,
@@ -1122,27 +1122,25 @@
 
         num_beams = kwargs.pop("num_beams", generation_config.num_beams)
         input_stride = 1 * 2  # encoder's conv1 stride * encoder's conv2 stride
 
         batch_size, total_input_frames = self._retrieve_total_input_frames(
             input_features=inputs, input_stride=input_stride, kwargs=kwargs
         )
-        num_segment_frames = (
-            input_stride * self.transformers_config.max_source_positions
-        )
+        num_segment_frames = input_stride * self.config.max_source_positions
         is_shortform = total_input_frames <= num_segment_frames
         if not is_shortform:
             raise ValueError(
                 "Whisper TensorRT-LLM implementation only supports short form for now. Please open an issue at https://github.com/huggingface/optimum-nvidia/issues."
             )
 
         init_tokens = self._retrieve_init_tokens(
             inputs,
             generation_config=generation_config,
-            config=self.transformers_config,
+            config=self.config,
             num_segment_frames=num_segment_frames,
             kwargs=kwargs,
         )
 
         begin_index = len(init_tokens)
         logits_processor = self._retrieve_logit_processors(
             generation_config=generation_config,
@@ -1167,24 +1165,24 @@
                     generation_config.max_length - decoder_input_ids.shape[1]
                 )
             else:
                 raise ValueError("Please specifiy the argument `max_new_tokens`.")
 
         if (
             max_new_tokens + decoder_input_ids.shape[-1]
-            > self.transformers_config.max_target_positions
+            > self.config.max_target_positions
         ):
             max_new_tokens = kwargs.get("max_new_tokens", 0)
             raise ValueError(
                 f"The length of `decoder_input_ids` equal `prompt_ids` plus special start tokens is {decoder_input_ids.shape[-1]}, and the `max_new_tokens` "
                 f"is {max_new_tokens}. Thus, the combined length of "
                 f"`decoder_input_ids` and `max_new_tokens` is: {max_new_tokens + decoder_input_ids.shape[-1]}. This exceeds the "
-                f"`max_target_positions` of the Whisper model: {self.transformers_config.max_target_positions}. "
+                f"`max_target_positions` of the Whisper model: {self.config.max_target_positions}. "
                 "You should either reduce the length of your prompt, or reduce the value of `max_new_tokens`, "
-                f"so that their combined length is less than {self.transformers_config.max_target_positions}."
+                f"so that their combined length is less than {self.config.max_target_positions}."
             )
 
         encoder_input_lengths = torch.tensor(
             [encoder_outputs.shape[1] for x in range(encoder_outputs.shape[0])],
             dtype=torch.int32,
             device=inputs.device,
         )
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/base.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/pipelines/text_generation.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/text_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,38 +34,34 @@
 
 class TextGenerationPipeline(Pipeline):
     TARGET_FACTORY = AutoModelForCausalLM
 
     __slots__ = (
         "tokenizer",
         "_runtime",
-        "_bos_token_id",
-        "_eos_token_id",
-        "_pad_token_id",
     )
 
     def __init__(self, model: CausalLM, tokenizer: PreTrainedTokenizer):
         super().__init__()
 
         if tokenizer.eos_token and not tokenizer.pad_token:
             tokenizer.pad_token = tokenizer.eos_token
 
         self.tokenizer = tokenizer
         self._runtime = model
 
-        self._bos_token_id = tokenizer.bos_token_id
-        self._eos_token_id = tokenizer.eos_token_id
-        self._pad_token_id = tokenizer.pad_token_id
-
-    def __call__(self, inputs: Union[str, List[str]], **kwargs):
+    def __call__(
+        self, inputs: Union[str, List[str]], add_special_tokens: bool = True, **kwargs
+    ):
         (
             preprocess_params,
             forward_params,
             postprocess_params,
-        ) = self._sanitize_parameters(**kwargs)
+        ) = self._sanitize_parameters(add_special_tokens=add_special_tokens, **kwargs)
+
         model_inputs = self.preprocess(inputs, **preprocess_params)
         model_outputs = self._forward(model_inputs, **forward_params)
         outputs = self.postprocess(model_outputs, **postprocess_params)
         return outputs
 
     def _sanitize_parameters(
         self,
@@ -143,15 +139,15 @@
         return preprocess_params, forward_params, postprocess_params
 
     def _forward(self, model_inputs, **generate_kwargs):
         input_ids = model_inputs["input_ids"]
         prompt_text = model_inputs.pop("prompt_text")
         attention_mask = model_inputs.get("attention_mask", None)
 
-        max_new_tokens = generate_kwargs.pop("max_new_tokens", -1)
+        max_new_tokens = generate_kwargs.pop("max_new_tokens", None)
         min_length = generate_kwargs.pop("min_length", -1)
         num_beams = generate_kwargs.pop("num_beams", 1)
         temperature = generate_kwargs.pop("temperature", 1.0)
         top_k = generate_kwargs.pop("top_k", 50)
         top_p = generate_kwargs.pop("top_p", 1.0)
         repetition_penalty = generate_kwargs.pop("repetition_penalty", 1.0)
         length_penalty = generate_kwargs.pop("length_penalty", 1.0)
@@ -184,17 +180,14 @@
             num_beams=num_beams,
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
             repetition_penalty=repetition_penalty,
             length_penalty=length_penalty,
             seed=seed,
-            bos_token_id=self._bos_token_id,
-            eos_token_id=self._eos_token_id,
-            pad_token_id=self._pad_token_id,
         )
 
         return {
             "generated_sequence": generated_sequence,
             "lengths": lengths,
             "input_ids": input_ids,
             "prompt_text": prompt_text,
@@ -239,17 +232,17 @@
         if return_type == ReturnType.TENSORS:
             return [
                 {"generated_token_ids": generated for generated in generated_sequence}
             ]
 
         for sequence in generated_sequence:
             # Decode text
-            beam_text = self.tokenizer.batch_decode(
+            text = self.tokenizer.decode(
                 sequence,
                 skip_special_tokens=True,
                 clean_up_tokenization_spaces=clean_up_tokenization_spaces,
             )
 
-            record = {"generated_text": beam_text}
+            record = {"generated_text": text}
             records.append(record)
 
         return records
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/ammo/config.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/ammo/quantizer.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/quantizer.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/quantization/datasets.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/datasets.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/runtime.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/runtime.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,27 +9,32 @@
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import copy
 import warnings
 from logging import getLogger
 from os import PathLike
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Union
 
 import tensorrt_llm.bindings as ctrrt
 import torch
 from transformers import GenerationConfig
+from transformers.generation.utils import GenerationMixin
 
 
 if TYPE_CHECKING:
-    from transformers import PretrainedConfig
+    from transformers import PretrainedConfig, PreTrainedModel
+    from transformers.generation.logits_process import LogitsProcessorList
+    from transformers.generation.stopping_criteria import StoppingCriteriaList
+    from transformers.generation.streamers import BaseStreamer
 
 LOGGER = getLogger(__name__)
 
 PackedTensor = List[torch.Tensor]
 
 
 DEFAULT_BATCH_SIZE: int = 1
@@ -49,15 +54,17 @@
         """
         Return the local path where the engine(s) is/are located
         :return: Path to the folder holding the engine(s) definition(s)
         """
         return self._engines_folders_path
 
 
-class CausalLM(CompiledModel):
+class CausalLM(CompiledModel, GenerationMixin):
+    main_input_name = "input_ids"
+
     __slots__ = (
         "_device",
         "_config",
         "_mapping",
         "_session",
         "_session_config",
         "_use_packed_inputs",
@@ -91,106 +98,195 @@
             self._config.pipeline_parallelism,
         )
         self._session_config = ctrrt.GptSessionConfig(
             max_batch_size=self._config.model_config.max_batch_size,
             max_beam_width=self._config.model_config.max_beam_width,
             max_sequence_length=self._config.model_config.max_seq_len,
         )
+
         self._session_config.cuda_graph_mode = use_cuda_graph
 
         # Create the engine
         engine_file = self._config.engine_filename(self._mapping)
-        self._session = ctrrt.GptSession(
-            config=self._session_config,
-            model_config=self._config.model_config,
-            world_config=self._mapping,
-            engine_file=str(engines_folder.joinpath(engine_file)),
-        )
+
+        try:
+            self._session = ctrrt.GptSession(
+                config=self._session_config,
+                model_config=self._config.model_config,
+                world_config=self._mapping,
+                engine_file=str(engines_folder.joinpath(engine_file)),
+            )
+        except RuntimeError as e:
+            if "maxTokensInPagedKvCache" in repr(
+                e
+            ) and "must be large enough to process at least 1 sequence" in repr(e):
+                raise RuntimeError(
+                    f"Could not initialize TensorRT-LLM decoder session, likely due a large maximum output length set at compilation time (max_output_len={self._config.model_config.max_seq_len}). Please try and set a lower value for `max_output_length` when building the engine. Error: {e}"
+                )
+            else:
+                raise e
 
         # Additional cached properties
         self._use_packed_inputs = self._config.model_config.use_packed_input
         self.max_batch_size = self._config.model_config.max_batch_size
         self.max_prompt_length = self._config.model_config.max_input_len
 
         self.max_output_length = self._config.model_config.max_seq_len
         self.max_beam_width = self._session_config.max_beam_width
 
         if generation_config is None:
             generation_config = GenerationConfig()
         self.generation_config = generation_config
 
-        self.transformers_config = transformers_config
-
-    @property
-    def config(self) -> ctrrt.GptJsonConfig:
-        return self._config
+        # Required for GenerationMixin compatibility.
+        self.config = transformers_config
 
+    @torch.no_grad()
     def generate(
         self,
-        input_ids: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        max_new_tokens: int = -1,
-        min_length: int = -1,
-        num_beams: int = 1,
-        temperature: float = 1.0,
-        top_k: int = 50,
-        top_p: float = 1.0,
-        repetition_penalty: float = 1.0,
-        length_penalty: float = 1.0,
-        seed: int = 0,
-        pad_token_id: int = 0,
-        bos_token_id: int = 1,
-        eos_token_id: int = 2,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        inputs: Optional[torch.Tensor] = None,
+        generation_config: Optional[GenerationConfig] = None,
+        logits_processor: Optional["LogitsProcessorList"] = None,
+        stopping_criteria: Optional["StoppingCriteriaList"] = None,
+        prefix_allowed_tokens_fn: Optional[
+            Callable[[int, torch.Tensor], List[int]]
+        ] = None,
+        synced_gpus: Optional[bool] = None,
+        assistant_model: Optional["PreTrainedModel"] = None,
+        streamer: Optional["BaseStreamer"] = None,
+        negative_prompt_ids: Optional[torch.Tensor] = None,
+        negative_prompt_attention_mask: Optional[torch.Tensor] = None,
+        **kwargs,
+    ) -> torch.LongTensor:
+        def raise_unsupported(value: Any, name: str, default: Any = None):
+            if value != default:
+                raise ValueError(
+                    f"{self.__class__.__name__}.generate does not support the argument {name} (got {name}={value}). Please open an issue at https://github.com/huggingface/optimum-nvidia/issues."
+                )
+
+        raise_unsupported(stopping_criteria, name="stopping_criteria")
+        raise_unsupported(prefix_allowed_tokens_fn, name="prefix_allowed_tokens_fn")
+        raise_unsupported(synced_gpus, name="synced_gpus")
+        raise_unsupported(logits_processor, name="logits_processor")
+        raise_unsupported(assistant_model, name="assistant_model")
+        raise_unsupported(streamer, name="streamer")
+        raise_unsupported(negative_prompt_ids, name="negative_prompt_ids")
+        raise_unsupported(
+            negative_prompt_attention_mask, name="negative_prompt_attention_mask"
+        )
+
+        # priority: `generation_config` argument > `model.generation_config` (the default generation config)
+        if generation_config is None:
+            # legacy: users may modify the model configuration to control generation. To trigger this legacy behavior,
+            # three conditions must be met
+            # 1) the generation config must have been created from the model config (`_from_model_config` field);
+            # 2) the generation config must have seen no modification since its creation (the hash is the same);
+            # 3) the user must have set generation parameters in the model config.
+            if (
+                self.generation_config._from_model_config
+                and self.generation_config._original_object_hash
+                == hash(self.generation_config)
+                and self.config._has_non_default_generation_parameters()
+            ):
+                new_generation_config = GenerationConfig.from_model_config(self.config)
+                if new_generation_config != self.generation_config:
+                    warnings.warn(
+                        "You have modified the pretrained model configuration to control generation. This is a"
+                        " deprecated strategy to control generation and will be removed soon, in a future version."
+                        " Please use and modify the model generation configuration (see"
+                        " https://huggingface.co/docs/transformers/generation_strategies#default-text-generation-configuration )"
+                    )
+                    self.generation_config = new_generation_config
+            generation_config = self.generation_config
+
+        generation_config = copy.deepcopy(generation_config)
+        model_kwargs = generation_config.update(
+            **kwargs
+        )  # All unused kwargs must be model kwargs
+
+        if (
+            generation_config.pad_token_id is None
+            and generation_config.eos_token_id is not None
+        ):
+            if model_kwargs.get("attention_mask", None) is None:
+                LOGGER.warning(
+                    "The attention mask and the pad token id were not set. As a consequence, you may observe "
+                    "unexpected behavior. Please pass your input's `attention_mask` to obtain reliable results."
+                )
+            eos_token_id = generation_config.eos_token_id
+            if isinstance(eos_token_id, list):
+                eos_token_id = eos_token_id[0]
+            LOGGER.warning(
+                f"Setting `pad_token_id` to `eos_token_id`:{eos_token_id} for open-end generation."
+            )
+            generation_config.pad_token_id = eos_token_id
+
         device = self._device
 
+        seed = model_kwargs.pop("seed", 42)
         # If no GenerationConfig is provided, let's allocate one with default settings
-        generation_config = ctrrt.SamplingConfig(min(num_beams, self.max_beam_width))
-        generation_config.random_seed = [seed]
-        generation_config.temperature = [temperature]
-        generation_config.top_k = [top_k]
-        generation_config.top_p = [top_p]
-        generation_config.repetition_penalty = [repetition_penalty]
-        generation_config.length_penalty = [length_penalty]
+        sampling_config = ctrrt.SamplingConfig(
+            min(generation_config.num_beams, self.max_beam_width)
+        )
+        sampling_config.random_seed = [seed]
+        sampling_config.temperature = [generation_config.temperature]
+        sampling_config.top_k = [generation_config.top_k]
+        sampling_config.top_p = [generation_config.top_p]
+        sampling_config.repetition_penalty = [generation_config.repetition_penalty]
+        sampling_config.length_penalty = [generation_config.length_penalty]
+
+        if generation_config.min_new_tokens is not None:
+            sampling_config.min_length = [generation_config.min_new_tokens]
 
-        if min_length > 0:
-            generation_config.min_length = [min_length]
+        input_ids, _, model_kwargs = self._prepare_model_inputs(
+            inputs, generation_config.bos_token_id, model_kwargs
+        )
 
         with torch.no_grad():
             if not isinstance(input_ids, torch.Tensor):
                 raise TypeError("input_ids should be a PyTorch tensor (torch.Tensor)")
 
+            attention_mask = model_kwargs["attention_mask"]
             input_ids, lengths = self._prepare_inputs(input_ids, attention_mask)
             if torch.any(torch.gt(lengths, self.max_prompt_length)):
                 raise ValueError(
                     f"Input length {lengths} is bigger than maximum prompt length ({self.max_prompt_length})."
                 )
 
+            input_length = input_ids.shape[1]
             trt_inputs = ctrrt.GenerationInput(
-                end_id=eos_token_id,
-                pad_id=pad_token_id,
+                end_id=generation_config.eos_token_id,
+                pad_id=generation_config.pad_token_id,
                 ids=input_ids.to(device),
                 lengths=lengths.to(device),
                 packed=self._use_packed_inputs,
             )
 
+            max_new_tokens = generation_config.max_new_tokens
             if max_new_tokens is None or max_new_tokens < 1:
                 max_new_tokens = self.max_output_length - input_ids.shape[1]
 
             trt_inputs.max_new_tokens = max_new_tokens
 
             # Tensors are being allocated as in/out parameters and TRTLLM will resize
             trt_outputs = ctrrt.GenerationOutput(
                 ids=torch.empty(0, device=device, dtype=torch.int32),
                 lengths=torch.empty(0, device=device, dtype=torch.int32),
             )
 
-            self._session.generate(trt_outputs, trt_inputs, generation_config)
+            self._session.generate(trt_outputs, trt_inputs, sampling_config)
+
+            total_length = trt_outputs.lengths
+            output_ids = trt_outputs.ids.flatten(0, 1)
+
+            # For some reason not in line with Transformers in case we finish early with BOS token (missing last BOS token).
+            if total_length - input_length < max_new_tokens:
+                total_length += 1
 
-            return trt_outputs.ids, trt_outputs.lengths
+            return output_ids[:, :total_length], total_length
 
     def _prepare_inputs(
         self, input_ids: torch.Tensor, attention_mask: Optional[torch.Tensor] = None
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         shape = input_ids.size()
         input_ids = input_ids.int()
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/cli.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/cli.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/constants.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/env.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/env.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/hub.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/hub.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/nvml.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/nvml.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/offload.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/offload.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/onnx.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/patching.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/patching.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/tests/__init__.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/utils/tests/utils.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/src/optimum/nvidia/version.py` & `optimum-nvidia-0.1.0b6/src/optimum/nvidia/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from distutils.version import StrictVersion
 
 
-__version__ = "0.1.0b5"
+__version__ = "0.1.0b6"
 VERSION = StrictVersion(__version__)
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/PKG-INFO` & `optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-nvidia
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Optimum Nvidia is the interface between the Hugging Face Transformers and NVIDIA GPUs. "
 Home-page: https://huggingface.co/hardware/nvidia
 Author: HuggingFace Inc. Machine Learning Optimization Team
 Author-email: "HuggingFace Inc. Machine Learning Optimization Team" <hardware@huggingface.co>
 License: Apache/2.0
 Project-URL: Homepage, https://huggingface.co/hardware/nvidia
 Project-URL: Repository, https://github.com/huggingface/optimum-nvidia
```

### Comparing `optimum-nvidia-0.1.0b5/src/optimum_nvidia.egg-info/SOURCES.txt` & `optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/tests/test_config.py` & `optimum-nvidia-0.1.0b6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/tests/test_dtype.py` & `optimum-nvidia-0.1.0b6/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/tests/test_hub.py` & `optimum-nvidia-0.1.0b6/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b5/tests/test_quantization.py` & `optimum-nvidia-0.1.0b6/tests/test_quantization.py`

 * *Files identical despite different names*

