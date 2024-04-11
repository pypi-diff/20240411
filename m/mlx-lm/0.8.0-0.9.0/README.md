# Comparing `tmp/mlx-lm-0.8.0.tar.gz` & `tmp/mlx-lm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx-lm-0.8.0.tar", last modified: Mon Apr  8 21:20:29 2024, max compression
+gzip compressed data, was "mlx-lm-0.9.0.tar", last modified: Thu Apr 11 20:20:15 2024, max compression
```

## Comparing `mlx-lm-0.8.0.tar` & `mlx-lm-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.603749 mlx-lm-0.8.0/
--rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.8.0/MANIFEST.in
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-08 21:20:29.603548 mlx-lm-0.8.0/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.8.0/README.md
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.594995 mlx-lm-0.8.0/mlx_lm/
--rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/mlx_lm/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.8.0/mlx_lm/convert.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/fuse.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/generate.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/merge.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.600303 mlx-lm-0.8.0/mlx_lm/models/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.8.0/mlx_lm/models/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.8.0/mlx_lm/models/base.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6061 2024-04-05 21:11:41.000000 mlx-lm-0.8.0/mlx_lm/models/cohere.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/dbrx.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/gemma.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/llama.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/mixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/olmo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/phi.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/phixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/models/plamo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/qwen.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/qwen2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/models/qwen2_moe.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7041 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/mlx_lm/models/stablelm.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/models/starcoder2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/mlx_lm/py.typed
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/requirements.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)     1354 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/mlx_lm/sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/server.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.601517 mlx-lm-0.8.0/mlx_lm/tuner/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/mlx_lm/tuner/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.8.0/mlx_lm/tuner/datasets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.8.0/mlx_lm/tuner/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/tuner/trainer.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.8.0/mlx_lm/tuner/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    19575 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/mlx_lm/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/mlx_lm/version.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.603313 mlx-lm-0.8.0/mlx_lm.egg-info/
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     1038 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/requires.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-08 21:20:29.000000 mlx-lm-0.8.0/mlx_lm.egg-info/top_level.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-08 21:20:29.603804 mlx-lm-0.8.0/setup.cfg
--rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.8.0/setup.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-08 21:20:29.603018 mlx-lm-0.8.0/tests/
--rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.8.0/tests/test_datsets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/tests/test_gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/tests/test_lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    10294 2024-04-08 21:20:20.000000 mlx-lm-0.8.0/tests/test_models.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.8.0/tests/test_sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-11 20:20:15.907082 mlx-lm-0.9.0/
+-rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.9.0/MANIFEST.in
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5059 2024-04-11 20:20:15.906892 mlx-lm-0.9.0/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.9.0/README.md
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-11 20:20:15.897814 mlx-lm-0.9.0/mlx_lm/
+-rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.9.0/mlx_lm/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.9.0/mlx_lm/convert.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/fuse.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/generate.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/merge.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-11 20:20:15.903039 mlx-lm-0.9.0/mlx_lm/models/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.9.0/mlx_lm/models/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.9.0/mlx_lm/models/base.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6061 2024-04-05 21:11:41.000000 mlx-lm-0.9.0/mlx_lm/models/cohere.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/models/dbrx.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/models/gemma.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.9.0/mlx_lm/models/llama.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/models/mixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/models/olmo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.9.0/mlx_lm/models/phi.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/models/phixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/mlx_lm/models/plamo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.9.0/mlx_lm/models/qwen.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.9.0/mlx_lm/models/qwen2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/models/qwen2_moe.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7041 2024-04-08 21:20:20.000000 mlx-lm-0.9.0/mlx_lm/models/stablelm.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.9.0/mlx_lm/models/starcoder2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.9.0/mlx_lm/py.typed
+-rw-r--r--   0 awnihannun   (501) staff       (20)       60 2024-04-11 20:20:08.000000 mlx-lm-0.9.0/mlx_lm/requirements.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1170 2024-04-11 20:20:08.000000 mlx-lm-0.9.0/mlx_lm/sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/server.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9345 2024-04-11 00:42:44.000000 mlx-lm-0.9.0/mlx_lm/tokenizer_utils.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-11 20:20:15.904379 mlx-lm-0.9.0/mlx_lm/tuner/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.9.0/mlx_lm/tuner/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.9.0/mlx_lm/tuner/datasets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.9.0/mlx_lm/tuner/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/tuner/trainer.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.9.0/mlx_lm/tuner/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    19702 2024-04-11 20:20:08.000000 mlx-lm-0.9.0/mlx_lm/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-11 20:20:08.000000 mlx-lm-0.9.0/mlx_lm/version.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-11 20:20:15.906499 mlx-lm-0.9.0/mlx_lm.egg-info/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5059 2024-04-11 20:20:15.000000 mlx-lm-0.9.0/mlx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1064 2024-04-11 20:20:15.000000 mlx-lm-0.9.0/mlx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-11 20:20:15.000000 mlx-lm-0.9.0/mlx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       60 2024-04-11 20:20:15.000000 mlx-lm-0.9.0/mlx_lm.egg-info/requires.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-11 20:20:15.000000 mlx-lm-0.9.0/mlx_lm.egg-info/top_level.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-11 20:20:15.907132 mlx-lm-0.9.0/setup.cfg
+-rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.9.0/setup.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-11 20:20:15.905998 mlx-lm-0.9.0/tests/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.9.0/tests/test_datsets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/tests/test_gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/tests/test_lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    10294 2024-04-08 21:20:20.000000 mlx-lm-0.9.0/tests/test_models.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.9.0/tests/test_sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.9.0/tests/test_utils.py
```

### Comparing `mlx-lm-0.8.0/PKG-INFO` & `mlx-lm-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.8.0
+Version: 0.9.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: mlx>=0.8
+Requires-Dist: mlx>=0.10
 Requires-Dist: numpy
-Requires-Dist: transformers>=4.38.0
+Requires-Dist: transformers>=4.39.3
 Requires-Dist: protobuf
 Requires-Dist: pyyaml
 Requires-Dist: jinja2
 
 ## Generate Text with LLMs and MLX
 
 The easiest way to get started is to install the `mlx-lm` package:
```

### Comparing `mlx-lm-0.8.0/README.md` & `mlx-lm-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/convert.py` & `mlx-lm-0.9.0/mlx_lm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/fuse.py` & `mlx-lm-0.9.0/mlx_lm/fuse.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/generate.py` & `mlx-lm-0.9.0/mlx_lm/generate.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/gguf.py` & `mlx-lm-0.9.0/mlx_lm/gguf.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/lora.py` & `mlx-lm-0.9.0/mlx_lm/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/merge.py` & `mlx-lm-0.9.0/mlx_lm/merge.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/cohere.py` & `mlx-lm-0.9.0/mlx_lm/models/cohere.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/dbrx.py` & `mlx-lm-0.9.0/mlx_lm/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/gemma.py` & `mlx-lm-0.9.0/mlx_lm/models/gemma.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/llama.py` & `mlx-lm-0.9.0/mlx_lm/models/llama.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/mixtral.py` & `mlx-lm-0.9.0/mlx_lm/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/olmo.py` & `mlx-lm-0.9.0/mlx_lm/models/olmo.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/phi.py` & `mlx-lm-0.9.0/mlx_lm/models/phi.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/phixtral.py` & `mlx-lm-0.9.0/mlx_lm/models/phixtral.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/plamo.py` & `mlx-lm-0.9.0/mlx_lm/models/plamo.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/qwen.py` & `mlx-lm-0.9.0/mlx_lm/models/qwen.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/qwen2.py` & `mlx-lm-0.9.0/mlx_lm/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/qwen2_moe.py` & `mlx-lm-0.9.0/mlx_lm/models/qwen2_moe.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/stablelm.py` & `mlx-lm-0.9.0/mlx_lm/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/models/starcoder2.py` & `mlx-lm-0.9.0/mlx_lm/models/starcoder2.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/sample_utils.py` & `mlx-lm-0.9.0/mlx_lm/sample_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,14 @@
     Args:
         logits: The logits from the model's output.
         top_p: The cumulative probability threshold for top-p filtering.
         temperature: Temperature parameter for softmax distribution reshaping.
     Returns:
         token selected based on the top-p criterion.
     """
-    if (
-        logits.dtype == mx.bfloat16
-    ):  # workaround for unable to load kernel contiguous_scan_inclusive_sum_bfloat16_bfloat16
-        logits = logits.astype(mx.float32)
-
     # referenced implementation from https://github.com/huggingface/transformers/blob/main/src/transformers/generation/logits_process.py#L449-L460
     probs = mx.softmax(logits / temperature, axis=-1)
 
     # sort probs in ascending order
     sorted_indices = mx.argsort(probs, axis=-1)
     sorted_probs = probs[..., sorted_indices.squeeze(0)]
```

### Comparing `mlx-lm-0.8.0/mlx_lm/server.py` & `mlx-lm-0.9.0/mlx_lm/server.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/tuner/datasets.py` & `mlx-lm-0.9.0/mlx_lm/tuner/datasets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/tuner/lora.py` & `mlx-lm-0.9.0/mlx_lm/tuner/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/tuner/trainer.py` & `mlx-lm-0.9.0/mlx_lm/tuner/trainer.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/tuner/utils.py` & `mlx-lm-0.9.0/mlx_lm/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/mlx_lm/utils.py` & `mlx-lm-0.9.0/mlx_lm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 import mlx.core as mx
 import mlx.nn as nn
 from huggingface_hub import snapshot_download
 from mlx.utils import tree_flatten
 from transformers import AutoConfig, AutoTokenizer, PreTrainedTokenizer
 
-from .sample_utils import top_p_sampling
-
 # Local imports
+from .sample_utils import top_p_sampling
+from .tokenizer_utils import TokenizerWrapper, load_tokenizer
 from .tuner.utils import apply_lora_layers
 from .tuner.utils import dequantize as dequantize_model
 
 # Constants
 MODEL_REMAPPING = {
     "mistral": "llama",  # mistral is compatible with llama
     "phi-msft": "phixtral",
@@ -82,14 +82,15 @@
                     "*.json",
                     "*.safetensors",
                     "*.py",
                     "tokenizer.model",
                     "*.tiktoken",
                     "*.txt",
                 ],
+                resume_download=True,
             )
         )
     return model_path
 
 
 def apply_repetition_penalty(logits: mx.array, generated_tokens: Any, penalty: float):
     """
@@ -164,15 +165,16 @@
     cache = None
 
     repetition_context = prompt.tolist()
 
     if repetition_context_size:
         repetition_context = repetition_context[-repetition_context_size:]
 
-    while True:
+    def _step(y):
+        nonlocal cache, repetition_context
         logits, cache = model(y[None], cache=cache)
         logits = logits[:, -1, :]
 
         if repetition_penalty:
             logits = apply_repetition_penalty(
                 logits, repetition_context, repetition_penalty
             )
@@ -180,20 +182,29 @@
             repetition_context.append(y.item())
         else:
             y, prob = sample(logits)
 
         if repetition_context_size:
             if len(repetition_context) > repetition_context_size:
                 repetition_context = repetition_context[-repetition_context_size:]
-        yield y, prob
+        return y, prob
+
+    y, prob = _step(y)
+
+    while True:
+        sync = mx.async_eval(y)
+        next_out = _step(y)
+        sync.wait()
+        yield y.item(), prob
+        y, prob = next_out
 
 
 def generate(
     model: nn.Module,
-    tokenizer: PreTrainedTokenizer,
+    tokenizer: Union[PreTrainedTokenizer, TokenizerWrapper],
     prompt: str,
     temp: float = 0.0,
     max_tokens: int = 100,
     verbose: bool = False,
     formatter: Optional[Callable] = None,
     repetition_penalty: Optional[float] = None,
     repetition_context_size: Optional[int] = None,
@@ -211,78 +222,69 @@
        verbose (bool): If ``True``, print tokens and timing information
            (default ``False``).
        formatter (Optional[Callable]): A function which takes a token and a
            probability and displays it.
        repetition_penalty (float, optional): The penalty factor for repeating tokens.
        repetition_context_size (int, optional): The number of tokens to consider for repetition penalty.
     """
+    if not isinstance(tokenizer, TokenizerWrapper):
+        tokenizer = TokenizerWrapper(tokenizer)
 
     if verbose:
         print("=" * 10)
         print("Prompt:", prompt)
 
     prompt_tokens = mx.array(tokenizer.encode(prompt))
+    detokenizer = tokenizer.detokenizer
 
     tic = time.perf_counter()
-    tokens = []
-    token_strings = []
-    skip = 0
-    REPLACEMENT_CHAR = "\ufffd"
+    detokenizer.reset()
 
     for (token, prob), n in zip(
         generate_step(
             prompt_tokens,
             model,
             temp,
             repetition_penalty,
             repetition_context_size,
             top_p,
         ),
         range(max_tokens),
     ):
-        token = token.item()
         if n == 0:
             prompt_time = time.perf_counter() - tic
             tic = time.perf_counter()
         if token == tokenizer.eos_token_id:
             break
-        tokens.append(token)
+        detokenizer.add_token(token)
 
         if verbose:
-            s = tokenizer.decode(tokens)
-            if not s:
-                continue
-            elif formatter:
-                formatter(s[skip:], prob.item())
-                skip = len(s)
-            elif s[-1] != REPLACEMENT_CHAR:
-                print(s[skip:], end="", flush=True)
-                skip = len(s)
-            # Reset token cache at line break
-            if s[-1] == "\n":
-                tokens = []
-                token_strings.append(s)
-                skip = 0
+            if formatter:
+                # We have to finalize so that the prob corresponds to the last segment
+                detokenizer.finalize()
+                formatter(detokenizer.last_segment, prob.item())
+            else:
+                print(detokenizer.last_segment, end="", flush=True)
 
     token_count = n + 1
-    token_strings.append(tokenizer.decode(tokens).replace(REPLACEMENT_CHAR, ""))
+    detokenizer.finalize()
 
     if verbose:
-        print(token_strings[-1][skip:], flush=True)
         gen_time = time.perf_counter() - tic
+        print(detokenizer.last_segment, flush=True)
         print("=" * 10)
         if token_count == 0:
             print("No tokens generated for this prompt")
             return
         prompt_tps = prompt_tokens.size / prompt_time
         gen_tps = (token_count - 1) / gen_time
         print(f"Prompt: {prompt_tps:.3f} tokens-per-sec")
         print(f"Generation: {gen_tps:.3f} tokens-per-sec")
 
-    return "".join(token_strings)
+    return detokenizer.text
 
 
 def load_model(model_path: Path, lazy: bool = False) -> nn.Module:
     """
     Load and initialize the model from a given path.
 
     Args:
@@ -380,25 +382,25 @@
     """
     model_path = get_model_path(path_or_hf_repo)
 
     model = load_model(model_path, lazy)
     if adapter_path is not None:
         model = apply_lora_layers(model, adapter_path)
         model.eval()
+    tokenizer = load_tokenizer(model_path, tokenizer_config)
 
-    tokenizer = AutoTokenizer.from_pretrained(model_path, **tokenizer_config)
     return model, tokenizer
 
 
 def fetch_from_hub(
     model_path: Path, lazy: bool = False
 ) -> Tuple[nn.Module, dict, PreTrainedTokenizer]:
     model = load_model(model_path, lazy)
     config = AutoConfig.from_pretrained(model_path)
-    tokenizer = AutoTokenizer.from_pretrained(model_path)
+    tokenizer = load_tokenizer(model_path)
 
     return model, config.to_dict(), tokenizer
 
 
 def make_shards(weights: dict, max_file_size_gb: int = MAX_FILE_SIZE_GB) -> list:
     """
     Splits the weights into smaller shards.
```

### Comparing `mlx-lm-0.8.0/mlx_lm.egg-info/PKG-INFO` & `mlx-lm-0.9.0/mlx_lm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.8.0
+Version: 0.9.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: mlx>=0.8
+Requires-Dist: mlx>=0.10
 Requires-Dist: numpy
-Requires-Dist: transformers>=4.38.0
+Requires-Dist: transformers>=4.39.3
 Requires-Dist: protobuf
 Requires-Dist: pyyaml
 Requires-Dist: jinja2
 
 ## Generate Text with LLMs and MLX
 
 The easiest way to get started is to install the `mlx-lm` package:
```

### Comparing `mlx-lm-0.8.0/mlx_lm.egg-info/SOURCES.txt` & `mlx-lm-0.9.0/mlx_lm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 mlx_lm/gguf.py
 mlx_lm/lora.py
 mlx_lm/merge.py
 mlx_lm/py.typed
 mlx_lm/requirements.txt
 mlx_lm/sample_utils.py
 mlx_lm/server.py
+mlx_lm/tokenizer_utils.py
 mlx_lm/utils.py
 mlx_lm/version.py
 mlx_lm.egg-info/PKG-INFO
 mlx_lm.egg-info/SOURCES.txt
 mlx_lm.egg-info/dependency_links.txt
 mlx_lm.egg-info/requires.txt
 mlx_lm.egg-info/top_level.txt
```

### Comparing `mlx-lm-0.8.0/setup.py` & `mlx-lm-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/tests/test_datsets.py` & `mlx-lm-0.9.0/tests/test_datsets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/tests/test_gguf.py` & `mlx-lm-0.9.0/tests/test_gguf.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/tests/test_lora.py` & `mlx-lm-0.9.0/tests/test_lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/tests/test_models.py` & `mlx-lm-0.9.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/tests/test_sample_utils.py` & `mlx-lm-0.9.0/tests/test_sample_utils.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.8.0/tests/test_utils.py` & `mlx-lm-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

