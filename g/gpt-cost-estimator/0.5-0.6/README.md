# Comparing `tmp/gpt_cost_estimator-0.5.tar.gz` & `tmp/gpt_cost_estimator-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_cost_estimator-0.5.tar", last modified: Thu Feb 15 10:53:49 2024, max compression
+gzip compressed data, was "gpt_cost_estimator-0.6.tar", last modified: Thu Apr 11 14:03:58 2024, max compression
```

## Comparing `gpt_cost_estimator-0.5.tar` & `gpt_cost_estimator-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 10:53:49.100440 gpt_cost_estimator-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-15 10:53:38.000000 gpt_cost_estimator-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-15 10:53:49.100440 gpt_cost_estimator-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-15 10:53:38.000000 gpt_cost_estimator-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 10:53:49.096440 gpt_cost_estimator-0.5/gpt_cost_estimator/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-15 10:53:38.000000 gpt_cost_estimator-0.5/gpt_cost_estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-02-15 10:53:38.000000 gpt_cost_estimator-0.5/gpt_cost_estimator/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-15 10:53:38.000000 gpt_cost_estimator-0.5/gpt_cost_estimator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 10:53:49.100440 gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-15 10:53:49.000000 gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-15 10:53:49.000000 gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 10:53:49.000000 gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-15 10:53:49.000000 gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-15 10:53:49.000000 gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 10:53:49.100440 gpt_cost_estimator-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-15 10:53:38.000000 gpt_cost_estimator-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:03:58.241536 gpt_cost_estimator-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 14:03:54.000000 gpt_cost_estimator-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-11 14:03:58.241536 gpt_cost_estimator-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-11 14:03:54.000000 gpt_cost_estimator-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:03:58.241536 gpt_cost_estimator-0.6/gpt_cost_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 14:03:54.000000 gpt_cost_estimator-0.6/gpt_cost_estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-11 14:03:54.000000 gpt_cost_estimator-0.6/gpt_cost_estimator/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-11 14:03:54.000000 gpt_cost_estimator-0.6/gpt_cost_estimator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:03:58.241536 gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-11 14:03:58.000000 gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 14:03:58.000000 gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:03:58.000000 gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 14:03:58.000000 gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 14:03:58.000000 gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:03:58.241536 gpt_cost_estimator-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-11 14:03:54.000000 gpt_cost_estimator-0.6/setup.py
```

### Comparing `gpt_cost_estimator-0.5/LICENSE` & `gpt_cost_estimator-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_cost_estimator-0.5/PKG-INFO` & `gpt_cost_estimator-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_cost_estimator
-Version: 0.5
+Version: 0.6
 Summary: A cost estimator for OpenAI API calls in tqdm loops.
 Home-page: https://github.com/michaelachmann/gpt-cost-estimator/
 Author: Michael Achmann
 Author-email: michael.achmann@informatik.uni-regensburg.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tiktoken
```

### Comparing `gpt_cost_estimator-0.5/README.md` & `gpt_cost_estimator-0.6/README.md`

 * *Files identical despite different names*

### Comparing `gpt_cost_estimator-0.5/gpt_cost_estimator/estimator.py` & `gpt_cost_estimator-0.6/gpt_cost_estimator/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     # Source: https://openai.com/pricing
     # Prices in $ per 1000 tokens
     # Last updated: 2024-01-26
     PRICES = {
         "gpt-4-0613": {"input": 0.03, "output": 0.06},
         "gpt-3.5-turbo-0613": {"input": 0.0015, "output": 0.002},
         "gpt-4-0125-preview": {"input": 0.01, "output": 0.03},
+        "gpt-4-turbo-preview": {"input": 0.01, "output": 0.03},
         "gpt-4-1106-preview": {"input": 0.01, "output": 0.03},
         "gpt-4-1106-vision-preview": {"input": 0.01, "output": 0.03},
+        "gpt-4-turbo-2024-04-09": {"input": 0.01, "output": 0.03},
+        "gpt-4-turbo": {"input": 0.01, "output": 0.03},
         "gpt-4": {"input": 0.03, "output": 0.06},
         "gpt-4-32k": {"input": 0.06, "output": 0.12},
         "gpt-3.5-turbo-0125": {"input": 0.0005, "output": 0.0015},
         "gpt-3.5-turbo-1106": {"input": 0.001, "output": 0.002},
         "gpt-3.5-turbo-instruct": {"input": 0.0015, "output": 0.002},
         "gpt-3.5-turbo-16k-0613": {"input": 0.003, "output": 0.004},
         "whisper-1": {"input": 0.006, "output": 0.006},
```

### Comparing `gpt_cost_estimator-0.5/gpt_cost_estimator/utils.py` & `gpt_cost_estimator-0.6/gpt_cost_estimator/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_cost_estimator-0.5/gpt_cost_estimator.egg-info/PKG-INFO` & `gpt_cost_estimator-0.6/gpt_cost_estimator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_cost_estimator
-Version: 0.5
+Version: 0.6
 Summary: A cost estimator for OpenAI API calls in tqdm loops.
 Home-page: https://github.com/michaelachmann/gpt-cost-estimator/
 Author: Michael Achmann
 Author-email: michael.achmann@informatik.uni-regensburg.de
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tiktoken
```

### Comparing `gpt_cost_estimator-0.5/setup.py` & `gpt_cost_estimator-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gpt_cost_estimator",
-    version="0.5",
+    version="0.6",
     packages=find_packages(),
     install_requires=[
         "tiktoken",
         "openai",
         "tqdm",
         "lorem_text"
     ],
```

