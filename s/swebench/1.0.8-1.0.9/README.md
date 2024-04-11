# Comparing `tmp/swebench-1.0.8.tar.gz` & `tmp/swebench-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.8.tar", last modified: Tue Apr  9 17:20:07 2024, max compression
+gzip compressed data, was "swebench-1.0.9.tar", last modified: Wed Apr 10 04:33:17 2024, max compression
```

## Comparing `swebench-1.0.8.tar` & `swebench-1.0.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.814625 swebench-1.0.8/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.8/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 17:20:07.814557 swebench-1.0.8/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.8/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.804450 swebench-1.0.8/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.805310 swebench-1.0.8/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.807673 swebench-1.0.8/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.8/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.8/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.8/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.8/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.8/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-09 17:20:07.814837 swebench-1.0.8/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.8/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.808002 swebench-1.0.8/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-09 17:19:55.000000 swebench-1.0.8/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.810023 swebench-1.0.8/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.811535 swebench-1.0.8/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    19019 2024-04-09 14:18:22.000000 swebench-1.0.8/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    31165 2024-04-09 15:28:28.000000 swebench-1.0.8/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.8/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.8/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.813228 swebench-1.0.8/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.8/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.0.8/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.8/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.814125 swebench-1.0.8/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.8/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-09 17:20:07.814326 swebench-1.0.8/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-09 17:20:07.000000 swebench-1.0.8/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.731325 swebench-1.0.9/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.9/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-10 04:33:17.731245 swebench-1.0.9/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.9/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.720539 swebench-1.0.9/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.721254 swebench-1.0.9/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.723521 swebench-1.0.9/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.9/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.9/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.9/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-10 04:33:17.731522 swebench-1.0.9/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.9/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.723817 swebench-1.0.9/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-10 04:32:33.000000 swebench-1.0.9/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.726066 swebench-1.0.9/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.727885 swebench-1.0.9/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    22538 2024-04-10 04:30:31.000000 swebench-1.0.9/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    31223 2024-04-09 19:56:34.000000 swebench-1.0.9/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.9/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.9/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.729936 swebench-1.0.9/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.9/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.0.9/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.9/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.730793 swebench-1.0.9/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.730973 swebench-1.0.9/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.8/LICENSE` & `swebench-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/PKG-INFO` & `swebench-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.8
+Version: 1.0.9
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.8 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.9 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.8/README.md` & `swebench-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/llamao/distributed_attention.py` & `swebench-1.0.9/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.9/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.9/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/make_datasets/create_instance.py` & `swebench-1.0.9/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.9/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.9/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.9/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/make_datasets/utils.py` & `swebench-1.0.9/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/run_api.py` & `swebench-1.0.9/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/run_live.py` & `swebench-1.0.9/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/inference/run_llama.py` & `swebench-1.0.9/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/setup.py` & `swebench-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/__init__.py` & `swebench-1.0.9/swebench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.8/swebench/collect/build_dataset.py` & `swebench-1.0.9/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/collect/build_dataset_ft.py` & `swebench-1.0.9/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.9/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/collect/get_top_pypi.py` & `swebench-1.0.9/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/collect/print_pulls.py` & `swebench-1.0.9/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/collect/utils.py` & `swebench-1.0.9/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/harness/constants.py` & `swebench-1.0.9/swebench/harness/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,81 @@
 MAP_VERSION_TO_INSTALL_SKLEARN = {
     k: {
         "python": "3.6",
         "packages": "numpy scipy cython pytest pandas matplotlib",
         "install": "pip install -v --no-use-pep517 --no-build-isolation -e .",
         "arch_specific_packages": {
             "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
-        }
+        },
+        "pip_packages": [
+            "numpy==1.19.2",
+            "scipy==1.5.2",
+        ],
     }
     for k in ["0.20", "0.21", "0.22"]
 }
 MAP_VERSION_TO_INSTALL_SKLEARN.update(
     {
         k: {
-            "python": "3.7",
-            "packages": "numpy scipy cython pytest pandas matplotlib",
-            "install": "pip install -v --no-use-pep517 --no-build-isolation -e .",
-            "arch_specific_packages": {
-                "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
-            }
-        }
-        for k in ["0.23", "0.24"]
-    }
-)
-MAP_VERSION_TO_INSTALL_SKLEARN.update(
-    {
-        k: {
             "python": "3.9",
             "packages": "numpy scipy cython pytest pandas matplotlib joblib threadpoolctl",
             "install": "pip install -v --no-use-pep517 --no-build-isolation -e .",
             "arch_specific_packages": {
                 "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
-            }
+            },
+            "pip_packages": [
+                "numpy==1.25.2",
+                "scipy==1.11.1",
+                "joblib==1.2.0",
+                "threadpoolctl==2.2.0",
+            ]
         }
-        for k in ["1.0", "1.1", "1.2", "1.3", "1.4"]
+        for k in ["1.3", "1.4"]
     }
 )
 
 MAP_VERSION_TO_INSTALL_FLASK = {
-    "0.11-dev": {
-        "python": "3.6",
-        "packages": "pytest",
-        "pip_packages": "tox",
-        "install": "python setup.py develop",
-    },
-    "1.0": {
-        "python": "3.8",
-        "packages": "pytest",
-        "pip_packages": "tox",
-        "install": 'pip install -e ".[dev]"',
-    },
-    "1.1": {
-        "python": "3.9",
-        "packages": "pytest",
-        "pip_packages": "tox",
-        "install": 'pip install -e ".[dev]"',
-    },
     "2.0": {
         "python": "3.9",
         "packages": "requirements.txt",
         "install": "pip install -e .",
-        "pip_packages": "Werkzeug==2.2.2",
+        "pip_packages": [
+            "Werkzeug==2.3.7",
+            "Jinja2==3.0.1",
+            "itsdangerous==2.1.2",
+            "click==8.0.1",
+            "MarkupSafe==2.1.3",
+        ],
     },
     "2.1": {
         "python": "3.10",
         "packages": "requirements.txt",
         "install": "pip install -e .",
-        "pip_packages": "Werkzeug==2.2.2",
+        "pip_packages": [
+            "click==8.1.3",
+            "itsdangerous==2.1.2",
+            "Jinja2==3.1.2",
+            "MarkupSafe==2.1.1",
+            "Werkzeug==2.3.7",
+        ],
     },
 }
 MAP_VERSION_TO_INSTALL_FLASK.update(
     {
         k: {
-            "python": "3.6",
-            "packages": "pytest",
-            "pip_packages": "tox",
-            "install": "pip install -e .",
-        }
-        for k in ["0.11", "0.12", "0.12-dev", "0.13-dev"]
-    }
-)
-MAP_VERSION_TO_INSTALL_FLASK.update(
-    {
-        k: {
             "python": "3.11",
             "packages": "requirements.txt",
             "install": "pip install -e .",
-            "pip_packages": "Werkzeug==2.2.2"
+            "pip_packages": [
+                "click==8.1.3",
+                "itsdangerous==2.1.2",
+                "Jinja2==3.1.2",
+                "MarkupSafe==2.1.1",
+                "Werkzeug==2.3.7",
+            ],
         }
         for k in ["2.2", "2.3"]
     }
 )
 
 MAP_VERSION_TO_INSTALL_DJANGO = {
     k: {
@@ -155,51 +141,137 @@
     for k in
         ["0.7", "0.8", "0.9", "0.11", "0.13", "0.14", "1.1", "1.2", "2.0", "2.2"] + \
         ["2.3", "2.4", "2.5", "2.7", "2.8", "2.9", "2.10", "2.11", "2.12", "2.17"] + \
         ["2.18", "2.19", "2.22", "2.26", "2.25", "2.27", "3.0"]
 }
 
 MAP_VERSION_TO_INSTALL_SEABORN = {
-    k: {"python": "3.9", "install": "pip install -e .", "pip_packages": "pytest"}
-    for k in ["0.3", "0.4", "0.5", "0.6", "0.7", "0.8", "0.9", "0.11"]
+    k: {
+        "python": "3.9",
+        "install": "pip install -e .",
+        "pip_packages": [
+            "contourpy==1.1.0",
+            "cycler==0.11.0",
+            "fonttools==4.42.1",
+            "importlib-resources==6.0.1",
+            "kiwisolver==1.4.5",
+            "matplotlib==3.7.2",
+            "numpy==1.25.2",
+            "packaging==23.1",
+            "pandas==2.1.0",
+            "pillow==10.0.0",
+            "pyparsing==3.0.9",
+            "pytest",
+            "python-dateutil==2.8.2",
+            "pytz==2023.3.post1",
+            "scipy==1.11.2",
+            "six==1.16.0",
+            "tzdata==2023.1",
+            "zipp==3.16.2",
+        ],
+    }
+    for k in ["0.11"]
 }
 MAP_VERSION_TO_INSTALL_SEABORN.update(
-    {k: {"python": "3.9", "install": "pip install -e .[dev]"} for k in ["0.12", "0.13"]}
+    {
+        k: {
+            "python": "3.9",
+            "install": "pip install -e .[dev]",
+            "pip_packages": [
+                "contourpy==1.1.0",
+                "cycler==0.11.0",
+                "fonttools==4.42.1",
+                "importlib-resources==6.0.1",
+                "kiwisolver==1.4.5",
+                "matplotlib==3.7.2",
+                "numpy==1.25.2",
+                "packaging==23.1",
+                "pandas==2.1.0",
+                "pillow==10.0.0",
+                "pyparsing==3.0.9",
+                "python-dateutil==2.8.2",
+                "pytz==2023.3.post1",
+                "scipy==1.11.2",
+                "six==1.16.0",
+                "tzdata==2023.1",
+                "zipp==3.16.2",
+            ],
+        } for k in ["0.12", "0.13"]
+    }
 )
 
 MAP_VERSION_TO_INSTALL_PYTEST = {
-    k: {"python": "3.9", "install": "pip install -e ."}
-    for k in ["3.10", "6.0", "6.2", "6.3", "8.0"]
-    + [
-        str(round(0.1 * x, 1))
-        for interval in [(30, 47), (50, 55), (70, 75)]
-        for x in range(interval[0], interval[1], 1)
+    k: {
+        "python": "3.9",
+        "install": "pip install -e ."
+    } for k in [
+        '4.4','4.5','4.6','5.0','5.1','5.2','5.3','5.4',
+        '6.0','6.2','6.3','7.0','7.1','7.2','7.4','8.0'
     ]
 }
+MAP_VERSION_TO_INSTALL_PYTEST["4.4"]["pip_packages"] = [
+    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0"
+    "pluggy==0.13.1", "py==1.11.0", "setuptools==68.0.0", "six==1.16.0",]
+MAP_VERSION_TO_INSTALL_PYTEST["4.5"]["pip_packages"] = [
+    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0"
+    "pluggy==0.11.0", "py==1.11.0", "setuptools==68.0.0", "six==1.16.0", "wcwidth==0.2.6"]
+MAP_VERSION_TO_INSTALL_PYTEST["4.6"]["pip_packages"] = [
+    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0",
+    "packaging==23.1", "pluggy==0.13.1", "py==1.11.0", "six==1.16.0", "wcwidth==0.2.6"]
+for k in ["5.0", "5.1", "5.2"]:
+    MAP_VERSION_TO_INSTALL_PYTEST[k]["pip_packages"] = [
+        "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0",
+        "packaging==23.1", "pluggy==0.13.1", "py==1.11.0", "wcwidth==0.2.6"]
+MAP_VERSION_TO_INSTALL_PYTEST["5.3"]["pip_packages"] = [
+    "attrs==23.1.0", "more-itertools==10.1.0", "packaging==23.1",
+    "pluggy==0.13.1", "py==1.11.0", "wcwidth==0.2.6"]
+MAP_VERSION_TO_INSTALL_PYTEST["5.4"]["pip_packages"] = [
+    "py==1.11.0", "packaging==23.1", "attrs==23.1.0",
+    "more-itertools==10.1.0", "pluggy==0.13.1"]
+MAP_VERSION_TO_INSTALL_PYTEST["6.0"]["pip_packages"] = [
+    "attrs==23.1.0", "iniconfig==2.0.0", "more-itertools==10.1.0",
+    "packaging==23.1", "pluggy==0.13.1", "py==1.11.0", "toml==0.10.2"]
+for k in ["6.2", "6.3"]:
+    MAP_VERSION_TO_INSTALL_PYTEST[k]["pip_packages"] = [
+        "attrs==23.1.0", "iniconfig==2.0.0", "packaging==23.1",
+        "pluggy==0.13.1", "py==1.11.0", "toml==0.10.2"]
+MAP_VERSION_TO_INSTALL_PYTEST["7.0"]["pip_packages"] = [
+    "attrs==23.1.0", "iniconfig==2.0.0", "packaging==23.1",
+    "pluggy==0.13.1", "py==1.11.0"]
+for k in ["7.1", "7.2"]:
+    MAP_VERSION_TO_INSTALL_PYTEST[k]["pip_packages"] = [
+        "attrs==23.1.0", "iniconfig==2.0.0", "packaging==23.1",
+        "pluggy==0.13.1", "py==1.11.0", "tomli==2.0.1"]
+MAP_VERSION_TO_INSTALL_PYTEST["7.4"]["pip_packages"] = [
+    "iniconfig==2.0.0", "packaging==23.1", "pluggy==1.3.0",
+    "exceptiongroup==1.1.3", "tomli==2.0.1"]
+MAP_VERSION_TO_INSTALL_PYTEST["8.0"]["pip_packages"] = [
+    "iniconfig==2.0.0", "packaging==23.1", "pluggy==1.3.0",
+    "exceptiongroup==1.1.3", "tomli==2.0.1"]
 
 MAP_VERSION_TO_INSTALL_MATPLOTLIB = {
     k: {
         "python": "3.11",
         "packages": "environment.yml",
         "install": "python -m pip install -e .",
-        "pip_packages": " ".join([
+        "pip_packages": [
             "contourpy==1.1.0",
             "cycler==0.11.0",
             "fonttools==4.42.1",
             "kiwisolver==1.4.5",
             "numpy==1.25.2",
             "packaging==23.1",
             "pillow==10.0.0",
             "pyparsing==3.0.9",
             "python-dateutil==2.8.2",
             "six==1.16.0",
             "setuptools==68.1.2",
             "setuptools-scm==7.1.0",
             "typing-extensions==4.7.1",
-        ]),
+        ],
         "arch_specific_packages": {
             "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
         }
     }
     for k in ["3.5", "3.6", "3.7"]
 }
 MAP_VERSION_TO_INSTALL_MATPLOTLIB.update(
@@ -240,15 +312,15 @@
         for k in ["2.0", "2.1", "2.2", "1.0", "1.1", "1.2", "1.3", "1.4", "1.5"]
     }
 )
 
 MAP_VERSION_TO_INSTALL_SPHINX = {
     k: {
         "python": "3.9",
-        "pip_packages": "tox",
+        "pip_packages": ["tox"],
         "install": "pip install -e .[test]",
         "pre_install": ["sed -i 's/pytest/pytest -rA/' tox.ini"],
         "arch_specific_packages": {
             "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
             "x86_64": "gxx_linux-64 gcc_linux-64 make",
         }
     } for k in
@@ -289,168 +361,164 @@
         MAP_VERSION_TO_INSTALL_SPHINX[k]["pre_install"].extend([
             "sed -i 's/sphinxcontrib-htmlhelp/sphinxcontrib-htmlhelp<=2.0.4/' setup.py",
             "sed -i 's/sphinxcontrib-serializinghtml/sphinxcontrib-serializinghtml<=1.1.9/' setup.py",
         ])
 
 
 MAP_VERSION_TO_INSTALL_ASTROPY = {
-    k: {"python": "3.9", "install": "pip install -e .[test]"}
+    k: {
+        "python": "3.9",
+        "install": "pip install -e .[test]",
+        "pip_packages": [
+            "attrs==23.1.0", "exceptiongroup==1.1.3", "execnet==2.0.2", "hypothesis==6.82.6",
+            "iniconfig==2.0.0", "numpy==1.25.2", "packaging==23.1", "pluggy==1.3.0",
+            "psutil==5.9.5", "pyerfa==2.0.0.3", "pytest-arraydiff==0.5.0", "pytest-astropy-header==0.2.2",
+            "pytest-astropy==0.10.0", "pytest-cov==4.1.0", "pytest-doctestplus==1.0.0", "pytest-filter-subpackage==0.1.2",
+            "pytest-mock==3.11.1", "pytest-openfiles==0.5.0", "pytest-remotedata==0.4.0", "pytest-xdist==3.3.1",
+            "pytest==7.4.0", "PyYAML==6.0.1", "setuptools==68.0.0", "sortedcontainers==2.4.0", "tomli==2.0.1",
+        ],
+    }
     for k in
         ["0.1", "0.2", "0.3", "0.4", "1.1", "1.2", "1.3", "3.0", "3.1", "3.2"] + \
         ["4.1", "4.2", "4.3", "5.0", "5.1", "5.2"]
 }
 
 MAP_VERSION_TO_INSTALL_SYMPY = {
     k: {
         "python": "3.9",
         "packages": "mpmath flake8",
-        "pip_packages": "flake8-comprehensions",
+        "pip_packages": ["mpmath==1.3.0", "flake8-comprehensions"],
         "install": "pip install -e .",
     }
     for k in
         ["0.7", "1.0", "1.1", "1.10", "1.11", "1.12", "1.2", "1.4", "1.5", "1.6"] + \
         ["1.7", "1.8", "1.9"]
 }
 MAP_VERSION_TO_INSTALL_SYMPY.update(
     {
         k: {
             "python": "3.9",
             "packages": "requirements.txt",
             "install": "pip install -e .",
+            "pip_packages": ["mpmath==1.3.0"],
         }
         for k in ["1.13"]
     }
 )
 
 MAP_VERSION_TO_INSTALL_PYLINT = {
     k: {"python": "3.9", "packages": "requirements.txt", "install": "pip install -e ."}
     for k in ["2.10", "2.11", "2.13", "2.14", "2.15", "2.16", "2.17", "2.8", "2.9", "3.0"]
 }
 MAP_VERSION_TO_INSTALL_PYLINT.update({
-    k: {**MAP_VERSION_TO_INSTALL_PYLINT[k], "pip_packages": " ".join([
+    k: {**MAP_VERSION_TO_INSTALL_PYLINT[k], "pip_packages": [
         "astroid==3.0.0a6"
-    ])} for k in ['3.0']})
+    ]} for k in ['3.0']})
 
 MAP_VERSION_TO_INSTALL_XARRAY = {
     k: {
         "python": "3.10",
         "packages": "environment.yml",
         "install": "pip install -e .",
-        "pip_packages": "pytest",
+        "pip_packages": [
+            "numpy==1.25.2",
+            "packaging==23.1",
+            "pandas==1.5.3",
+            "pytest==7.4.0",
+            "python-dateutil==2.8.2",
+            "pytz==2023.3",
+            "six==1.16.0",
+        ],
         "no_use_env": True,
     }
     for k in ["0.12", "0.18", "0.19", "0.20", "2022.03", "2022.06", "2022.09"]
 }
 
-MAP_VERSION_TO_INSTALL_TRANSFORMERS = {
-    k: {
-        "python": "3.10",
-        "install": "pip install -e .",
-        "pip_packages": "pytest torch tensorflow flax",
-    }
-    for k in [
-        '4.28', '4.29', '4.30', '4.31', '4.32', '4.16', '4.14', '4.15', '4.17',
-        '4.19', '4.18', '4.22', '4.20', '4.11', '4.13', '4.12', '4.6', '4.7',
-        '4.9', '4.8', '4.10', '3.1', '3.2', '3.4', '3.3', '4.0', '3.5', '4.1',
-        '2.5', '2.8', '2.9', '2.11', '2.10', '3.0', '4.3', '4.2', '4.5', '4.4',
-        '4.21', '4.23', '4.24', '4.26', '4.25', '4.27'
-    ]
-}
-
 MAP_VERSION_TO_INSTALL_SQLFLUFF = {
     k: {
         "python": "3.9",
         "packages": "requirements.txt",
         "install": "pip install -e .",
     }
     for k in [
-        '0.10', '0.11', '0.12', '0.13', '0.4', '0.5', '0.6', '0.8', '0.9',
-        '1.0', '1.1', '1.2', '1.3', '1.4', '2.0', '2.1', '2.2'
-    ]
-}
-
-MAP_VERSION_TO_INSTALL_DBT_CORE = {
-    k: {
-        "python": "3.9",
-        "packages": "requirements.txt",
-        "install": "pip install -e .",
-    }
-    for k in [
-        '0.13', '0.14', '0.15', '0.16', '0.17', '0.18', '0.19', '0.20',
-        '0.21', '1.0', '1.1', '1.2', '1.3', '1.4', '1.5', '1.6', '1.7'
+        '0.10', '0.11', '0.12', '0.13', '0.4', '0.6', '0.8', '0.9',
+        '1.1', '1.2', '1.3', '1.4', '2.0', '2.1', '2.2'
     ]
 }
 
 MAP_VERSION_TO_INSTALL_PYVISTA = {
     k: {
         "python": "3.9",
         "install": "pip install -e .",
-        "pip_packages": "pytest",
+        "pip_packages": ["pytest"],
     }
     for k in ['0.20', '0.21', '0.22', '0.23']
 }
 MAP_VERSION_TO_INSTALL_PYVISTA.update({
     k: {
         "python": "3.9",
         "packages": "requirements.txt",
         "install": "pip install -e .",
-        "pip_packages": "pytest",
+        "pip_packages": ["pytest"],
     }
     for k in [
         '0.24', '0.25', '0.26', '0.27', '0.28', '0.29', '0.30', '0.31',
         '0.32', '0.33', '0.34', '0.35', '0.36', '0.37', '0.38', '0.39',
         '0.40', '0.41', '0.42', '0.43'
     ]
 })
 
 MAP_VERSION_TO_INSTALL_ASTROID = {
     k: {
         "python": "3.9",
         "install": "pip install -e .",
-        "pip_packages": "pytest",
+        "pip_packages": ["pytest"],
     }
-    for k in [
-        '2.10', '2.12', '2.13', '2.14', '2.15', '2.16', '2.5', '2.6',
-        '2.7', '2.8', '2.9', '3.0'
-    ]
+    for k in ['2.10', '2.12', '2.13', '2.14', '2.15', '2.5', '2.6', '2.7', '2.9', '3.0']
 }
+for k in ["2.5", "2.6"]:
+    MAP_VERSION_TO_INSTALL_ASTROID[k]["pip_packages"] = [
+        "lazy_object_proxy==1.9.0", "wrapt==1.12.1"]
+for k in ["2.9", "2.10"]:
+    MAP_VERSION_TO_INSTALL_ASTROID[k]["pip_packages"] = [
+        "lazy_object_proxy==1.9.0", "wrapt==1.13.3",
+        "typing-extensions==4.8.0", "setuptools==68.0.0"]
+for k in ["2.12", "2.13", "2.14", "2.15"]:
+    MAP_VERSION_TO_INSTALL_ASTROID[k]["pip_packages"] = [
+        "lazy_object_proxy==1.9.0", "wrapt==1.15.0", "typing-extensions==4.8.0"]
+MAP_VERSION_TO_INSTALL_ASTROID["2.7"]["pip_packages"] = [
+    "lazy_object_proxy==1.9.0", "wrapt==1.12.1", "typing-extensions==4.8.0"]
+MAP_VERSION_TO_INSTALL_ASTROID["3.0"]["pip_packages"] = ["typing-extensions==4.8.0"]
+
 
 MAP_VERSION_TO_INSTALL_MARSHMALLOW = {
     k: {
         "python": "3.9",
         "install": "pip install -e '.[dev]'",
     }
-    for k in [
-        '2.18', '2.19', '2.20', '3.0', '3.1', '3.10', '3.11', '3.12',
-        '3.13', '3.15', '3.16', '3.19', '3.2', '3.4', '3.8', '3.9'
-    ]
+    for k in ['2.18', '2.19', '2.20', '3.0', '3.12', '3.19', '3.9']
 }
 
 MAP_VERSION_TO_INSTALL_PVLIB = {
     k: {
         "python": "3.9",
         "install": "pip install -e .[all]",
         "packages": "pandas scipy",
-        "pip_packages": "jupyter ipython matplotlib pytest flake8"
+        "pip_packages": ["jupyter", "ipython", "matplotlib", "pytest", "flake8"]
     }
-    for k in [
-        '0.1', '0.2', '0.3', '0.4', '0.5', '0.6', '0.7', '0.8', '0.9'
-    ]
+    for k in ['0.5', '0.6', '0.7', '0.8', '0.9']
 }
 
 MAP_VERSION_TO_INSTALL_PYDICOM = {
     k: {
         "python": "3.6",
         "install": "pip install -e .",
         "packages": "numpy"
     }
-    for k in [
-        '1.0', '1.1', '1.2', '1.3', '1.4',
-        '2.0', '2.1', '2.2', '2.3', '2.4', '3.0'
-    ]
+    for k in ['1.2', '1.3', '1.4', '2.0', '2.1', '2.2', '2.3']
 }
 MAP_VERSION_TO_INSTALL_PYDICOM.update({
     k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.8"}
     for k in ['1.4', '2.0']})
 MAP_VERSION_TO_INSTALL_PYDICOM.update({
     k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.9"}
     for k in ['2.1', '2.2']})
@@ -462,17 +530,15 @@
     for k in ['2.4', '3.0']})
 
 MAP_VERSION_TO_INSTALL_HUMANEVAL= {k: { "python": "3.9" } for k in ['1.0']}
 
 # Constants - Task Instance Instllation Environment
 MAP_VERSION_TO_INSTALL = {
     "astropy/astropy": MAP_VERSION_TO_INSTALL_ASTROPY,
-    "dbt-labs/dbt-core": MAP_VERSION_TO_INSTALL_DBT_CORE,
     "django/django": MAP_VERSION_TO_INSTALL_DJANGO,
-    "huggingface/transformers": MAP_VERSION_TO_INSTALL_TRANSFORMERS,
     "matplotlib/matplotlib": MAP_VERSION_TO_INSTALL_MATPLOTLIB,
     "marshmallow-code/marshmallow": MAP_VERSION_TO_INSTALL_MARSHMALLOW,
     "mwaskom/seaborn": MAP_VERSION_TO_INSTALL_SEABORN,
     "pallets/flask": MAP_VERSION_TO_INSTALL_FLASK,
     "psf/requests": MAP_VERSION_TO_INSTALL_REQUESTS,
     "pvlib/pvlib-python": MAP_VERSION_TO_INSTALL_PVLIB,
     "pydata/xarray": MAP_VERSION_TO_INSTALL_XARRAY,
```

### Comparing `swebench-1.0.8/swebench/harness/context_manager.py` & `swebench-1.0.9/swebench/harness/context_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,16 @@
                 if arch_specific_packages:
                     cmd = f". {path_activate} {env_name} && conda install {arch_specific_packages} -y"
                     self.log.write(f"Installing arch-specific packages for {env_name}; Command: {cmd}")
                     self.exec(cmd, shell=True)
 
                 # Install additional packages if specified
                 if "pip_packages" in install:
-                    cmd = f". {path_activate} {env_name} && pip install {install['pip_packages']}"
+                    pip_packages = " ".join(install["pip_packages"])
+                    cmd = f". {path_activate} {env_name} && pip install {pip_packages}"
                     self.log.write(f"Installing pip packages for {env_name}; Command: {cmd}")
                     self.exec(cmd, shell=True)
 
         return self
 
     def get_distributed_tasks(self) -> list:
         """
```

### Comparing `swebench-1.0.8/swebench/harness/engine_evaluation.py` & `swebench-1.0.9/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/harness/engine_validation.py` & `swebench-1.0.9/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/harness/run_evaluation.py` & `swebench-1.0.9/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/harness/utils.py` & `swebench-1.0.9/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/constants.py` & `swebench-1.0.9/swebench/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/conversion.py` & `swebench-1.0.9/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/getters.py` & `swebench-1.0.9/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/log_parsers.py` & `swebench-1.0.9/swebench/metrics/log_parsers.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/metrics.py` & `swebench-1.0.9/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/monitor.py` & `swebench-1.0.9/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/metrics/report.py` & `swebench-1.0.9/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/versioning/constants.py` & `swebench-1.0.9/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/versioning/get_versions.py` & `swebench-1.0.9/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench/versioning/utils.py` & `swebench-1.0.9/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.8/swebench.egg-info/PKG-INFO` & `swebench-1.0.9/swebench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.8
+Version: 1.0.9
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.8 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.9 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.8/swebench.egg-info/SOURCES.txt` & `swebench-1.0.9/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

