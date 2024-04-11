# Comparing `tmp/ms2query-1.3.0.tar.gz` & `tmp/ms2query-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms2query-1.3.0.tar", last modified: Fri Jan 19 16:57:50 2024, max compression
+gzip compressed data, was "dist/ms2query-1.4.0.tar", last modified: Thu Apr 11 15:35:31 2024, max compression
```

## Comparing `ms2query-1.3.0.tar` & `ms2query-1.4.0.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:50.000000 ms2query-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-01-19 16:57:50.000000 ms2query-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23066 2024-01-19 16:57:38.000000 ms2query-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:50.000000 ms2query-1.3.0/ms2query/
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:50.000000 ms2query-1.3.0/ms2query/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21655 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/benchmarking/collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/benchmarking/k_fold_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/benchmarking/visualize_mass_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/clean_and_filter_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:50.000000 ms2query-1.3.0/ms2query/create_new_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/add_classifire_classifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/create_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/train_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/create_new_library/train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/ms2library.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/old_query_from_sqlite_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/query_from_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/results_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-01-19 16:57:38.000000 ms2query-1.3.0/ms2query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:50.000000 ms2query-1.3.0/ms2query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-01-19 16:57:49.000000 ms2query-1.3.0/ms2query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-19 16:57:50.000000 ms2query-1.3.0/ms2query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 16:57:49.000000 ms2query-1.3.0/ms2query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-19 16:57:49.000000 ms2query-1.3.0/ms2query.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 16:57:49.000000 ms2query-1.3.0/ms2query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-19 16:57:49.000000 ms2query-1.3.0/ms2query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-19 16:57:49.000000 ms2query-1.3.0/ms2query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-19 16:57:50.000000 ms2query-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-01-19 16:57:38.000000 ms2query-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:50.000000 ms2query-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 16:57:38.000000 ms2query-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-01-19 16:57:38.000000 ms2query-1.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-19 16:57:38.000000 ms2query-1.3.0/tests/test_add_classifier_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-01-19 16:57:38.000000 ms2query-1.3.0/tests/test_calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-01-19 16:57:38.000000 ms2query-1.3.0/tests/test_clean_and_filter_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-01-19 16:57:38.000000 ms2query-1.3.0/tests/test_collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_ms2library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_results_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_train_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-01-19 16:57:39.000000 ms2query-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:31.000000 ms2query-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-04-11 15:35:31.000000 ms2query-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23066 2024-04-11 15:35:21.000000 ms2query-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query/
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21655 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/benchmarking/collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/benchmarking/k_fold_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/benchmarking/visualize_mass_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/clean_and_filter_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query/create_new_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/add_classifire_classifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/create_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/train_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/create_new_library/train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/old_query_from_sqlite_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/query_from_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-11 15:35:21.000000 ms2query-1.4.0/ms2query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 15:35:31.000000 ms2query-1.4.0/ms2query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-11 15:35:31.000000 ms2query-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-11 15:35:22.000000 ms2query-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:31.000000 ms2query-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_add_classifier_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_clean_and_filter_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_results_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_train_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-11 15:35:22.000000 ms2query-1.4.0/tests/test_utils.py
```

### Comparing `ms2query-1.3.0/PKG-INFO` & `ms2query-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.3.0
+Version: 1.4.0
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-1.3.0/README.md` & `ms2query-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/__init__.py` & `ms2query-1.4.0/ms2query/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/benchmarking/collect_test_data_results.py` & `ms2query-1.4.0/ms2query/benchmarking/collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py` & `ms2query-1.4.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/benchmarking/k_fold_cross_validation.py` & `ms2query-1.4.0/ms2query/benchmarking/k_fold_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/benchmarking/visualize_mass_distribution.py` & `ms2query-1.4.0/ms2query/benchmarking/visualize_mass_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py` & `ms2query-1.4.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/clean_and_filter_spectra.py` & `ms2query-1.4.0/ms2query/clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/add_classifire_classifications.py` & `ms2query-1.4.0/ms2query/create_new_library/add_classifire_classifications.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/calculate_tanimoto_scores.py` & `ms2query-1.4.0/ms2query/create_new_library/calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/create_sqlite_database.py` & `ms2query-1.4.0/ms2query/create_new_library/create_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/library_files_creator.py` & `ms2query-1.4.0/ms2query/create_new_library/library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/split_data_for_training.py` & `ms2query-1.4.0/ms2query/create_new_library/split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/train_models.py` & `ms2query-1.4.0/ms2query/create_new_library/train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/create_new_library/train_ms2query_model.py` & `ms2query-1.4.0/ms2query/create_new_library/train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/ms2library.py` & `ms2query-1.4.0/ms2query/ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/old_query_from_sqlite_functions.py` & `ms2query-1.4.0/ms2query/old_query_from_sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/query_from_sqlite_database.py` & `ms2query-1.4.0/ms2query/query_from_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/results_table.py` & `ms2query-1.4.0/ms2query/results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/run_ms2query.py` & `ms2query-1.4.0/ms2query/run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query/utils.py` & `ms2query-1.4.0/ms2query/utils.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/ms2query.egg-info/PKG-INFO` & `ms2query-1.4.0/ms2query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.3.0
+Version: 1.4.0
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-1.3.0/ms2query.egg-info/SOURCES.txt` & `ms2query-1.4.0/ms2query.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,9 @@
 tests/test_library_files_creator.py
 tests/test_ms2library.py
 tests/test_results_table.py
 tests/test_run_ms2query.py
 tests/test_split_data_for_training.py
 tests/test_sqlite.py
 tests/test_train_models.py
-tests/test_train_ms2deepscore.py
 tests/test_train_ms2query_model.py
 tests/test_utils.py
```

### Comparing `ms2query-1.3.0/setup.py` & `ms2query-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     install_requires=[
         "matchms>=0.24.0",
         "numpy",
         "spec2vec>=0.6.0",
         "h5py",
         "pyarrow",
         "scikit-learn",
-        "ms2deepscore<=0.4.0",
+        "ms2deepscore==0.5.0",
         "gensim>=4.0.0",
         "pandas",
         "tqdm",
         "matplotlib",
         "skl2onnx",
         "onnxruntime<1.16", # 1.16 breaks the code due to the issue https://github.com/iomega/ms2query/issues/208
     ],
```

### Comparing `ms2query-1.3.0/tests/conftest.py` & `ms2query-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_add_classifier_annotations.py` & `ms2query-1.4.0/tests/test_add_classifier_annotations.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_calculate_tanimoto_scores.py` & `ms2query-1.4.0/tests/test_calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_clean_and_filter_spectra.py` & `ms2query-1.4.0/tests/test_clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_collect_test_data_results.py` & `ms2query-1.4.0/tests/test_collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_library_files_creator.py` & `ms2query-1.4.0/tests/test_library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_ms2library.py` & `ms2query-1.4.0/tests/test_ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_results_table.py` & `ms2query-1.4.0/tests/test_results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_run_ms2query.py` & `ms2query-1.4.0/tests/test_run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_split_data_for_training.py` & `ms2query-1.4.0/tests/test_split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_sqlite.py` & `ms2query-1.4.0/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_train_models.py` & `ms2query-1.4.0/tests/test_train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_train_ms2query_model.py` & `ms2query-1.4.0/tests/test_train_ms2query_model.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.3.0/tests/test_utils.py` & `ms2query-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

