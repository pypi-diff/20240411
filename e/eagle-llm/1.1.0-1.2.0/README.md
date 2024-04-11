# Comparing `tmp/eagle-llm-1.1.0.tar.gz` & `tmp/eagle-llm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagle-llm-1.1.0.tar", last modified: Wed Apr 10 17:39:27 2024, max compression
+gzip compressed data, was "eagle-llm-1.2.0.tar", last modified: Thu Apr 11 05:19:27 2024, max compression
```

## Comparing `eagle-llm-1.1.0.tar` & `eagle-llm-1.2.0.tar`

### file list

```diff
@@ -1,49 +1,59 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.347089 eagle-llm-1.1.0/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11347 2024-04-10 14:47:11.000000 eagle-llm-1.1.0/LICENSE
--rw-r--r--   0 lyh       (1000) lyh       (1000)    15859 2024-04-10 17:39:27.347089 eagle-llm-1.1.0/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15011 2024-04-10 16:40:59.000000 eagle-llm-1.1.0/README.md
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.343089 eagle-llm-1.1.0/eagle/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:49:30.000000 eagle-llm-1.1.0/eagle/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.343089 eagle-llm-1.1.0/eagle/application/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:11.000000 eagle-llm-1.1.0/eagle/application/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    12290 2024-04-10 15:59:04.000000 eagle-llm-1.1.0/eagle/application/webui.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.343089 eagle-llm-1.1.0/eagle/evaluation/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:11.000000 eagle-llm-1.1.0/eagle/evaluation/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    16068 2024-04-10 15:55:15.000000 eagle-llm-1.1.0/eagle/evaluation/gen_baseline_answer_llama2chat.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15070 2024-04-10 15:55:09.000000 eagle-llm-1.1.0/eagle/evaluation/gen_baseline_answer_mix.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14908 2024-04-10 15:55:03.000000 eagle-llm-1.1.0/eagle/evaluation/gen_baseline_answer_vicuna.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    17020 2024-04-10 15:54:50.000000 eagle-llm-1.1.0/eagle/evaluation/gen_ea_alpha_llama2chat.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    16048 2024-04-10 15:54:31.000000 eagle-llm-1.1.0/eagle/evaluation/gen_ea_alpha_vicuna.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    16913 2024-04-10 15:54:22.000000 eagle-llm-1.1.0/eagle/evaluation/gen_ea_answer_llama2chat.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15936 2024-04-10 15:54:13.000000 eagle-llm-1.1.0/eagle/evaluation/gen_ea_answer_mix.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15765 2024-04-10 15:48:36.000000 eagle-llm-1.1.0/eagle/evaluation/gen_ea_answer_vicuna.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1368 2024-04-10 14:47:11.000000 eagle-llm-1.1.0/eagle/evaluation/speed.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.343089 eagle-llm-1.1.0/eagle/ge_data/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/ge_data/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2010 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/ge_data/allocation.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     7651 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/ge_data/ge_data_all_llama2chat.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     6162 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/ge_data/ge_data_all_vicuna.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.343089 eagle-llm-1.1.0/eagle/model/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      234 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/choices.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    41222 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/cnets.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     7550 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/configs.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15721 2024-04-10 14:54:46.000000 eagle-llm-1.1.0/eagle/model/ea_model.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     5859 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/kv_cache.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    55095 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/modeling_llama_kv.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    52286 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/modeling_mixtral_kv.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    17795 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/utils.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    17367 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/utils_alpha.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     6214 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/model/utils_c.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    73143 2024-04-10 14:47:12.000000 eagle-llm-1.1.0/eagle/modeling_eagle.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.343089 eagle-llm-1.1.0/eagle/train/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 16:55:02.000000 eagle-llm-1.1.0/eagle/train/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    20466 2024-04-10 16:34:21.000000 eagle-llm-1.1.0/eagle/train/main.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-10 17:39:27.347089 eagle-llm-1.1.0/eagle_llm.egg-info/
--rw-r--r--   0 lyh       (1000) lyh       (1000)    15859 2024-04-10 17:39:27.000000 eagle-llm-1.1.0/eagle_llm.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1146 2024-04-10 17:39:27.000000 eagle-llm-1.1.0/eagle_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2024-04-10 17:39:27.000000 eagle-llm-1.1.0/eagle_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      145 2024-04-10 17:39:27.000000 eagle-llm-1.1.0/eagle_llm.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        6 2024-04-10 17:39:27.000000 eagle-llm-1.1.0/eagle_llm.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2024-04-10 17:39:27.347089 eagle-llm-1.1.0/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1025 2024-04-10 17:38:12.000000 eagle-llm-1.1.0/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.360856 eagle-llm-1.2.0/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11347 2024-04-10 14:47:11.000000 eagle-llm-1.2.0/LICENSE
+-rw-r--r--   0 lyh       (1000) lyh       (1000)    16023 2024-04-11 05:19:27.360856 eagle-llm-1.2.0/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15175 2024-04-11 05:19:00.000000 eagle-llm-1.2.0/README.md
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.356856 eagle-llm-1.2.0/eagle/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:49:30.000000 eagle-llm-1.2.0/eagle/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.356856 eagle-llm-1.2.0/eagle/application/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:11.000000 eagle-llm-1.2.0/eagle/application/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    12290 2024-04-10 15:59:04.000000 eagle-llm-1.2.0/eagle/application/webui.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.356856 eagle-llm-1.2.0/eagle/evaluation/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:11.000000 eagle-llm-1.2.0/eagle/evaluation/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    16068 2024-04-10 15:55:15.000000 eagle-llm-1.2.0/eagle/evaluation/gen_baseline_answer_llama2chat.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15070 2024-04-10 15:55:09.000000 eagle-llm-1.2.0/eagle/evaluation/gen_baseline_answer_mix.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14908 2024-04-10 15:55:03.000000 eagle-llm-1.2.0/eagle/evaluation/gen_baseline_answer_vicuna.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    17020 2024-04-10 15:54:50.000000 eagle-llm-1.2.0/eagle/evaluation/gen_ea_alpha_llama2chat.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    16048 2024-04-10 15:54:31.000000 eagle-llm-1.2.0/eagle/evaluation/gen_ea_alpha_vicuna.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    16913 2024-04-10 15:54:22.000000 eagle-llm-1.2.0/eagle/evaluation/gen_ea_answer_llama2chat.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15936 2024-04-10 15:54:13.000000 eagle-llm-1.2.0/eagle/evaluation/gen_ea_answer_mix.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15765 2024-04-10 15:48:36.000000 eagle-llm-1.2.0/eagle/evaluation/gen_ea_answer_vicuna.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1368 2024-04-10 14:47:11.000000 eagle-llm-1.2.0/eagle/evaluation/speed.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.356856 eagle-llm-1.2.0/eagle/ge_data/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/ge_data/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2010 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/ge_data/allocation.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     7651 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/ge_data/ge_data_all_llama2chat.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     6162 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/ge_data/ge_data_all_vicuna.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.356856 eagle-llm-1.2.0/eagle/model/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      236 2024-04-11 03:32:03.000000 eagle-llm-1.2.0/eagle/model/choices.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    41222 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/cnets.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     7550 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/configs.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15721 2024-04-10 14:54:46.000000 eagle-llm-1.2.0/eagle/model/ea_model.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     5859 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/kv_cache.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    55095 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/modeling_llama_kv.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    52286 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/modeling_mixtral_kv.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    17795 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/utils.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    17367 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/utils_alpha.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     6214 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/model/utils_c.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.360856 eagle-llm-1.2.0/eagle/modelbsne1/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      234 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/choices.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    42089 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/cnets.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     7550 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/configs.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    16501 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/ea_model.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     5865 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/kv_cache.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    55161 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/modeling_llama_kv.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19392 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/utils.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     6102 2024-04-11 03:28:35.000000 eagle-llm-1.2.0/eagle/modelbsne1/utils_c.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    73143 2024-04-10 14:47:12.000000 eagle-llm-1.2.0/eagle/modeling_eagle.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.360856 eagle-llm-1.2.0/eagle/train/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2024-04-10 16:55:02.000000 eagle-llm-1.2.0/eagle/train/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    20466 2024-04-10 16:34:21.000000 eagle-llm-1.2.0/eagle/train/main.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2024-04-11 05:19:27.360856 eagle-llm-1.2.0/eagle_llm.egg-info/
+-rw-r--r--   0 lyh       (1000) lyh       (1000)    16023 2024-04-11 05:19:27.000000 eagle-llm-1.2.0/eagle_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1407 2024-04-11 05:19:27.000000 eagle-llm-1.2.0/eagle_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2024-04-11 05:19:27.000000 eagle-llm-1.2.0/eagle_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      145 2024-04-11 05:19:27.000000 eagle-llm-1.2.0/eagle_llm.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        6 2024-04-11 05:19:27.000000 eagle-llm-1.2.0/eagle_llm.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2024-04-11 05:19:27.360856 eagle-llm-1.2.0/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1025 2024-04-11 03:36:15.000000 eagle-llm-1.2.0/setup.py
```

### Comparing `eagle-llm-1.1.0/LICENSE` & `eagle-llm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/PKG-INFO` & `eagle-llm-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eagle-llm
-Version: 1.1.0
+Version: 1.2.0
 Summary: Accelerating LLMs by 3x with No Quality Loss
 Home-page: https://github.com/SafeAILab/EAGLE
 Author-email: yuhui.li@stu.pku.edu.cn
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -110,18 +110,30 @@
 - [With gpt-fast](#with-gpt-fast)
   - [Setup](#setup)
   - [Quantizing Weights](quantizing-weights)
   - [Modifying Path](modifying-path)
 
 ## Setup & Installation
 
+### With pip 
+
+
+```bash
+pip install eagle-llm
+```
+
+### From the source
+
 ```bash
-pip install -r requirements.txt
+git clone https://github.com/SafeAILab/EAGLE.git
+cd EAGLE
+pip install -e .
 ```
 
+
 ## EAGLE Weights
 
 | Base Model  | EAGLE on Hugging Face  | \# EAGLE Parameters | Base Model  | EAGLE on Hugging Face  | \# EAGLE Parameters |
 |------|------|------|------|------|------|
 | Vicuna-7B-v1.3 | [yuhuili/EAGLE-Vicuna-7B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B | LLaMA2-Chat 7B | [yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-7B) | 0.24B |
 | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-Chat 13B | [yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-13B) | 0.37B |
 | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-Chat 70B| [yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-70B)| 0.99B |
@@ -174,22 +186,17 @@
 output=model.tokenizer.decode(output_ids[0])
 ```
 
 **_Note: Vicuna and LLaMA2-Chat are both chat models. You need to use the correct chat template, otherwise it will cause abnormal output from the model and affect the performance of EAGLE._**
 
 ### Batch size > 1
 
-Switch to the *bsne1* branch.
-
-```bash
-git checkout bsne1
-```
 Here is an example. Note that left padding is needed.
 ```python
-from model.ea_model import EaModel
+from modelbsne1.ea_model import EaModel
 from fastchat.model import get_conversation_template
 
 model = EaModel.from_pretrained(
     base_model_path=base_model_path,
     ea_model_path=EAGLE_model_path,
     torch_dtype=torch.float16,
     low_cpu_mem_usage=True,
@@ -234,14 +241,15 @@
 python -m eagle.ge_data.allocation --outdir [path of data]
 ```
 ### Train the Auto-regression Head
 ```bash
 accelerate launch -m --mixed_precision=bf16 eagle.train.main --tmpdir [path of data]\
 --cpdir [path of checkpoints] -- configpath [path of config file]
 ```
+*eagle/train* provides examples of configuration files.
 
 ### Inference on custom models
 
 If the original LLM structure differs from LLaMA and Mixtral, you can utilize EAGLE in two ways.
 
 #### 1. Using the generic modeling_eagle.py
 
@@ -311,14 +319,15 @@
 In EAGLE, using gpt-fast only requires three steps: setting up the environment, quantizing weights, and modifying the model path.
 
 ### Setup
 
 Switch to the *eaglefast* branch.
 
 ```bash
+git clone https://github.com/SafeAILab/EAGLE.git
 git checkout eaglefast
 ```
 
 Install the Preview (Nightly) version of PyTorch with CUDA 12.1, do not use "pip install torch" as it installs the Stable version, which lacks some of the new features used by gpt-fast. 
 
 _This is a requirement for gpt-fast, whereas other branches of eagle can use the Stable version of PyTorch._
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eagle-llm Version: 1.1.0 Summary: Accelerating LLMs
+Metadata-Version: 2.1 Name: eagle-llm Version: 1.2.0 Summary: Accelerating LLMs
 by 3x with No Quality Loss Home-page: https://github.com/SafeAILab/EAGLE
 Author-email: yuhui.li@stu.pku.edu.cn Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: torch Requires-Dist: transformers Requires-Dist:
@@ -47,32 +47,33 @@
 Installation](#setup--installation) - [EAGLE Weights](#eagle-weights) -
 [Inference](#inference) - [With UI](#with-ui) - [With Code](#with-code) -
 [Batch size > 1](#batch-size--1) - [Train](#train) - [Generate Train Data]
 (#generate-train-data) - [Train the Auto-regression Head](#train-the-auto-
 regression-head) - [Inference on custom models](#inference-on-custom-models) -
 [Evaluation](#evaluation) - [With gpt-fast](#with-gpt-fast) - [Setup](#setup) -
 [Quantizing Weights](quantizing-weights) - [Modifying Path](modifying-path) ##
-Setup & Installation ```bash pip install -r requirements.txt ``` ## EAGLE
-Weights | Base Model | EAGLE on Hugging Face | \# EAGLE Parameters | Base Model
-| EAGLE on Hugging Face | \# EAGLE Parameters | |------|------|------|------|--
-----|------| | Vicuna-7B-v1.3 | [yuhuili/EAGLE-Vicuna-7B-v1.3](https://
-huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B | LLaMA2-Chat 7B |
-[yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-7B) | 0.24B | | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-v1.3](https://
-huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-Chat 13B |
-[yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-13B) | 0.37B | | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-v1.3](https:/
-/huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-Chat 70B|
-[yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-70B)| 0.99B | | Mixtral-8x7B-Instruct-v0.1 | [yuhuili/EAGLE-mixtral-
-instruct-8x7B](https://huggingface.co/yuhuili/EAGLE-mixtral-instruct-8x7B)|
-0.28B | ## Inference The inference code we provide automatically allocates
-model weights (loading a model across multiple GPUs), allowing you to run
-models that exceed the memory of a single GPU. ### With UI We have provided a
-suggested web interface, which you can use by running the following command.
+Setup & Installation ### With pip ```bash pip install eagle-llm ``` ### From
+the source ```bash git clone https://github.com/SafeAILab/EAGLE.git cd EAGLE
+pip install -e . ``` ## EAGLE Weights | Base Model | EAGLE on Hugging Face | \#
+EAGLE Parameters | Base Model | EAGLE on Hugging Face | \# EAGLE Parameters |
+|------|------|------|------|------|------| | Vicuna-7B-v1.3 | [yuhuili/EAGLE-
+Vicuna-7B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B |
+LLaMA2-Chat 7B | [yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/
+EAGLE-llama2-chat-7B) | 0.24B | | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-
+v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-
+Chat 13B | [yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/
+EAGLE-llama2-chat-13B) | 0.37B | | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-
+v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-
+Chat 70B| [yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-
+llama2-chat-70B)| 0.99B | | Mixtral-8x7B-Instruct-v0.1 | [yuhuili/EAGLE-
+mixtral-instruct-8x7B](https://huggingface.co/yuhuili/EAGLE-mixtral-instruct-
+8x7B)| 0.28B | ## Inference The inference code we provide automatically
+allocates model weights (loading a model across multiple GPUs), allowing you to
+run models that exceed the memory of a single GPU. ### With UI We have provided
+a suggested web interface, which you can use by running the following command.
 After the model is fully loaded, a URL will be output in the terminal, which
 you can enter into your browser to access. ```bash python -
 m eagle.application.webui --ea-model-path [path of EAGLE weight]\ --base-model-
 path [path of the original model]\ --model-type [vicuna or llama-2-chat] ```
 ### With Code You can use our provided "eagenerate" for speedup generation just
 like using 'generate' from Hugging Face. Here is an example. ```python from
 eagle.model.ea_model import EaModel from fastchat.model import
@@ -93,18 +94,17 @@
 ("vicuna") conv.append_message(conv.roles[0], your_message) conv.append_message
 (conv.roles[1], None) prompt = conv.get_prompt() input_ids=model.tokenizer(
 [prompt]).input_ids input_ids = torch.as_tensor(input_ids).cuda()
 output_ids=model.eagenerate(input_ids,temperature=0.5,max_new_tokens=512)
 output=model.tokenizer.decode(output_ids[0]) ``` **_Note: Vicuna and LLaMA2-
 Chat are both chat models. You need to use the correct chat template, otherwise
 it will cause abnormal output from the model and affect the performance of
-EAGLE._** ### Batch size > 1 Switch to the *bsne1* branch. ```bash git checkout
-bsne1 ``` Here is an example. Note that left padding is needed. ```python from
-model.ea_model import EaModel from fastchat.model import
-get_conversation_template model = EaModel.from_pretrained
+EAGLE._** ### Batch size > 1 Here is an example. Note that left padding is
+needed. ```python from modelbsne1.ea_model import EaModel from fastchat.model
+import get_conversation_template model = EaModel.from_pretrained
 ( base_model_path=base_model_path, ea_model_path=EAGLE_model_path,
 torch_dtype=torch.float16, low_cpu_mem_usage=True, device_map="auto" ) # left
 padding model.eval() model.tokenizer.padding_side = "left"
 model.tokenizer.pad_token = model.tokenizer.eos_token model.config.pad_token_id
 = model.config.eos_token_id sys_p = "You are a helpful, respectful and honest
 assistant. Always answer as helpfully as possible, while being safe. Your
 answers should not include any harmful, unethical, racist, sexist, toxic,
@@ -126,19 +126,20 @@
 output=model.tokenizer.batch_decode(output_ids) print(output) # vanilla auto-
 regression # output_ids, new_token, idx=model.naivegenerate
 (input_s.input_ids,input_s.attention_mask,temperature=0.0,max_new_tokens=512,top_k=15,log=True)
 ``` ## Train ### Generate Train Data You can run the following command to
 generate the training data. ```bash python -m eagle.ge_data.allocation --outdir
 [path of data] ``` ### Train the Auto-regression Head ```bash accelerate launch
 -m --mixed_precision=bf16 eagle.train.main --tmpdir [path of data]\ --cpdir
-[path of checkpoints] -- configpath [path of config file] ``` ### Inference on
-custom models If the original LLM structure differs from LLaMA and Mixtral, you
-can utilize EAGLE in two ways. #### 1. Using the generic modeling_eagle.py This
-approach directly encapsulates the native Transformers LLM. Here is an example.
-**Note: transformers version should be higher than 4.36.** ```python from
+[path of checkpoints] -- configpath [path of config file] ``` *eagle/train*
+provides examples of configuration files. ### Inference on custom models If the
+original LLM structure differs from LLaMA and Mixtral, you can utilize EAGLE in
+two ways. #### 1. Using the generic modeling_eagle.py This approach directly
+encapsulates the native Transformers LLM. Here is an example. **Note:
+transformers version should be higher than 4.36.** ```python from
 eagle.modeling_eagle import EAGLE from transformers import
 AutoModelForCausalLM,AutoTokenizer tokenizer=AutoTokenizer.from_pretrained
 (base_model_path) model=AutoModelForCausalLM.from_pretrained
 ("base_model_path",torch_dtype=torch.float16,device_map="auto",) # for bs>1,
 the padding side should be right if bs>1: tokenizer.padding_side = "left"
 tokenizer.pad_token = tokenizer.eos_token model.config.pad_token_id =
 model.config.eos_token_id text=prompt1 # text=[prompt1,prompt2] inputs =
@@ -168,30 +169,31 @@
 vanilla | 24.5 tokens/s | N/A | | gpt-fast | 55.1 tokens/s | 106.9 tokens/s | |
 EAGLE+gpt-fast | 100.2 tokens/s | 160.4 tokens/s |
                                    [demogif]
 _Inference is conducted on a single RTX3090 GPU at int4 precision using the
 LLaMA2-chat 7B model. No additional training required._ In EAGLE, using gpt-
 fast only requires three steps: setting up the environment, quantizing weights,
 and modifying the model path. ### Setup Switch to the *eaglefast* branch.
-```bash git checkout eaglefast ``` Install the Preview (Nightly) version of
-PyTorch with CUDA 12.1, do not use "pip install torch" as it installs the
-Stable version, which lacks some of the new features used by gpt-fast. _This is
-a requirement for gpt-fast, whereas other branches of eagle can use the Stable
-version of PyTorch._ ### Quantizing Weights Convert Huggingface weights to the
-format required by gpt-fast. ```bash python convert/convert_hf_checkpoint.py --
-checkpoint_dir path_of_base_model python convert/convert_hf_checkpoint_EAGLE.py
---checkpoint_dir path_of_eagle ``` Quantize weights. ```bash python -
-m model.quantize_llama --checkpoint_path path_of_base_model/model.pth python -
-m model.quantize_EAGLE --checkpoint_path path_of_eagle/model.pth ``` ###
-Modifying Path When specifying the model weights (including the base model and
-EAGLE), change "path" to "path/model_int4.g32.pth". ## ð Our Contributors A
-heartfelt thank you to all our contributors. ![Contributors](https://
-contrib.rocks/image?repo=SafeAILab/EAGLE) ## Reference For technical details
-and full experimental results, please check [the paper](https://arxiv.org/pdf/
-2401.15077.pdf). ``` @article{li2024eagle, author = {Yuhui Li and Fangyun Wei
-and Chao Zhang and Hongyang Zhang}, title = {EAGLE: Speculative Sampling
-Requires Rethinking Feature Uncertainty}, journal = {arXiv preprint arXiv:
-2401.15077}, year = {2024} } ``` ## Acknowledgements This project has been
-influenced by many excellent projects in the LLM community, such as [Medusa]
-(https://github.com/FasterDecoding/Medusa), [FastChat](https://github.com/lm-
-sys/FastChat), and others. The logo is designed by GPT-4. We also appreciate
-many valuable discussions with Tianle Cai, Hao Zhang, Ziteng Sun, and others.
+```bash git clone https://github.com/SafeAILab/EAGLE.git git checkout eaglefast
+``` Install the Preview (Nightly) version of PyTorch with CUDA 12.1, do not use
+"pip install torch" as it installs the Stable version, which lacks some of the
+new features used by gpt-fast. _This is a requirement for gpt-fast, whereas
+other branches of eagle can use the Stable version of PyTorch._ ### Quantizing
+Weights Convert Huggingface weights to the format required by gpt-fast. ```bash
+python convert/convert_hf_checkpoint.py --checkpoint_dir path_of_base_model
+python convert/convert_hf_checkpoint_EAGLE.py --checkpoint_dir path_of_eagle
+``` Quantize weights. ```bash python -m model.quantize_llama --checkpoint_path
+path_of_base_model/model.pth python -m model.quantize_EAGLE --checkpoint_path
+path_of_eagle/model.pth ``` ### Modifying Path When specifying the model
+weights (including the base model and EAGLE), change "path" to "path/
+model_int4.g32.pth". ## ð Our Contributors A heartfelt thank you to all our
+contributors. ![Contributors](https://contrib.rocks/image?repo=SafeAILab/EAGLE)
+## Reference For technical details and full experimental results, please check
+[the paper](https://arxiv.org/pdf/2401.15077.pdf). ``` @article{li2024eagle,
+author = {Yuhui Li and Fangyun Wei and Chao Zhang and Hongyang Zhang}, title =
+{EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty}, journal
+= {arXiv preprint arXiv:2401.15077}, year = {2024} } ``` ## Acknowledgements
+This project has been influenced by many excellent projects in the LLM
+community, such as [Medusa](https://github.com/FasterDecoding/Medusa),
+[FastChat](https://github.com/lm-sys/FastChat), and others. The logo is
+designed by GPT-4. We also appreciate many valuable discussions with Tianle
+Cai, Hao Zhang, Ziteng Sun, and others.
```

### Comparing `eagle-llm-1.1.0/README.md` & `eagle-llm-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,30 @@
 - [With gpt-fast](#with-gpt-fast)
   - [Setup](#setup)
   - [Quantizing Weights](quantizing-weights)
   - [Modifying Path](modifying-path)
 
 ## Setup & Installation
 
+### With pip 
+
+
+```bash
+pip install eagle-llm
+```
+
+### From the source
+
 ```bash
-pip install -r requirements.txt
+git clone https://github.com/SafeAILab/EAGLE.git
+cd EAGLE
+pip install -e .
 ```
 
+
 ## EAGLE Weights
 
 | Base Model  | EAGLE on Hugging Face  | \# EAGLE Parameters | Base Model  | EAGLE on Hugging Face  | \# EAGLE Parameters |
 |------|------|------|------|------|------|
 | Vicuna-7B-v1.3 | [yuhuili/EAGLE-Vicuna-7B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B | LLaMA2-Chat 7B | [yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-7B) | 0.24B |
 | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-Chat 13B | [yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-13B) | 0.37B |
 | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-Chat 70B| [yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-70B)| 0.99B |
@@ -149,22 +161,17 @@
 output=model.tokenizer.decode(output_ids[0])
 ```
 
 **_Note: Vicuna and LLaMA2-Chat are both chat models. You need to use the correct chat template, otherwise it will cause abnormal output from the model and affect the performance of EAGLE._**
 
 ### Batch size > 1
 
-Switch to the *bsne1* branch.
-
-```bash
-git checkout bsne1
-```
 Here is an example. Note that left padding is needed.
 ```python
-from model.ea_model import EaModel
+from modelbsne1.ea_model import EaModel
 from fastchat.model import get_conversation_template
 
 model = EaModel.from_pretrained(
     base_model_path=base_model_path,
     ea_model_path=EAGLE_model_path,
     torch_dtype=torch.float16,
     low_cpu_mem_usage=True,
@@ -209,14 +216,15 @@
 python -m eagle.ge_data.allocation --outdir [path of data]
 ```
 ### Train the Auto-regression Head
 ```bash
 accelerate launch -m --mixed_precision=bf16 eagle.train.main --tmpdir [path of data]\
 --cpdir [path of checkpoints] -- configpath [path of config file]
 ```
+*eagle/train* provides examples of configuration files.
 
 ### Inference on custom models
 
 If the original LLM structure differs from LLaMA and Mixtral, you can utilize EAGLE in two ways.
 
 #### 1. Using the generic modeling_eagle.py
 
@@ -286,14 +294,15 @@
 In EAGLE, using gpt-fast only requires three steps: setting up the environment, quantizing weights, and modifying the model path.
 
 ### Setup
 
 Switch to the *eaglefast* branch.
 
 ```bash
+git clone https://github.com/SafeAILab/EAGLE.git
 git checkout eaglefast
 ```
 
 Install the Preview (Nightly) version of PyTorch with CUDA 12.1, do not use "pip install torch" as it installs the Stable version, which lacks some of the new features used by gpt-fast. 
 
 _This is a requirement for gpt-fast, whereas other branches of eagle can use the Stable version of PyTorch._
```

#### html2text {}

```diff
@@ -36,32 +36,33 @@
 Installation](#setup--installation) - [EAGLE Weights](#eagle-weights) -
 [Inference](#inference) - [With UI](#with-ui) - [With Code](#with-code) -
 [Batch size > 1](#batch-size--1) - [Train](#train) - [Generate Train Data]
 (#generate-train-data) - [Train the Auto-regression Head](#train-the-auto-
 regression-head) - [Inference on custom models](#inference-on-custom-models) -
 [Evaluation](#evaluation) - [With gpt-fast](#with-gpt-fast) - [Setup](#setup) -
 [Quantizing Weights](quantizing-weights) - [Modifying Path](modifying-path) ##
-Setup & Installation ```bash pip install -r requirements.txt ``` ## EAGLE
-Weights | Base Model | EAGLE on Hugging Face | \# EAGLE Parameters | Base Model
-| EAGLE on Hugging Face | \# EAGLE Parameters | |------|------|------|------|--
-----|------| | Vicuna-7B-v1.3 | [yuhuili/EAGLE-Vicuna-7B-v1.3](https://
-huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B | LLaMA2-Chat 7B |
-[yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-7B) | 0.24B | | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-v1.3](https://
-huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-Chat 13B |
-[yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-13B) | 0.37B | | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-v1.3](https:/
-/huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-Chat 70B|
-[yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-70B)| 0.99B | | Mixtral-8x7B-Instruct-v0.1 | [yuhuili/EAGLE-mixtral-
-instruct-8x7B](https://huggingface.co/yuhuili/EAGLE-mixtral-instruct-8x7B)|
-0.28B | ## Inference The inference code we provide automatically allocates
-model weights (loading a model across multiple GPUs), allowing you to run
-models that exceed the memory of a single GPU. ### With UI We have provided a
-suggested web interface, which you can use by running the following command.
+Setup & Installation ### With pip ```bash pip install eagle-llm ``` ### From
+the source ```bash git clone https://github.com/SafeAILab/EAGLE.git cd EAGLE
+pip install -e . ``` ## EAGLE Weights | Base Model | EAGLE on Hugging Face | \#
+EAGLE Parameters | Base Model | EAGLE on Hugging Face | \# EAGLE Parameters |
+|------|------|------|------|------|------| | Vicuna-7B-v1.3 | [yuhuili/EAGLE-
+Vicuna-7B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B |
+LLaMA2-Chat 7B | [yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/
+EAGLE-llama2-chat-7B) | 0.24B | | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-
+v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-
+Chat 13B | [yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/
+EAGLE-llama2-chat-13B) | 0.37B | | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-
+v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-
+Chat 70B| [yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-
+llama2-chat-70B)| 0.99B | | Mixtral-8x7B-Instruct-v0.1 | [yuhuili/EAGLE-
+mixtral-instruct-8x7B](https://huggingface.co/yuhuili/EAGLE-mixtral-instruct-
+8x7B)| 0.28B | ## Inference The inference code we provide automatically
+allocates model weights (loading a model across multiple GPUs), allowing you to
+run models that exceed the memory of a single GPU. ### With UI We have provided
+a suggested web interface, which you can use by running the following command.
 After the model is fully loaded, a URL will be output in the terminal, which
 you can enter into your browser to access. ```bash python -
 m eagle.application.webui --ea-model-path [path of EAGLE weight]\ --base-model-
 path [path of the original model]\ --model-type [vicuna or llama-2-chat] ```
 ### With Code You can use our provided "eagenerate" for speedup generation just
 like using 'generate' from Hugging Face. Here is an example. ```python from
 eagle.model.ea_model import EaModel from fastchat.model import
@@ -82,18 +83,17 @@
 ("vicuna") conv.append_message(conv.roles[0], your_message) conv.append_message
 (conv.roles[1], None) prompt = conv.get_prompt() input_ids=model.tokenizer(
 [prompt]).input_ids input_ids = torch.as_tensor(input_ids).cuda()
 output_ids=model.eagenerate(input_ids,temperature=0.5,max_new_tokens=512)
 output=model.tokenizer.decode(output_ids[0]) ``` **_Note: Vicuna and LLaMA2-
 Chat are both chat models. You need to use the correct chat template, otherwise
 it will cause abnormal output from the model and affect the performance of
-EAGLE._** ### Batch size > 1 Switch to the *bsne1* branch. ```bash git checkout
-bsne1 ``` Here is an example. Note that left padding is needed. ```python from
-model.ea_model import EaModel from fastchat.model import
-get_conversation_template model = EaModel.from_pretrained
+EAGLE._** ### Batch size > 1 Here is an example. Note that left padding is
+needed. ```python from modelbsne1.ea_model import EaModel from fastchat.model
+import get_conversation_template model = EaModel.from_pretrained
 ( base_model_path=base_model_path, ea_model_path=EAGLE_model_path,
 torch_dtype=torch.float16, low_cpu_mem_usage=True, device_map="auto" ) # left
 padding model.eval() model.tokenizer.padding_side = "left"
 model.tokenizer.pad_token = model.tokenizer.eos_token model.config.pad_token_id
 = model.config.eos_token_id sys_p = "You are a helpful, respectful and honest
 assistant. Always answer as helpfully as possible, while being safe. Your
 answers should not include any harmful, unethical, racist, sexist, toxic,
@@ -115,19 +115,20 @@
 output=model.tokenizer.batch_decode(output_ids) print(output) # vanilla auto-
 regression # output_ids, new_token, idx=model.naivegenerate
 (input_s.input_ids,input_s.attention_mask,temperature=0.0,max_new_tokens=512,top_k=15,log=True)
 ``` ## Train ### Generate Train Data You can run the following command to
 generate the training data. ```bash python -m eagle.ge_data.allocation --outdir
 [path of data] ``` ### Train the Auto-regression Head ```bash accelerate launch
 -m --mixed_precision=bf16 eagle.train.main --tmpdir [path of data]\ --cpdir
-[path of checkpoints] -- configpath [path of config file] ``` ### Inference on
-custom models If the original LLM structure differs from LLaMA and Mixtral, you
-can utilize EAGLE in two ways. #### 1. Using the generic modeling_eagle.py This
-approach directly encapsulates the native Transformers LLM. Here is an example.
-**Note: transformers version should be higher than 4.36.** ```python from
+[path of checkpoints] -- configpath [path of config file] ``` *eagle/train*
+provides examples of configuration files. ### Inference on custom models If the
+original LLM structure differs from LLaMA and Mixtral, you can utilize EAGLE in
+two ways. #### 1. Using the generic modeling_eagle.py This approach directly
+encapsulates the native Transformers LLM. Here is an example. **Note:
+transformers version should be higher than 4.36.** ```python from
 eagle.modeling_eagle import EAGLE from transformers import
 AutoModelForCausalLM,AutoTokenizer tokenizer=AutoTokenizer.from_pretrained
 (base_model_path) model=AutoModelForCausalLM.from_pretrained
 ("base_model_path",torch_dtype=torch.float16,device_map="auto",) # for bs>1,
 the padding side should be right if bs>1: tokenizer.padding_side = "left"
 tokenizer.pad_token = tokenizer.eos_token model.config.pad_token_id =
 model.config.eos_token_id text=prompt1 # text=[prompt1,prompt2] inputs =
@@ -157,30 +158,31 @@
 vanilla | 24.5 tokens/s | N/A | | gpt-fast | 55.1 tokens/s | 106.9 tokens/s | |
 EAGLE+gpt-fast | 100.2 tokens/s | 160.4 tokens/s |
                                    [demogif]
 _Inference is conducted on a single RTX3090 GPU at int4 precision using the
 LLaMA2-chat 7B model. No additional training required._ In EAGLE, using gpt-
 fast only requires three steps: setting up the environment, quantizing weights,
 and modifying the model path. ### Setup Switch to the *eaglefast* branch.
-```bash git checkout eaglefast ``` Install the Preview (Nightly) version of
-PyTorch with CUDA 12.1, do not use "pip install torch" as it installs the
-Stable version, which lacks some of the new features used by gpt-fast. _This is
-a requirement for gpt-fast, whereas other branches of eagle can use the Stable
-version of PyTorch._ ### Quantizing Weights Convert Huggingface weights to the
-format required by gpt-fast. ```bash python convert/convert_hf_checkpoint.py --
-checkpoint_dir path_of_base_model python convert/convert_hf_checkpoint_EAGLE.py
---checkpoint_dir path_of_eagle ``` Quantize weights. ```bash python -
-m model.quantize_llama --checkpoint_path path_of_base_model/model.pth python -
-m model.quantize_EAGLE --checkpoint_path path_of_eagle/model.pth ``` ###
-Modifying Path When specifying the model weights (including the base model and
-EAGLE), change "path" to "path/model_int4.g32.pth". ## ð Our Contributors A
-heartfelt thank you to all our contributors. ![Contributors](https://
-contrib.rocks/image?repo=SafeAILab/EAGLE) ## Reference For technical details
-and full experimental results, please check [the paper](https://arxiv.org/pdf/
-2401.15077.pdf). ``` @article{li2024eagle, author = {Yuhui Li and Fangyun Wei
-and Chao Zhang and Hongyang Zhang}, title = {EAGLE: Speculative Sampling
-Requires Rethinking Feature Uncertainty}, journal = {arXiv preprint arXiv:
-2401.15077}, year = {2024} } ``` ## Acknowledgements This project has been
-influenced by many excellent projects in the LLM community, such as [Medusa]
-(https://github.com/FasterDecoding/Medusa), [FastChat](https://github.com/lm-
-sys/FastChat), and others. The logo is designed by GPT-4. We also appreciate
-many valuable discussions with Tianle Cai, Hao Zhang, Ziteng Sun, and others.
+```bash git clone https://github.com/SafeAILab/EAGLE.git git checkout eaglefast
+``` Install the Preview (Nightly) version of PyTorch with CUDA 12.1, do not use
+"pip install torch" as it installs the Stable version, which lacks some of the
+new features used by gpt-fast. _This is a requirement for gpt-fast, whereas
+other branches of eagle can use the Stable version of PyTorch._ ### Quantizing
+Weights Convert Huggingface weights to the format required by gpt-fast. ```bash
+python convert/convert_hf_checkpoint.py --checkpoint_dir path_of_base_model
+python convert/convert_hf_checkpoint_EAGLE.py --checkpoint_dir path_of_eagle
+``` Quantize weights. ```bash python -m model.quantize_llama --checkpoint_path
+path_of_base_model/model.pth python -m model.quantize_EAGLE --checkpoint_path
+path_of_eagle/model.pth ``` ### Modifying Path When specifying the model
+weights (including the base model and EAGLE), change "path" to "path/
+model_int4.g32.pth". ## ð Our Contributors A heartfelt thank you to all our
+contributors. ![Contributors](https://contrib.rocks/image?repo=SafeAILab/EAGLE)
+## Reference For technical details and full experimental results, please check
+[the paper](https://arxiv.org/pdf/2401.15077.pdf). ``` @article{li2024eagle,
+author = {Yuhui Li and Fangyun Wei and Chao Zhang and Hongyang Zhang}, title =
+{EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty}, journal
+= {arXiv preprint arXiv:2401.15077}, year = {2024} } ``` ## Acknowledgements
+This project has been influenced by many excellent projects in the LLM
+community, such as [Medusa](https://github.com/FasterDecoding/Medusa),
+[FastChat](https://github.com/lm-sys/FastChat), and others. The logo is
+designed by GPT-4. We also appreciate many valuable discussions with Tianle
+Cai, Hao Zhang, Ziteng Sun, and others.
```

### Comparing `eagle-llm-1.1.0/eagle/application/webui.py` & `eagle-llm-1.2.0/eagle/application/webui.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_baseline_answer_llama2chat.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_baseline_answer_llama2chat.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_baseline_answer_mix.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_baseline_answer_mix.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_baseline_answer_vicuna.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_baseline_answer_vicuna.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_ea_alpha_llama2chat.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_ea_alpha_llama2chat.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_ea_alpha_vicuna.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_ea_alpha_vicuna.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_ea_answer_llama2chat.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_ea_answer_llama2chat.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_ea_answer_mix.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_ea_answer_mix.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/gen_ea_answer_vicuna.py` & `eagle-llm-1.2.0/eagle/evaluation/gen_ea_answer_vicuna.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/evaluation/speed.py` & `eagle-llm-1.2.0/eagle/evaluation/speed.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/ge_data/allocation.py` & `eagle-llm-1.2.0/eagle/ge_data/allocation.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/ge_data/ge_data_all_llama2chat.py` & `eagle-llm-1.2.0/eagle/ge_data/ge_data_all_llama2chat.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/ge_data/ge_data_all_vicuna.py` & `eagle-llm-1.2.0/eagle/ge_data/ge_data_all_vicuna.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/cnets.py` & `eagle-llm-1.2.0/eagle/model/cnets.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/configs.py` & `eagle-llm-1.2.0/eagle/model/configs.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/ea_model.py` & `eagle-llm-1.2.0/eagle/model/ea_model.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/kv_cache.py` & `eagle-llm-1.2.0/eagle/model/kv_cache.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/modeling_llama_kv.py` & `eagle-llm-1.2.0/eagle/model/modeling_llama_kv.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/modeling_mixtral_kv.py` & `eagle-llm-1.2.0/eagle/model/modeling_mixtral_kv.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/utils.py` & `eagle-llm-1.2.0/eagle/model/utils.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/utils_alpha.py` & `eagle-llm-1.2.0/eagle/model/utils_alpha.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/model/utils_c.py` & `eagle-llm-1.2.0/eagle/model/utils_c.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/modeling_eagle.py` & `eagle-llm-1.2.0/eagle/modeling_eagle.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle/train/main.py` & `eagle-llm-1.2.0/eagle/train/main.py`

 * *Files identical despite different names*

### Comparing `eagle-llm-1.1.0/eagle_llm.egg-info/PKG-INFO` & `eagle-llm-1.2.0/eagle_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eagle-llm
-Version: 1.1.0
+Version: 1.2.0
 Summary: Accelerating LLMs by 3x with No Quality Loss
 Home-page: https://github.com/SafeAILab/EAGLE
 Author-email: yuhui.li@stu.pku.edu.cn
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -110,18 +110,30 @@
 - [With gpt-fast](#with-gpt-fast)
   - [Setup](#setup)
   - [Quantizing Weights](quantizing-weights)
   - [Modifying Path](modifying-path)
 
 ## Setup & Installation
 
+### With pip 
+
+
+```bash
+pip install eagle-llm
+```
+
+### From the source
+
 ```bash
-pip install -r requirements.txt
+git clone https://github.com/SafeAILab/EAGLE.git
+cd EAGLE
+pip install -e .
 ```
 
+
 ## EAGLE Weights
 
 | Base Model  | EAGLE on Hugging Face  | \# EAGLE Parameters | Base Model  | EAGLE on Hugging Face  | \# EAGLE Parameters |
 |------|------|------|------|------|------|
 | Vicuna-7B-v1.3 | [yuhuili/EAGLE-Vicuna-7B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B | LLaMA2-Chat 7B | [yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-7B) | 0.24B |
 | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-Chat 13B | [yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-13B) | 0.37B |
 | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-Chat 70B| [yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-llama2-chat-70B)| 0.99B |
@@ -174,22 +186,17 @@
 output=model.tokenizer.decode(output_ids[0])
 ```
 
 **_Note: Vicuna and LLaMA2-Chat are both chat models. You need to use the correct chat template, otherwise it will cause abnormal output from the model and affect the performance of EAGLE._**
 
 ### Batch size > 1
 
-Switch to the *bsne1* branch.
-
-```bash
-git checkout bsne1
-```
 Here is an example. Note that left padding is needed.
 ```python
-from model.ea_model import EaModel
+from modelbsne1.ea_model import EaModel
 from fastchat.model import get_conversation_template
 
 model = EaModel.from_pretrained(
     base_model_path=base_model_path,
     ea_model_path=EAGLE_model_path,
     torch_dtype=torch.float16,
     low_cpu_mem_usage=True,
@@ -234,14 +241,15 @@
 python -m eagle.ge_data.allocation --outdir [path of data]
 ```
 ### Train the Auto-regression Head
 ```bash
 accelerate launch -m --mixed_precision=bf16 eagle.train.main --tmpdir [path of data]\
 --cpdir [path of checkpoints] -- configpath [path of config file]
 ```
+*eagle/train* provides examples of configuration files.
 
 ### Inference on custom models
 
 If the original LLM structure differs from LLaMA and Mixtral, you can utilize EAGLE in two ways.
 
 #### 1. Using the generic modeling_eagle.py
 
@@ -311,14 +319,15 @@
 In EAGLE, using gpt-fast only requires three steps: setting up the environment, quantizing weights, and modifying the model path.
 
 ### Setup
 
 Switch to the *eaglefast* branch.
 
 ```bash
+git clone https://github.com/SafeAILab/EAGLE.git
 git checkout eaglefast
 ```
 
 Install the Preview (Nightly) version of PyTorch with CUDA 12.1, do not use "pip install torch" as it installs the Stable version, which lacks some of the new features used by gpt-fast. 
 
 _This is a requirement for gpt-fast, whereas other branches of eagle can use the Stable version of PyTorch._
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eagle-llm Version: 1.1.0 Summary: Accelerating LLMs
+Metadata-Version: 2.1 Name: eagle-llm Version: 1.2.0 Summary: Accelerating LLMs
 by 3x with No Quality Loss Home-page: https://github.com/SafeAILab/EAGLE
 Author-email: yuhui.li@stu.pku.edu.cn Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: torch Requires-Dist: transformers Requires-Dist:
@@ -47,32 +47,33 @@
 Installation](#setup--installation) - [EAGLE Weights](#eagle-weights) -
 [Inference](#inference) - [With UI](#with-ui) - [With Code](#with-code) -
 [Batch size > 1](#batch-size--1) - [Train](#train) - [Generate Train Data]
 (#generate-train-data) - [Train the Auto-regression Head](#train-the-auto-
 regression-head) - [Inference on custom models](#inference-on-custom-models) -
 [Evaluation](#evaluation) - [With gpt-fast](#with-gpt-fast) - [Setup](#setup) -
 [Quantizing Weights](quantizing-weights) - [Modifying Path](modifying-path) ##
-Setup & Installation ```bash pip install -r requirements.txt ``` ## EAGLE
-Weights | Base Model | EAGLE on Hugging Face | \# EAGLE Parameters | Base Model
-| EAGLE on Hugging Face | \# EAGLE Parameters | |------|------|------|------|--
-----|------| | Vicuna-7B-v1.3 | [yuhuili/EAGLE-Vicuna-7B-v1.3](https://
-huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B | LLaMA2-Chat 7B |
-[yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-7B) | 0.24B | | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-v1.3](https://
-huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-Chat 13B |
-[yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-13B) | 0.37B | | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-v1.3](https:/
-/huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-Chat 70B|
-[yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-llama2-
-chat-70B)| 0.99B | | Mixtral-8x7B-Instruct-v0.1 | [yuhuili/EAGLE-mixtral-
-instruct-8x7B](https://huggingface.co/yuhuili/EAGLE-mixtral-instruct-8x7B)|
-0.28B | ## Inference The inference code we provide automatically allocates
-model weights (loading a model across multiple GPUs), allowing you to run
-models that exceed the memory of a single GPU. ### With UI We have provided a
-suggested web interface, which you can use by running the following command.
+Setup & Installation ### With pip ```bash pip install eagle-llm ``` ### From
+the source ```bash git clone https://github.com/SafeAILab/EAGLE.git cd EAGLE
+pip install -e . ``` ## EAGLE Weights | Base Model | EAGLE on Hugging Face | \#
+EAGLE Parameters | Base Model | EAGLE on Hugging Face | \# EAGLE Parameters |
+|------|------|------|------|------|------| | Vicuna-7B-v1.3 | [yuhuili/EAGLE-
+Vicuna-7B-v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-7B-v1.3) | 0.24B |
+LLaMA2-Chat 7B | [yuhuili/EAGLE-llama2-chat-7B](https://huggingface.co/yuhuili/
+EAGLE-llama2-chat-7B) | 0.24B | | Vicuna-13B-v1.3 | [yuhuili/EAGLE-Vicuna-13B-
+v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-13B-v1.3) | 0.37B | LLaMA2-
+Chat 13B | [yuhuili/EAGLE-llama2-chat-13B](https://huggingface.co/yuhuili/
+EAGLE-llama2-chat-13B) | 0.37B | | Vicuna-33B-v1.3 | [yuhuili/EAGLE-Vicuna-33B-
+v1.3](https://huggingface.co/yuhuili/EAGLE-Vicuna-33B-v1.3)| 0.56B | LLaMA2-
+Chat 70B| [yuhuili/EAGLE-llama2-chat-70B](https://huggingface.co/yuhuili/EAGLE-
+llama2-chat-70B)| 0.99B | | Mixtral-8x7B-Instruct-v0.1 | [yuhuili/EAGLE-
+mixtral-instruct-8x7B](https://huggingface.co/yuhuili/EAGLE-mixtral-instruct-
+8x7B)| 0.28B | ## Inference The inference code we provide automatically
+allocates model weights (loading a model across multiple GPUs), allowing you to
+run models that exceed the memory of a single GPU. ### With UI We have provided
+a suggested web interface, which you can use by running the following command.
 After the model is fully loaded, a URL will be output in the terminal, which
 you can enter into your browser to access. ```bash python -
 m eagle.application.webui --ea-model-path [path of EAGLE weight]\ --base-model-
 path [path of the original model]\ --model-type [vicuna or llama-2-chat] ```
 ### With Code You can use our provided "eagenerate" for speedup generation just
 like using 'generate' from Hugging Face. Here is an example. ```python from
 eagle.model.ea_model import EaModel from fastchat.model import
@@ -93,18 +94,17 @@
 ("vicuna") conv.append_message(conv.roles[0], your_message) conv.append_message
 (conv.roles[1], None) prompt = conv.get_prompt() input_ids=model.tokenizer(
 [prompt]).input_ids input_ids = torch.as_tensor(input_ids).cuda()
 output_ids=model.eagenerate(input_ids,temperature=0.5,max_new_tokens=512)
 output=model.tokenizer.decode(output_ids[0]) ``` **_Note: Vicuna and LLaMA2-
 Chat are both chat models. You need to use the correct chat template, otherwise
 it will cause abnormal output from the model and affect the performance of
-EAGLE._** ### Batch size > 1 Switch to the *bsne1* branch. ```bash git checkout
-bsne1 ``` Here is an example. Note that left padding is needed. ```python from
-model.ea_model import EaModel from fastchat.model import
-get_conversation_template model = EaModel.from_pretrained
+EAGLE._** ### Batch size > 1 Here is an example. Note that left padding is
+needed. ```python from modelbsne1.ea_model import EaModel from fastchat.model
+import get_conversation_template model = EaModel.from_pretrained
 ( base_model_path=base_model_path, ea_model_path=EAGLE_model_path,
 torch_dtype=torch.float16, low_cpu_mem_usage=True, device_map="auto" ) # left
 padding model.eval() model.tokenizer.padding_side = "left"
 model.tokenizer.pad_token = model.tokenizer.eos_token model.config.pad_token_id
 = model.config.eos_token_id sys_p = "You are a helpful, respectful and honest
 assistant. Always answer as helpfully as possible, while being safe. Your
 answers should not include any harmful, unethical, racist, sexist, toxic,
@@ -126,19 +126,20 @@
 output=model.tokenizer.batch_decode(output_ids) print(output) # vanilla auto-
 regression # output_ids, new_token, idx=model.naivegenerate
 (input_s.input_ids,input_s.attention_mask,temperature=0.0,max_new_tokens=512,top_k=15,log=True)
 ``` ## Train ### Generate Train Data You can run the following command to
 generate the training data. ```bash python -m eagle.ge_data.allocation --outdir
 [path of data] ``` ### Train the Auto-regression Head ```bash accelerate launch
 -m --mixed_precision=bf16 eagle.train.main --tmpdir [path of data]\ --cpdir
-[path of checkpoints] -- configpath [path of config file] ``` ### Inference on
-custom models If the original LLM structure differs from LLaMA and Mixtral, you
-can utilize EAGLE in two ways. #### 1. Using the generic modeling_eagle.py This
-approach directly encapsulates the native Transformers LLM. Here is an example.
-**Note: transformers version should be higher than 4.36.** ```python from
+[path of checkpoints] -- configpath [path of config file] ``` *eagle/train*
+provides examples of configuration files. ### Inference on custom models If the
+original LLM structure differs from LLaMA and Mixtral, you can utilize EAGLE in
+two ways. #### 1. Using the generic modeling_eagle.py This approach directly
+encapsulates the native Transformers LLM. Here is an example. **Note:
+transformers version should be higher than 4.36.** ```python from
 eagle.modeling_eagle import EAGLE from transformers import
 AutoModelForCausalLM,AutoTokenizer tokenizer=AutoTokenizer.from_pretrained
 (base_model_path) model=AutoModelForCausalLM.from_pretrained
 ("base_model_path",torch_dtype=torch.float16,device_map="auto",) # for bs>1,
 the padding side should be right if bs>1: tokenizer.padding_side = "left"
 tokenizer.pad_token = tokenizer.eos_token model.config.pad_token_id =
 model.config.eos_token_id text=prompt1 # text=[prompt1,prompt2] inputs =
@@ -168,30 +169,31 @@
 vanilla | 24.5 tokens/s | N/A | | gpt-fast | 55.1 tokens/s | 106.9 tokens/s | |
 EAGLE+gpt-fast | 100.2 tokens/s | 160.4 tokens/s |
                                    [demogif]
 _Inference is conducted on a single RTX3090 GPU at int4 precision using the
 LLaMA2-chat 7B model. No additional training required._ In EAGLE, using gpt-
 fast only requires three steps: setting up the environment, quantizing weights,
 and modifying the model path. ### Setup Switch to the *eaglefast* branch.
-```bash git checkout eaglefast ``` Install the Preview (Nightly) version of
-PyTorch with CUDA 12.1, do not use "pip install torch" as it installs the
-Stable version, which lacks some of the new features used by gpt-fast. _This is
-a requirement for gpt-fast, whereas other branches of eagle can use the Stable
-version of PyTorch._ ### Quantizing Weights Convert Huggingface weights to the
-format required by gpt-fast. ```bash python convert/convert_hf_checkpoint.py --
-checkpoint_dir path_of_base_model python convert/convert_hf_checkpoint_EAGLE.py
---checkpoint_dir path_of_eagle ``` Quantize weights. ```bash python -
-m model.quantize_llama --checkpoint_path path_of_base_model/model.pth python -
-m model.quantize_EAGLE --checkpoint_path path_of_eagle/model.pth ``` ###
-Modifying Path When specifying the model weights (including the base model and
-EAGLE), change "path" to "path/model_int4.g32.pth". ## ð Our Contributors A
-heartfelt thank you to all our contributors. ![Contributors](https://
-contrib.rocks/image?repo=SafeAILab/EAGLE) ## Reference For technical details
-and full experimental results, please check [the paper](https://arxiv.org/pdf/
-2401.15077.pdf). ``` @article{li2024eagle, author = {Yuhui Li and Fangyun Wei
-and Chao Zhang and Hongyang Zhang}, title = {EAGLE: Speculative Sampling
-Requires Rethinking Feature Uncertainty}, journal = {arXiv preprint arXiv:
-2401.15077}, year = {2024} } ``` ## Acknowledgements This project has been
-influenced by many excellent projects in the LLM community, such as [Medusa]
-(https://github.com/FasterDecoding/Medusa), [FastChat](https://github.com/lm-
-sys/FastChat), and others. The logo is designed by GPT-4. We also appreciate
-many valuable discussions with Tianle Cai, Hao Zhang, Ziteng Sun, and others.
+```bash git clone https://github.com/SafeAILab/EAGLE.git git checkout eaglefast
+``` Install the Preview (Nightly) version of PyTorch with CUDA 12.1, do not use
+"pip install torch" as it installs the Stable version, which lacks some of the
+new features used by gpt-fast. _This is a requirement for gpt-fast, whereas
+other branches of eagle can use the Stable version of PyTorch._ ### Quantizing
+Weights Convert Huggingface weights to the format required by gpt-fast. ```bash
+python convert/convert_hf_checkpoint.py --checkpoint_dir path_of_base_model
+python convert/convert_hf_checkpoint_EAGLE.py --checkpoint_dir path_of_eagle
+``` Quantize weights. ```bash python -m model.quantize_llama --checkpoint_path
+path_of_base_model/model.pth python -m model.quantize_EAGLE --checkpoint_path
+path_of_eagle/model.pth ``` ### Modifying Path When specifying the model
+weights (including the base model and EAGLE), change "path" to "path/
+model_int4.g32.pth". ## ð Our Contributors A heartfelt thank you to all our
+contributors. ![Contributors](https://contrib.rocks/image?repo=SafeAILab/EAGLE)
+## Reference For technical details and full experimental results, please check
+[the paper](https://arxiv.org/pdf/2401.15077.pdf). ``` @article{li2024eagle,
+author = {Yuhui Li and Fangyun Wei and Chao Zhang and Hongyang Zhang}, title =
+{EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty}, journal
+= {arXiv preprint arXiv:2401.15077}, year = {2024} } ``` ## Acknowledgements
+This project has been influenced by many excellent projects in the LLM
+community, such as [Medusa](https://github.com/FasterDecoding/Medusa),
+[FastChat](https://github.com/lm-sys/FastChat), and others. The logo is
+designed by GPT-4. We also appreciate many valuable discussions with Tianle
+Cai, Hao Zhang, Ziteng Sun, and others.
```

### Comparing `eagle-llm-1.1.0/eagle_llm.egg-info/SOURCES.txt` & `eagle-llm-1.2.0/eagle_llm.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,23 @@
 eagle/model/ea_model.py
 eagle/model/kv_cache.py
 eagle/model/modeling_llama_kv.py
 eagle/model/modeling_mixtral_kv.py
 eagle/model/utils.py
 eagle/model/utils_alpha.py
 eagle/model/utils_c.py
+eagle/modelbsne1/__init__.py
+eagle/modelbsne1/choices.py
+eagle/modelbsne1/cnets.py
+eagle/modelbsne1/configs.py
+eagle/modelbsne1/ea_model.py
+eagle/modelbsne1/kv_cache.py
+eagle/modelbsne1/modeling_llama_kv.py
+eagle/modelbsne1/utils.py
+eagle/modelbsne1/utils_c.py
 eagle/train/__init__.py
 eagle/train/main.py
 eagle_llm.egg-info/PKG-INFO
 eagle_llm.egg-info/SOURCES.txt
 eagle_llm.egg-info/dependency_links.txt
 eagle_llm.egg-info/requires.txt
 eagle_llm.egg-info/top_level.txt
```

### Comparing `eagle-llm-1.1.0/setup.py` & `eagle-llm-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eagle-llm',
-    version='1.1.0',
+    version='1.2.0',
     description='Accelerating LLMs by 3x with No Quality Loss',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author_email='yuhui.li@stu.pku.edu.cn',
     url='https://github.com/SafeAILab/EAGLE',
     packages=find_packages(),
     install_requires=[
```

