# Comparing `tmp/self-rewarding-lm-pytorch-0.2.8.tar.gz` & `tmp/self-rewarding-lm-pytorch-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self-rewarding-lm-pytorch-0.2.8.tar", last modified: Mon Feb 19 02:21:05 2024, max compression
+gzip compressed data, was "self-rewarding-lm-pytorch-0.2.9.tar", last modified: Wed Mar 27 01:04:07 2024, max compression
```

## Comparing `self-rewarding-lm-pytorch-0.2.8.tar` & `self-rewarding-lm-pytorch-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 02:21:05.685718 self-rewarding-lm-pytorch-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-19 02:21:05.685718 self-rewarding-lm-pytorch-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 02:21:05.685718 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/sampling_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34535 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/self_rewarding_lm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/spin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 02:21:05.685718 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-19 02:21:05.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-19 02:21:05.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 02:21:05.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-19 02:21:05.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-19 02:21:05.000000 self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 02:21:05.689718 self-rewarding-lm-pytorch-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-19 02:20:57.000000 self-rewarding-lm-pytorch-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:04:07.235720 self-rewarding-lm-pytorch-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-27 01:04:07.235720 self-rewarding-lm-pytorch-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:04:07.235720 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/sampling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34540 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/self_rewarding_lm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/spin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:04:07.235720 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-27 01:04:07.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-27 01:04:07.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 01:04:07.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-27 01:04:07.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-27 01:04:07.000000 self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 01:04:07.235720 self-rewarding-lm-pytorch-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-27 01:04:00.000000 self-rewarding-lm-pytorch-0.2.9/setup.py
```

### Comparing `self-rewarding-lm-pytorch-0.2.8/LICENSE` & `self-rewarding-lm-pytorch-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/PKG-INFO` & `self-rewarding-lm-pytorch-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-rewarding-lm-pytorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: Self Rewarding LM - Pytorch
 Home-page: https://github.com/lucidrains/self-rewarding-lm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,self rewarding,direct preference optimization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `self-rewarding-lm-pytorch-0.2.8/README.md` & `self-rewarding-lm-pytorch-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/__init__.py` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/dpo.py` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/dpo.py`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/mocks.py` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/mocks.py`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/sampling_utils.py` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/self_rewarding_lm_pytorch.py` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/self_rewarding_lm_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
 
         reward_prompt_str = template_fn(prompt = prompt, response = response)
         reward_prompt = self.tokenizer_encode(reward_prompt_str).to(device)
 
         reward_prompt = repeat(reward_prompt, 'n -> b n', b = self.num_evals_to_average)
 
         reward_prompt = reward_prompt.to(device)
-        self_reward_model = self_reward_model.to(device)
+        self_reward_model = self.self_reward_model.to(device)
 
         reward_responses = sample(
             self_reward_model,
             prompts = reward_prompt,
             seq_len = self.generate_reward_max_seq_len,
             temperature = self.eval_temperature,
             filter_fn = self.eval_filter_fn,
```

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch/spin.py` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch/spin.py`

 * *Files identical despite different names*

### Comparing `self-rewarding-lm-pytorch-0.2.8/self_rewarding_lm_pytorch.egg-info/PKG-INFO` & `self-rewarding-lm-pytorch-0.2.9/self_rewarding_lm_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-rewarding-lm-pytorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: Self Rewarding LM - Pytorch
 Home-page: https://github.com/lucidrains/self-rewarding-lm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,self rewarding,direct preference optimization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `self-rewarding-lm-pytorch-0.2.8/setup.py` & `self-rewarding-lm-pytorch-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'self-rewarding-lm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.8',
+  version = '0.2.9',
   license='MIT',
   description = 'Self Rewarding LM - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/self-rewarding-lm-pytorch',
   keywords = [
```

