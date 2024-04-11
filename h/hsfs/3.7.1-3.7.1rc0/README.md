# Comparing `tmp/hsfs-3.7.1.tar.gz` & `tmp/hsfs-3.7.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.7.1.tar", last modified: Thu Apr 11 18:10:02 2024, max compression
+gzip compressed data, was "hsfs-3.7.1rc0.tar", last modified: Thu Mar 28 13:36:25 2024, max compression
```

## Comparing `hsfs-3.7.1.tar` & `hsfs-3.7.1rc0.tar`

### file list

```diff
@@ -1,135 +1,132 @@
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.174503 hsfs-3.7.1/
--rw-r--r--   0     1006     1006       40 2024-01-11 15:40:27.000000 hsfs-3.7.1/MANIFEST.in
--rw-r--r--   0     1006     1006     8378 2024-04-11 18:10:02.170503 hsfs-3.7.1/PKG-INFO
--rw-r--r--   0     1006     1006     5951 2024-04-11 18:10:01.000000 hsfs-3.7.1/README.md
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.154504 hsfs-3.7.1/hsfs/
--rw-r--r--   0     1006     1006     1421 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.158504 hsfs-3.7.1/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1401 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     9570 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/client/base.py
--rw-r--r--   0     1006     1006     3028 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    11825 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/client/external.py
--rw-r--r--   0     1006     1006     6207 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006    15180 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/client/online_store_rest_client.py
--rw-r--r--   0     1006     1006     1554 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/code.py
--rw-r--r--   0     1006     1006    14393 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.158504 hsfs-3.7.1/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1497 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5612 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     3635 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1749 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2161 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1587 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    29539 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3349 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.170503 hsfs-3.7.1/hsfs/core/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006    15490 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/arrow_flight_client.py
--rw-r--r--   0     1006     1006     4156 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     2032 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3629 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     7809 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/delta_engine.py
--rw-r--r--   0     1006     1006     1040 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1627 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4060 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9810 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     6198 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    11207 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_descriptive_statistics.py
--rw-r--r--   0     1006     1006    13837 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6663 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    14833 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006    34734 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_monitoring_config.py
--rw-r--r--   0     1006     1006    10497 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_monitoring_config_api.py
--rw-r--r--   0     1006     1006    21382 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_monitoring_config_engine.py
--rw-r--r--   0     1006     1006     7864 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_monitoring_result.py
--rw-r--r--   0     1006     1006     5921 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_monitoring_result_api.py
--rw-r--r--   0     1006     1006    24868 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_monitoring_result_engine.py
--rw-r--r--   0     1006     1006     1238 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006    10499 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    32376 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5023 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11737 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1229 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1087 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     8626 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/job.py
--rw-r--r--   0     1006     1006     2814 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2065 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     3079 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/job_schedule.py
--rw-r--r--   0     1006     1006     1205 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006    11557 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/monitoring_window_config.py
--rw-r--r--   0     1006     1006    17012 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/monitoring_window_config_engine.py
--rw-r--r--   0     1006     1006     8709 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/online_store_rest_client_api.py
--rw-r--r--   0     1006     1006    32516 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/online_store_rest_client_engine.py
--rw-r--r--   0     1006     1006     3090 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/opensearch.py
--rw-r--r--   0     1006     1006     4419 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/opensearch_api.py
--rw-r--r--   0     1006     1006      898 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     1981 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/spine_group_engine.py
--rw-r--r--   0     1006     1006    12655 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006    20903 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     3072 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6210 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    12712 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     2297 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    11843 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/vector_db_client.py
--rwxr-xr-x   0     1006     1006    41829 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2024-01-11 15:40:27.000000 hsfs-3.7.1/hsfs/decorators.py
--rw-r--r--   0     1006     1006     5552 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/embedding.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.170503 hsfs-3.7.1/hsfs/engine/
--rw-r--r--   0     1006     1006     2486 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    53717 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    47336 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006     1118 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/engine/spark_no_metastore.py
--rw-r--r--   0     1006     1006    23612 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6960 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/feature.py
--rw-r--r--   0     1006     1006   156932 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3955 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1992 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    78556 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/feature_store.py
--rw-r--r--   0     1006     1006   163846 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8651 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     3456 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/serving_key.py
--rw-r--r--   0     1006     1006     2081 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     8298 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3331 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    49738 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1868 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/tag.py
--rw-r--r--   0     1006     1006    39576 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     4836 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2816 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8947 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2197 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     7760 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/usage.py
--rw-r--r--   0     1006     1006     3323 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/user.py
--rw-r--r--   0     1006     1006    15871 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/util.py
--rw-r--r--   0     1006     1006     7537 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      628 2024-04-11 18:09:58.000000 hsfs-3.7.1/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.154504 hsfs-3.7.1/hsfs.egg-info/
--rw-r--r--   0     1006     1006     8378 2024-04-11 18:10:02.000000 hsfs-3.7.1/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     3650 2024-04-11 18:10:02.000000 hsfs-3.7.1/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2024-04-11 18:10:02.000000 hsfs-3.7.1/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      892 2024-04-11 18:10:02.000000 hsfs-3.7.1/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2024-04-11 18:10:02.000000 hsfs-3.7.1/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2024-04-11 18:10:02.174503 hsfs-3.7.1/setup.cfg
--rw-r--r--   0     1006     1006     3310 2024-04-11 18:09:58.000000 hsfs-3.7.1/setup.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:10:02.170503 hsfs-3.7.1/tests/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.1/tests/__init__.py
--rw-r--r--   0     1006     1006    34202 2024-04-11 18:09:58.000000 hsfs-3.7.1/tests/test_storage_connector.py
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.290977 hsfs-3.7.1rc0/
+-rw-r--r--   0     1006     1006       40 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     8384 2024-03-28 13:36:25.290977 hsfs-3.7.1rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     5951 2024-03-28 13:36:24.000000 hsfs-3.7.1rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.254977 hsfs-3.7.1rc0/hsfs/
+-rw-r--r--   0     1006     1006     1421 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.254977 hsfs-3.7.1rc0/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1401 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     9570 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     3028 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    11825 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     6207 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006    15180 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/client/online_store_rest_client.py
+-rw-r--r--   0     1006     1006     1554 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/code.py
+-rw-r--r--   0     1006     1006    14393 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.258977 hsfs-3.7.1rc0/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1497 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5612 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     3635 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1749 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2161 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1587 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    28409 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3349 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.282977 hsfs-3.7.1rc0/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006    15490 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/arrow_flight_client.py
+-rw-r--r--   0     1006     1006     4156 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     2032 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3629 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7809 2024-03-28 10:37:34.000000 hsfs-3.7.1rc0/hsfs/core/delta_engine.py
+-rw-r--r--   0     1006     1006     1040 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1627 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4060 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9810 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     6198 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    11207 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_descriptive_statistics.py
+-rw-r--r--   0     1006     1006    13837 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6663 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    14833 2024-03-28 10:37:34.000000 hsfs-3.7.1rc0/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006    34734 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_monitoring_config.py
+-rw-r--r--   0     1006     1006    10497 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_monitoring_config_api.py
+-rw-r--r--   0     1006     1006    21382 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_monitoring_config_engine.py
+-rw-r--r--   0     1006     1006     7864 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_monitoring_result.py
+-rw-r--r--   0     1006     1006     5921 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_monitoring_result_api.py
+-rw-r--r--   0     1006     1006    24868 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_monitoring_result_engine.py
+-rw-r--r--   0     1006     1006     1238 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006    10499 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    32376 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5023 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11737 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1229 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1087 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     8626 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2814 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2065 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     3079 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/job_schedule.py
+-rw-r--r--   0     1006     1006     1205 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006    11557 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/monitoring_window_config.py
+-rw-r--r--   0     1006     1006    17012 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/monitoring_window_config_engine.py
+-rw-r--r--   0     1006     1006     8709 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/online_store_rest_client_api.py
+-rw-r--r--   0     1006     1006    32516 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/online_store_rest_client_engine.py
+-rw-r--r--   0     1006     1006     3090 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/opensearch.py
+-rw-r--r--   0     1006     1006     4419 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/opensearch_api.py
+-rw-r--r--   0     1006     1006      898 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     1981 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/spine_group_engine.py
+-rw-r--r--   0     1006     1006    12655 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006    20903 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     3072 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6210 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    12712 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     2297 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    11843 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/vector_db_client.py
+-rwxr-xr-x   0     1006     1006    41829 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/decorators.py
+-rw-r--r--   0     1006     1006     5552 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/embedding.py
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.290977 hsfs-3.7.1rc0/hsfs/engine/
+-rw-r--r--   0     1006     1006     2486 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    53717 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    47336 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006     1118 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/engine/spark_no_metastore.py
+-rw-r--r--   0     1006     1006    23612 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6960 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/feature.py
+-rw-r--r--   0     1006     1006   156353 2024-03-28 10:37:34.000000 hsfs-3.7.1rc0/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3955 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1992 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    78556 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006   163846 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2024-01-11 15:40:27.000000 hsfs-3.7.1rc0/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8651 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     3456 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/serving_key.py
+-rw-r--r--   0     1006     1006     2081 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     8298 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3331 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    49738 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1868 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/tag.py
+-rw-r--r--   0     1006     1006    39576 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     4836 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2816 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8947 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2197 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     7760 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/usage.py
+-rw-r--r--   0     1006     1006     3323 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/user.py
+-rw-r--r--   0     1006     1006    15871 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/util.py
+-rw-r--r--   0     1006     1006     7537 2024-03-19 04:15:28.000000 hsfs-3.7.1rc0/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      631 2024-03-28 10:37:34.000000 hsfs-3.7.1rc0/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2024-03-28 13:36:25.254977 hsfs-3.7.1rc0/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     8384 2024-03-28 13:36:25.000000 hsfs-3.7.1rc0/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     3600 2024-03-28 13:36:25.000000 hsfs-3.7.1rc0/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2024-03-28 13:36:25.000000 hsfs-3.7.1rc0/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      892 2024-03-28 13:36:25.000000 hsfs-3.7.1rc0/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2024-03-28 13:36:25.000000 hsfs-3.7.1rc0/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2024-03-28 13:36:25.290977 hsfs-3.7.1rc0/setup.cfg
+-rw-r--r--   0     1006     1006     3310 2024-03-19 09:15:34.000000 hsfs-3.7.1rc0/setup.py
```

### Comparing `hsfs-3.7.1/PKG-INFO` & `hsfs-3.7.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.7.1
+Version: 3.7.1rc0
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1rc0
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.7.1 Summary: HSFS: An environment
-independent client to interact with the Hopsworks Featurestore Home-page:
-https://github.com/logicalclocks/feature-store-api Author: Hopsworks AB Author-
-email: moritz@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1
+Metadata-Version: 2.1 Name: hsfs Version: 3.7.1rc0 Summary: HSFS: An
+environment independent client to interact with the Hopsworks Featurestore
+Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
+AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1rc0
 Description: # Hopsworks Feature Store
 _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _F_e_a_t_u_r_e_ _S_t_o_r_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_S_c_a_l_a_/
                 _J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.7.1/README.md` & `hsfs-3.7.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/__init__.py` & `hsfs-3.7.1rc0/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/__init__.py` & `hsfs-3.7.1rc0/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/auth.py` & `hsfs-3.7.1rc0/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/base.py` & `hsfs-3.7.1rc0/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/exceptions.py` & `hsfs-3.7.1rc0/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/external.py` & `hsfs-3.7.1rc0/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/hopsworks.py` & `hsfs-3.7.1rc0/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/client/online_store_rest_client.py` & `hsfs-3.7.1rc0/hsfs/client/online_store_rest_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/code.py` & `hsfs-3.7.1rc0/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/connection.py` & `hsfs-3.7.1rc0/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/__init__.py` & `hsfs-3.7.1rc0/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.7.1rc0/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/filter.py` & `hsfs-3.7.1rc0/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/fs_query.py` & `hsfs-3.7.1rc0/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.7.1rc0/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/join.py` & `hsfs-3.7.1rc0/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.7.1rc0/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/constructor/query.py` & `hsfs-3.7.1rc0/hsfs/constructor/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import json
 import humps
-import warnings
 from typing import Optional, List, Union
 from datetime import datetime, date
 
 from hsfs import util, engine, feature_group
 from hsfs.core import query_constructor_api, storage_connector_api, arrow_flight_client
 from hsfs.constructor import join
 from hsfs.constructor.filter import Filter, Logic
@@ -66,15 +65,14 @@
         self._joins = joins or []
         self._filter = Logic.from_response_json(filter)
         self._python_engine = True if engine.get_type() == "python" else False
         self._query_constructor_api = query_constructor_api.QueryConstructorApi()
         self._storage_connector_api = storage_connector_api.StorageConnectorApi()
 
     def _prep_read(self, online, read_options):
-        self._check_read_supported(online)
         fs_query = self._query_constructor_api.construct_query(self)
 
         if online:
             sql_query = self._to_string(fs_query, online)
             online_conn = self._storage_connector_api.get_online_connector(
                 self._feature_store_id
             )
@@ -144,22 +142,17 @@
                 * key "hive_config" to pass a dictionary of hive or tez configurations.
                   For example: `{"hive_config": {"hive.tez.cpu.vcores": 2, "tez.grouping.split-count": "3"}}`
                 Defaults to `{}`.
 
         # Returns
             `DataFrame`: DataFrame depending on the chosen type.
         """
-        if not isinstance(online, bool):
-            warnings.warn(
-                f"Passed {online} as value to online kwarg for `read` method. The `online` parameter is expected to be a boolean"
-                + " to specify whether to read from the Online Feature Store.",
-                stacklevel=1,
-            )
         if not read_options:
             read_options = {}
+        self._check_read_supported(online)
         sql_query, online_conn = self._prep_read(online, read_options)
 
         schema = None
         if (
             read_options
             and "pandas_types" in read_options
             and read_options["pandas_types"]
@@ -491,33 +484,20 @@
             ],
             filter=json_decamelized.get("filter", None),
         )
 
     def _check_read_supported(self, online):
         if not online:
             return
-        if not isinstance(online, bool):
-            warnings.warn(
-                f"Passed {online} as value to online kwarg for `read` method. The `online` parameter is expected to be a boolean"
-                + " to specify whether to read from the Online Feature Store.",
-                stacklevel=1,
-            )
         for fg in self.featuregroups:
             if fg.embedding_index:
                 raise FeatureStoreException(
                     "Reading from query containing embedding is not supported."
                     " Use `feature_view.get_feature_vector(s) instead."
                 )
-            elif fg.online_enabled is False:
-                raise FeatureStoreException(
-                    f"Found {fg.name} in query Feature Groups which is not `online_enabled`."
-                    + "If you intend to use the Online Feature Store, please enable the Feature Group"
-                    + " for online serving by setting `online=True` on creation. Otherwise, set online=False"
-                    + " when using the `read` method."
-                )
 
     @classmethod
     def _hopsworks_json(cls, json_dict):
         """
         This method is used by the Hopsworks helper job.
         It does not fully deserialize the message as the usecase is to
         send it straight back to Hopsworks to read the content of the query
```

### Comparing `hsfs-3.7.1/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.7.1rc0/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/__init__.py` & `hsfs-3.7.1rc0/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/arrow_flight_client.py` & `hsfs-3.7.1rc0/hsfs/core/arrow_flight_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/builtin_transformation_function.py` & `hsfs-3.7.1rc0/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/code_api.py` & `hsfs-3.7.1rc0/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/code_engine.py` & `hsfs-3.7.1rc0/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/dataset_api.py` & `hsfs-3.7.1rc0/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/delta_engine.py` & `hsfs-3.7.1rc0/hsfs/core/delta_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.7.1rc0/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/execution.py` & `hsfs-3.7.1rc0/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/expectation_api.py` & `hsfs-3.7.1rc0/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/expectation_engine.py` & `hsfs-3.7.1rc0/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/expectation_suite_api.py` & `hsfs-3.7.1rc0/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/expectation_suite_engine.py` & `hsfs-3.7.1rc0/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/explicit_provenance.py` & `hsfs-3.7.1rc0/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/external_feature_group_engine.py` & `hsfs-3.7.1rc0/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_descriptive_statistics.py` & `hsfs-3.7.1rc0/hsfs/core/feature_descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_group_api.py` & `hsfs-3.7.1rc0/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_group_base_engine.py` & `hsfs-3.7.1rc0/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_group_engine.py` & `hsfs-3.7.1rc0/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_monitoring_config.py` & `hsfs-3.7.1rc0/hsfs/core/feature_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_monitoring_config_api.py` & `hsfs-3.7.1rc0/hsfs/core/feature_monitoring_config_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_monitoring_config_engine.py` & `hsfs-3.7.1rc0/hsfs/core/feature_monitoring_config_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_monitoring_result.py` & `hsfs-3.7.1rc0/hsfs/core/feature_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_monitoring_result_api.py` & `hsfs-3.7.1rc0/hsfs/core/feature_monitoring_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_monitoring_result_engine.py` & `hsfs-3.7.1rc0/hsfs/core/feature_monitoring_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_store_api.py` & `hsfs-3.7.1rc0/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_view_api.py` & `hsfs-3.7.1rc0/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/feature_view_engine.py` & `hsfs-3.7.1rc0/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/great_expectation_engine.py` & `hsfs-3.7.1rc0/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/hosts_api.py` & `hsfs-3.7.1rc0/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/hudi_engine.py` & `hsfs-3.7.1rc0/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/ingestion_job.py` & `hsfs-3.7.1rc0/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/ingestion_job_conf.py` & `hsfs-3.7.1rc0/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/inode.py` & `hsfs-3.7.1rc0/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/job.py` & `hsfs-3.7.1rc0/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/job_api.py` & `hsfs-3.7.1rc0/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/job_configuration.py` & `hsfs-3.7.1rc0/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/job_schedule.py` & `hsfs-3.7.1rc0/hsfs/core/job_schedule.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/kafka_api.py` & `hsfs-3.7.1rc0/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/monitoring_window_config.py` & `hsfs-3.7.1rc0/hsfs/core/monitoring_window_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/monitoring_window_config_engine.py` & `hsfs-3.7.1rc0/hsfs/core/monitoring_window_config_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/online_store_rest_client_api.py` & `hsfs-3.7.1rc0/hsfs/core/online_store_rest_client_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/online_store_rest_client_engine.py` & `hsfs-3.7.1rc0/hsfs/core/online_store_rest_client_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/opensearch.py` & `hsfs-3.7.1rc0/hsfs/core/opensearch.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/opensearch_api.py` & `hsfs-3.7.1rc0/hsfs/core/opensearch_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/project_api.py` & `hsfs-3.7.1rc0/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/query_constructor_api.py` & `hsfs-3.7.1rc0/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/services_api.py` & `hsfs-3.7.1rc0/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/spine_group_engine.py` & `hsfs-3.7.1rc0/hsfs/core/spine_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/statistics_api.py` & `hsfs-3.7.1rc0/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/statistics_engine.py` & `hsfs-3.7.1rc0/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/storage_connector_api.py` & `hsfs-3.7.1rc0/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/tags_api.py` & `hsfs-3.7.1rc0/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/training_dataset_api.py` & `hsfs-3.7.1rc0/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/training_dataset_engine.py` & `hsfs-3.7.1rc0/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.7.1rc0/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/transformation_function_api.py` & `hsfs-3.7.1rc0/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/transformation_function_engine.py` & `hsfs-3.7.1rc0/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/validation_report_api.py` & `hsfs-3.7.1rc0/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/validation_report_engine.py` & `hsfs-3.7.1rc0/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/validation_result_api.py` & `hsfs-3.7.1rc0/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/validation_result_engine.py` & `hsfs-3.7.1rc0/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/variable_api.py` & `hsfs-3.7.1rc0/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/vector_db_client.py` & `hsfs-3.7.1rc0/hsfs/core/vector_db_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/core/vector_server.py` & `hsfs-3.7.1rc0/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/decorators.py` & `hsfs-3.7.1rc0/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/embedding.py` & `hsfs-3.7.1rc0/hsfs/embedding.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/engine/__init__.py` & `hsfs-3.7.1rc0/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/engine/python.py` & `hsfs-3.7.1rc0/hsfs/engine/python.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/engine/spark.py` & `hsfs-3.7.1rc0/hsfs/engine/spark.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/engine/spark_no_metastore.py` & `hsfs-3.7.1rc0/hsfs/engine/spark_no_metastore.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/expectation_suite.py` & `hsfs-3.7.1rc0/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/feature.py` & `hsfs-3.7.1rc0/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/feature_group.py` & `hsfs-3.7.1rc0/hsfs/feature_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -5035,4775 +5035,4739 @@
 00013aa0: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
 00013ab0: 6f72 602e 204e 6f20 6461 7461 2069 7320  or`. No data is 
 00013ac0: 6176 6169 6c61 626c 6520 666f 7220 6665  available for fe
 00013ad0: 6174 7572 6520 6772 6f75 7020 7769 7468  ature group with
 00013ae0: 2074 6869 7320 636f 6d6d 6974 2064 6174   this commit dat
 00013af0: 652c 2049 6620 7469 6d65 2074 7261 7665  e, If time trave
 00013b00: 6c20 656e 6162 6c65 642e 0a20 2020 2020  l enabled..     
-00013b10: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00013b20: 6620 7761 6c6c 636c 6f63 6b5f 7469 6d65  f wallclock_time
-00013b30: 2061 6e64 2073 656c 662e 5f74 696d 655f   and self._time_
-00013b40: 7472 6176 656c 5f66 6f72 6d61 7420 6973  travel_format is
-00013b50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00013b60: 2020 2072 6169 7365 2046 6561 7475 7265     raise Feature
-00013b70: 5374 6f72 6545 7863 6570 7469 6f6e 280a  StoreException(.
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b90: 2254 696d 6520 7472 6176 656c 2066 6f72  "Time travel for
-00013ba0: 6d61 7420 6973 206e 6f74 2073 6574 2066  mat is not set f
-00013bb0: 6f72 2074 6865 2066 6561 7475 7265 2067  or the feature g
-00013bc0: 726f 7570 2c20 6361 6e6e 6f74 2072 6561  roup, cannot rea
-00013bd0: 6420 6173 206f 6620 7370 6563 6966 6963  d as of specific
-00013be0: 2070 6f69 6e74 2069 6e20 7469 6d65 2e22   point in time."
-00013bf0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00013c00: 2020 2020 2020 2065 6c69 6620 7761 6c6c         elif wall
-00013c10: 636c 6f63 6b5f 7469 6d65 2061 6e64 2065  clock_time and e
-00013c20: 6e67 696e 652e 6765 745f 7479 7065 2829  ngine.get_type()
-00013c30: 203d 3d20 2270 7974 686f 6e22 3a0a 2020   == "python":.  
-00013c40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00013c50: 4665 6174 7572 6553 746f 7265 4578 6365  FeatureStoreExce
-00013c60: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-00013c70: 2020 2020 2020 2022 5079 7468 6f6e 2065         "Python e
-00013c80: 6e76 6972 6f6e 6d65 6e74 7320 646f 6573  nvironments does
-00013c90: 206e 6f74 2073 7570 706f 7274 2069 6e63   not support inc
-00013ca0: 7265 6d65 6e74 616c 2071 7565 7269 6573  remental queries
-00013cb0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-00013cc0: 2020 2020 2b20 2252 6561 6420 6665 6174      + "Read feat
-00013cd0: 7572 6520 6772 6f75 7020 7769 7468 6f75  ure group withou
-00013ce0: 7420 7469 6d65 7374 616d 7020 746f 2072  t timestamp to r
-00013cf0: 6574 7269 6576 6520 6c61 7465 7374 2073  etrieve latest s
-00013d00: 6e61 7073 686f 7420 6f72 2073 7769 7463  napshot or switc
-00013d10: 6820 746f 2022 0a20 2020 2020 2020 2020  h to ".         
-00013d20: 2020 2020 2020 202b 2022 656e 7669 726f         + "enviro
-00013d30: 6e6d 656e 7420 7769 7468 2053 7061 726b  nment with Spark
-00013d40: 2045 6e67 696e 652e 220a 2020 2020 2020   Engine.".      
-00013d50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00013d60: 2065 6e67 696e 652e 6765 745f 696e 7374   engine.get_inst
-00013d70: 616e 6365 2829 2e73 6574 5f6a 6f62 5f67  ance().set_job_g
-00013d80: 726f 7570 280a 2020 2020 2020 2020 2020  roup(.          
-00013d90: 2020 2246 6574 6368 696e 6720 4665 6174    "Fetching Feat
-00013da0: 7572 6520 6772 6f75 7022 2c0a 2020 2020  ure group",.    
-00013db0: 2020 2020 2020 2020 2247 6574 7469 6e67          "Getting
-00013dc0: 2066 6561 7475 7265 2067 726f 7570 3a20   feature group: 
-00013dd0: 7b7d 2066 726f 6d20 7468 6520 6665 6174  {} from the feat
-00013de0: 7572 6573 746f 7265 207b 7d22 2e66 6f72  urestore {}".for
-00013df0: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00013e00: 2020 2020 2073 656c 662e 5f6e 616d 652c       self._name,
-00013e10: 2073 656c 662e 5f66 6561 7475 7265 5f73   self._feature_s
-00013e20: 746f 7265 5f6e 616d 650a 2020 2020 2020  tore_name.      
-00013e30: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00013e40: 2029 0a0a 2020 2020 2020 2020 6966 2077   )..        if w
-00013e50: 616c 6c63 6c6f 636b 5f74 696d 653a 0a20  allclock_time:. 
-00013e60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00013e70: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-00013e80: 2020 2020 7365 6c66 2e73 656c 6563 745f      self.select_
-00013e90: 616c 6c28 290a 2020 2020 2020 2020 2020  all().          
-00013ea0: 2020 2020 2020 2e61 735f 6f66 2877 616c        .as_of(wal
-00013eb0: 6c63 6c6f 636b 5f74 696d 6529 0a20 2020  lclock_time).   
-00013ec0: 2020 2020 2020 2020 2020 2020 202e 7265               .re
-00013ed0: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
-00013ee0: 2020 2020 2020 2020 6f6e 6c69 6e65 2c0a          online,.
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2020 2020 6461 7461 6672 616d 655f 7479      dataframe_ty
-00013f10: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00013f20: 2020 2020 2020 2020 7265 6164 5f6f 7074          read_opt
-00013f30: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00013f40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00013f50: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00013f60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00013f70: 7265 7475 726e 2073 656c 662e 7365 6c65  return self.sele
-00013f80: 6374 5f61 6c6c 2829 2e72 6561 6428 0a20  ct_all().read(. 
-00013f90: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00013fa0: 6e6c 696e 652c 0a20 2020 2020 2020 2020  nline,.         
-00013fb0: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-00013fc0: 5f74 7970 652c 0a20 2020 2020 2020 2020  _type,.         
-00013fd0: 2020 2020 2020 2072 6561 645f 6f70 7469         read_opti
-00013fe0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-00013ff0: 2029 0a0a 2020 2020 6465 6620 7265 6164   )..    def read
-00014000: 5f63 6861 6e67 6573 280a 2020 2020 2020  _changes(.      
-00014010: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00014020: 7374 6172 745f 7761 6c6c 636c 6f63 6b5f  start_wallclock_
-00014030: 7469 6d65 3a20 556e 696f 6e5b 7374 722c  time: Union[str,
-00014040: 2069 6e74 2c20 6461 7465 7469 6d65 2c20   int, datetime, 
-00014050: 6461 7465 5d2c 0a20 2020 2020 2020 2065  date],.        e
-00014060: 6e64 5f77 616c 6c63 6c6f 636b 5f74 696d  nd_wallclock_tim
-00014070: 653a 2055 6e69 6f6e 5b73 7472 2c20 696e  e: Union[str, in
-00014080: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
-00014090: 655d 2c0a 2020 2020 2020 2020 7265 6164  e],.        read
-000140a0: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-000140b0: 616c 5b64 6963 745d 203d 207b 7d2c 0a20  al[dict] = {},. 
-000140c0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-000140d0: 2252 6561 6473 2075 7064 6174 6573 206f  "Reads updates o
-000140e0: 6620 7468 6973 2066 6561 7475 7265 2074  f this feature t
-000140f0: 6861 7420 6f63 6375 7272 6564 2062 6574  hat occurred bet
-00014100: 7765 656e 2073 7065 6369 6669 6564 2070  ween specified p
-00014110: 6f69 6e74 7320 696e 2074 696d 652e 0a0a  oints in time...
-00014120: 2020 2020 2020 2020 2121 2120 7761 726e          !!! warn
-00014130: 696e 6720 2244 6570 7265 6361 7465 6422  ing "Deprecated"
-00014140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014150: 2020 2020 2060 7265 6164 5f63 6861 6e67       `read_chang
-00014160: 6573 6020 6d65 7468 6f64 2069 7320 6465  es` method is de
-00014170: 7072 6563 6174 6564 2e20 5573 650a 2020  precated. Use.  
-00014180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014190: 2020 6061 735f 6f66 2865 6e64 5f77 616c    `as_of(end_wal
-000141a0: 6c63 6c6f 636b 5f74 696d 652c 2065 7863  lclock_time, exc
-000141b0: 6c75 6465 5f75 6e74 696c 3d73 7461 7274  lude_until=start
-000141c0: 5f77 616c 6c63 6c6f 636b 5f74 696d 6529  _wallclock_time)
-000141d0: 2e72 6561 6428 7265 6164 5f6f 7074 696f  .read(read_optio
-000141e0: 6e73 3d72 6561 645f 6f70 7469 6f6e 7329  ns=read_options)
-000141f0: 600a 2020 2020 2020 2020 2020 2020 2020  `.              
-00014200: 2020 2020 2020 696e 7374 6561 642e 0a0a        instead...
-00014210: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
-00014220: 6374 696f 6e20 6f6e 6c79 2077 6f72 6b73  ction only works
-00014230: 206f 6e20 6665 6174 7572 6520 6772 6f75   on feature grou
-00014240: 7073 2077 6974 6820 6048 5544 4960 2074  ps with `HUDI` t
-00014250: 696d 6520 7472 6176 656c 2066 6f72 6d61  ime travel forma
-00014260: 742e 0a0a 2020 2020 2020 2020 2320 4172  t...        # Ar
-00014270: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
-00014280: 2020 2020 7374 6172 745f 7761 6c6c 636c      start_wallcl
-00014290: 6f63 6b5f 7469 6d65 3a20 5374 6172 7420  ock_time: Start 
-000142a0: 7469 6d65 206f 6620 7468 6520 7469 6d65  time of the time
-000142b0: 2074 7261 7665 6c20 7175 6572 792e 2053   travel query. S
-000142c0: 7472 696e 6773 2073 686f 756c 6420 6265  trings should be
-000142d0: 2066 6f72 6d61 7474 6564 2069 6e20 6f6e   formatted in on
-000142e0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-000142f0: 6e67 2066 6f72 6d61 7473 2060 2559 2d25  ng formats `%Y-%
-00014300: 6d2d 2564 602c 2060 2559 2d25 6d2d 2564  m-%d`, `%Y-%m-%d
-00014310: 2025 4860 2c20 6025 592d 256d 2d25 6420   %H`, `%Y-%m-%d 
-00014320: 2548 3a25 4d60 2c0a 2020 2020 2020 2020  %H:%M`,.        
-00014330: 2020 2020 2020 2020 6025 592d 256d 2d25          `%Y-%m-%
-00014340: 6420 2548 3a25 4d3a 2553 602c 206f 7220  d %H:%M:%S`, or 
-00014350: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-00014360: 2553 2e25 6660 2e0a 2020 2020 2020 2020  %S.%f`..        
-00014370: 2020 2020 656e 645f 7761 6c6c 636c 6f63      end_wallcloc
-00014380: 6b5f 7469 6d65 3a20 456e 6420 7469 6d65  k_time: End time
-00014390: 206f 6620 7468 6520 7469 6d65 2074 7261   of the time tra
-000143a0: 7665 6c20 7175 6572 792e 2053 7472 696e  vel query. Strin
-000143b0: 6773 2073 686f 756c 6420 6265 2066 6f72  gs should be for
-000143c0: 6d61 7474 6564 2069 6e20 6f6e 6520 6f66  matted in one of
-000143d0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-000143e0: 6f72 6d61 7473 2060 2559 2d25 6d2d 2564  ormats `%Y-%m-%d
-000143f0: 602c 2060 2559 2d25 6d2d 2564 2025 4860  `, `%Y-%m-%d %H`
-00014400: 2c20 6025 592d 256d 2d25 6420 2548 3a25  , `%Y-%m-%d %H:%
-00014410: 4d60 2c0a 2020 2020 2020 2020 2020 2020  M`,.            
-00014420: 2020 2020 6025 592d 256d 2d25 6420 2548      `%Y-%m-%d %H
-00014430: 3a25 4d3a 2553 602c 206f 7220 6025 592d  :%M:%S`, or `%Y-
-00014440: 256d 2d25 6420 2548 3a25 4d3a 2553 2e25  %m-%d %H:%M:%S.%
-00014450: 6660 2e0a 2020 2020 2020 2020 2020 2020  f`..            
-00014460: 7265 6164 5f6f 7074 696f 6e73 3a20 4164  read_options: Ad
-00014470: 6469 7469 6f6e 616c 206f 7074 696f 6e73  ditional options
-00014480: 2061 7320 6b65 792f 7661 6c75 6520 7061   as key/value pa
-00014490: 6972 7320 746f 2070 6173 7320 746f 2074  irs to pass to t
-000144a0: 6865 2065 7865 6375 7469 6f6e 2065 6e67  he execution eng
-000144b0: 696e 652e 0a20 2020 2020 2020 2020 2020  ine..           
-000144c0: 2020 2020 2046 6f72 2073 7061 726b 2065       For spark e
-000144d0: 6e67 696e 653a 2044 6963 7469 6f6e 6172  ngine: Dictionar
-000144e0: 7920 6f66 2072 6561 6420 6f70 7469 6f6e  y of read option
-000144f0: 7320 666f 7220 5370 6172 6b2e 0a20 2020  s for Spark..   
-00014500: 2020 2020 2020 2020 2020 2020 2046 6f72               For
-00014510: 2070 7974 686f 6e20 656e 6769 6e65 3a0a   python engine:.
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2a20 6b65 7920 6022 6869 7665 5f63 6f6e  * key `"hive_con
-00014540: 6669 6722 6020 746f 2070 6173 7320 6120  fig"` to pass a 
-00014550: 6469 6374 696f 6e61 7279 206f 6620 6869  dictionary of hi
-00014560: 7665 206f 7220 7465 7a20 636f 6e66 6967  ve or tez config
-00014570: 7572 6174 696f 6e73 2e0a 2020 2020 2020  urations..      
-00014580: 2020 2020 2020 2020 2020 2020 466f 7220              For 
-00014590: 6578 616d 706c 653a 2060 7b22 6869 7665  example: `{"hive
-000145a0: 5f63 6f6e 6669 6722 3a20 7b22 6869 7665  _config": {"hive
-000145b0: 2e74 657a 2e63 7075 2e76 636f 7265 7322  .tez.cpu.vcores"
-000145c0: 3a20 322c 2022 7465 7a2e 6772 6f75 7069  : 2, "tez.groupi
-000145d0: 6e67 2e73 706c 6974 2d63 6f75 6e74 223a  ng.split-count":
-000145e0: 2022 3322 7d7d 600a 2020 2020 2020 2020   "3"}}`.        
-000145f0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00014600: 2074 6f20 607b 7d60 2e0a 0a20 2020 2020   to `{}`...     
-00014610: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-00014620: 2020 2020 2020 2020 2060 4461 7461 4672           `DataFr
-00014630: 616d 6560 2e20 5468 6520 7370 6172 6b20  ame`. The spark 
-00014640: 6461 7461 6672 616d 6520 636f 6e74 6169  dataframe contai
-00014650: 6e69 6e67 2074 6865 2069 6e63 7265 6d65  ning the increme
-00014660: 6e74 616c 2063 6861 6e67 6573 206f 660a  ntal changes of.
-00014670: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00014680: 7572 6520 6461 7461 2e0a 0a20 2020 2020  ure data...     
-00014690: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
-000146a0: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
-000146b0: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
-000146c0: 5265 7374 4150 4945 7272 6f72 602e 2020  RestAPIError`.  
-000146d0: 4e6f 2064 6174 6120 6973 2061 7661 696c  No data is avail
-000146e0: 6162 6c65 2066 6f72 2066 6561 7475 7265  able for feature
-000146f0: 2067 726f 7570 2077 6974 6820 7468 6973   group with this
-00014700: 2063 6f6d 6d69 7420 6461 7465 2e0a 2020   commit date..  
-00014710: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
-00014720: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
-00014730: 732e 4665 6174 7572 6553 746f 7265 4578  s.FeatureStoreEx
-00014740: 6365 7074 696f 6e60 2e20 4966 2074 6865  ception`. If the
-00014750: 2066 6561 7475 7265 2067 726f 7570 2064   feature group d
-00014760: 6f65 7320 6e6f 7420 6861 7665 2060 4855  oes not have `HU
-00014770: 4449 6020 7469 6d65 2074 7261 7665 6c20  DI` time travel 
-00014780: 666f 726d 6174 0a20 2020 2020 2020 2022  format.        "
-00014790: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-000147a0: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-000147b0: 7365 6c66 2e73 656c 6563 745f 616c 6c28  self.select_all(
-000147c0: 290a 2020 2020 2020 2020 2020 2020 2e70  ).            .p
-000147d0: 756c 6c5f 6368 616e 6765 7328 7374 6172  ull_changes(star
-000147e0: 745f 7761 6c6c 636c 6f63 6b5f 7469 6d65  t_wallclock_time
-000147f0: 2c20 656e 645f 7761 6c6c 636c 6f63 6b5f  , end_wallclock_
-00014800: 7469 6d65 290a 2020 2020 2020 2020 2020  time).          
-00014810: 2020 2e72 6561 6428 4661 6c73 652c 2022    .read(False, "
-00014820: 6465 6661 756c 7422 2c20 7265 6164 5f6f  default", read_o
-00014830: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
-00014840: 290a 0a20 2020 2064 6566 2066 696e 645f  )..    def find_
-00014850: 6e65 6967 6862 6f72 7328 0a20 2020 2020  neighbors(.     
-00014860: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00014870: 2065 6d62 6564 6469 6e67 3a20 4c69 7374   embedding: List
-00014880: 5b55 6e69 6f6e 5b69 6e74 2c20 666c 6f61  [Union[int, floa
-00014890: 745d 5d2c 0a20 2020 2020 2020 2063 6f6c  t]],.        col
-000148a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-000148b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000148c0: 6b3a 204f 7074 696f 6e61 6c5b 696e 745d  k: Optional[int]
-000148d0: 203d 2031 302c 0a20 2020 2020 2020 2066   = 10,.        f
-000148e0: 696c 7465 723a 204f 7074 696f 6e61 6c5b  ilter: Optional[
-000148f0: 556e 696f 6e5b 4669 6c74 6572 2c20 4c6f  Union[Filter, Lo
-00014900: 6769 635d 5d20 3d20 4e6f 6e65 2c0a 2020  gic]] = None,.  
-00014910: 2020 2020 2020 6d69 6e5f 7363 6f72 653a        min_score:
-00014920: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-00014930: 203d 2030 2c0a 2020 2020 2920 2d3e 204c   = 0,.    ) -> L
-00014940: 6973 745b 5475 706c 655b 666c 6f61 742c  ist[Tuple[float,
-00014950: 204c 6973 745b 416e 795d 5d5d 3a0a 2020   List[Any]]]:.  
-00014960: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014970: 2020 4669 6e64 7320 7468 6520 6e65 6172    Finds the near
-00014980: 6573 7420 6e65 6967 6862 6f72 7320 666f  est neighbors fo
-00014990: 7220 6120 6769 7665 6e20 656d 6265 6464  r a given embedd
-000149a0: 696e 6720 696e 2074 6865 2076 6563 746f  ing in the vecto
-000149b0: 7220 6461 7461 6261 7365 2e0a 0a20 2020  r database...   
-000149c0: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-000149d0: 0a20 2020 2020 2020 2020 2020 2065 6d62  .            emb
-000149e0: 6564 6469 6e67 3a20 5468 6520 7461 7267  edding: The targ
-000149f0: 6574 2065 6d62 6564 6469 6e67 2066 6f72  et embedding for
-00014a00: 2077 6869 6368 206e 6569 6768 626f 7273   which neighbors
-00014a10: 2061 7265 2074 6f20 6265 2066 6f75 6e64   are to be found
-00014a20: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00014a30: 6c3a 2054 6865 2063 6f6c 756d 6e20 6e61  l: The column na
-00014a40: 6d65 2075 7365 6420 746f 2063 6f6d 7075  me used to compu
-00014a50: 7465 2073 696d 696c 6172 6974 7920 7363  te similarity sc
-00014a60: 6f72 652e 2052 6571 7569 7265 6420 6f6e  ore. Required on
-00014a70: 6c79 2069 6620 7468 6572 650a 2020 2020  ly if there.    
-00014a80: 2020 2020 2020 2020 6172 6520 6d75 6c74          are mult
-00014a90: 6970 6c65 2065 6d62 6564 6469 6e67 7320  iple embeddings 
-00014aa0: 286f 7074 696f 6e61 6c29 2e0a 2020 2020  (optional)..    
-00014ab0: 2020 2020 2020 2020 6b3a 2054 6865 206e          k: The n
-00014ac0: 756d 6265 7220 6f66 206e 6561 7265 7374  umber of nearest
-00014ad0: 206e 6569 6768 626f 7273 2074 6f20 7265   neighbors to re
-00014ae0: 7472 6965 7665 2028 6465 6661 756c 7420  trieve (default 
-00014af0: 6973 2031 3029 2e0a 2020 2020 2020 2020  is 10)..        
-00014b00: 2020 2020 6669 6c74 6572 3a20 4120 6669      filter: A fi
-00014b10: 6c74 6572 2065 7870 7265 7373 696f 6e20  lter expression 
-00014b20: 746f 2072 6573 7472 6963 7420 7468 6520  to restrict the 
-00014b30: 7365 6172 6368 2073 7061 6365 2028 6f70  search space (op
-00014b40: 7469 6f6e 616c 292e 0a20 2020 2020 2020  tional)..       
-00014b50: 2020 2020 206d 696e 5f73 636f 7265 3a20       min_score: 
-00014b60: 5468 6520 6d69 6e69 6d75 6d20 7369 6d69  The minimum simi
-00014b70: 6c61 7269 7479 2073 636f 7265 2066 6f72  larity score for
-00014b80: 206e 6569 6768 626f 7273 2074 6f20 6265   neighbors to be
-00014b90: 2063 6f6e 7369 6465 7265 6420 2864 6566   considered (def
-00014ba0: 6175 6c74 2069 7320 3029 2e0a 0a20 2020  ault is 0)...   
-00014bb0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
-00014bc0: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
-00014bd0: 7420 6f66 2074 7570 6c65 7320 7265 7072  t of tuples repr
-00014be0: 6573 656e 7469 6e67 2074 6865 206e 6561  esenting the nea
-00014bf0: 7265 7374 206e 6569 6768 626f 7273 2e0a  rest neighbors..
-00014c00: 2020 2020 2020 2020 2020 2020 4561 6368              Each
-00014c10: 2074 7570 6c65 2063 6f6e 7461 696e 733a   tuple contains:
-00014c20: 2060 2854 6865 2073 696d 696c 6172 6974   `(The similarit
-00014c30: 7920 7363 6f72 652c 2041 206c 6973 7420  y score, A list 
-00014c40: 6f66 2066 6561 7475 7265 2076 616c 7565  of feature value
-00014c50: 7329 600a 0a20 2020 2020 2020 2021 2121  s)`..        !!!
-00014c60: 2045 7861 6d70 6c65 0a20 2020 2020 2020   Example.       
-00014c70: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-00014c80: 2020 2020 2065 6d62 6564 6469 6e67 5f69       embedding_i
-00014c90: 6e64 6578 203d 2045 6d62 6564 6469 6e67  ndex = Embedding
-00014ca0: 496e 6465 7828 290a 2020 2020 2020 2020  Index().        
-00014cb0: 2020 2020 656d 6265 6464 696e 675f 696e      embedding_in
-00014cc0: 6465 782e 6164 645f 656d 6265 6464 696e  dex.add_embeddin
-00014cd0: 6728 6e61 6d65 3d22 7573 6572 5f76 6563  g(name="user_vec
-00014ce0: 746f 7222 2c20 6469 6d65 6e73 696f 6e3d  tor", dimension=
-00014cf0: 3329 0a20 2020 2020 2020 2020 2020 2066  3).            f
-00014d00: 6720 3d20 6673 2e63 7265 6174 655f 6665  g = fs.create_fe
-00014d10: 6174 7572 655f 6772 6f75 7028 0a20 2020  ature_group(.   
-00014d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d30: 2020 2020 206e 616d 653d 2761 6972 5f71       name='air_q
-00014d40: 7561 6c69 7479 272c 0a20 2020 2020 2020  uality',.       
-00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d60: 2065 6d62 6564 6469 6e67 5f69 6e64 6578   embedding_index
-00014d70: 203d 2065 6d62 6564 6469 6e67 5f69 6e64   = embedding_ind
-00014d80: 6578 2c0a 2020 2020 2020 2020 2020 2020  ex,.            
-00014d90: 2020 2020 2020 2020 2020 2020 7665 7273              vers
-00014da0: 696f 6e3d 312c 0a20 2020 2020 2020 2020  ion=1,.         
-00014db0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00014dc0: 7269 6d61 7279 5f6b 6579 3d5b 2769 6431  rimary_key=['id1
-00014dd0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00014de0: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
-00014df0: 6e65 5f65 6e61 626c 6564 3d54 7275 652c  ne_enabled=True,
-00014e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e10: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00014e20: 2020 2066 672e 696e 7365 7274 2864 6174     fg.insert(dat
-00014e30: 6129 0a20 2020 2020 2020 2020 2020 2066  a).            f
-00014e40: 672e 6669 6e64 5f6e 6569 6768 626f 7273  g.find_neighbors
-00014e50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014e60: 2020 5b30 2e31 2c20 302e 322c 2030 2e33    [0.1, 0.2, 0.3
-00014e70: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00014e80: 2020 206b 3d35 2c0a 2020 2020 2020 2020     k=5,.        
-00014e90: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00014ea0: 2020 2023 2061 7070 6c79 2066 696c 7465     # apply filte
-00014eb0: 720a 2020 2020 2020 2020 2020 2020 6667  r.            fg
-00014ec0: 2e66 696e 645f 6e65 6967 6862 6f72 7328  .find_neighbors(
-00014ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ee0: 205b 302e 312c 2030 2e32 2c20 302e 335d   [0.1, 0.2, 0.3]
-00014ef0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014f00: 2020 6b3d 352c 0a20 2020 2020 2020 2020    k=5,.         
-00014f10: 2020 2020 2020 2066 696c 7465 723d 2866         filter=(f
-00014f20: 672e 6964 3120 3e20 3130 2920 2620 2866  g.id1 > 10) & (f
-00014f30: 672e 6964 3120 3c20 3330 290a 2020 2020  g.id1 < 30).    
-00014f40: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00014f50: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00014f60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00014f70: 2073 656c 662e 5f76 6563 746f 725f 6462   self._vector_db
-00014f80: 5f63 6c69 656e 7420 6973 204e 6f6e 6520  _client is None 
-00014f90: 616e 6420 7365 6c66 2e5f 656d 6265 6464  and self._embedd
-00014fa0: 696e 675f 696e 6465 783a 0a20 2020 2020  ing_index:.     
-00014fb0: 2020 2020 2020 2073 656c 662e 5f76 6563         self._vec
-00014fc0: 746f 725f 6462 5f63 6c69 656e 7420 3d20  tor_db_client = 
-00014fd0: 5665 6374 6f72 4462 436c 6965 6e74 2873  VectorDbClient(s
-00014fe0: 656c 662e 7365 6c65 6374 5f61 6c6c 2829  elf.select_all()
-00014ff0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-00015000: 7320 3d20 7365 6c66 2e5f 7665 6374 6f72  s = self._vector
-00015010: 5f64 625f 636c 6965 6e74 2e66 696e 645f  _db_client.find_
-00015020: 6e65 6967 6862 6f72 7328 0a20 2020 2020  neighbors(.     
-00015030: 2020 2020 2020 2065 6d62 6564 6469 6e67         embedding
-00015040: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
-00015050: 6174 7572 653d 2873 656c 662e 5f5f 6765  ature=(self.__ge
-00015060: 7461 7474 725f 5f28 636f 6c29 2069 6620  tattr__(col) if 
-00015070: 636f 6c20 656c 7365 204e 6f6e 6529 2c0a  col else None),.
-00015080: 2020 2020 2020 2020 2020 2020 6b3d 6b2c              k=k,
-00015090: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-000150a0: 7465 723d 6669 6c74 6572 2c0a 2020 2020  ter=filter,.    
-000150b0: 2020 2020 2020 2020 6d69 6e5f 7363 6f72          min_scor
-000150c0: 653d 6d69 6e5f 7363 6f72 652c 0a20 2020  e=min_score,.   
-000150d0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-000150e0: 6574 7572 6e20 5b0a 2020 2020 2020 2020  eturn [.        
-000150f0: 2020 2020 2872 6573 756c 745b 305d 2c20      (result[0], 
-00015100: 5b72 6573 756c 745b 315d 5b66 2e6e 616d  [result[1][f.nam
-00015110: 655d 2066 6f72 2066 2069 6e20 7365 6c66  e] for f in self
-00015120: 2e66 6561 7475 7265 735d 290a 2020 2020  .features]).    
-00015130: 2020 2020 2020 2020 666f 7220 7265 7375          for resu
-00015140: 6c74 2069 6e20 7265 7375 6c74 730a 2020  lt in results.  
-00015150: 2020 2020 2020 5d0a 0a20 2020 2064 6566        ]..    def
-00015160: 2073 686f 7728 7365 6c66 2c20 6e3a 2069   show(self, n: i
-00015170: 6e74 2c20 6f6e 6c69 6e65 3a20 4f70 7469  nt, online: Opti
-00015180: 6f6e 616c 5b62 6f6f 6c5d 203d 2046 616c  onal[bool] = Fal
-00015190: 7365 293a 0a20 2020 2020 2020 2022 2222  se):.        """
-000151a0: 5368 6f77 2074 6865 2066 6972 7374 2060  Show the first `
-000151b0: 6e60 2072 6f77 7320 6f66 2074 6865 2066  n` rows of the f
-000151c0: 6561 7475 7265 2067 726f 7570 2e0a 0a20  eature group... 
-000151d0: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-000151e0: 6c65 0a20 2020 2020 2020 2020 2020 2060  le.            `
-000151f0: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-00015200: 2020 2020 2023 2063 6f6e 6e65 6374 2074       # connect t
-00015210: 6f20 7468 6520 4665 6174 7572 6520 5374  o the Feature St
-00015220: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
-00015230: 6673 203d 202e 2e2e 0a0a 2020 2020 2020  fs = .....      
-00015240: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
-00015250: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
-00015260: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
-00015270: 2020 2066 6720 3d20 6673 2e67 6574 5f6f     fg = fs.get_o
-00015280: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
-00015290: 5f67 726f 7570 282e 2e2e 290a 0a20 2020  _group(...)..   
-000152a0: 2020 2020 2020 2020 2023 206d 616b 6520           # make 
-000152b0: 6120 7175 6572 7920 616e 6420 7368 6f77  a query and show
-000152c0: 2074 6f70 2035 2072 6f77 730a 2020 2020   top 5 rows.    
-000152d0: 2020 2020 2020 2020 6667 2e73 656c 6563          fg.selec
-000152e0: 7428 5b27 6461 7465 272c 2777 6565 6b6c  t(['date','weekl
-000152f0: 795f 7361 6c65 7327 2c27 6973 5f68 6f6c  y_sales','is_hol
-00015300: 6964 6179 275d 292e 7368 6f77 2835 290a  iday']).show(5).
-00015310: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
-00015320: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-00015330: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00015340: 206e 3a20 696e 742e 204e 756d 6265 7220   n: int. Number 
-00015350: 6f66 2072 6f77 7320 746f 2073 686f 772e  of rows to show.
-00015360: 0a20 2020 2020 2020 2020 2020 206f 6e6c  .            onl
-00015370: 696e 653a 2062 6f6f 6c2c 206f 7074 696f  ine: bool, optio
-00015380: 6e61 6c2e 2049 6620 6054 7275 6560 2072  nal. If `True` r
-00015390: 6561 6420 6672 6f6d 206f 6e6c 696e 6520  ead from online 
-000153a0: 6665 6174 7572 6520 7374 6f72 652c 2064  feature store, d
-000153b0: 6566 6175 6c74 730a 2020 2020 2020 2020  efaults.        
-000153c0: 2020 2020 2020 2020 746f 2060 4661 6c73          to `Fals
-000153d0: 6560 2e0a 2020 2020 2020 2020 2222 220a  e`..        """.
-000153e0: 2020 2020 2020 2020 656e 6769 6e65 2e67          engine.g
-000153f0: 6574 5f69 6e73 7461 6e63 6528 292e 7365  et_instance().se
-00015400: 745f 6a6f 625f 6772 6f75 7028 0a20 2020  t_job_group(.   
-00015410: 2020 2020 2020 2020 2022 4665 7463 6869           "Fetchi
-00015420: 6e67 2046 6561 7475 7265 2067 726f 7570  ng Feature group
-00015430: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00015440: 4765 7474 696e 6720 6665 6174 7572 6520  Getting feature 
-00015450: 6772 6f75 703a 207b 7d20 6672 6f6d 2074  group: {} from t
-00015460: 6865 2066 6561 7475 7265 7374 6f72 6520  he featurestore 
-00015470: 7b7d 222e 666f 726d 6174 280a 2020 2020  {}".format(.    
-00015480: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015490: 2e5f 6e61 6d65 2c20 7365 6c66 2e5f 6665  ._name, self._fe
-000154a0: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
-000154b0: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-000154c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000154d0: 2020 6966 206f 6e6c 696e 6520 616e 6420    if online and 
-000154e0: 7365 6c66 2e65 6d62 6564 6469 6e67 5f69  self.embedding_i
-000154f0: 6e64 6578 3a0a 2020 2020 2020 2020 2020  ndex:.          
-00015500: 2020 6966 2073 656c 662e 5f76 6563 746f    if self._vecto
-00015510: 725f 6462 5f63 6c69 656e 7420 6973 204e  r_db_client is N
-00015520: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00015530: 2020 2020 2073 656c 662e 5f76 6563 746f       self._vecto
-00015540: 725f 6462 5f63 6c69 656e 7420 3d20 5665  r_db_client = Ve
-00015550: 6374 6f72 4462 436c 6965 6e74 2873 656c  ctorDbClient(sel
-00015560: 662e 7365 6c65 6374 5f61 6c6c 2829 290a  f.select_all()).
-00015570: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00015580: 6c74 7320 3d20 7365 6c66 2e5f 7665 6374  lts = self._vect
-00015590: 6f72 5f64 625f 636c 6965 6e74 2e72 6561  or_db_client.rea
-000155a0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-000155b0: 2020 2073 656c 662e 6964 2c0a 2020 2020     self.id,.    
-000155c0: 2020 2020 2020 2020 2020 2020 7b7d 2c0a              {},.
-000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 706b 3d73 656c 662e 656d 6265 6464 696e  pk=self.embeddin
-000155f0: 675f 696e 6465 782e 636f 6c5f 7072 6566  g_index.col_pref
-00015600: 6978 202b 2073 656c 662e 7072 696d 6172  ix + self.primar
-00015610: 795f 6b65 795b 305d 2c0a 2020 2020 2020  y_key[0],.      
-00015620: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-00015630: 6e61 6d65 3d73 656c 662e 656d 6265 6464  name=self.embedd
-00015640: 696e 675f 696e 6465 782e 696e 6465 785f  ing_index.index_
-00015650: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00015660: 2020 2020 2020 6e3d 6e2c 0a20 2020 2020        n=n,.     
-00015670: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00015680: 2020 2020 2072 6574 7572 6e20 5b5b 7265       return [[re
-00015690: 7375 6c74 5b66 2e6e 616d 655d 2066 6f72  sult[f.name] for
-000156a0: 2066 2069 6e20 7365 6c66 2e66 6561 7475   f in self.featu
-000156b0: 7265 735d 2066 6f72 2072 6573 756c 7420  res] for result 
-000156c0: 696e 2072 6573 756c 7473 5d0a 2020 2020  in results].    
-000156d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000156e0: 7365 6c65 6374 5f61 6c6c 2829 2e73 686f  select_all().sho
-000156f0: 7728 6e2c 206f 6e6c 696e 6529 0a0a 2020  w(n, online)..  
-00015700: 2020 6465 6620 7361 7665 280a 2020 2020    def save(.    
-00015710: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00015720: 2020 6665 6174 7572 6573 3a20 556e 696f    features: Unio
-00015730: 6e5b 0a20 2020 2020 2020 2020 2020 2070  n[.            p
-00015740: 642e 4461 7461 4672 616d 652c 0a20 2020  d.DataFrame,.   
-00015750: 2020 2020 2020 2020 2054 7970 6556 6172           TypeVar
-00015760: 2822 7079 7370 6172 6b2e 7371 6c2e 4461  ("pyspark.sql.Da
-00015770: 7461 4672 616d 6522 292c 2020 2320 6e6f  taFrame"),  # no
-00015780: 7161 3a20 4638 3231 0a20 2020 2020 2020  qa: F821.       
-00015790: 2020 2020 2054 7970 6556 6172 2822 7079       TypeVar("py
-000157a0: 7370 6172 6b2e 5244 4422 292c 2020 2320  spark.RDD"),  # 
-000157b0: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-000157c0: 2020 2020 2020 206e 702e 6e64 6172 7261         np.ndarra
-000157d0: 792c 0a20 2020 2020 2020 2020 2020 204c  y,.            L
-000157e0: 6973 745b 6665 6174 7572 652e 4665 6174  ist[feature.Feat
-000157f0: 7572 655d 2c0a 2020 2020 2020 2020 5d20  ure],.        ] 
-00015800: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00015810: 7772 6974 655f 6f70 7469 6f6e 733a 204f  write_options: O
-00015820: 7074 696f 6e61 6c5b 4469 6374 5b41 6e79  ptional[Dict[Any
-00015830: 2c20 416e 795d 5d20 3d20 7b7d 2c0a 2020  , Any]] = {},.  
-00015840: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00015850: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-00015860: 616c 5b44 6963 745b 416e 792c 2041 6e79  al[Dict[Any, Any
-00015870: 5d5d 203d 207b 7d2c 0a20 2020 2020 2020  ]] = {},.       
-00015880: 2077 6169 743a 2062 6f6f 6c20 3d20 4661   wait: bool = Fa
-00015890: 6c73 652c 0a20 2020 2029 3a0a 2020 2020  lse,.    ):.    
-000158a0: 2020 2020 2222 2250 6572 7369 7374 2074      """Persist t
-000158b0: 6865 206d 6574 6164 6174 6120 616e 6420  he metadata and 
-000158c0: 6d61 7465 7269 616c 697a 6520 7468 6520  materialize the 
-000158d0: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
-000158e0: 2074 6865 2066 6561 7475 7265 2073 746f   the feature sto
-000158f0: 7265 2e0a 0a20 2020 2020 2020 2021 2121  re...        !!!
-00015900: 2077 6172 6e69 6e67 2022 4368 616e 6765   warning "Change
-00015910: 6420 696e 2033 2e33 2e30 220a 2020 2020  d in 3.3.0".    
-00015920: 2020 2020 2020 2020 6069 6e73 6572 7460          `insert`
-00015930: 2061 6e64 2060 7361 7665 6020 6d65 7468   and `save` meth
-00015940: 6f64 7320 6172 6520 6e6f 7720 6173 796e  ods are now asyn
-00015950: 6320 6279 2064 6566 6175 6c74 2069 6e20  c by default in 
-00015960: 6e6f 6e2d 7370 6172 6b20 636c 6965 6e74  non-spark client
-00015970: 732e 0a20 2020 2020 2020 2020 2020 2054  s..            T
-00015980: 6f20 6163 6869 6576 6520 7468 6520 6f6c  o achieve the ol
-00015990: 6420 6265 6861 7669 6f75 722c 2073 6574  d behaviour, set
-000159a0: 2060 7761 6974 6020 6172 6775 6d65 6e74   `wait` argument
-000159b0: 2074 6f20 6054 7275 6560 2e0a 0a20 2020   to `True`...   
-000159c0: 2020 2020 2043 616c 6c69 6e67 2060 7361       Calling `sa
-000159d0: 7665 6020 6372 6561 7465 7320 7468 6520  ve` creates the 
-000159e0: 6d65 7461 6461 7461 2066 6f72 2074 6865  metadata for the
-000159f0: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
-00015a00: 6e20 7468 6520 6665 6174 7572 6520 7374  n the feature st
-00015a10: 6f72 652e 0a20 2020 2020 2020 2049 6620  ore..        If 
-00015a20: 6120 4461 7461 4672 616d 652c 2052 4444  a DataFrame, RDD
-00015a30: 206f 7220 4e64 6172 7261 7920 6973 2070   or Ndarray is p
-00015a40: 726f 7669 6465 642c 2074 6865 2064 6174  rovided, the dat
-00015a50: 6120 6973 2077 7269 7474 656e 2074 6f20  a is written to 
-00015a60: 7468 650a 2020 2020 2020 2020 6f6e 6c69  the.        onli
-00015a70: 6e65 2f6f 6666 6c69 6e65 2066 6561 7475  ne/offline featu
-00015a80: 7265 2073 746f 7265 2061 7320 7370 6563  re store as spec
-00015a90: 6966 6965 642e 0a20 2020 2020 2020 2042  ified..        B
-00015aa0: 7920 6465 6661 756c 742c 2074 6869 7320  y default, this 
-00015ab0: 7772 6974 6573 2074 6865 2066 6561 7475  writes the featu
-00015ac0: 7265 2067 726f 7570 2074 6f20 7468 6520  re group to the 
-00015ad0: 6f66 666c 696e 6520 7374 6f72 6167 652c  offline storage,
-00015ae0: 2061 6e64 2069 660a 2020 2020 2020 2020   and if.        
-00015af0: 606f 6e6c 696e 655f 656e 6162 6c65 6460  `online_enabled`
-00015b00: 2066 6f72 2074 6865 2066 6561 7475 7265   for the feature
-00015b10: 2067 726f 7570 2c20 616c 736f 2074 6f20   group, also to 
-00015b20: 7468 6520 6f6e 6c69 6e65 2066 6561 7475  the online featu
-00015b30: 7265 2073 746f 7265 2e0a 2020 2020 2020  re store..      
-00015b40: 2020 5468 6520 6066 6561 7475 7265 7360    The `features`
-00015b50: 2064 6174 6166 7261 6d65 2063 616e 2062   dataframe can b
-00015b60: 6520 6120 5370 6172 6b20 4461 7461 4672  e a Spark DataFr
-00015b70: 616d 6520 6f72 2052 4444 2c20 6120 5061  ame or RDD, a Pa
-00015b80: 6e64 6173 2044 6174 6146 7261 6d65 2c0a  ndas DataFrame,.
-00015b90: 2020 2020 2020 2020 6f72 2061 2074 776f          or a two
-00015ba0: 2d64 696d 656e 7369 6f6e 616c 204e 756d  -dimensional Num
-00015bb0: 7079 2061 7272 6179 206f 7220 6120 7477  py array or a tw
-00015bc0: 6f2d 6469 6d65 6e73 696f 6e61 6c20 5079  o-dimensional Py
-00015bd0: 7468 6f6e 206e 6573 7465 6420 6c69 7374  thon nested list
-00015be0: 2e0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
-00015bf0: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
-00015c00: 2020 6665 6174 7572 6573 3a20 4461 7461    features: Data
-00015c10: 4672 616d 652c 2052 4444 2c20 4e64 6172  Frame, RDD, Ndar
-00015c20: 7261 7920 6f72 2061 206c 6973 7420 6f66  ray or a list of
-00015c30: 2066 6561 7475 7265 732e 2046 6561 7475   features. Featu
-00015c40: 7265 7320 746f 2062 6520 7361 7665 642e  res to be saved.
-00015c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c60: 2054 6869 7320 6172 6775 6d65 6e74 2069   This argument i
-00015c70: 7320 6f70 7469 6f6e 616c 2069 6620 7468  s optional if th
-00015c80: 6520 6665 6174 7572 6520 6c69 7374 2069  e feature list i
-00015c90: 7320 7072 6f76 6964 6564 2069 6e20 7468  s provided in th
-00015ca0: 6520 6372 6561 7465 5f66 6561 7475 7265  e create_feature
-00015cb0: 5f67 726f 7570 206f 720a 2020 2020 2020  _group or.      
-00015cc0: 2020 2020 2020 2020 2020 696e 2074 6865            in the
-00015cd0: 2067 6574 5f6f 725f 6372 6561 7465 5f66   get_or_create_f
-00015ce0: 6561 7475 7265 5f67 726f 7570 206d 6574  eature_group met
-00015cf0: 686f 6420 696e 766f 6b61 7469 6f6e 2e0a  hod invokation..
-00015d00: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00015d10: 655f 6f70 7469 6f6e 733a 2041 6464 6974  e_options: Addit
-00015d20: 696f 6e61 6c20 7772 6974 6520 6f70 7469  ional write opti
-00015d30: 6f6e 7320 6173 206b 6579 2d76 616c 7565  ons as key-value
-00015d40: 2070 6169 7273 2c20 6465 6661 756c 7473   pairs, defaults
-00015d50: 2074 6f20 607b 7d60 2e0a 2020 2020 2020   to `{}`..      
-00015d60: 2020 2020 2020 2020 2020 5768 656e 2075            When u
-00015d70: 7369 6e67 2074 6865 2060 7079 7468 6f6e  sing the `python
-00015d80: 6020 656e 6769 6e65 2c20 7772 6974 655f  ` engine, write_
-00015d90: 6f70 7469 6f6e 7320 6361 6e20 636f 6e74  options can cont
-00015da0: 6169 6e20 7468 650a 2020 2020 2020 2020  ain the.        
-00015db0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
-00015dc0: 6720 656e 7472 6965 733a 0a20 2020 2020  g entries:.     
-00015dd0: 2020 2020 2020 2020 2020 202a 206b 6579             * key
-00015de0: 2060 7370 6172 6b60 2061 6e64 2076 616c   `spark` and val
-00015df0: 7565 2061 6e20 6f62 6a65 6374 206f 6620  ue an object of 
-00015e00: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
-00015e10: 2020 2020 205b 6873 6673 2e63 6f72 652e       [hsfs.core.
-00015e20: 6a6f 625f 636f 6e66 6967 7572 6174 696f  job_configuratio
-00015e30: 6e2e 4a6f 6243 6f6e 6669 6775 7261 7469  n.JobConfigurati
-00015e40: 6f6e 5d28 2e2e 2f6a 6f62 5f63 6f6e 6669  on](../job_confi
-00015e50: 6775 7261 7469 6f6e 290a 2020 2020 2020  guration).      
-00015e60: 2020 2020 2020 2020 2020 2020 746f 2063              to c
-00015e70: 6f6e 6669 6775 7265 2074 6865 2048 6f70  onfigure the Hop
-00015e80: 7377 6f72 6b73 204a 6f62 2075 7365 6420  sworks Job used 
-00015e90: 746f 2077 7269 7465 2064 6174 6120 696e  to write data in
-00015ea0: 746f 2074 6865 0a20 2020 2020 2020 2020  to the.         
-00015eb0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-00015ec0: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
-00015ed0: 2020 2020 2020 2020 2a20 6b65 7920 6077          * key `w
-00015ee0: 6169 745f 666f 725f 6a6f 6260 2061 6e64  ait_for_job` and
-00015ef0: 2076 616c 7565 2060 5472 7565 6020 6f72   value `True` or
-00015f00: 2060 4661 6c73 6560 2074 6f20 636f 6e66   `False` to conf
-00015f10: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
-00015f20: 2020 2020 2020 2020 7768 6574 6865 7220          whether 
-00015f30: 6f72 206e 6f74 2074 6f20 7468 6520 7361  or not to the sa
-00015f40: 7665 2063 616c 6c20 7368 6f75 6c64 2072  ve call should r
-00015f50: 6574 7572 6e20 6f6e 6c79 0a20 2020 2020  eturn only.     
-00015f60: 2020 2020 2020 2020 2020 2020 2061 6674               aft
-00015f70: 6572 2074 6865 2048 6f70 7377 6f72 6b73  er the Hopsworks
-00015f80: 204a 6f62 2068 6173 2066 696e 6973 6865   Job has finishe
-00015f90: 642e 2042 7920 6465 6661 756c 7420 6974  d. By default it
-00015fa0: 2064 6f65 7320 6e6f 7420 7761 6974 2e0a   does not wait..
-00015fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fc0: 2a20 6b65 7920 6073 7461 7274 5f6f 6666  * key `start_off
-00015fd0: 6c69 6e65 5f62 6163 6b66 696c 6c60 2061  line_backfill` a
-00015fe0: 6e64 2076 616c 7565 2060 5472 7565 6020  nd value `True` 
-00015ff0: 6f72 2060 4661 6c73 6560 2074 6f20 636f  or `False` to co
-00016000: 6e66 6967 7572 650a 2020 2020 2020 2020  nfigure.        
-00016010: 2020 2020 2020 2020 2020 7768 6574 6865            whethe
-00016020: 7220 6f72 206e 6f74 2074 6f20 7374 6172  r or not to star
-00016030: 7420 7468 6520 6d61 7465 7269 616c 697a  t the materializ
-00016040: 6174 696f 6e20 6a6f 6220 746f 2077 7269  ation job to wri
-00016050: 7465 2064 6174 6120 746f 2074 6865 206f  te data to the o
-00016060: 6666 6c69 6e65 0a20 2020 2020 2020 2020  ffline.         
-00016070: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-00016080: 2e20 6073 7461 7274 5f6f 6666 6c69 6e65  . `start_offline
-00016090: 5f62 6163 6b66 696c 6c60 2069 7320 6465  _backfill` is de
-000160a0: 7072 6563 6174 6564 2e20 5573 6520 6073  precated. Use `s
-000160b0: 7461 7274 5f6f 6666 6c69 6e65 5f6d 6174  tart_offline_mat
-000160c0: 6572 6961 6c69 7a61 7469 6f6e 6020 696e  erialization` in
-000160d0: 7374 6561 642e 0a20 2020 2020 2020 2020  stead..         
-000160e0: 2020 2020 2020 202a 206b 6579 2060 7374         * key `st
-000160f0: 6172 745f 6f66 666c 696e 655f 6d61 7465  art_offline_mate
-00016100: 7269 616c 697a 6174 696f 6e60 2061 6e64  rialization` and
-00016110: 2076 616c 7565 2060 5472 7565 6020 6f72   value `True` or
-00016120: 2060 4661 6c73 6560 2074 6f20 636f 6e66   `False` to conf
-00016130: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
-00016140: 2020 2020 2020 2020 7768 6574 6865 7220          whether 
-00016150: 6f72 206e 6f74 2074 6f20 7374 6172 7420  or not to start 
-00016160: 7468 6520 6d61 7465 7269 616c 697a 6174  the materializat
-00016170: 696f 6e20 6a6f 6220 746f 2077 7269 7465  ion job to write
-00016180: 2064 6174 6120 746f 2074 6865 206f 6666   data to the off
-00016190: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
-000161a0: 2020 2020 2020 2073 746f 7261 6765 2e20         storage. 
-000161b0: 4279 2064 6566 6175 6c74 2074 6865 206d  By default the m
-000161c0: 6174 6572 6961 6c69 7a61 7469 6f6e 206a  aterialization j
-000161d0: 6f62 2067 6574 7320 7374 6172 7465 6420  ob gets started 
-000161e0: 696d 6d65 6469 6174 656c 792e 0a20 2020  immediately..   
-000161f0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
-00016200: 6579 2060 6b61 666b 615f 7072 6f64 7563  ey `kafka_produc
-00016210: 6572 5f63 6f6e 6669 6760 2061 6e64 2076  er_config` and v
-00016220: 616c 7565 2061 6e20 6f62 6a65 6374 206f  alue an object o
-00016230: 6620 7479 7065 205b 7072 6f70 6572 7469  f type [properti
-00016240: 6573 5d28 6874 7470 733a 2f2f 646f 6373  es](https://docs
-00016250: 2e63 6f6e 666c 7565 6e74 2e69 6f2f 706c  .confluent.io/pl
-00016260: 6174 666f 726d 2f63 7572 7265 6e74 2f63  atform/current/c
-00016270: 6c69 656e 7473 2f6c 6962 7264 6b61 666b  lients/librdkafk
-00016280: 612f 6874 6d6c 2f6d 645f 434f 4e46 4947  a/html/md_CONFIG
-00016290: 5552 4154 494f 4e2e 6874 6d6c 6e29 0a20  URATION.htmln). 
-000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 2075 7365 6420 746f 2063 6f6e 6669 6775   used to configu
-000162c0: 7265 2074 6865 204b 6166 6b61 2063 6c69  re the Kafka cli
-000162d0: 656e 742e 2054 6f20 6f70 7469 6d69 7a65  ent. To optimize
-000162e0: 2066 6f72 2074 6872 6f75 6768 7075 7420   for throughput 
-000162f0: 696e 2068 6967 6820 6c61 7465 6e63 7920  in high latency 
-00016300: 636f 6e6e 6563 7469 6f6e 2c20 636f 6e73  connection, cons
-00016310: 6964 6572 0a20 2020 2020 2020 2020 2020  ider.           
-00016320: 2020 2020 2020 2063 6861 6e67 696e 6720         changing 
-00016330: 7468 6520 5b70 726f 6475 6365 7220 7072  the [producer pr
-00016340: 6f70 6572 7469 6573 5d28 6874 7470 733a  operties](https:
-00016350: 2f2f 646f 6373 2e63 6f6e 666c 7565 6e74  //docs.confluent
-00016360: 2e69 6f2f 636c 6f75 642f 6375 7272 656e  .io/cloud/curren
-00016370: 742f 636c 6965 6e74 2d61 7070 732f 6f70  t/client-apps/op
-00016380: 7469 6d69 7a69 6e67 2f74 6872 6f75 6768  timizing/through
-00016390: 7075 742e 6874 6d6c 2370 726f 6475 6365  put.html#produce
-000163a0: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
-000163b0: 2020 2020 2a20 6b65 7920 6069 6e74 6572      * key `inter
-000163c0: 6e61 6c5f 6b61 666b 6160 2061 6e64 2076  nal_kafka` and v
-000163d0: 616c 7565 2060 5472 7565 6020 6f72 2060  alue `True` or `
-000163e0: 4661 6c73 6560 2069 6e20 6361 7365 2079  False` in case y
-000163f0: 6f75 2065 7374 6162 6c69 7368 6564 0a20  ou established. 
-00016400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016410: 2063 6f6e 6e65 6374 6976 6974 7920 6672   connectivity fr
-00016420: 6f6d 2079 6f75 2050 7974 686f 6e20 656e  om you Python en
-00016430: 7669 726f 6e6d 656e 7420 746f 2074 6865  vironment to the
-00016440: 2069 6e74 6572 6e61 6c20 6164 7665 7274   internal advert
-00016450: 6973 6564 0a20 2020 2020 2020 2020 2020  ised.           
-00016460: 2020 2020 2020 206c 6973 7465 6e65 7273         listeners
-00016470: 206f 6620 7468 6520 486f 7073 776f 726b   of the Hopswork
-00016480: 7320 4b61 666b 6120 436c 7573 7465 722e  s Kafka Cluster.
-00016490: 2044 6566 6175 6c74 7320 746f 2060 4661   Defaults to `Fa
-000164a0: 6c73 6560 2061 6e64 0a20 2020 2020 2020  lse` and.       
-000164b0: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
-000164c0: 7573 6520 6578 7465 726e 616c 206c 6973  use external lis
-000164d0: 7465 6e65 7273 2077 6865 6e20 636f 6e6e  teners when conn
-000164e0: 6563 7469 6e67 2066 726f 6d20 6f75 7473  ecting from outs
-000164f0: 6964 6520 6f66 2048 6f70 7377 6f72 6b73  ide of Hopsworks
-00016500: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00016510: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-00016520: 3a20 4164 6469 7469 6f6e 616c 2076 616c  : Additional val
-00016530: 6964 6174 696f 6e20 6f70 7469 6f6e 7320  idation options 
-00016540: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
-00016550: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-00016560: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
-00016570: 2020 2020 2020 2a20 6b65 7920 6072 756e        * key `run
-00016580: 5f76 616c 6964 6174 696f 6e60 2062 6f6f  _validation` boo
-00016590: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
-000165a0: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
-000165b0: 6970 2076 616c 6964 6174 696f 6e20 7465  ip validation te
-000165c0: 6d70 6f72 6172 696c 7920 6f6e 2069 6e67  mporarily on ing
-000165d0: 6573 7469 6f6e 2e0a 2020 2020 2020 2020  estion..        
-000165e0: 2020 2020 2020 2020 2a20 6b65 7920 6073          * key `s
-000165f0: 6176 655f 7265 706f 7274 6020 626f 6f6c  ave_report` bool
-00016600: 6561 6e20 7661 6c75 652c 2073 6574 2074  ean value, set t
-00016610: 6f20 6046 616c 7365 6020 746f 2073 6b69  o `False` to ski
-00016620: 7020 7570 6c6f 6164 206f 6620 7468 6520  p upload of the 
-00016630: 7661 6c69 6461 7469 6f6e 2072 6570 6f72  validation repor
-00016640: 7420 746f 2048 6f70 7377 6f72 6b73 2e0a  t to Hopsworks..
-00016650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016660: 2a20 6b65 7920 6067 655f 7661 6c69 6461  * key `ge_valida
-00016670: 7465 5f6b 7761 7267 7360 2061 2064 6963  te_kwargs` a dic
-00016680: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-00016690: 6e67 206b 7761 7267 7320 666f 7220 7468  ng kwargs for th
-000166a0: 6520 7661 6c69 6461 7465 206d 6574 686f  e validate metho
-000166b0: 6420 6f66 2047 7265 6174 2045 7870 6563  d of Great Expec
-000166c0: 7461 7469 6f6e 732e 0a20 2020 2020 2020  tations..       
-000166d0: 2020 2020 2077 6169 743a 2057 6169 7420       wait: Wait 
-000166e0: 666f 7220 6a6f 6220 746f 2066 696e 6973  for job to finis
-000166f0: 6820 6265 666f 7265 2072 6574 7572 6e69  h before returni
-00016700: 6e67 2c20 6465 6661 756c 7473 2074 6f20  ng, defaults to 
-00016710: 6046 616c 7365 602e 0a20 2020 2020 2020  `False`..       
-00016720: 2020 2020 2020 2020 2053 686f 7274 6375           Shortcu
-00016730: 7420 666f 7220 7265 6164 5f6f 7074 696f  t for read_optio
-00016740: 6e73 2060 7b22 7761 6974 5f66 6f72 5f6a  ns `{"wait_for_j
-00016750: 6f62 223a 2046 616c 7365 7d60 2e0a 0a20  ob": False}`... 
-00016760: 2020 2020 2020 2023 2052 6574 7572 6e73         # Returns
-00016770: 0a20 2020 2020 2020 2020 2020 2060 4a6f  .            `Jo
-00016780: 6260 3a20 5768 656e 2075 7369 6e67 2074  b`: When using t
-00016790: 6865 2060 7079 7468 6f6e 6020 656e 6769  he `python` engi
-000167a0: 6e65 2c20 6974 2072 6574 7572 6e73 2074  ne, it returns t
-000167b0: 6865 2048 6f70 7377 6f72 6b73 204a 6f62  he Hopsworks Job
-000167c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000167d0: 2074 6861 7420 7761 7320 6c61 756e 6368   that was launch
-000167e0: 6564 2074 6f20 696e 6765 7374 2074 6865  ed to ingest the
-000167f0: 2066 6561 7475 7265 2067 726f 7570 2064   feature group d
-00016800: 6174 612e 0a0a 2020 2020 2020 2020 2320  ata...        # 
-00016810: 5261 6973 6573 0a20 2020 2020 2020 2020  Raises.         
-00016820: 2020 2060 6873 6673 2e63 6c69 656e 742e     `hsfs.client.
-00016830: 6578 6365 7074 696f 6e73 2e52 6573 7441  exceptions.RestA
-00016840: 5049 4572 726f 7260 2e20 556e 6162 6c65  PIError`. Unable
-00016850: 2074 6f20 6372 6561 7465 2066 6561 7475   to create featu
-00016860: 7265 2067 726f 7570 2e0a 2020 2020 2020  re group..      
-00016870: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00016880: 2028 6665 6174 7572 6573 2069 7320 4e6f   (features is No
-00016890: 6e65 2061 6e64 206c 656e 2873 656c 662e  ne and len(self.
-000168a0: 5f66 6561 7475 7265 7329 203e 2030 2920  _features) > 0) 
-000168b0: 6f72 2028 0a20 2020 2020 2020 2020 2020  or (.           
-000168c0: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
-000168d0: 7572 6573 2c20 4c69 7374 290a 2020 2020  ures, List).    
-000168e0: 2020 2020 2020 2020 616e 6420 6c65 6e28          and len(
-000168f0: 6665 6174 7572 6573 2920 3e20 300a 2020  features) > 0.  
-00016900: 2020 2020 2020 2020 2020 616e 6420 616c            and al
-00016910: 6c28 5b69 7369 6e73 7461 6e63 6528 662c  l([isinstance(f,
-00016920: 2066 6561 7475 7265 2e46 6561 7475 7265   feature.Feature
-00016930: 2920 666f 7220 6620 696e 2066 6561 7475  ) for f in featu
-00016940: 7265 735d 290a 2020 2020 2020 2020 293a  res]).        ):
-00016950: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00016960: 6869 7320 6973 2064 6f6e 6520 666f 7220  his is done for 
-00016970: 636f 6d70 6174 6962 696c 6974 792e 2055  compatibility. U
-00016980: 7365 7273 2063 616e 2073 7065 6369 6679  sers can specify
-00016990: 2074 6865 2066 6561 7475 7265 206c 6973   the feature lis
-000169a0: 7420 696e 2074 6865 0a20 2020 2020 2020  t in the.       
-000169b0: 2020 2020 2023 2028 6765 745f 6f72 5f29       # (get_or_)
-000169c0: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
-000169d0: 726f 7570 2e20 5573 6572 7320 6361 6e20  roup. Users can 
-000169e0: 616c 736f 2070 726f 7669 6465 2074 6865  also provide the
-000169f0: 2066 6561 7475 7265 206c 6973 7420 696e   feature list in
-00016a00: 2074 6865 2073 6176 6528 292e 0a20 2020   the save()..   
-00016a10: 2020 2020 2020 2020 2023 2054 686f 7567           # Thoug
-00016a20: 6820 6974 2773 2061 6e20 6f70 7469 6f6e  h it's an option
-00016a30: 616c 2070 6172 616d 6574 6572 2e0a 2020  al parameter..  
-00016a40: 2020 2020 2020 2020 2020 2320 466f 7220            # For 
-00016a50: 636f 6e73 6973 7465 6e63 7920 7265 6173  consistency reas
-00016a60: 6f6e 7320 6966 2074 6865 2075 7365 7220  ons if the user 
-00016a70: 7370 6563 6966 7920 626f 7468 2074 6865  specify both the
-00016a80: 2066 6561 7475 7265 206c 6973 7420 696e   feature list in
-00016a90: 2074 6865 2028 6765 745f 6f72 5f29 6372   the (get_or_)cr
-00016aa0: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-00016ab0: 7570 0a20 2020 2020 2020 2020 2020 2023  up.            #
-00016ac0: 2061 6e64 2069 6e20 7468 6520 6073 6176   and in the `sav
-00016ad0: 6528 2960 2063 616c 6c2c 2074 6865 6e20  e()` call, then 
-00016ae0: 7468 6520 2867 6574 5f6f 725f 2963 7265  the (get_or_)cre
-00016af0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
-00016b00: 7020 7769 6e73 2e0a 2020 2020 2020 2020  p wins..        
-00016b10: 2020 2020 2320 5468 6973 2069 7320 636f      # This is co
-00016b20: 6e73 6973 7465 6e74 2077 6974 6820 7468  nsistent with th
-00016b30: 6520 6265 6861 7669 6f72 206f 6620 7468  e behavior of th
-00016b40: 6520 696e 7365 7274 206d 6574 686f 6420  e insert method 
-00016b50: 7768 6572 6520 7468 6520 6665 6174 7572  where the featur
-00016b60: 6520 6c69 7374 2077 696e 7320 6f76 6572  e list wins over
-00016b70: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00016b80: 2023 2064 6174 6166 7261 6d65 2073 7472   # dataframe str
-00016b90: 7563 7475 7265 0a20 2020 2020 2020 2020  ucture.         
-00016ba0: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
-00016bb0: 7320 3d20 7365 6c66 2e5f 6665 6174 7572  s = self._featur
-00016bc0: 6573 2069 6620 6c65 6e28 7365 6c66 2e5f  es if len(self._
-00016bd0: 6665 6174 7572 6573 2920 3e20 3020 656c  features) > 0 el
-00016be0: 7365 2066 6561 7475 7265 730a 2020 2020  se features.    
-00016bf0: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
-00016c00: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-00016c10: 6e65 2e73 6176 655f 6665 6174 7572 655f  ne.save_feature_
-00016c20: 6772 6f75 705f 6d65 7461 6461 7461 280a  group_metadata(.
-00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c40: 7365 6c66 2c20 4e6f 6e65 2c20 7772 6974  self, None, writ
-00016c50: 655f 6f70 7469 6f6e 730a 2020 2020 2020  e_options.      
-00016c60: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00016c70: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00016c80: 2c20 4e6f 6e65 0a0a 2020 2020 2020 2020  , None..        
-00016c90: 6966 2066 6561 7475 7265 7320 6973 204e  if features is N
-00016ca0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016cb0: 2072 6169 7365 2046 6561 7475 7265 5374   raise FeatureSt
-00016cc0: 6f72 6545 7863 6570 7469 6f6e 280a 2020  oreException(.  
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2246                "F
-00016ce0: 6561 7475 7265 206c 6973 7420 6e6f 7420  eature list not 
-00016cf0: 7072 6f76 6964 6564 2069 6e20 7468 6520  provided in the 
-00016d00: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
-00016d10: 726f 7570 206f 7220 6765 745f 6f72 5f63  roup or get_or_c
-00016d20: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-00016d30: 6f75 7020 696e 766f 6b61 7469 6f6e 732e  oup invokations.
-00016d40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00016d50: 2020 2b20 2220 506c 6561 7365 2070 726f    + " Please pro
-00016d60: 7669 6465 2061 206c 6973 7420 6f66 2066  vide a list of f
-00016d70: 6561 7475 7265 7320 6f72 2061 2044 6174  eatures or a Dat
-00016d80: 6166 7261 6d65 220a 2020 2020 2020 2020  aframe".        
-00016d90: 2020 2020 290a 0a20 2020 2020 2020 2066      )..        f
-00016da0: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
-00016db0: 203d 2065 6e67 696e 652e 6765 745f 696e   = engine.get_in
-00016dc0: 7374 616e 6365 2829 2e63 6f6e 7665 7274  stance().convert
-00016dd0: 5f74 6f5f 6465 6661 756c 745f 6461 7461  _to_default_data
-00016de0: 6672 616d 6528 6665 6174 7572 6573 290a  frame(features).
-00016df0: 0a20 2020 2020 2020 2075 7365 725f 7665  .        user_ve
-00016e00: 7273 696f 6e20 3d20 7365 6c66 2e5f 7665  rsion = self._ve
-00016e10: 7273 696f 6e0a 0a20 2020 2020 2020 2069  rsion..        i
-00016e20: 6620 7772 6974 655f 6f70 7469 6f6e 7320  f write_options 
-00016e30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00016e40: 2020 2020 2077 7269 7465 5f6f 7074 696f       write_optio
-00016e50: 6e73 203d 207b 7d0a 2020 2020 2020 2020  ns = {}.        
-00016e60: 6966 2022 7761 6974 5f66 6f72 5f6a 6f62  if "wait_for_job
-00016e70: 2220 6e6f 7420 696e 2077 7269 7465 5f6f  " not in write_o
-00016e80: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
-00016e90: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
-00016ea0: 735b 2277 6169 745f 666f 725f 6a6f 6222  s["wait_for_job"
-00016eb0: 5d20 3d20 7761 6974 0a0a 2020 2020 2020  ] = wait..      
-00016ec0: 2020 2320 6667 5f6a 6f62 2069 7320 7573    # fg_job is us
-00016ed0: 6564 206f 6e6c 7920 6966 2074 6865 2070  ed only if the p
-00016ee0: 7974 686f 6e20 656e 6769 6e65 2069 7320  ython engine is 
-00016ef0: 7573 6564 0a20 2020 2020 2020 2066 675f  used.        fg_
-00016f00: 6a6f 622c 2067 655f 7265 706f 7274 203d  job, ge_report =
-00016f10: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
-00016f20: 726f 7570 5f65 6e67 696e 652e 7361 7665  roup_engine.save
-00016f30: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00016f40: 6c66 2c20 6665 6174 7572 655f 6461 7461  lf, feature_data
-00016f50: 6672 616d 652c 2077 7269 7465 5f6f 7074  frame, write_opt
-00016f60: 696f 6e73 2c20 7661 6c69 6461 7469 6f6e  ions, validation
-00016f70: 5f6f 7074 696f 6e73 0a20 2020 2020 2020  _options.       
-00016f80: 2029 0a20 2020 2020 2020 2069 6620 6765   ).        if ge
-00016f90: 5f72 6570 6f72 7420 6973 204e 6f6e 6520  _report is None 
-00016fa0: 6f72 2067 655f 7265 706f 7274 2e69 6e67  or ge_report.ing
-00016fb0: 6573 7469 6f6e 5f72 6573 756c 7420 3d3d  estion_result ==
-00016fc0: 2022 494e 4745 5354 4544 223a 0a20 2020   "INGESTED":.   
-00016fd0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00016fe0: 6f64 655f 656e 6769 6e65 2e73 6176 655f  ode_engine.save_
-00016ff0: 636f 6465 2873 656c 6629 0a0a 2020 2020  code(self)..    
-00017000: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00017010: 6973 7469 6373 5f63 6f6e 6669 672e 656e  istics_config.en
-00017020: 6162 6c65 6420 616e 6420 656e 6769 6e65  abled and engine
-00017030: 2e67 6574 5f74 7970 6528 292e 7374 6172  .get_type().star
-00017040: 7473 7769 7468 2822 7370 6172 6b22 293a  tswith("spark"):
-00017050: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
-00017060: 6e6c 7920 636f 6d70 7574 6520 7374 6174  nly compute stat
-00017070: 6973 7469 6373 2069 6620 7468 6520 656e  istics if the en
-00017080: 6769 6e65 2069 7320 5370 6172 6b2e 0a20  gine is Spark.. 
-00017090: 2020 2020 2020 2020 2020 2023 2046 6f72             # For
-000170a0: 2050 7974 686f 6e20 656e 6769 6e65 2c20   Python engine, 
-000170b0: 7468 6520 636f 6d70 7574 6174 696f 6e20  the computation 
-000170c0: 6861 7070 656e 7320 696e 2074 6865 2048  happens in the H
-000170d0: 6f70 7377 6f72 6b73 2061 7070 6c69 6361  opsworks applica
-000170e0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-000170f0: 2073 656c 662e 5f73 7461 7469 7374 6963   self._statistic
-00017100: 735f 656e 6769 6e65 2e63 6f6d 7075 7465  s_engine.compute
-00017110: 5f61 6e64 5f73 6176 655f 7374 6174 6973  _and_save_statis
-00017120: 7469 6373 2873 656c 662c 2066 6561 7475  tics(self, featu
-00017130: 7265 5f64 6174 6166 7261 6d65 290a 2020  re_dataframe).  
-00017140: 2020 2020 2020 6966 2075 7365 725f 7665        if user_ve
-00017150: 7273 696f 6e20 6973 204e 6f6e 653a 0a20  rsion is None:. 
-00017160: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-00017170: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-00017180: 2020 2020 2020 2020 2020 224e 6f20 7665            "No ve
-00017190: 7273 696f 6e20 7072 6f76 6964 6564 2066  rsion provided f
-000171a0: 6f72 2063 7265 6174 696e 6720 6665 6174  or creating feat
-000171b0: 7572 6520 6772 6f75 7020 607b 7d60 2c20  ure group `{}`, 
-000171c0: 696e 6372 656d 656e 7465 6420 7665 7273  incremented vers
-000171d0: 696f 6e20 746f 2060 7b7d 602e 222e 666f  ion to `{}`.".fo
-000171e0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000171f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00017200: 6e61 6d65 2c20 7365 6c66 2e5f 7665 7273  name, self._vers
-00017210: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00017220: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00017230: 2020 2020 2020 2075 7469 6c2e 5665 7273         util.Vers
-00017240: 696f 6e57 6172 6e69 6e67 2c0a 2020 2020  ionWarning,.    
-00017250: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017260: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-00017270: 2020 2020 2020 2066 675f 6a6f 622c 0a20         fg_job,. 
-00017280: 2020 2020 2020 2020 2020 2067 655f 7265             ge_re
-00017290: 706f 7274 2e74 6f5f 6765 5f74 7970 6528  port.to_ge_type(
-000172a0: 2920 6966 2067 655f 7265 706f 7274 2069  ) if ge_report i
-000172b0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-000172c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 290a  None,.        ).
-000172d0: 0a20 2020 2064 6566 2069 6e73 6572 7428  .    def insert(
-000172e0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000172f0: 2020 2020 2020 2066 6561 7475 7265 733a         features:
-00017300: 2055 6e69 6f6e 5b0a 2020 2020 2020 2020   Union[.        
-00017310: 2020 2020 7064 2e44 6174 6146 7261 6d65      pd.DataFrame
-00017320: 2c0a 2020 2020 2020 2020 2020 2020 5479  ,.            Ty
-00017330: 7065 5661 7228 2270 7973 7061 726b 2e73  peVar("pyspark.s
-00017340: 716c 2e44 6174 6146 7261 6d65 2229 2c20  ql.DataFrame"), 
-00017350: 2023 206e 6f71 613a 2046 3832 310a 2020   # noqa: F821.  
-00017360: 2020 2020 2020 2020 2020 5479 7065 5661            TypeVa
-00017370: 7228 2270 7973 7061 726b 2e52 4444 2229  r("pyspark.RDD")
-00017380: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
-00017390: 2020 2020 2020 2020 2020 2020 6e70 2e6e              np.n
-000173a0: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
-000173b0: 2020 2020 4c69 7374 5b6c 6973 745d 2c0a      List[list],.
-000173c0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-000173d0: 2020 206f 7665 7277 7269 7465 3a20 4f70     overwrite: Op
-000173e0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
-000173f0: 616c 7365 2c0a 2020 2020 2020 2020 6f70  alse,.        op
-00017400: 6572 6174 696f 6e3a 204f 7074 696f 6e61  eration: Optiona
-00017410: 6c5b 7374 725d 203d 2022 7570 7365 7274  l[str] = "upsert
-00017420: 222c 0a20 2020 2020 2020 2073 746f 7261  ",.        stora
-00017430: 6765 3a20 4f70 7469 6f6e 616c 5b73 7472  ge: Optional[str
-00017440: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00017450: 2020 7772 6974 655f 6f70 7469 6f6e 733a    write_options:
-00017460: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-00017470: 7472 2c20 416e 795d 5d20 3d20 7b7d 2c0a  tr, Any]] = {},.
-00017480: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
-00017490: 6f6e 5f6f 7074 696f 6e73 3a20 4f70 7469  on_options: Opti
-000174a0: 6f6e 616c 5b44 6963 745b 7374 722c 2041  onal[Dict[str, A
-000174b0: 6e79 5d5d 203d 207b 7d2c 0a20 2020 2020  ny]] = {},.     
-000174c0: 2020 2073 6176 655f 636f 6465 3a20 4f70     save_code: Op
-000174d0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2054  tional[bool] = T
-000174e0: 7275 652c 0a20 2020 2020 2020 2077 6169  rue,.        wai
-000174f0: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-00017500: 0a20 2020 2029 202d 3e20 5475 706c 655b  .    ) -> Tuple[
-00017510: 4f70 7469 6f6e 616c 5b4a 6f62 5d2c 204f  Optional[Job], O
-00017520: 7074 696f 6e61 6c5b 5661 6c69 6461 7469  ptional[Validati
-00017530: 6f6e 5265 706f 7274 5d5d 3a0a 2020 2020  onReport]]:.    
-00017540: 2020 2020 2222 2250 6572 7369 7374 2074      """Persist t
-00017550: 6865 206d 6574 6164 6174 6120 616e 6420  he metadata and 
-00017560: 6d61 7465 7269 616c 697a 6520 7468 6520  materialize the 
-00017570: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
-00017580: 2074 6865 2066 6561 7475 7265 2073 746f   the feature sto
-00017590: 7265 0a20 2020 2020 2020 206f 7220 696e  re.        or in
-000175a0: 7365 7274 2064 6174 6120 6672 6f6d 2061  sert data from a
-000175b0: 2064 6174 6166 7261 6d65 2069 6e74 6f20   dataframe into 
-000175c0: 7468 6520 6578 6973 7469 6e67 2066 6561  the existing fea
-000175d0: 7475 7265 2067 726f 7570 2e0a 0a20 2020  ture group...   
-000175e0: 2020 2020 2049 6e63 7265 6d65 6e74 616c       Incremental
-000175f0: 6c79 2069 6e73 6572 7420 6461 7461 2074  ly insert data t
-00017600: 6f20 6120 6665 6174 7572 6520 6772 6f75  o a feature grou
-00017610: 7020 6f72 206f 7665 7277 7269 7465 2061  p or overwrite a
-00017620: 6c6c 2064 6174 6120 636f 6e74 6169 6e65  ll data containe
-00017630: 6420 696e 2074 6865 2066 6561 7475 7265  d in the feature
-00017640: 2067 726f 7570 2e20 4279 0a20 2020 2020   group. By.     
-00017650: 2020 2064 6566 6175 6c74 2c20 7468 6520     default, the 
-00017660: 6461 7461 2069 7320 696e 7365 7274 6564  data is inserted
-00017670: 2069 6e74 6f20 7468 6520 6f66 666c 696e   into the offlin
-00017680: 6520 7374 6f72 6167 6520 6173 2077 656c  e storage as wel
-00017690: 6c20 6173 2074 6865 206f 6e6c 696e 6520  l as the online 
-000176a0: 7374 6f72 6167 6520 6966 2074 6865 2066  storage if the f
-000176b0: 6561 7475 7265 2067 726f 7570 2069 730a  eature group is.
-000176c0: 2020 2020 2020 2020 606f 6e6c 696e 655f          `online_
-000176d0: 656e 6162 6c65 643d 5472 7565 602e 0a0a  enabled=True`...
-000176e0: 2020 2020 2020 2020 5468 6520 6066 6561          The `fea
-000176f0: 7475 7265 7360 2064 6174 6166 7261 6d65  tures` dataframe
-00017700: 2063 616e 2062 6520 6120 5370 6172 6b20   can be a Spark 
-00017710: 4461 7461 4672 616d 6520 6f72 2052 4444  DataFrame or RDD
-00017720: 2c20 6120 5061 6e64 6173 2044 6174 6146  , a Pandas DataF
-00017730: 7261 6d65 2c0a 2020 2020 2020 2020 6f72  rame,.        or
-00017740: 2061 2074 776f 2d64 696d 656e 7369 6f6e   a two-dimension
-00017750: 616c 204e 756d 7079 2061 7272 6179 206f  al Numpy array o
-00017760: 7220 6120 7477 6f2d 6469 6d65 6e73 696f  r a two-dimensio
-00017770: 6e61 6c20 5079 7468 6f6e 206e 6573 7465  nal Python neste
-00017780: 6420 6c69 7374 2e0a 2020 2020 2020 2020  d list..        
-00017790: 4966 2073 7461 7469 7374 6963 7320 6172  If statistics ar
-000177a0: 6520 656e 6162 6c65 642c 2073 7461 7469  e enabled, stati
-000177b0: 7374 6963 7320 6172 6520 7265 636f 6d70  stics are recomp
-000177c0: 7574 6564 2066 6f72 2074 6865 2065 6e74  uted for the ent
-000177d0: 6972 6520 6665 6174 7572 650a 2020 2020  ire feature.    
-000177e0: 2020 2020 6772 6f75 702e 0a20 2020 2020      group..     
-000177f0: 2020 2049 6620 6665 6174 7572 6520 6772     If feature gr
-00017800: 6f75 7027 7320 7469 6d65 2074 7261 7665  oup's time trave
-00017810: 6c20 666f 726d 6174 2069 7320 6048 5544  l format is `HUD
-00017820: 4960 2074 6865 6e20 606f 7065 7261 7469  I` then `operati
-00017830: 6f6e 6020 6172 6775 6d65 6e74 2063 616e  on` argument can
-00017840: 2062 650a 2020 2020 2020 2020 6569 7468   be.        eith
-00017850: 6572 2060 696e 7365 7274 6020 6f72 2060  er `insert` or `
-00017860: 7570 7365 7274 602e 0a0a 2020 2020 2020  upsert`...      
-00017870: 2020 4966 2066 6561 7475 7265 2067 726f    If feature gro
-00017880: 7570 2064 6f65 736e 2774 2065 7869 7374  up doesn't exist
-00017890: 2074 6865 2069 6e73 6572 7420 6d65 7468   the insert meth
-000178a0: 6f64 2077 696c 6c20 6372 6561 7465 2074  od will create t
-000178b0: 6865 206e 6563 6573 7361 7279 206d 6574  he necessary met
-000178c0: 6164 6174 6120 7468 6520 6669 7273 7420  adata the first 
-000178d0: 7469 6d65 2069 7420 6973 0a20 2020 2020  time it is.     
-000178e0: 2020 2069 6e76 6f6b 6564 2061 6e64 2077     invoked and w
-000178f0: 7269 7465 7320 7468 6520 7370 6563 6966  rites the specif
-00017900: 6965 6420 6066 6561 7475 7265 7360 2064  ied `features` d
-00017910: 6174 6166 7261 6d65 2061 7320 6665 6174  ataframe as feat
-00017920: 7572 6520 6772 6f75 7020 746f 2074 6865  ure group to the
-00017930: 206f 6e6c 696e 652f 6f66 666c 696e 6520   online/offline 
-00017940: 6665 6174 7572 6520 7374 6f72 652e 0a0a  feature store...
-00017950: 2020 2020 2020 2020 2121 2120 7761 726e          !!! warn
-00017960: 696e 6720 2243 6861 6e67 6564 2069 6e20  ing "Changed in 
-00017970: 332e 332e 3022 0a20 2020 2020 2020 2020  3.3.0".         
-00017980: 2020 2060 696e 7365 7274 6020 616e 6420     `insert` and 
-00017990: 6073 6176 6560 206d 6574 686f 6473 2061  `save` methods a
-000179a0: 7265 206e 6f77 2061 7379 6e63 2062 7920  re now async by 
-000179b0: 6465 6661 756c 7420 696e 206e 6f6e 2d73  default in non-s
-000179c0: 7061 726b 2063 6c69 656e 7473 2e0a 2020  park clients..  
-000179d0: 2020 2020 2020 2020 2020 546f 2061 6368            To ach
-000179e0: 6965 7665 2074 6865 206f 6c64 2062 6568  ieve the old beh
-000179f0: 6176 696f 7572 2c20 7365 7420 6077 6169  aviour, set `wai
-00017a00: 7460 2061 7267 756d 656e 7420 746f 2060  t` argument to `
-00017a10: 5472 7565 602e 0a0a 2020 2020 2020 2020  True`...        
-00017a20: 2121 2120 6578 616d 706c 6520 2255 7073  !!! example "Ups
-00017a30: 6572 7420 6e65 7720 6665 6174 7572 6520  ert new feature 
-00017a40: 6461 7461 2077 6974 6820 7469 6d65 2074  data with time t
-00017a50: 7261 7665 6c20 666f 726d 6174 2060 4855  ravel format `HU
-00017a60: 4449 6022 0a20 2020 2020 2020 2020 2020  DI`".           
-00017a70: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00017a80: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-00017a90: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-00017aa0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-00017ab0: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-00017ac0: 2020 2020 2020 2020 6667 203d 2066 732e          fg = fs.
-00017ad0: 6765 745f 6f72 5f63 7265 6174 655f 6665  get_or_create_fe
-00017ae0: 6174 7572 655f 6772 6f75 7028 0a20 2020  ature_group(.   
-00017af0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00017b00: 653d 2762 6974 636f 696e 5f70 7269 6365  e='bitcoin_price
-00017b10: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00017b20: 2020 2064 6573 6372 6970 7469 6f6e 3d27     description='
-00017b30: 4269 7463 6f69 6e20 7072 6963 6520 6167  Bitcoin price ag
-00017b40: 6772 6567 6174 6564 2066 6f72 2064 6179  gregated for day
-00017b50: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-00017b60: 2020 2020 7665 7273 696f 6e3d 312c 0a20      version=1,. 
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00017b80: 7269 6d61 7279 5f6b 6579 3d5b 2775 6e69  rimary_key=['uni
-00017b90: 7827 5d2c 0a20 2020 2020 2020 2020 2020  x'],.           
-00017ba0: 2020 2020 206f 6e6c 696e 655f 656e 6162       online_enab
-00017bb0: 6c65 643d 5472 7565 2c0a 2020 2020 2020  led=True,.      
-00017bc0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
-00017bd0: 7469 6d65 3d27 756e 6978 270a 2020 2020  time='unix'.    
-00017be0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00017bf0: 2020 2020 2020 2066 672e 696e 7365 7274         fg.insert
-00017c00: 2864 665f 6269 7463 6f69 6e5f 7072 6f63  (df_bitcoin_proc
-00017c10: 6573 7365 6429 0a20 2020 2020 2020 2020  essed).         
-00017c20: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
-00017c30: 2121 2120 6578 616d 706c 6520 2241 7379  !!! example "Asy
-00017c40: 6e63 2069 6e73 6572 7422 0a20 2020 2020  nc insert".     
-00017c50: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00017c60: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00017c70: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
-00017c80: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
-00017c90: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
-00017ca0: 0a0a 2020 2020 2020 2020 2020 2020 6667  ..            fg
-00017cb0: 3120 3d20 6673 2e67 6574 5f6f 725f 6372  1 = fs.get_or_cr
-00017cc0: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-00017cd0: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
-00017ce0: 2020 2020 6e61 6d65 3d27 6665 6174 7572      name='featur
-00017cf0: 655f 6772 6f75 705f 6e61 6d65 3127 2c0a  e_group_name1',.
-00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d10: 6465 7363 7269 7074 696f 6e3d 2744 6573  description='Des
-00017d20: 6372 6970 7469 6f6e 206f 6620 7468 6520  cription of the 
-00017d30: 6669 7273 7420 4647 272c 0a20 2020 2020  first FG',.     
-00017d40: 2020 2020 2020 2020 2020 2076 6572 7369             versi
-00017d50: 6f6e 3d31 2c0a 2020 2020 2020 2020 2020  on=1,.          
-00017d60: 2020 2020 2020 7072 696d 6172 795f 6b65        primary_ke
-00017d70: 793d 5b27 756e 6978 275d 2c0a 2020 2020  y=['unix'],.    
-00017d80: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
-00017d90: 6e65 5f65 6e61 626c 6564 3d54 7275 652c  ne_enabled=True,
-00017da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017db0: 2065 7665 6e74 5f74 696d 653d 2775 6e69   event_time='uni
-00017dc0: 7827 0a20 2020 2020 2020 2020 2020 2029  x'.            )
-00017dd0: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
-00017de0: 7379 6e63 2069 6e73 6572 7469 6f6e 2069  sync insertion i
-00017df0: 6e20 6f72 6465 7220 6e6f 7420 746f 2077  n order not to w
-00017e00: 6169 7420 7469 6c6c 2066 696e 6973 6820  ait till finish 
-00017e10: 6f66 2074 6865 206a 6f62 0a20 2020 2020  of the job.     
-00017e20: 2020 2020 2020 2066 672e 696e 7365 7274         fg.insert
-00017e30: 2864 665f 666f 725f 6667 312c 2077 7269  (df_for_fg1, wri
-00017e40: 7465 5f6f 7074 696f 6e73 3d7b 2277 6169  te_options={"wai
-00017e50: 745f 666f 725f 6a6f 6222 203a 2046 616c  t_for_job" : Fal
-00017e60: 7365 7d29 0a0a 2020 2020 2020 2020 2020  se})..          
-00017e70: 2020 6667 3220 3d20 6673 2e67 6574 5f6f    fg2 = fs.get_o
-00017e80: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
-00017e90: 5f67 726f 7570 280a 2020 2020 2020 2020  _group(.        
-00017ea0: 2020 2020 2020 2020 6e61 6d65 3d27 6665          name='fe
-00017eb0: 6174 7572 655f 6772 6f75 705f 6e61 6d65  ature_group_name
-00017ec0: 3227 2c0a 2020 2020 2020 2020 2020 2020  2',.            
-00017ed0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00017ee0: 2744 6573 6372 6970 7469 6f6e 206f 6620  'Description of 
-00017ef0: 7468 6520 7365 636f 6e64 2046 4727 2c0a  the second FG',.
-00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f10: 7665 7273 696f 6e3d 312c 0a20 2020 2020  version=1,.     
-00017f20: 2020 2020 2020 2020 2020 2070 7269 6d61             prima
-00017f30: 7279 5f6b 6579 3d5b 2775 6e69 7827 5d2c  ry_key=['unix'],
-00017f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017f50: 206f 6e6c 696e 655f 656e 6162 6c65 643d   online_enabled=
-00017f60: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00017f70: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
-00017f80: 3d27 756e 6978 270a 2020 2020 2020 2020  ='unix'.        
-00017f90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00017fa0: 2020 6667 2e69 6e73 6572 7428 6466 5f66    fg.insert(df_f
-00017fb0: 6f72 5f66 6732 290a 2020 2020 2020 2020  or_fg2).        
-00017fc0: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
-00017fd0: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
-00017fe0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-00017ff0: 733a 2044 6174 6146 7261 6d65 2c20 5244  s: DataFrame, RD
-00018000: 442c 204e 6461 7272 6179 2c20 6c69 7374  D, Ndarray, list
-00018010: 2e20 4665 6174 7572 6573 2074 6f20 6265  . Features to be
-00018020: 2073 6176 6564 2e0a 2020 2020 2020 2020   saved..        
-00018030: 2020 2020 6f76 6572 7772 6974 653a 2044      overwrite: D
-00018040: 726f 7020 616c 6c20 6461 7461 2069 6e20  rop all data in 
-00018050: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-00018060: 7020 6265 666f 7265 0a20 2020 2020 2020  p before.       
-00018070: 2020 2020 2020 2020 2069 6e73 6572 7469           inserti
-00018080: 6e67 206e 6577 2064 6174 612e 2054 6869  ng new data. Thi
-00018090: 7320 646f 6573 206e 6f74 2061 6666 6563  s does not affec
-000180a0: 7420 6d65 7461 6461 7461 2c20 6465 6661  t metadata, defa
-000180b0: 756c 7473 2074 6f20 4661 6c73 652e 0a20  ults to False.. 
-000180c0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-000180d0: 7469 6f6e 3a20 4170 6163 6865 2048 7564  tion: Apache Hud
-000180e0: 6920 6f70 6572 6174 696f 6e20 7479 7065  i operation type
-000180f0: 2060 2269 6e73 6572 7422 6020 6f72 2060   `"insert"` or `
-00018100: 2275 7073 6572 7422 602e 0a20 2020 2020  "upsert"`..     
-00018110: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00018120: 6c74 7320 746f 2060 2275 7073 6572 7422  lts to `"upsert"
-00018130: 602e 0a20 2020 2020 2020 2020 2020 2073  `..            s
-00018140: 746f 7261 6765 3a20 4f76 6572 7772 6974  torage: Overwrit
-00018150: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
-00018160: 6f75 722c 2077 7269 7465 2074 6f20 6f66  our, write to of
-00018170: 666c 696e 650a 2020 2020 2020 2020 2020  fline.          
-00018180: 2020 2020 2020 7374 6f72 6167 6520 6f6e        storage on
-00018190: 6c79 2077 6974 6820 6022 6f66 666c 696e  ly with `"offlin
-000181a0: 6522 6020 6f72 206f 6e6c 696e 6520 6f6e  e"` or online on
-000181b0: 6c79 2077 6974 6820 6022 6f6e 6c69 6e65  ly with `"online
-000181c0: 2260 2c20 6465 6661 756c 7473 0a20 2020  "`, defaults.   
-000181d0: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
-000181e0: 604e 6f6e 6560 2028 4966 2074 6865 2073  `None` (If the s
-000181f0: 7472 6561 6d69 6e67 2041 5049 7320 6172  treaming APIs ar
-00018200: 6520 656e 6162 6c65 642c 2073 7065 6369  e enabled, speci
-00018210: 6679 696e 6720 7468 6520 7374 6f72 6167  fying the storag
-00018220: 6520 6f70 7469 6f6e 2069 7320 6e6f 7420  e option is not 
-00018230: 7375 7070 6f72 7465 6429 2e0a 2020 2020  supported)..    
-00018240: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-00018250: 7469 6f6e 733a 2041 6464 6974 696f 6e61  tions: Additiona
-00018260: 6c20 7772 6974 6520 6f70 7469 6f6e 7320  l write options 
-00018270: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
-00018280: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-00018290: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
-000182a0: 2020 2020 2020 5768 656e 2075 7369 6e67        When using
-000182b0: 2074 6865 2060 7079 7468 6f6e 6020 656e   the `python` en
-000182c0: 6769 6e65 2c20 7772 6974 655f 6f70 7469  gine, write_opti
-000182d0: 6f6e 7320 6361 6e20 636f 6e74 6169 6e20  ons can contain 
-000182e0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-000182f0: 2020 2020 666f 6c6c 6f77 696e 6720 656e      following en
-00018300: 7472 6965 733a 0a20 2020 2020 2020 2020  tries:.         
-00018310: 2020 2020 2020 202a 206b 6579 2060 7370         * key `sp
-00018320: 6172 6b60 2061 6e64 2076 616c 7565 2061  ark` and value a
-00018330: 6e20 6f62 6a65 6374 206f 6620 7479 7065  n object of type
-00018340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018350: 205b 6873 6673 2e63 6f72 652e 6a6f 625f   [hsfs.core.job_
-00018360: 636f 6e66 6967 7572 6174 696f 6e2e 4a6f  configuration.Jo
-00018370: 6243 6f6e 6669 6775 7261 7469 6f6e 5d28  bConfiguration](
-00018380: 2e2e 2f6a 6f62 5f63 6f6e 6669 6775 7261  ../job_configura
-00018390: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-000183a0: 2020 2020 2020 2020 746f 2063 6f6e 6669          to confi
-000183b0: 6775 7265 2074 6865 2048 6f70 7377 6f72  gure the Hopswor
-000183c0: 6b73 204a 6f62 2075 7365 6420 746f 2077  ks Job used to w
-000183d0: 7269 7465 2064 6174 6120 696e 746f 2074  rite data into t
-000183e0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
-000183f0: 2020 2020 2066 6561 7475 7265 2067 726f       feature gro
-00018400: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
-00018410: 2020 2020 2a20 6b65 7920 6077 6169 745f      * key `wait_
-00018420: 666f 725f 6a6f 6260 2061 6e64 2076 616c  for_job` and val
-00018430: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
-00018440: 6c73 6560 2074 6f20 636f 6e66 6967 7572  lse` to configur
-00018450: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00018460: 2020 2020 7768 6574 6865 7220 6f72 206e      whether or n
-00018470: 6f74 2074 6f20 7468 6520 696e 7365 7274  ot to the insert
-00018480: 2063 616c 6c20 7368 6f75 6c64 2072 6574   call should ret
-00018490: 7572 6e20 6f6e 6c79 0a20 2020 2020 2020  urn only.       
-000184a0: 2020 2020 2020 2020 2020 2061 6674 6572             after
-000184b0: 2074 6865 2048 6f70 7377 6f72 6b73 204a   the Hopsworks J
-000184c0: 6f62 2068 6173 2066 696e 6973 6865 642e  ob has finished.
-000184d0: 2042 7920 6465 6661 756c 7420 6974 2077   By default it w
-000184e0: 6169 7473 2e0a 2020 2020 2020 2020 2020  aits..          
-000184f0: 2020 2020 2020 2a20 6b65 7920 6073 7461        * key `sta
-00018500: 7274 5f6f 6666 6c69 6e65 5f62 6163 6b66  rt_offline_backf
-00018510: 696c 6c60 2061 6e64 2076 616c 7565 2060  ill` and value `
-00018520: 5472 7565 6020 6f72 2060 4661 6c73 6560  True` or `False`
-00018530: 2074 6f20 636f 6e66 6967 7572 650a 2020   to configure.  
-00018540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018550: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
-00018560: 6f20 7374 6172 7420 7468 6520 6d61 7465  o start the mate
-00018570: 7269 616c 697a 6174 696f 6e20 6a6f 6220  rialization job 
-00018580: 746f 2077 7269 7465 2064 6174 6120 746f  to write data to
-00018590: 2074 6865 206f 6666 6c69 6e65 0a20 2020   the offline.   
-000185a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000185b0: 746f 7261 6765 2e20 6073 7461 7274 5f6f  torage. `start_o
-000185c0: 6666 6c69 6e65 5f62 6163 6b66 696c 6c60  ffline_backfill`
-000185d0: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-000185e0: 5573 6520 6073 7461 7274 5f6f 6666 6c69  Use `start_offli
-000185f0: 6e65 5f6d 6174 6572 6961 6c69 7a61 7469  ne_materializati
-00018600: 6f6e 6020 696e 7374 6561 642e 0a20 2020  on` instead..   
-00018610: 2020 2020 2020 2020 2020 2020 202a 206b               * k
-00018620: 6579 2060 7374 6172 745f 6f66 666c 696e  ey `start_offlin
-00018630: 655f 6d61 7465 7269 616c 697a 6174 696f  e_materializatio
-00018640: 6e60 2061 6e64 2076 616c 7565 2060 5472  n` and value `Tr
-00018650: 7565 6020 6f72 2060 4661 6c73 6560 2074  ue` or `False` t
-00018660: 6f20 636f 6e66 6967 7572 650a 2020 2020  o configure.    
-00018670: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-00018680: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
-00018690: 7374 6172 7420 7468 6520 6d61 7465 7269  start the materi
-000186a0: 616c 697a 6174 696f 6e20 6a6f 6220 746f  alization job to
-000186b0: 2077 7269 7465 2064 6174 6120 746f 2074   write data to t
-000186c0: 6865 206f 6666 6c69 6e65 0a20 2020 2020  he offline.     
-000186d0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-000186e0: 7261 6765 2e20 4279 2064 6566 6175 6c74  rage. By default
-000186f0: 2074 6865 206d 6174 6572 6961 6c69 7a61   the materializa
-00018700: 7469 6f6e 206a 6f62 2067 6574 7320 7374  tion job gets st
-00018710: 6172 7465 6420 696d 6d65 6469 6174 656c  arted immediatel
-00018720: 792e 0a20 2020 2020 2020 2020 2020 2020  y..             
-00018730: 2020 202a 206b 6579 2060 6b61 666b 615f     * key `kafka_
-00018740: 7072 6f64 7563 6572 5f63 6f6e 6669 6760  producer_config`
-00018750: 2061 6e64 2076 616c 7565 2061 6e20 6f62   and value an ob
-00018760: 6a65 6374 206f 6620 7479 7065 205b 7072  ject of type [pr
-00018770: 6f70 6572 7469 6573 5d28 6874 7470 733a  operties](https:
-00018780: 2f2f 646f 6373 2e63 6f6e 666c 7565 6e74  //docs.confluent
-00018790: 2e69 6f2f 706c 6174 666f 726d 2f63 7572  .io/platform/cur
-000187a0: 7265 6e74 2f63 6c69 656e 7473 2f6c 6962  rent/clients/lib
-000187b0: 7264 6b61 666b 612f 6874 6d6c 2f6d 645f  rdkafka/html/md_
-000187c0: 434f 4e46 4947 5552 4154 494f 4e2e 6874  CONFIGURATION.ht
-000187d0: 6d6c 6e29 0a20 2020 2020 2020 2020 2020  mln).           
-000187e0: 2020 2020 2020 2075 7365 6420 746f 2063         used to c
-000187f0: 6f6e 6669 6775 7265 2074 6865 204b 6166  onfigure the Kaf
-00018800: 6b61 2063 6c69 656e 742e 2054 6f20 6f70  ka client. To op
-00018810: 7469 6d69 7a65 2066 6f72 2074 6872 6f75  timize for throu
-00018820: 6768 7075 7420 696e 2068 6967 6820 6c61  ghput in high la
-00018830: 7465 6e63 7920 636f 6e6e 6563 7469 6f6e  tency connection
-00018840: 2063 6f6e 7369 6465 720a 2020 2020 2020   consider.      
-00018850: 2020 2020 2020 2020 2020 2020 6368 616e              chan
-00018860: 6769 6e67 205b 7072 6f64 7563 6572 2070  ging [producer p
-00018870: 726f 7065 7274 6965 735d 2868 7474 7073  roperties](https
-00018880: 3a2f 2f64 6f63 732e 636f 6e66 6c75 656e  ://docs.confluen
-00018890: 742e 696f 2f63 6c6f 7564 2f63 7572 7265  t.io/cloud/curre
-000188a0: 6e74 2f63 6c69 656e 742d 6170 7073 2f6f  nt/client-apps/o
-000188b0: 7074 696d 697a 696e 672f 7468 726f 7567  ptimizing/throug
-000188c0: 6870 7574 2e68 746d 6c23 7072 6f64 7563  hput.html#produc
-000188d0: 6572 292e 0a20 2020 2020 2020 2020 2020  er)..           
-000188e0: 2020 2020 202a 206b 6579 2060 696e 7465       * key `inte
-000188f0: 726e 616c 5f6b 6166 6b61 6020 616e 6420  rnal_kafka` and 
-00018900: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
-00018910: 6046 616c 7365 6020 696e 2063 6173 6520  `False` in case 
-00018920: 796f 7520 6573 7461 626c 6973 6865 640a  you established.
-00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018940: 2020 636f 6e6e 6563 7469 7669 7479 2066    connectivity f
-00018950: 726f 6d20 796f 7520 5079 7468 6f6e 2065  rom you Python e
-00018960: 6e76 6972 6f6e 6d65 6e74 2074 6f20 7468  nvironment to th
-00018970: 6520 696e 7465 726e 616c 2061 6476 6572  e internal adver
-00018980: 7469 7365 640a 2020 2020 2020 2020 2020  tised.          
-00018990: 2020 2020 2020 2020 6c69 7374 656e 6572          listener
-000189a0: 7320 6f66 2074 6865 2048 6f70 7377 6f72  s of the Hopswor
-000189b0: 6b73 204b 6166 6b61 2043 6c75 7374 6572  ks Kafka Cluster
-000189c0: 2e20 4465 6661 756c 7473 2074 6f20 6046  . Defaults to `F
-000189d0: 616c 7365 6020 616e 640a 2020 2020 2020  alse` and.      
-000189e0: 2020 2020 2020 2020 2020 2020 7769 6c6c              will
-000189f0: 2075 7365 2065 7874 6572 6e61 6c20 6c69   use external li
-00018a00: 7374 656e 6572 7320 7768 656e 2063 6f6e  steners when con
-00018a10: 6e65 6374 696e 6720 6672 6f6d 206f 7574  necting from out
-00018a20: 7369 6465 206f 6620 486f 7073 776f 726b  side of Hopswork
-00018a30: 732e 0a20 2020 2020 2020 2020 2020 2076  s..            v
-00018a40: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
-00018a50: 733a 2041 6464 6974 696f 6e61 6c20 7661  s: Additional va
-00018a60: 6c69 6461 7469 6f6e 206f 7074 696f 6e73  lidation options
-00018a70: 2061 7320 6b65 792d 7661 6c75 6520 7061   as key-value pa
-00018a80: 6972 732c 2064 6566 6175 6c74 7320 746f  irs, defaults to
-00018a90: 2060 7b7d 602e 0a20 2020 2020 2020 2020   `{}`..         
-00018aa0: 2020 2020 2020 202a 206b 6579 2060 7275         * key `ru
-00018ab0: 6e5f 7661 6c69 6461 7469 6f6e 6020 626f  n_validation` bo
-00018ac0: 6f6c 6561 6e20 7661 6c75 652c 2073 6574  olean value, set
-00018ad0: 2074 6f20 6046 616c 7365 6020 746f 2073   to `False` to s
-00018ae0: 6b69 7020 7661 6c69 6461 7469 6f6e 2074  kip validation t
-00018af0: 656d 706f 7261 7269 6c79 206f 6e20 696e  emporarily on in
-00018b00: 6765 7374 696f 6e2e 0a20 2020 2020 2020  gestion..       
-00018b10: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-00018b20: 7361 7665 5f72 6570 6f72 7460 2062 6f6f  save_report` boo
-00018b30: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
-00018b40: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
-00018b50: 6970 2075 706c 6f61 6420 6f66 2074 6865  ip upload of the
-00018b60: 2076 616c 6964 6174 696f 6e20 7265 706f   validation repo
-00018b70: 7274 2074 6f20 486f 7073 776f 726b 732e  rt to Hopsworks.
-00018b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018b90: 202a 206b 6579 2060 6765 5f76 616c 6964   * key `ge_valid
-00018ba0: 6174 655f 6b77 6172 6773 6020 6120 6469  ate_kwargs` a di
-00018bb0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-00018bc0: 696e 6720 6b77 6172 6773 2066 6f72 2074  ing kwargs for t
-00018bd0: 6865 2076 616c 6964 6174 6520 6d65 7468  he validate meth
-00018be0: 6f64 206f 6620 4772 6561 7420 4578 7065  od of Great Expe
-00018bf0: 6374 6174 696f 6e73 2e0a 2020 2020 2020  ctations..      
-00018c00: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
-00018c10: 6066 6574 6368 5f65 7870 6563 7461 7469  `fetch_expectati
-00018c20: 6f6e 5f73 7569 7465 6020 6120 626f 6f6c  on_suite` a bool
-00018c30: 6561 6e20 7661 6c75 652c 2062 7920 6465  ean value, by de
-00018c40: 6661 756c 7420 6054 7275 6560 2c20 746f  fault `True`, to
-00018c50: 2063 6f6e 7472 6f6c 2077 6865 7468 6572   control whether
-00018c60: 2074 6865 2065 7870 6563 7461 7469 6f6e   the expectation
-00018c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c80: 2020 2020 7375 6974 6520 6f66 2074 6865      suite of the
-00018c90: 2066 6561 7475 7265 2067 726f 7570 2073   feature group s
-00018ca0: 686f 756c 6420 6265 2066 6574 6368 6564  hould be fetched
-00018cb0: 2062 6566 6f72 6520 6576 6572 7920 696e   before every in
-00018cc0: 7365 7274 2e0a 2020 2020 2020 2020 2020  sert..          
-00018cd0: 2020 7361 7665 5f63 6f64 653a 2057 6865    save_code: Whe
-00018ce0: 6e20 7275 6e6e 696e 6720 4853 4653 206f  n running HSFS o
-00018cf0: 6e20 486f 7073 776f 726b 7320 6f72 2044  n Hopsworks or D
-00018d00: 6174 6162 7269 636b 732c 2048 5346 5320  atabricks, HSFS 
-00018d10: 6361 6e20 7361 7665 2074 6865 2063 6f64  can save the cod
-00018d20: 652f 6e6f 7465 626f 6f6b 2075 7365 6420  e/notebook used 
-00018d30: 746f 2063 7265 6174 650a 2020 2020 2020  to create.      
-00018d40: 2020 2020 2020 2020 2020 7468 6520 6665            the fe
-00018d50: 6174 7572 6520 6772 6f75 7020 6f72 2075  ature group or u
-00018d60: 7365 6420 746f 2069 6e73 6572 7420 6461  sed to insert da
-00018d70: 7461 2074 6f20 6974 2e20 5768 656e 2063  ta to it. When c
-00018d80: 616c 6c69 6e67 2074 6865 2060 696e 7365  alling the `inse
-00018d90: 7274 6020 6d65 7468 6f64 2072 6570 6561  rt` method repea
-00018da0: 7465 646c 790a 2020 2020 2020 2020 2020  tedly.          
-00018db0: 2020 2020 2020 7769 7468 2073 6d61 6c6c        with small
-00018dc0: 2062 6174 6368 6573 206f 6620 6461 7461   batches of data
-00018dd0: 2c20 7468 6973 2063 616e 2073 6c6f 7720  , this can slow 
-00018de0: 646f 776e 2074 6865 2077 7269 7465 732e  down the writes.
-00018df0: 2055 7365 2074 6869 7320 6f70 7469 6f6e   Use this option
-00018e00: 2074 6f20 7475 726e 206f 6666 2073 6176   to turn off sav
-00018e10: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00018e20: 2020 2020 636f 6465 2e20 4465 6661 756c      code. Defaul
-00018e30: 7473 2074 6f20 6054 7275 6560 2e0a 2020  ts to `True`..  
-00018e40: 2020 2020 2020 2020 2020 7761 6974 3a20            wait: 
-00018e50: 5761 6974 2066 6f72 206a 6f62 2074 6f20  Wait for job to 
-00018e60: 6669 6e69 7368 2062 6566 6f72 6520 7265  finish before re
-00018e70: 7475 726e 696e 672c 2064 6566 6175 6c74  turning, default
-00018e80: 7320 746f 2060 4661 6c73 6560 2e0a 2020  s to `False`..  
-00018e90: 2020 2020 2020 2020 2020 2020 2020 5368                Sh
-00018ea0: 6f72 7463 7574 2066 6f72 2072 6561 645f  ortcut for read_
-00018eb0: 6f70 7469 6f6e 7320 607b 2277 6169 745f  options `{"wait_
-00018ec0: 666f 725f 6a6f 6222 3a20 4661 6c73 657d  for_job": False}
-00018ed0: 602e 0a0a 2020 2020 2020 2020 2320 5265  `...        # Re
-00018ee0: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
-00018ef0: 2020 2860 4a6f 6260 2c20 6056 616c 6964    (`Job`, `Valid
-00018f00: 6174 696f 6e52 6570 6f72 7460 2920 4120  ationReport`) A 
-00018f10: 7475 706c 6520 7769 7468 206a 6f62 2069  tuple with job i
-00018f20: 6e66 6f72 6d61 7469 6f6e 2069 6620 7079  nformation if py
-00018f30: 7468 6f6e 2065 6e67 696e 6520 6973 2075  thon engine is u
-00018f40: 7365 6420 616e 6420 7468 6520 7661 6c69  sed and the vali
-00018f50: 6461 7469 6f6e 2072 6570 6f72 7420 6966  dation report if
-00018f60: 2076 616c 6964 6174 696f 6e20 6973 2065   validation is e
-00018f70: 6e61 626c 6564 2e0a 0a20 2020 2020 2020  nabled...       
-00018f80: 2023 2052 6169 7365 730a 2020 2020 2020   # Raises.      
-00018f90: 2020 2020 2020 6068 7366 732e 636c 6965        `hsfs.clie
-00018fa0: 6e74 2e65 7863 6570 7469 6f6e 732e 5265  nt.exceptions.Re
-00018fb0: 7374 4150 4945 7272 6f72 602e 2065 2e67  stAPIError`. e.g
-00018fc0: 2066 6169 6c20 746f 2063 7265 6174 6520   fail to create 
-00018fd0: 6665 6174 7572 6520 6772 6f75 702c 2064  feature group, d
-00018fe0: 6174 6166 7261 6d65 2073 6368 656d 6120  ataframe schema 
-00018ff0: 646f 6573 206e 6f74 206d 6174 6368 0a20  does not match. 
-00019000: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019010: 7869 7374 696e 6720 6665 6174 7572 6520  xisting feature 
-00019020: 6772 6f75 7020 7363 6865 6d61 2c20 6574  group schema, et
-00019030: 632e 0a20 2020 2020 2020 2020 2020 2060  c..            `
-00019040: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
-00019050: 7074 696f 6e73 2e44 6174 6156 616c 6964  ptions.DataValid
-00019060: 6174 696f 6e45 7863 6570 7469 6f6e 602e  ationException`.
-00019070: 2049 6620 6461 7461 2076 616c 6964 6174   If data validat
-00019080: 696f 6e20 6661 696c 7320 616e 6420 7468  ion fails and th
-00019090: 6520 6578 7065 6374 6174 696f 6e0a 2020  e expectation.  
-000190a0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000190b0: 6974 6520 6076 616c 6964 6174 696f 6e5f  ite `validation_
-000190c0: 696e 6765 7374 696f 6e5f 706f 6c69 6379  ingestion_policy
-000190d0: 6020 6973 2073 6574 2074 6f20 6053 5452  ` is set to `STR
-000190e0: 4943 5460 2e20 4461 7461 2069 7320 4e4f  ICT`. Data is NO
-000190f0: 5420 696e 6765 7374 6564 2e0a 2020 2020  T ingested..    
-00019100: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00019110: 6966 2073 746f 7261 6765 2061 6e64 2073  if storage and s
-00019120: 656c 662e 7374 7265 616d 3a0a 2020 2020  elf.stream:.    
-00019130: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00019140: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-00019150: 2020 2020 2020 2022 5370 6563 6966 7969         "Specifyi
-00019160: 6e67 2074 6865 2073 746f 7261 6765 206f  ng the storage o
-00019170: 7074 696f 6e20 6973 206e 6f74 2073 7570  ption is not sup
-00019180: 706f 7274 6564 2069 6620 7468 6520 7374  ported if the st
-00019190: 7265 616d 696e 6720 4150 4973 2061 7265  reaming APIs are
-000191a0: 2065 6e61 626c 6564 220a 2020 2020 2020   enabled".      
-000191b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000191c0: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
-000191d0: 6d65 203d 2065 6e67 696e 652e 6765 745f  me = engine.get_
-000191e0: 696e 7374 616e 6365 2829 2e63 6f6e 7665  instance().conve
-000191f0: 7274 5f74 6f5f 6465 6661 756c 745f 6461  rt_to_default_da
-00019200: 7461 6672 616d 6528 6665 6174 7572 6573  taframe(features
-00019210: 290a 0a20 2020 2020 2020 2069 6620 7772  )..        if wr
-00019220: 6974 655f 6f70 7469 6f6e 7320 6973 204e  ite_options is N
-00019230: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00019240: 2077 7269 7465 5f6f 7074 696f 6e73 203d   write_options =
-00019250: 207b 7d0a 2020 2020 2020 2020 6966 2022   {}.        if "
-00019260: 7761 6974 5f66 6f72 5f6a 6f62 2220 6e6f  wait_for_job" no
-00019270: 7420 696e 2077 7269 7465 5f6f 7074 696f  t in write_optio
-00019280: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00019290: 7772 6974 655f 6f70 7469 6f6e 735b 2277  write_options["w
-000192a0: 6169 745f 666f 725f 6a6f 6222 5d20 3d20  ait_for_job"] = 
-000192b0: 7761 6974 0a0a 2020 2020 2020 2020 6a6f  wait..        jo
-000192c0: 622c 2067 655f 7265 706f 7274 203d 2073  b, ge_report = s
-000192d0: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
-000192e0: 7570 5f65 6e67 696e 652e 696e 7365 7274  up_engine.insert
-000192f0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00019300: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00019310: 6665 6174 7572 655f 6461 7461 6672 616d  feature_datafram
-00019320: 653d 6665 6174 7572 655f 6461 7461 6672  e=feature_datafr
-00019330: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00019340: 206f 7665 7277 7269 7465 3d6f 7665 7277   overwrite=overw
-00019350: 7269 7465 2c0a 2020 2020 2020 2020 2020  rite,.          
-00019360: 2020 6f70 6572 6174 696f 6e3d 6f70 6572    operation=oper
-00019370: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-00019380: 2020 2073 746f 7261 6765 3d73 746f 7261     storage=stora
-00019390: 6765 2e6c 6f77 6572 2829 2069 6620 7374  ge.lower() if st
-000193a0: 6f72 6167 6520 6973 206e 6f74 204e 6f6e  orage is not Non
-000193b0: 6520 656c 7365 204e 6f6e 652c 0a20 2020  e else None,.   
-000193c0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-000193d0: 7074 696f 6e73 3d77 7269 7465 5f6f 7074  ptions=write_opt
-000193e0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-000193f0: 2020 7661 6c69 6461 7469 6f6e 5f6f 7074    validation_opt
-00019400: 696f 6e73 3d7b 2273 6176 655f 7265 706f  ions={"save_repo
-00019410: 7274 223a 2054 7275 652c 202a 2a76 616c  rt": True, **val
-00019420: 6964 6174 696f 6e5f 6f70 7469 6f6e 737d  idation_options}
-00019430: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00019440: 2020 2020 6966 2073 6176 655f 636f 6465      if save_code
-00019450: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
-00019460: 2020 2067 655f 7265 706f 7274 2069 7320     ge_report is 
-00019470: 4e6f 6e65 206f 7220 6765 5f72 6570 6f72  None or ge_repor
-00019480: 742e 696e 6765 7374 696f 6e5f 7265 7375  t.ingestion_resu
-00019490: 6c74 203d 3d20 2249 4e47 4553 5445 4422  lt == "INGESTED"
-000194a0: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-000194b0: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-000194c0: 6465 5f65 6e67 696e 652e 7361 7665 5f63  de_engine.save_c
-000194d0: 6f64 6528 7365 6c66 290a 0a20 2020 2020  ode(self)..     
-000194e0: 2020 2069 6620 656e 6769 6e65 2e67 6574     if engine.get
-000194f0: 5f74 7970 6528 292e 7374 6172 7473 7769  _type().startswi
-00019500: 7468 2822 7370 6172 6b22 2920 616e 6420  th("spark") and 
-00019510: 6e6f 7420 7365 6c66 2e73 7472 6561 6d3a  not self.stream:
-00019520: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-00019530: 6c73 6f2c 206f 6e6c 7920 636f 6d70 7574  lso, only comput
-00019540: 6520 7374 6174 6973 7469 6373 2069 6620  e statistics if 
-00019550: 7374 7265 616d 2069 7320 4661 6c73 652e  stream is False.
-00019560: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00019570: 6620 5472 7565 2c20 7468 6520 6261 636b  f True, the back
-00019580: 6669 6c6c 206a 6f62 2068 6173 206e 6f74  fill job has not
-00019590: 2062 6565 6e20 7472 6967 6765 7265 6420   been triggered 
-000195a0: 616e 6420 7468 6520 6461 7461 2068 6173  and the data has
-000195b0: 206e 6f74 2062 6565 6e20 696e 7365 7274   not been insert
-000195c0: 6564 2028 6974 2773 2069 6e20 4b61 666b  ed (it's in Kafk
-000195d0: 6129 0a20 2020 2020 2020 2020 2020 2073  a).            s
-000195e0: 656c 662e 636f 6d70 7574 655f 7374 6174  elf.compute_stat
-000195f0: 6973 7469 6373 2829 0a0a 2020 2020 2020  istics()..      
-00019600: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-00019610: 2020 2020 2020 206a 6f62 2c0a 2020 2020         job,.    
-00019620: 2020 2020 2020 2020 6765 5f72 6570 6f72          ge_repor
-00019630: 742e 746f 5f67 655f 7479 7065 2829 2069  t.to_ge_type() i
-00019640: 6620 6765 5f72 6570 6f72 7420 6973 206e  f ge_report is n
-00019650: 6f74 204e 6f6e 6520 656c 7365 204e 6f6e  ot None else Non
-00019660: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-00019670: 2020 6465 6620 6d75 6c74 695f 7061 7274    def multi_part
-00019680: 5f69 6e73 6572 7428 0a20 2020 2020 2020  _insert(.       
-00019690: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
-000196a0: 6561 7475 7265 733a 2055 6e69 6f6e 5b0a  eatures: Union[.
-000196b0: 2020 2020 2020 2020 2020 2020 7064 2e44              pd.D
-000196c0: 6174 6146 7261 6d65 2c0a 2020 2020 2020  ataFrame,.      
-000196d0: 2020 2020 2020 5479 7065 5661 7228 2270        TypeVar("p
-000196e0: 7973 7061 726b 2e73 716c 2e44 6174 6146  yspark.sql.DataF
-000196f0: 7261 6d65 2229 2c20 2023 206e 6f71 613a  rame"),  # noqa:
-00019700: 2046 3832 310a 2020 2020 2020 2020 2020   F821.          
-00019710: 2020 5479 7065 5661 7228 2270 7973 7061    TypeVar("pyspa
-00019720: 726b 2e52 4444 2229 2c20 2023 206e 6f71  rk.RDD"),  # noq
-00019730: 613a 2046 3832 310a 2020 2020 2020 2020  a: F821.        
-00019740: 2020 2020 6e70 2e6e 6461 7272 6179 2c0a      np.ndarray,.
-00019750: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-00019760: 5b6c 6973 745d 2c0a 2020 2020 2020 2020  [list],.        
-00019770: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00019780: 2020 6f76 6572 7772 6974 653a 204f 7074    overwrite: Opt
-00019790: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4661  ional[bool] = Fa
-000197a0: 6c73 652c 0a20 2020 2020 2020 206f 7065  lse,.        ope
-000197b0: 7261 7469 6f6e 3a20 4f70 7469 6f6e 616c  ration: Optional
-000197c0: 5b73 7472 5d20 3d20 2275 7073 6572 7422  [str] = "upsert"
-000197d0: 2c0a 2020 2020 2020 2020 7374 6f72 6167  ,.        storag
-000197e0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-000197f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00019800: 2077 7269 7465 5f6f 7074 696f 6e73 3a20   write_options: 
-00019810: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-00019820: 722c 2041 6e79 5d5d 203d 207b 7d2c 0a20  r, Any]] = {},. 
-00019830: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-00019840: 6e5f 6f70 7469 6f6e 733a 204f 7074 696f  n_options: Optio
-00019850: 6e61 6c5b 4469 6374 5b73 7472 2c20 416e  nal[Dict[str, An
-00019860: 795d 5d20 3d20 7b7d 2c0a 2020 2020 2920  y]] = {},.    ) 
-00019870: 2d3e 2055 6e69 6f6e 5b0a 2020 2020 2020  -> Union[.      
-00019880: 2020 5475 706c 655b 4f70 7469 6f6e 616c    Tuple[Optional
-00019890: 5b4a 6f62 5d2c 204f 7074 696f 6e61 6c5b  [Job], Optional[
-000198a0: 5661 6c69 6461 7469 6f6e 5265 706f 7274  ValidationReport
-000198b0: 5d5d 2c0a 2020 2020 2020 2020 6665 6174  ]],.        feat
-000198c0: 7572 655f 6772 6f75 705f 7772 6974 6572  ure_group_writer
-000198d0: 2e46 6561 7475 7265 4772 6f75 7057 7269  .FeatureGroupWri
-000198e0: 7465 722c 0a20 2020 205d 3a0a 2020 2020  ter,.    ]:.    
-000198f0: 2020 2020 2222 2247 6574 2046 6561 7475      """Get Featu
-00019900: 7265 4772 6f75 7057 7269 7465 7220 666f  reGroupWriter fo
-00019910: 7220 6f70 7469 6d69 7a65 6420 6d75 6c74  r optimized mult
-00019920: 6920 7061 7274 2069 6e73 6572 7473 206f  i part inserts o
-00019930: 7220 6361 6c6c 2074 6869 7320 6d65 7468  r call this meth
-00019940: 6f64 0a20 2020 2020 2020 2074 6f20 7374  od.        to st
-00019950: 6172 7420 6d61 6e75 616c 206d 756c 7469  art manual multi
-00019960: 2070 6172 7420 6f70 7469 6d69 7a65 6420   part optimized 
-00019970: 696e 7365 7274 732e 0a0a 2020 2020 2020  inserts...      
-00019980: 2020 496e 2075 7365 2063 6173 6573 2077    In use cases w
-00019990: 6865 7265 2076 6572 7920 736d 616c 6c20  here very small 
-000199a0: 6261 7463 6865 7320 2831 2074 6f20 3130  batches (1 to 10
-000199b0: 3030 2920 726f 7773 2070 6572 2044 6174  00) rows per Dat
-000199c0: 6166 7261 6d65 206e 6565 640a 2020 2020  aframe need.    
-000199d0: 2020 2020 746f 2062 6520 7772 6974 7465      to be writte
-000199e0: 6e20 746f 2074 6865 2066 6561 7475 7265  n to the feature
-000199f0: 2073 746f 7265 2072 6570 6561 7465 646c   store repeatedl
-00019a00: 792c 2069 7420 6d69 6768 7420 6265 2069  y, it might be i
-00019a10: 6e65 6666 6963 6965 6e74 2074 6f20 7573  nefficient to us
-00019a20: 650a 2020 2020 2020 2020 7468 6520 7374  e.        the st
-00019a30: 616e 6461 7264 2060 6665 6174 7572 655f  andard `feature_
-00019a40: 6772 6f75 702e 696e 7365 7274 2829 6020  group.insert()` 
-00019a50: 6d65 7468 6f64 2061 7320 6974 2070 6572  method as it per
-00019a60: 666f 726d 7320 736f 6d65 2062 6163 6b67  forms some backg
-00019a70: 726f 756e 640a 2020 2020 2020 2020 6163  round.        ac
-00019a80: 7469 6f6e 7320 746f 2075 7064 6174 6520  tions to update 
-00019a90: 7468 6520 6d65 7461 6461 7461 206f 6620  the metadata of 
-00019aa0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-00019ab0: 7020 6f62 6a65 6374 2066 6972 7374 2e0a  p object first..
-00019ac0: 0a20 2020 2020 2020 2046 6f72 2074 6865  .        For the
-00019ad0: 7365 2063 6173 6573 2c20 7468 6520 6665  se cases, the fe
-00019ae0: 6174 7572 6520 6772 6f75 7020 7072 6f76  ature group prov
-00019af0: 6964 6573 2074 6865 2060 6d75 6c74 695f  ides the `multi_
-00019b00: 7061 7274 5f69 6e73 6572 7460 2041 5049  part_insert` API
-00019b10: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
-00019b20: 6973 206f 7074 696d 697a 6564 2066 6f72  is optimized for
-00019b30: 2077 7269 7469 6e67 206d 616e 7920 736d   writing many sm
-00019b40: 616c 6c20 4461 7461 6672 616d 6573 2061  all Dataframes a
-00019b50: 6674 6572 2061 6e6f 7468 6572 2e0a 0a20  fter another... 
-00019b60: 2020 2020 2020 2054 6865 7265 2061 7265         There are
-00019b70: 2074 776f 2077 6179 7320 746f 2075 7365   two ways to use
-00019b80: 2074 6869 7320 4150 493a 0a20 2020 2020   this API:.     
-00019b90: 2020 2021 2121 2065 7861 6d70 6c65 2022     !!! example "
-00019ba0: 5079 7468 6f6e 2043 6f6e 7465 7874 204d  Python Context M
-00019bb0: 616e 6167 6572 220a 2020 2020 2020 2020  anager".        
-00019bc0: 2020 2020 5573 696e 6720 7468 6520 5079      Using the Py
-00019bd0: 7468 6f6e 2060 7769 7468 6020 7379 6e74  thon `with` synt
-00019be0: 6178 2079 6f75 2063 616e 2061 6371 7569  ax you can acqui
-00019bf0: 7265 2061 2046 6561 7475 7265 4772 6f75  re a FeatureGrou
-00019c00: 7057 7269 7465 720a 2020 2020 2020 2020  pWriter.        
-00019c10: 2020 2020 6f62 6a65 6374 2074 6861 7420      object that 
-00019c20: 696d 706c 656d 656e 7473 2074 6865 2073  implements the s
-00019c30: 616d 6520 606d 756c 7469 5f70 6172 745f  ame `multi_part_
-00019c40: 696e 7365 7274 6020 4150 492e 0a20 2020  insert` API..   
-00019c50: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
-00019c60: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
-00019c70: 6561 7475 7265 5f67 726f 7570 203d 2066  eature_group = f
-00019c80: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-00019c90: 6665 6174 7572 655f 6772 6f75 7028 2266  feature_group("f
-00019ca0: 675f 6e61 6d65 222c 2076 6572 7369 6f6e  g_name", version
-00019cb0: 3d31 290a 0a20 2020 2020 2020 2020 2020  =1)..           
-00019cc0: 2077 6974 6820 6665 6174 7572 655f 6772   with feature_gr
-00019cd0: 6f75 702e 6d75 6c74 695f 7061 7274 5f69  oup.multi_part_i
-00019ce0: 6e73 6572 7428 2920 6173 2077 7269 7465  nsert() as write
-00019cf0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00019d00: 2020 2023 2072 756e 2069 6e73 6572 7473     # run inserts
-00019d10: 2069 6e20 6120 6c6f 6f70 3a0a 2020 2020   in a loop:.    
-00019d20: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-00019d30: 6520 6c6f 6f70 3a0a 2020 2020 2020 2020  e loop:.        
-00019d40: 2020 2020 2020 2020 2020 2020 736d 616c              smal
-00019d50: 6c5f 6261 7463 685f 6466 203d 202e 2e2e  l_batch_df = ...
-00019d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019d70: 2020 2020 2077 7269 7465 722e 696e 7365       writer.inse
-00019d80: 7274 2873 6d61 6c6c 5f62 6174 6368 5f64  rt(small_batch_d
-00019d90: 6629 0a20 2020 2020 2020 2020 2020 2060  f).            `
-00019da0: 6060 0a20 2020 2020 2020 2020 2020 2054  ``.            T
-00019db0: 6865 2077 7269 7465 7220 6261 7463 6865  he writer batche
-00019dc0: 7320 7468 6520 736d 616c 6c20 4461 7461  s the small Data
-00019dd0: 6672 616d 6573 2061 6e64 2074 7261 6e73  frames and trans
-00019de0: 6d69 7473 2074 6865 6d20 746f 2048 6f70  mits them to Hop
-00019df0: 7377 6f72 6b73 0a20 2020 2020 2020 2020  sworks.         
-00019e00: 2020 2065 6666 6963 6965 6e74 6c79 2e0a     efficiently..
-00019e10: 2020 2020 2020 2020 2020 2020 5768 656e              When
-00019e20: 2065 7869 7469 6e67 2074 6865 2063 6f6e   exiting the con
-00019e30: 7465 7874 2c20 7468 6520 6665 6174 7572  text, the featur
-00019e40: 6520 6772 6f75 7020 7772 6974 6572 2069  e group writer i
-00019e50: 7320 7375 7265 2074 6f20 6578 6974 0a20  s sure to exit. 
-00019e60: 2020 2020 2020 2020 2020 206f 6e6c 7920             only 
-00019e70: 6f6e 6365 2061 6c6c 2074 6865 2072 6f77  once all the row
-00019e80: 7320 6861 7665 2062 6565 6e20 7472 616e  s have been tran
-00019e90: 736d 6974 7465 642e 0a0a 2020 2020 2020  smitted...      
-00019ea0: 2020 2121 2120 6578 616d 706c 6520 224d    !!! example "M
-00019eb0: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
-00019ec0: 2077 6974 6820 6d61 6e75 616c 2063 6f6e   with manual con
-00019ed0: 7465 7874 206d 616e 6167 656d 656e 7422  text management"
-00019ee0: 0a20 2020 2020 2020 2020 2020 2049 6e73  .            Ins
-00019ef0: 7465 6164 206f 6620 6c65 7474 696e 6720  tead of letting 
-00019f00: 5079 7468 6f6e 2068 616e 646c 6520 7468  Python handle th
-00019f10: 6520 656e 7465 7269 6e67 2061 6e64 2065  e entering and e
-00019f20: 7869 7469 6e67 206f 6620 7468 650a 2020  xiting of the.  
-00019f30: 2020 2020 2020 2020 2020 6d75 6c74 6920            multi 
-00019f40: 7061 7274 2069 6e73 6572 7420 636f 6e74  part insert cont
-00019f50: 6578 742c 2079 6f75 2063 616e 2073 7461  ext, you can sta
-00019f60: 7274 2061 6e64 2066 696e 616c 697a 6520  rt and finalize 
-00019f70: 7468 6520 636f 6e74 6578 740a 2020 2020  the context.    
-00019f80: 2020 2020 2020 2020 6d61 6e75 616c 6c79          manually
-00019f90: 2e0a 2020 2020 2020 2020 2020 2020 6060  ..            ``
-00019fa0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00019fb0: 2020 2020 6665 6174 7572 655f 6772 6f75      feature_grou
-00019fc0: 7020 3d20 6673 2e67 6574 5f6f 725f 6372  p = fs.get_or_cr
-00019fd0: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-00019fe0: 7570 2822 6667 5f6e 616d 6522 2c20 7665  up("fg_name", ve
-00019ff0: 7273 696f 6e3d 3129 0a0a 2020 2020 2020  rsion=1)..      
-0001a000: 2020 2020 2020 7768 696c 6520 6c6f 6f70        while loop
-0001a010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a020: 2020 736d 616c 6c5f 6261 7463 685f 6466    small_batch_df
-0001a030: 203d 202e 2e2e 0a20 2020 2020 2020 2020   = ....         
-0001a040: 2020 2020 2020 2066 6561 7475 7265 5f67         feature_g
-0001a050: 726f 7570 2e6d 756c 7469 5f70 6172 745f  roup.multi_part_
-0001a060: 696e 7365 7274 2873 6d61 6c6c 5f62 6174  insert(small_bat
-0001a070: 6368 5f64 6629 0a0a 2020 2020 2020 2020  ch_df)..        
-0001a080: 2020 2020 2320 494d 504f 5254 414e 543a      # IMPORTANT:
-0001a090: 2066 696e 616c 697a 6520 7468 6520 6d75   finalize the mu
-0001a0a0: 6c74 6920 7061 7274 2069 6e73 6572 7420  lti part insert 
-0001a0b0: 746f 206d 616b 6520 7375 7265 2061 6c6c  to make sure all
-0001a0c0: 2072 6f77 730a 2020 2020 2020 2020 2020   rows.          
-0001a0d0: 2020 2320 6861 7665 2062 6565 6e20 7472    # have been tr
-0001a0e0: 616e 736d 6974 7465 640a 2020 2020 2020  ansmitted.      
-0001a0f0: 2020 2020 2020 6665 6174 7572 655f 6772        feature_gr
-0001a100: 6f75 702e 6669 6e61 6c69 7a65 5f6d 756c  oup.finalize_mul
-0001a110: 7469 5f70 6172 745f 696e 7365 7274 2829  ti_part_insert()
-0001a120: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-0001a130: 0a20 2020 2020 2020 2020 2020 204e 6f74  .            Not
-0001a140: 6520 7468 6174 2074 6865 2066 6972 7374  e that the first
-0001a150: 2063 616c 6c20 746f 2060 6d75 6c74 695f   call to `multi_
-0001a160: 7061 7274 5f69 6e73 6572 7460 2069 6e69  part_insert` ini
-0001a170: 7469 6174 6573 2074 6865 2063 6f6e 7465  tiates the conte
-0001a180: 7874 0a20 2020 2020 2020 2020 2020 2061  xt.            a
-0001a190: 6e64 2062 6520 7375 7265 2074 6f20 6669  nd be sure to fi
-0001a1a0: 6e61 6c69 7a65 2069 742e 2054 6865 2060  nalize it. The `
-0001a1b0: 6669 6e61 6c69 7a65 5f6d 756c 7469 5f70  finalize_multi_p
-0001a1c0: 6172 745f 696e 7365 7274 6020 6973 2061  art_insert` is a
-0001a1d0: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
-0001a1e0: 636b 696e 6720 6361 6c6c 2074 6861 7420  cking call that 
-0001a1f0: 7265 7475 726e 7320 6f6e 6365 2061 6c6c  returns once all
-0001a200: 2072 6f77 7320 6861 7665 2062 6565 6e20   rows have been 
-0001a210: 7472 616e 736d 6974 7465 642e 0a0a 2020  transmitted...  
-0001a220: 2020 2020 2020 2020 2020 4f6e 6365 2079            Once y
-0001a230: 6f75 2061 7265 2064 6f6e 6520 7769 7468  ou are done with
-0001a240: 2074 6865 206d 756c 7469 2070 6172 7420   the multi part 
-0001a250: 696e 7365 7274 2c20 6974 2069 7320 676f  insert, it is go
-0001a260: 6f64 2070 7261 6374 6963 6520 746f 0a20  od practice to. 
-0001a270: 2020 2020 2020 2020 2020 2073 7461 7274             start
-0001a280: 2074 6865 206d 6174 6572 6961 6c69 7a61   the materializa
-0001a290: 7469 6f6e 206a 6f62 2069 6e20 6f72 6465  tion job in orde
-0001a2a0: 7220 746f 2077 7269 7465 2074 6865 2064  r to write the d
-0001a2b0: 6174 6120 746f 2074 6865 206f 6666 6c69  ata to the offli
-0001a2c0: 6e65 0a20 2020 2020 2020 2020 2020 2073  ne.            s
-0001a2d0: 746f 7261 6765 3a0a 2020 2020 2020 2020  torage:.        
-0001a2e0: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
-0001a2f0: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-0001a300: 655f 6772 6f75 702e 6d61 7465 7269 616c  e_group.material
-0001a310: 697a 6174 696f 6e5f 6a6f 622e 7275 6e28  ization_job.run(
-0001a320: 6177 6169 745f 7465 726d 696e 6174 696f  await_terminatio
-0001a330: 6e3d 5472 7565 290a 2020 2020 2020 2020  n=True).        
-0001a340: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
-0001a350: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
-0001a360: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-0001a370: 733a 2044 6174 6146 7261 6d65 2c20 5244  s: DataFrame, RD
-0001a380: 442c 204e 6461 7272 6179 2c20 6c69 7374  D, Ndarray, list
-0001a390: 2e20 4665 6174 7572 6573 2074 6f20 6265  . Features to be
-0001a3a0: 2073 6176 6564 2e0a 2020 2020 2020 2020   saved..        
-0001a3b0: 2020 2020 6f76 6572 7772 6974 653a 2044      overwrite: D
-0001a3c0: 726f 7020 616c 6c20 6461 7461 2069 6e20  rop all data in 
-0001a3d0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-0001a3e0: 7020 6265 666f 7265 0a20 2020 2020 2020  p before.       
-0001a3f0: 2020 2020 2020 2020 2069 6e73 6572 7469           inserti
-0001a400: 6e67 206e 6577 2064 6174 612e 2054 6869  ng new data. Thi
-0001a410: 7320 646f 6573 206e 6f74 2061 6666 6563  s does not affec
-0001a420: 7420 6d65 7461 6461 7461 2c20 6465 6661  t metadata, defa
-0001a430: 756c 7473 2074 6f20 4661 6c73 652e 0a20  ults to False.. 
-0001a440: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-0001a450: 7469 6f6e 3a20 4170 6163 6865 2048 7564  tion: Apache Hud
-0001a460: 6920 6f70 6572 6174 696f 6e20 7479 7065  i operation type
-0001a470: 2060 2269 6e73 6572 7422 6020 6f72 2060   `"insert"` or `
-0001a480: 2275 7073 6572 7422 602e 0a20 2020 2020  "upsert"`..     
-0001a490: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-0001a4a0: 6c74 7320 746f 2060 2275 7073 6572 7422  lts to `"upsert"
-0001a4b0: 602e 0a20 2020 2020 2020 2020 2020 2073  `..            s
-0001a4c0: 746f 7261 6765 3a20 4f76 6572 7772 6974  torage: Overwrit
-0001a4d0: 6520 6465 6661 756c 7420 6265 6861 7669  e default behavi
-0001a4e0: 6f75 722c 2077 7269 7465 2074 6f20 6f66  our, write to of
-0001a4f0: 666c 696e 650a 2020 2020 2020 2020 2020  fline.          
-0001a500: 2020 2020 2020 7374 6f72 6167 6520 6f6e        storage on
-0001a510: 6c79 2077 6974 6820 6022 6f66 666c 696e  ly with `"offlin
-0001a520: 6522 6020 6f72 206f 6e6c 696e 6520 6f6e  e"` or online on
-0001a530: 6c79 2077 6974 6820 6022 6f6e 6c69 6e65  ly with `"online
-0001a540: 2260 2c20 6465 6661 756c 7473 0a20 2020  "`, defaults.   
-0001a550: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
-0001a560: 604e 6f6e 6560 2e0a 2020 2020 2020 2020  `None`..        
-0001a570: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
-0001a580: 733a 2041 6464 6974 696f 6e61 6c20 7772  s: Additional wr
-0001a590: 6974 6520 6f70 7469 6f6e 7320 6173 206b  ite options as k
-0001a5a0: 6579 2d76 616c 7565 2070 6169 7273 2c20  ey-value pairs, 
-0001a5b0: 6465 6661 756c 7473 2074 6f20 607b 7d60  defaults to `{}`
-0001a5c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a5d0: 2020 5768 656e 2075 7369 6e67 2074 6865    When using the
-0001a5e0: 2060 7079 7468 6f6e 6020 656e 6769 6e65   `python` engine
-0001a5f0: 2c20 7772 6974 655f 6f70 7469 6f6e 7320  , write_options 
-0001a600: 6361 6e20 636f 6e74 6169 6e20 7468 650a  can contain the.
-0001a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a620: 666f 6c6c 6f77 696e 6720 656e 7472 6965  following entrie
-0001a630: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001a640: 2020 202a 206b 6579 2060 7370 6172 6b60     * key `spark`
-0001a650: 2061 6e64 2076 616c 7565 2061 6e20 6f62   and value an ob
-0001a660: 6a65 6374 206f 6620 7479 7065 0a20 2020  ject of type.   
-0001a670: 2020 2020 2020 2020 2020 2020 205b 6873               [hs
-0001a680: 6673 2e63 6f72 652e 6a6f 625f 636f 6e66  fs.core.job_conf
-0001a690: 6967 7572 6174 696f 6e2e 4a6f 6243 6f6e  iguration.JobCon
-0001a6a0: 6669 6775 7261 7469 6f6e 5d28 2e2e 2f6a  figuration](../j
-0001a6b0: 6f62 5f63 6f6e 6669 6775 7261 7469 6f6e  ob_configuration
-0001a6c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001a6d0: 2020 2020 746f 2063 6f6e 6669 6775 7265      to configure
-0001a6e0: 2074 6865 2048 6f70 7377 6f72 6b73 204a   the Hopsworks J
-0001a6f0: 6f62 2075 7365 6420 746f 2077 7269 7465  ob used to write
-0001a700: 2064 6174 6120 696e 746f 2074 6865 0a20   data into the. 
-0001a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a720: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-0001a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a740: 2a20 6b65 7920 6077 6169 745f 666f 725f  * key `wait_for_
-0001a750: 6a6f 6260 2061 6e64 2076 616c 7565 2060  job` and value `
-0001a760: 5472 7565 6020 6f72 2060 4661 6c73 6560  True` or `False`
-0001a770: 2074 6f20 636f 6e66 6967 7572 650a 2020   to configure.  
-0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a790: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
-0001a7a0: 6f20 7468 6520 696e 7365 7274 2063 616c  o the insert cal
-0001a7b0: 6c20 7368 6f75 6c64 2072 6574 7572 6e20  l should return 
-0001a7c0: 6f6e 6c79 0a20 2020 2020 2020 2020 2020  only.           
-0001a7d0: 2020 2020 2020 2061 6674 6572 2074 6865         after the
-0001a7e0: 2048 6f70 7377 6f72 6b73 204a 6f62 2068   Hopsworks Job h
-0001a7f0: 6173 2066 696e 6973 6865 642e 2042 7920  as finished. By 
-0001a800: 6465 6661 756c 7420 6974 2077 6169 7473  default it waits
-0001a810: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a820: 2020 2a20 6b65 7920 6073 7461 7274 5f6f    * key `start_o
-0001a830: 6666 6c69 6e65 5f62 6163 6b66 696c 6c60  ffline_backfill`
-0001a840: 2061 6e64 2076 616c 7565 2060 5472 7565   and value `True
-0001a850: 6020 6f72 2060 4661 6c73 6560 2074 6f20  ` or `False` to 
-0001a860: 636f 6e66 6967 7572 650a 2020 2020 2020  configure.      
-0001a870: 2020 2020 2020 2020 2020 2020 7768 6574              whet
-0001a880: 6865 7220 6f72 206e 6f74 2074 6f20 7374  her or not to st
-0001a890: 6172 7420 7468 6520 6d61 7465 7269 616c  art the material
-0001a8a0: 697a 6174 696f 6e20 6a6f 6220 746f 2077  ization job to w
-0001a8b0: 7269 7465 2064 6174 6120 746f 2074 6865  rite data to the
-0001a8c0: 206f 6666 6c69 6e65 0a20 2020 2020 2020   offline.       
-0001a8d0: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-0001a8e0: 6765 2e20 6073 7461 7274 5f6f 6666 6c69  ge. `start_offli
-0001a8f0: 6e65 5f62 6163 6b66 696c 6c60 2069 7320  ne_backfill` is 
-0001a900: 6465 7072 6563 6174 6564 2e20 5573 6520  deprecated. Use 
-0001a910: 6073 7461 7274 5f6f 6666 6c69 6e65 5f6d  `start_offline_m
-0001a920: 6174 6572 6961 6c69 7a61 7469 6f6e 6020  aterialization` 
-0001a930: 696e 7374 6561 642e 0a20 2020 2020 2020  instead..       
-0001a940: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-0001a950: 7374 6172 745f 6f66 666c 696e 655f 6d61  start_offline_ma
-0001a960: 7465 7269 616c 697a 6174 696f 6e60 2061  terialization` a
-0001a970: 6e64 2076 616c 7565 2060 5472 7565 6020  nd value `True` 
-0001a980: 6f72 2060 4661 6c73 6560 2074 6f20 636f  or `False` to co
-0001a990: 6e66 6967 7572 650a 2020 2020 2020 2020  nfigure.        
-0001a9a0: 2020 2020 2020 2020 2020 7768 6574 6865            whethe
-0001a9b0: 7220 6f72 206e 6f74 2074 6f20 7374 6172  r or not to star
-0001a9c0: 7420 7468 6520 6d61 7465 7269 616c 697a  t the materializ
-0001a9d0: 6174 696f 6e20 6a6f 6220 746f 2077 7269  ation job to wri
-0001a9e0: 7465 2064 6174 6120 746f 2074 6865 206f  te data to the o
-0001a9f0: 6666 6c69 6e65 0a20 2020 2020 2020 2020  ffline.         
-0001aa00: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-0001aa10: 2e20 4279 2064 6566 6175 6c74 2074 6865  . By default the
-0001aa20: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
-0001aa30: 206a 6f62 2064 6f65 7320 6e6f 7420 6765   job does not ge
-0001aa40: 7420 7374 6172 7465 6420 6175 746f 6d61  t started automa
-0001aa50: 7469 6361 6c6c 790a 2020 2020 2020 2020  tically.        
-0001aa60: 2020 2020 2020 2020 2020 666f 7220 6d75            for mu
-0001aa70: 6c74 6920 7061 7274 2069 6e73 6572 7473  lti part inserts
-0001aa80: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aa90: 2020 2a20 6b65 7920 606b 6166 6b61 5f70    * key `kafka_p
-0001aaa0: 726f 6475 6365 725f 636f 6e66 6967 6020  roducer_config` 
-0001aab0: 616e 6420 7661 6c75 6520 616e 206f 626a  and value an obj
-0001aac0: 6563 7420 6f66 2074 7970 6520 5b70 726f  ect of type [pro
-0001aad0: 7065 7274 6965 735d 2868 7474 7073 3a2f  perties](https:/
-0001aae0: 2f64 6f63 732e 636f 6e66 6c75 656e 742e  /docs.confluent.
-0001aaf0: 696f 2f70 6c61 7466 6f72 6d2f 6375 7272  io/platform/curr
-0001ab00: 656e 742f 636c 6965 6e74 732f 6c69 6272  ent/clients/libr
-0001ab10: 646b 6166 6b61 2f68 746d 6c2f 6d64 5f43  dkafka/html/md_C
-0001ab20: 4f4e 4649 4755 5241 5449 4f4e 2e68 746d  ONFIGURATION.htm
-0001ab30: 6c6e 290a 2020 2020 2020 2020 2020 2020  ln).            
-0001ab40: 2020 2020 2020 7573 6564 2074 6f20 636f        used to co
-0001ab50: 6e66 6967 7572 6520 7468 6520 4b61 666b  nfigure the Kafk
-0001ab60: 6120 636c 6965 6e74 2e20 546f 206f 7074  a client. To opt
-0001ab70: 696d 697a 6520 666f 7220 7468 726f 7567  imize for throug
-0001ab80: 6870 7574 2069 6e20 6869 6768 206c 6174  hput in high lat
-0001ab90: 656e 6379 2063 6f6e 6e65 6374 696f 6e20  ency connection 
-0001aba0: 636f 6e73 6964 6572 0a20 2020 2020 2020  consider.       
-0001abb0: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
-0001abc0: 696e 6720 5b70 726f 6475 6365 7220 7072  ing [producer pr
-0001abd0: 6f70 6572 7469 6573 5d28 6874 7470 733a  operties](https:
-0001abe0: 2f2f 646f 6373 2e63 6f6e 666c 7565 6e74  //docs.confluent
-0001abf0: 2e69 6f2f 636c 6f75 642f 6375 7272 656e  .io/cloud/curren
-0001ac00: 742f 636c 6965 6e74 2d61 7070 732f 6f70  t/client-apps/op
-0001ac10: 7469 6d69 7a69 6e67 2f74 6872 6f75 6768  timizing/through
-0001ac20: 7075 742e 6874 6d6c 2370 726f 6475 6365  put.html#produce
-0001ac30: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
-0001ac40: 2020 2020 2a20 6b65 7920 6069 6e74 6572      * key `inter
-0001ac50: 6e61 6c5f 6b61 666b 6160 2061 6e64 2076  nal_kafka` and v
-0001ac60: 616c 7565 2060 5472 7565 6020 6f72 2060  alue `True` or `
-0001ac70: 4661 6c73 6560 2069 6e20 6361 7365 2079  False` in case y
-0001ac80: 6f75 2065 7374 6162 6c69 7368 6564 0a20  ou established. 
-0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aca0: 2063 6f6e 6e65 6374 6976 6974 7920 6672   connectivity fr
-0001acb0: 6f6d 2079 6f75 2050 7974 686f 6e20 656e  om you Python en
-0001acc0: 7669 726f 6e6d 656e 7420 746f 2074 6865  vironment to the
-0001acd0: 2069 6e74 6572 6e61 6c20 6164 7665 7274   internal advert
-0001ace0: 6973 6564 0a20 2020 2020 2020 2020 2020  ised.           
-0001acf0: 2020 2020 2020 206c 6973 7465 6e65 7273         listeners
-0001ad00: 206f 6620 7468 6520 486f 7073 776f 726b   of the Hopswork
-0001ad10: 7320 4b61 666b 6120 436c 7573 7465 722e  s Kafka Cluster.
-0001ad20: 2044 6566 6175 6c74 7320 746f 2060 4661   Defaults to `Fa
-0001ad30: 6c73 6560 2061 6e64 0a20 2020 2020 2020  lse` and.       
-0001ad40: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
-0001ad50: 7573 6520 6578 7465 726e 616c 206c 6973  use external lis
-0001ad60: 7465 6e65 7273 2077 6865 6e20 636f 6e6e  teners when conn
-0001ad70: 6563 7469 6e67 2066 726f 6d20 6f75 7473  ecting from outs
-0001ad80: 6964 6520 6f66 2048 6f70 7377 6f72 6b73  ide of Hopsworks
-0001ad90: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0001ada0: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-0001adb0: 3a20 4164 6469 7469 6f6e 616c 2076 616c  : Additional val
-0001adc0: 6964 6174 696f 6e20 6f70 7469 6f6e 7320  idation options 
-0001add0: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
-0001ade0: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-0001adf0: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
-0001ae00: 2020 2020 2020 2a20 6b65 7920 6072 756e        * key `run
-0001ae10: 5f76 616c 6964 6174 696f 6e60 2062 6f6f  _validation` boo
-0001ae20: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
-0001ae30: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
-0001ae40: 6970 2076 616c 6964 6174 696f 6e20 7465  ip validation te
-0001ae50: 6d70 6f72 6172 696c 7920 6f6e 2069 6e67  mporarily on ing
-0001ae60: 6573 7469 6f6e 2e0a 2020 2020 2020 2020  estion..        
-0001ae70: 2020 2020 2020 2020 2a20 6b65 7920 6073          * key `s
-0001ae80: 6176 655f 7265 706f 7274 6020 626f 6f6c  ave_report` bool
-0001ae90: 6561 6e20 7661 6c75 652c 2073 6574 2074  ean value, set t
-0001aea0: 6f20 6046 616c 7365 6020 746f 2073 6b69  o `False` to ski
-0001aeb0: 7020 7570 6c6f 6164 206f 6620 7468 6520  p upload of the 
-0001aec0: 7661 6c69 6461 7469 6f6e 2072 6570 6f72  validation repor
-0001aed0: 7420 746f 2048 6f70 7377 6f72 6b73 2e0a  t to Hopsworks..
-0001aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aef0: 2a20 6b65 7920 6067 655f 7661 6c69 6461  * key `ge_valida
-0001af00: 7465 5f6b 7761 7267 7360 2061 2064 6963  te_kwargs` a dic
-0001af10: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-0001af20: 6e67 206b 7761 7267 7320 666f 7220 7468  ng kwargs for th
-0001af30: 6520 7661 6c69 6461 7465 206d 6574 686f  e validate metho
-0001af40: 6420 6f66 2047 7265 6174 2045 7870 6563  d of Great Expec
-0001af50: 7461 7469 6f6e 732e 0a20 2020 2020 2020  tations..       
-0001af60: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-0001af70: 6665 7463 685f 6578 7065 6374 6174 696f  fetch_expectatio
-0001af80: 6e5f 7375 6974 6560 2061 2062 6f6f 6c65  n_suite` a boole
-0001af90: 616e 2076 616c 7565 2c20 6279 2064 6566  an value, by def
-0001afa0: 6175 6c74 2060 4661 6c73 6560 2066 6f72  ault `False` for
-0001afb0: 206d 756c 7469 2070 6172 7420 696e 7365   multi part inse
-0001afc0: 7274 732c 0a20 2020 2020 2020 2020 2020  rts,.           
-0001afd0: 2020 2020 2020 2020 746f 2063 6f6e 7472          to contr
-0001afe0: 6f6c 2077 6865 7468 6572 2074 6865 2065  ol whether the e
-0001aff0: 7870 6563 7461 7469 6f6e 2073 7569 7465  xpectation suite
-0001b000: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
-0001b010: 6772 6f75 7020 7368 6f75 6c64 2062 6520  group should be 
-0001b020: 6665 7463 6865 6420 6265 666f 7265 2065  fetched before e
-0001b030: 7665 7279 2069 6e73 6572 742e 0a0a 2020  very insert...  
-0001b040: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
-0001b050: 2020 2020 2020 2020 2020 2020 2860 4a6f              (`Jo
-0001b060: 6260 2c20 6056 616c 6964 6174 696f 6e52  b`, `ValidationR
-0001b070: 6570 6f72 7460 2920 4120 7475 706c 6520  eport`) A tuple 
-0001b080: 7769 7468 206a 6f62 2069 6e66 6f72 6d61  with job informa
-0001b090: 7469 6f6e 2069 6620 7079 7468 6f6e 2065  tion if python e
-0001b0a0: 6e67 696e 6520 6973 2075 7365 6420 616e  ngine is used an
-0001b0b0: 6420 7468 6520 7661 6c69 6461 7469 6f6e  d the validation
-0001b0c0: 2072 6570 6f72 7420 6966 2076 616c 6964   report if valid
-0001b0d0: 6174 696f 6e20 6973 2065 6e61 626c 6564  ation is enabled
-0001b0e0: 2e0a 2020 2020 2020 2020 2020 2020 6046  ..            `F
-0001b0f0: 6561 7475 7265 4772 6f75 7057 7269 7465  eatureGroupWrite
-0001b100: 7260 2057 6865 6e20 7573 6564 2061 7320  r` When used as 
-0001b110: 6120 636f 6e74 6578 7420 6d61 6e61 6765  a context manage
-0001b120: 7220 7769 7468 2050 7974 686f 6e20 6077  r with Python `w
-0001b130: 6974 6860 2073 7461 7465 6d65 6e74 2e0a  ith` statement..
-0001b140: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001b150: 2020 2020 7365 6c66 2e5f 6d75 6c74 695f      self._multi_
-0001b160: 7061 7274 5f69 6e73 6572 7420 3d20 5472  part_insert = Tr
-0001b170: 7565 0a20 2020 2020 2020 206d 756c 7469  ue.        multi
-0001b180: 5f70 6172 745f 7772 6974 6572 203d 2066  _part_writer = f
-0001b190: 6561 7475 7265 5f67 726f 7570 5f77 7269  eature_group_wri
-0001b1a0: 7465 722e 4665 6174 7572 6547 726f 7570  ter.FeatureGroup
-0001b1b0: 5772 6974 6572 2873 656c 6629 0a20 2020  Writer(self).   
-0001b1c0: 2020 2020 2069 6620 6665 6174 7572 6573       if features
-0001b1d0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0001b1e0: 2020 2020 2020 7265 7475 726e 206d 756c        return mul
-0001b1f0: 7469 5f70 6172 745f 7772 6974 6572 0a20  ti_part_writer. 
-0001b200: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001b210: 2020 2020 2020 2020 2023 2067 6f20 7468           # go th
-0001b220: 726f 7567 6820 7772 6974 6572 2074 6f20  rough writer to 
-0001b230: 6176 6f69 6420 7365 7474 696e 6720 6d75  avoid setting mu
-0001b240: 6c74 6920 696e 7365 7274 2064 6566 6175  lti insert defau
-0001b250: 6c74 7320 6167 6169 6e0a 2020 2020 2020  lts again.      
-0001b260: 2020 2020 2020 7265 7475 726e 206d 756c        return mul
-0001b270: 7469 5f70 6172 745f 7772 6974 6572 2e69  ti_part_writer.i
-0001b280: 6e73 6572 7428 0a20 2020 2020 2020 2020  nsert(.         
-0001b290: 2020 2020 2020 2066 6561 7475 7265 732c         features,
-0001b2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b2b0: 206f 7665 7277 7269 7465 2c0a 2020 2020   overwrite,.    
-0001b2c0: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
-0001b2d0: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-0001b2e0: 2020 2020 2020 2073 746f 7261 6765 2c0a         storage,.
-0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b300: 7772 6974 655f 6f70 7469 6f6e 732c 0a20  write_options,. 
-0001b310: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0001b320: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
-0001b330: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
-0001b340: 0a0a 2020 2020 6465 6620 6669 6e61 6c69  ..    def finali
-0001b350: 7a65 5f6d 756c 7469 5f70 6172 745f 696e  ze_multi_part_in
-0001b360: 7365 7274 2873 656c 6629 3a0a 2020 2020  sert(self):.    
-0001b370: 2020 2020 2222 2246 696e 616c 697a 6573      """Finalizes
-0001b380: 2061 6e64 2065 7869 7473 2074 6865 206d   and exits the m
-0001b390: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
-0001b3a0: 2063 6f6e 7465 7874 206f 7065 6e65 6420   context opened 
-0001b3b0: 6279 2060 6d75 6c74 695f 7061 7274 5f69  by `multi_part_i
-0001b3c0: 6e73 6572 7460 0a20 2020 2020 2020 2069  nsert`.        i
-0001b3d0: 6e20 6120 626c 6f63 6b69 6e67 2066 6173  n a blocking fas
-0001b3e0: 6869 6f6e 206f 6e63 6520 616c 6c20 726f  hion once all ro
-0001b3f0: 7773 2068 6176 6520 6265 656e 2074 7261  ws have been tra
-0001b400: 6e73 6d69 7474 6564 2e0a 0a20 2020 2020  nsmitted...     
-0001b410: 2020 2021 2121 2065 7861 6d70 6c65 2022     !!! example "
-0001b420: 4d75 6c74 6920 7061 7274 2069 6e73 6572  Multi part inser
-0001b430: 7420 7769 7468 206d 616e 7561 6c20 636f  t with manual co
-0001b440: 6e74 6578 7420 6d61 6e61 6765 6d65 6e74  ntext management
-0001b450: 220a 2020 2020 2020 2020 2020 2020 496e  ".            In
-0001b460: 7374 6561 6420 6f66 206c 6574 7469 6e67  stead of letting
-0001b470: 2050 7974 686f 6e20 6861 6e64 6c65 2074   Python handle t
-0001b480: 6865 2065 6e74 6572 696e 6720 616e 6420  he entering and 
-0001b490: 6578 6974 696e 6720 6f66 2074 6865 0a20  exiting of the. 
-0001b4a0: 2020 2020 2020 2020 2020 206d 756c 7469             multi
-0001b4b0: 2070 6172 7420 696e 7365 7274 2063 6f6e   part insert con
-0001b4c0: 7465 7874 2c20 796f 7520 6361 6e20 7374  text, you can st
-0001b4d0: 6172 7420 616e 6420 6669 6e61 6c69 7a65  art and finalize
-0001b4e0: 2074 6865 2063 6f6e 7465 7874 0a20 2020   the context.   
-0001b4f0: 2020 2020 2020 2020 206d 616e 7561 6c6c           manuall
-0001b500: 792e 0a20 2020 2020 2020 2020 2020 2060  y..            `
-0001b510: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-0001b520: 2020 2020 2066 6561 7475 7265 5f67 726f       feature_gro
-0001b530: 7570 203d 2066 732e 6765 745f 6f72 5f63  up = fs.get_or_c
-0001b540: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-0001b550: 6f75 7028 2266 675f 6e61 6d65 222c 2076  oup("fg_name", v
-0001b560: 6572 7369 6f6e 3d31 290a 0a20 2020 2020  ersion=1)..     
-0001b570: 2020 2020 2020 2077 6869 6c65 206c 6f6f         while loo
-0001b580: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-0001b590: 2020 2073 6d61 6c6c 5f62 6174 6368 5f64     small_batch_d
-0001b5a0: 6620 3d20 2e2e 2e0a 2020 2020 2020 2020  f = ....        
-0001b5b0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
-0001b5c0: 6772 6f75 702e 6d75 6c74 695f 7061 7274  group.multi_part
-0001b5d0: 5f69 6e73 6572 7428 736d 616c 6c5f 6261  _insert(small_ba
-0001b5e0: 7463 685f 6466 290a 0a20 2020 2020 2020  tch_df)..       
-0001b5f0: 2020 2020 2023 2049 4d50 4f52 5441 4e54       # IMPORTANT
-0001b600: 3a20 6669 6e61 6c69 7a65 2074 6865 206d  : finalize the m
-0001b610: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
-0001b620: 2074 6f20 6d61 6b65 2073 7572 6520 616c   to make sure al
-0001b630: 6c20 726f 7773 0a20 2020 2020 2020 2020  l rows.         
-0001b640: 2020 2023 2068 6176 6520 6265 656e 2074     # have been t
-0001b650: 7261 6e73 6d69 7474 6564 0a20 2020 2020  ransmitted.     
-0001b660: 2020 2020 2020 2066 6561 7475 7265 5f67         feature_g
-0001b670: 726f 7570 2e66 696e 616c 697a 655f 6d75  roup.finalize_mu
-0001b680: 6c74 695f 7061 7274 5f69 6e73 6572 7428  lti_part_insert(
-0001b690: 290a 2020 2020 2020 2020 2020 2020 6060  ).            ``
-0001b6a0: 600a 2020 2020 2020 2020 2020 2020 4e6f  `.            No
-0001b6b0: 7465 2074 6861 7420 7468 6520 6669 7273  te that the firs
-0001b6c0: 7420 6361 6c6c 2074 6f20 606d 756c 7469  t call to `multi
-0001b6d0: 5f70 6172 745f 696e 7365 7274 6020 696e  _part_insert` in
-0001b6e0: 6974 6961 7465 7320 7468 6520 636f 6e74  itiates the cont
-0001b6f0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-0001b700: 616e 6420 6265 2073 7572 6520 746f 2066  and be sure to f
-0001b710: 696e 616c 697a 6520 6974 2e20 5468 6520  inalize it. The 
-0001b720: 6066 696e 616c 697a 655f 6d75 6c74 695f  `finalize_multi_
-0001b730: 7061 7274 5f69 6e73 6572 7460 2069 7320  part_insert` is 
-0001b740: 610a 2020 2020 2020 2020 2020 2020 626c  a.            bl
-0001b750: 6f63 6b69 6e67 2063 616c 6c20 7468 6174  ocking call that
-0001b760: 2072 6574 7572 6e73 206f 6e63 6520 616c   returns once al
-0001b770: 6c20 726f 7773 2068 6176 6520 6265 656e  l rows have been
-0001b780: 2074 7261 6e73 6d69 7474 6564 2e0a 2020   transmitted..  
-0001b790: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001b7a0: 2020 6966 2073 656c 662e 5f6b 6166 6b61    if self._kafka
-0001b7b0: 5f70 726f 6475 6365 7220 6973 206e 6f74  _producer is not
-0001b7c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001b7d0: 2020 2073 656c 662e 5f6b 6166 6b61 5f70     self._kafka_p
-0001b7e0: 726f 6475 6365 722e 666c 7573 6828 290a  roducer.flush().
-0001b7f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001b800: 2e5f 6b61 666b 615f 7072 6f64 7563 6572  ._kafka_producer
-0001b810: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0001b820: 7365 6c66 2e5f 6665 6174 7572 655f 7772  self._feature_wr
-0001b830: 6974 6572 7320 3d20 4e6f 6e65 0a20 2020  iters = None.   
-0001b840: 2020 2020 2073 656c 662e 5f77 7269 7465       self._write
-0001b850: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
-0001b860: 2073 656c 662e 5f6d 756c 7469 5f70 6172   self._multi_par
-0001b870: 745f 696e 7365 7274 203d 2046 616c 7365  t_insert = False
-0001b880: 0a0a 2020 2020 6465 6620 696e 7365 7274  ..    def insert
-0001b890: 5f73 7472 6561 6d28 0a20 2020 2020 2020  _stream(.       
-0001b8a0: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
-0001b8b0: 6561 7475 7265 733a 2054 7970 6556 6172  eatures: TypeVar
-0001b8c0: 2822 7079 7370 6172 6b2e 7371 6c2e 4461  ("pyspark.sql.Da
-0001b8d0: 7461 4672 616d 6522 292c 2020 2320 6e6f  taFrame"),  # no
-0001b8e0: 7161 3a20 4638 3231 0a20 2020 2020 2020  qa: F821.       
-0001b8f0: 2071 7565 7279 5f6e 616d 653a 204f 7074   query_name: Opt
-0001b900: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001b910: 652c 0a20 2020 2020 2020 206f 7574 7075  e,.        outpu
-0001b920: 745f 6d6f 6465 3a20 4f70 7469 6f6e 616c  t_mode: Optional
-0001b930: 5b73 7472 5d20 3d20 2261 7070 656e 6422  [str] = "append"
-0001b940: 2c0a 2020 2020 2020 2020 6177 6169 745f  ,.        await_
-0001b950: 7465 726d 696e 6174 696f 6e3a 204f 7074  termination: Opt
-0001b960: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4661  ional[bool] = Fa
-0001b970: 6c73 652c 0a20 2020 2020 2020 2074 696d  lse,.        tim
-0001b980: 656f 7574 3a20 4f70 7469 6f6e 616c 5b69  eout: Optional[i
-0001b990: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-0001b9a0: 2020 2020 6368 6563 6b70 6f69 6e74 5f64      checkpoint_d
-0001b9b0: 6972 3a20 4f70 7469 6f6e 616c 5b73 7472  ir: Optional[str
-0001b9c0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0001b9d0: 2020 7772 6974 655f 6f70 7469 6f6e 733a    write_options:
-0001b9e0: 204f 7074 696f 6e61 6c5b 4469 6374 5b41   Optional[Dict[A
-0001b9f0: 6e79 2c20 416e 795d 5d20 3d20 7b7d 2c0a  ny, Any]] = {},.
-0001ba00: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0001ba10: 2222 496e 6765 7374 2061 2053 7061 726b  ""Ingest a Spark
-0001ba20: 2053 7472 7563 7475 7265 6420 5374 7265   Structured Stre
-0001ba30: 616d 696e 6720 4461 7461 6672 616d 6520  aming Dataframe 
-0001ba40: 746f 2074 6865 206f 6e6c 696e 6520 6665  to the online fe
-0001ba50: 6174 7572 6520 7374 6f72 652e 0a0a 2020  ature store...  
-0001ba60: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
-0001ba70: 6420 6372 6561 7465 7320 6120 6c6f 6e67  d creates a long
-0001ba80: 2072 756e 6e69 6e67 2053 7061 726b 2053   running Spark S
-0001ba90: 7472 6561 6d69 6e67 2051 7565 7279 2c20  treaming Query, 
-0001baa0: 796f 7520 6361 6e20 636f 6e74 726f 6c20  you can control 
-0001bab0: 7468 650a 2020 2020 2020 2020 7465 726d  the.        term
-0001bac0: 696e 6174 696f 6e20 6f66 2074 6865 2071  ination of the q
-0001bad0: 7565 7279 2074 6872 6f75 6768 2074 6865  uery through the
-0001bae0: 2061 7267 756d 656e 7473 2e0a 0a20 2020   arguments...   
-0001baf0: 2020 2020 2049 7420 6973 2070 6f73 7369       It is possi
-0001bb00: 626c 6520 746f 2073 746f 7020 7468 6520  ble to stop the 
-0001bb10: 7265 7475 726e 6564 2071 7565 7279 2077  returned query w
-0001bb20: 6974 6820 7468 6520 602e 7374 6f70 2829  ith the `.stop()
-0001bb30: 6020 616e 6420 6368 6563 6b20 6974 730a  ` and check its.
-0001bb40: 2020 2020 2020 2020 7374 6174 7573 2077          status w
-0001bb50: 6974 6820 602e 6973 4163 7469 7665 602e  ith `.isActive`.
-0001bb60: 0a0a 2020 2020 2020 2020 546f 2067 6574  ..        To get
-0001bb70: 2061 206c 6973 7420 6f66 2061 6c6c 2061   a list of all a
-0001bb80: 6374 6976 6520 7175 6572 6965 732c 2075  ctive queries, u
-0001bb90: 7365 3a0a 0a20 2020 2020 2020 2060 6060  se:..        ```
-0001bba0: 7079 7468 6f6e 0a20 2020 2020 2020 2073  python.        s
-0001bbb0: 716d 203d 2073 7061 726b 2e73 7472 6561  qm = spark.strea
-0001bbc0: 6d73 0a0a 2020 2020 2020 2020 2320 6765  ms..        # ge
-0001bbd0: 7420 7468 6520 6c69 7374 206f 6620 6163  t the list of ac
-0001bbe0: 7469 7665 2073 7472 6561 6d69 6e67 2071  tive streaming q
-0001bbf0: 7565 7269 6573 0a20 2020 2020 2020 205b  ueries.        [
-0001bc00: 712e 6e61 6d65 2066 6f72 2071 2069 6e20  q.name for q in 
-0001bc10: 7371 6d2e 6163 7469 7665 5d0a 2020 2020  sqm.active].    
-0001bc20: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
-0001bc30: 2021 2121 2077 6172 6e69 6e67 2022 456e   !!! warning "En
-0001bc40: 6769 6e65 2053 7570 706f 7274 220a 2020  gine Support".  
-0001bc50: 2020 2020 2020 2020 2020 2a2a 5370 6172            **Spar
-0001bc60: 6b20 6f6e 6c79 2a2a 0a0a 2020 2020 2020  k only**..      
-0001bc70: 2020 2020 2020 5374 7265 616d 2069 6e67        Stream ing
-0001bc80: 6573 7469 6f6e 2075 7369 6e67 2050 616e  estion using Pan
-0001bc90: 6461 732f 5079 7468 6f6e 2061 7320 656e  das/Python as en
-0001bca0: 6769 6e65 2069 7320 6375 7272 656e 746c  gine is currentl
-0001bcb0: 7920 6e6f 7420 7375 7070 6f72 7465 642e  y not supported.
-0001bcc0: 0a20 2020 2020 2020 2020 2020 2050 7974  .            Pyt
-0001bcd0: 686f 6e2f 5061 6e64 6173 2068 6173 206e  hon/Pandas has n
-0001bce0: 6f20 6e6f 7469 6f6e 206f 6620 7374 7265  o notion of stre
-0001bcf0: 616d 696e 672e 0a0a 2020 2020 2020 2020  aming...        
-0001bd00: 2121 2120 7761 726e 696e 6720 2244 6174  !!! warning "Dat
-0001bd10: 6120 5661 6c69 6461 7469 6f6e 2053 7570  a Validation Sup
-0001bd20: 706f 7274 220a 2020 2020 2020 2020 2020  port".          
-0001bd30: 2020 6069 6e73 6572 745f 7374 7265 616d    `insert_stream
-0001bd40: 6020 646f 6573 206e 6f74 2070 6572 666f  ` does not perfo
-0001bd50: 726d 2061 6e79 2064 6174 6120 7661 6c69  rm any data vali
-0001bd60: 6461 7469 6f6e 2075 7369 6e67 2047 7265  dation using Gre
-0001bd70: 6174 2045 7870 6563 7461 7469 6f6e 730a  at Expectations.
-0001bd80: 2020 2020 2020 2020 2020 2020 6576 656e              even
-0001bd90: 2077 6865 6e20 6120 6578 7065 6374 6174   when a expectat
-0001bda0: 696f 6e20 7375 6974 6520 6973 2061 7474  ion suite is att
-0001bdb0: 6163 6865 642e 0a0a 2020 2020 2020 2020  ached...        
-0001bdc0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
-0001bdd0: 2020 2020 2020 2020 6665 6174 7572 6573          features
-0001bde0: 3a20 4665 6174 7572 6573 2069 6e20 5374  : Features in St
-0001bdf0: 7265 616d 696e 6720 4461 7461 6672 616d  reaming Datafram
-0001be00: 6520 746f 2062 6520 7361 7665 642e 0a20  e to be saved.. 
-0001be10: 2020 2020 2020 2020 2020 2071 7565 7279             query
-0001be20: 5f6e 616d 653a 2049 7420 6973 2070 6f73  _name: It is pos
-0001be30: 7369 626c 6520 746f 206f 7074 696f 6e61  sible to optiona
-0001be40: 6c6c 7920 7370 6563 6966 7920 6120 6e61  lly specify a na
-0001be50: 6d65 2066 6f72 2074 6865 2071 7565 7279  me for the query
-0001be60: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-0001be70: 2020 2020 6d61 6b65 2069 7420 6561 7369      make it easi
-0001be80: 6572 2074 6f20 7265 636f 676e 6973 6520  er to recognise 
-0001be90: 696e 2074 6865 2053 7061 726b 2055 492e  in the Spark UI.
-0001bea0: 2044 6566 6175 6c74 7320 746f 2060 4e6f   Defaults to `No
-0001beb0: 6e65 602e 0a20 2020 2020 2020 2020 2020  ne`..           
-0001bec0: 206f 7574 7075 745f 6d6f 6465 3a20 5370   output_mode: Sp
-0001bed0: 6563 6966 6965 7320 686f 7720 6461 7461  ecifies how data
-0001bee0: 206f 6620 6120 7374 7265 616d 696e 6720   of a streaming 
-0001bef0: 4461 7461 4672 616d 652f 4461 7461 7365  DataFrame/Datase
-0001bf00: 7420 6973 0a20 2020 2020 2020 2020 2020  t is.           
-0001bf10: 2020 2020 2077 7269 7474 656e 2074 6f20       written to 
-0001bf20: 6120 7374 7265 616d 696e 6720 7369 6e6b  a streaming sink
-0001bf30: 2e20 2831 2920 6022 6170 7065 6e64 2260  . (1) `"append"`
-0001bf40: 3a20 4f6e 6c79 2074 6865 206e 6577 2072  : Only the new r
-0001bf50: 6f77 7320 696e 2074 6865 0a20 2020 2020  ows in the.     
-0001bf60: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-0001bf70: 6d69 6e67 2044 6174 6146 7261 6d65 2f44  ming DataFrame/D
-0001bf80: 6174 6173 6574 2077 696c 6c20 6265 2077  ataset will be w
-0001bf90: 7269 7474 656e 2074 6f20 7468 6520 7369  ritten to the si
-0001bfa0: 6e6b 2e20 2832 290a 2020 2020 2020 2020  nk. (2).        
-0001bfb0: 2020 2020 2020 2020 6022 636f 6d70 6c65          `"comple
-0001bfc0: 7465 2260 3a20 416c 6c20 7468 6520 726f  te"`: All the ro
-0001bfd0: 7773 2069 6e20 7468 6520 7374 7265 616d  ws in the stream
-0001bfe0: 696e 6720 4461 7461 4672 616d 652f 4461  ing DataFrame/Da
-0001bff0: 7461 7365 7420 7769 6c6c 2062 650a 2020  taset will be.  
-0001c000: 2020 2020 2020 2020 2020 2020 2020 7772                wr
-0001c010: 6974 7465 6e20 746f 2074 6865 2073 696e  itten to the sin
-0001c020: 6b20 6576 6572 7920 7469 6d65 2074 6865  k every time the
-0001c030: 7265 2069 7320 736f 6d65 2075 7064 6174  re is some updat
-0001c040: 652e 2028 3329 2060 2275 7064 6174 6522  e. (3) `"update"
-0001c050: 603a 0a20 2020 2020 2020 2020 2020 2020  `:.             
-0001c060: 2020 206f 6e6c 7920 7468 6520 726f 7773     only the rows
-0001c070: 2074 6861 7420 7765 7265 2075 7064 6174   that were updat
-0001c080: 6564 2069 6e20 7468 6520 7374 7265 616d  ed in the stream
-0001c090: 696e 6720 4461 7461 4672 616d 652f 4461  ing DataFrame/Da
-0001c0a0: 7461 7365 7420 7769 6c6c 0a20 2020 2020  taset will.     
-0001c0b0: 2020 2020 2020 2020 2020 2062 6520 7772             be wr
-0001c0c0: 6974 7465 6e20 746f 2074 6865 2073 696e  itten to the sin
-0001c0d0: 6b20 6576 6572 7920 7469 6d65 2074 6865  k every time the
-0001c0e0: 7265 2061 7265 2073 6f6d 6520 7570 6461  re are some upda
-0001c0f0: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
-0001c100: 2020 2020 2049 6620 7468 6520 7175 6572       If the quer
-0001c110: 7920 646f 6573 6ee2 8099 7420 636f 6e74  y doesn...t cont
-0001c120: 6169 6e20 6167 6772 6567 6174 696f 6e73  ain aggregations
-0001c130: 2c20 6974 2077 696c 6c20 6265 2065 7175  , it will be equ
-0001c140: 6976 616c 656e 7420 746f 0a20 2020 2020  ivalent to.     
-0001c150: 2020 2020 2020 2020 2020 2061 7070 656e             appen
-0001c160: 6420 6d6f 6465 2e20 4465 6661 756c 7473  d mode. Defaults
-0001c170: 2074 6f20 6022 6170 7065 6e64 2260 2e0a   to `"append"`..
-0001c180: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-0001c190: 745f 7465 726d 696e 6174 696f 6e3a 2057  t_termination: W
-0001c1a0: 6169 7473 2066 6f72 2074 6865 2074 6572  aits for the ter
-0001c1b0: 6d69 6e61 7469 6f6e 206f 6620 7468 6973  mination of this
-0001c1c0: 2071 7565 7279 2c20 6569 7468 6572 2062   query, either b
-0001c1d0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0001c1e0: 2020 7175 6572 792e 7374 6f70 2829 206f    query.stop() o
-0001c1f0: 7220 6279 2061 6e20 6578 6365 7074 696f  r by an exceptio
-0001c200: 6e2e 2049 6620 7468 6520 7175 6572 7920  n. If the query 
-0001c210: 6861 7320 7465 726d 696e 6174 6564 2077  has terminated w
-0001c220: 6974 6820 616e 0a20 2020 2020 2020 2020  ith an.         
-0001c230: 2020 2020 2020 2065 7863 6570 7469 6f6e         exception
-0001c240: 2c20 7468 656e 2074 6865 2065 7863 6570  , then the excep
-0001c250: 7469 6f6e 2077 696c 6c20 6265 2074 6872  tion will be thr
-0001c260: 6f77 6e2e 2049 6620 7469 6d65 6f75 7420  own. If timeout 
-0001c270: 6973 2073 6574 2c20 6974 0a20 2020 2020  is set, it.     
-0001c280: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001c290: 6e73 2077 6865 7468 6572 2074 6865 2071  ns whether the q
-0001c2a0: 7565 7279 2068 6173 2074 6572 6d69 6e61  uery has termina
-0001c2b0: 7465 6420 6f72 206e 6f74 2077 6974 6869  ted or not withi
-0001c2c0: 6e20 7468 6520 7469 6d65 6f75 740a 2020  n the timeout.  
-0001c2d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001c2e0: 636f 6e64 732e 2044 6566 6175 6c74 7320  conds. Defaults 
-0001c2f0: 746f 2060 4661 6c73 6560 2e0a 2020 2020  to `False`..    
-0001c300: 2020 2020 2020 2020 7469 6d65 6f75 743a          timeout:
-0001c310: 204f 6e6c 7920 7265 6c65 7661 6e74 2069   Only relevant i
-0001c320: 6e20 636f 6d62 696e 6174 696f 6e20 7769  n combination wi
-0001c330: 7468 2060 6177 6169 745f 7465 726d 696e  th `await_termin
-0001c340: 6174 696f 6e3d 5472 7565 602e 0a20 2020  ation=True`..   
-0001c350: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-0001c360: 6175 6c74 7320 746f 2060 4e6f 6e65 602e  aults to `None`.
-0001c370: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-0001c380: 636b 706f 696e 745f 6469 723a 2043 6865  ckpoint_dir: Che
-0001c390: 636b 706f 696e 7420 6469 7265 6374 6f72  ckpoint director
-0001c3a0: 7920 6c6f 6361 7469 6f6e 2e20 5468 6973  y location. This
-0001c3b0: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
-0001c3c0: 2061 7320 6120 7265 6665 7265 6e63 6520   as a reference 
-0001c3d0: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
-0001c3e0: 2020 2066 726f 6d20 7768 6572 6520 746f     from where to
-0001c3f0: 2072 6573 756d 6520 7468 6520 7374 7265   resume the stre
-0001c400: 616d 696e 6720 6a6f 622e 2049 6620 604e  aming job. If `N
-0001c410: 6f6e 6560 2074 6865 6e20 6873 6673 2077  one` then hsfs w
-0001c420: 696c 6c20 636f 6e73 7472 7563 7420 6173  ill construct as
-0001c430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c440: 2022 696e 7365 7274 5f73 7472 6561 6d5f   "insert_stream_
-0001c450: 2220 2b20 6f6e 6c69 6e65 5f74 6f70 6963  " + online_topic
-0001c460: 5f6e 616d 652e 2044 6566 6175 6c74 7320  _name. Defaults 
-0001c470: 746f 2060 4e6f 6e65 602e 0a20 2020 2020  to `None`..     
-0001c480: 2020 2020 2020 2020 2020 2077 7269 7465             write
-0001c490: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
-0001c4a0: 6f6e 616c 2077 7269 7465 206f 7074 696f  onal write optio
-0001c4b0: 6e73 2066 6f72 2053 7061 726b 2061 7320  ns for Spark as 
-0001c4c0: 6b65 792d 7661 6c75 6520 7061 6972 732e  key-value pairs.
-0001c4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c4e0: 2044 6566 6175 6c74 7320 746f 2060 7b7d   Defaults to `{}
-0001c4f0: 602e 0a0a 2020 2020 2020 2020 2320 5265  `...        # Re
-0001c500: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
-0001c510: 2020 6053 7472 6561 6d69 6e67 5175 6572    `StreamingQuer
-0001c520: 7960 3a20 5370 6172 6b20 5374 7275 6374  y`: Spark Struct
-0001c530: 7572 6564 2053 7472 6561 6d69 6e67 2051  ured Streaming Q
-0001c540: 7565 7279 206f 626a 6563 742e 0a20 2020  uery object..   
-0001c550: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001c560: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-0001c570: 2020 6e6f 7420 656e 6769 6e65 2e67 6574    not engine.get
-0001c580: 5f69 6e73 7461 6e63 6528 292e 6973 5f73  _instance().is_s
-0001c590: 7061 726b 5f64 6174 6166 7261 6d65 2866  park_dataframe(f
-0001c5a0: 6561 7475 7265 7329 0a20 2020 2020 2020  eatures).       
-0001c5b0: 2020 2020 206f 7220 6e6f 7420 6665 6174       or not feat
-0001c5c0: 7572 6573 2e69 7353 7472 6561 6d69 6e67  ures.isStreaming
-0001c5d0: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-0001c5e0: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-0001c5f0: 7065 4572 726f 7228 0a20 2020 2020 2020  peError(.       
-0001c600: 2020 2020 2020 2020 2022 4665 6174 7572           "Featur
-0001c610: 6573 2068 6176 6520 746f 2062 6520 6120  es have to be a 
-0001c620: 7374 7265 616d 696e 6720 7479 7065 2073  streaming type s
-0001c630: 7061 726b 2064 6174 6166 7261 6d65 2e20  park dataframe. 
-0001c640: 5573 6520 6069 6e73 6572 7428 2960 206d  Use `insert()` m
-0001c650: 6574 686f 6420 696e 7374 6561 642e 220a  ethod instead.".
-0001c660: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001c670: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001c680: 2020 2020 2020 2020 2320 6c6f 7765 7220          # lower 
-0001c690: 6361 7369 6e67 2066 6561 7475 7265 206e  casing feature n
-0001c6a0: 616d 6573 0a20 2020 2020 2020 2020 2020  ames.           
-0001c6b0: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
-0001c6c0: 6d65 203d 2065 6e67 696e 652e 6765 745f  me = engine.get_
-0001c6d0: 696e 7374 616e 6365 2829 2e63 6f6e 7665  instance().conve
-0001c6e0: 7274 5f74 6f5f 6465 6661 756c 745f 6461  rt_to_default_da
-0001c6f0: 7461 6672 616d 6528 0a20 2020 2020 2020  taframe(.       
-0001c700: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-0001c710: 730a 2020 2020 2020 2020 2020 2020 290a  s.            ).
-0001c720: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-0001c730: 696e 6773 2e77 6172 6e28 0a20 2020 2020  ings.warn(.     
-0001c740: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-0001c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c760: 2022 5374 7265 616d 2069 6e67 6573 7469   "Stream ingesti
-0001c770: 6f6e 2066 6f72 2066 6561 7475 7265 2067  on for feature g
-0001c780: 726f 7570 2060 7b7d 602c 2077 6974 6820  roup `{}`, with 
-0001c790: 7665 7273 696f 6e22 0a20 2020 2020 2020  version".       
-0001c7a0: 2020 2020 2020 2020 2020 2020 2022 2060               " `
-0001c7b0: 7b7d 6020 7769 6c6c 206e 6f74 2063 6f6d  {}` will not com
-0001c7c0: 7075 7465 2073 7461 7469 7374 6963 732e  pute statistics.
-0001c7d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001c7e0: 2020 292e 666f 726d 6174 2873 656c 662e    ).format(self.
-0001c7f0: 5f6e 616d 652c 2073 656c 662e 5f76 6572  _name, self._ver
-0001c800: 7369 6f6e 292c 0a20 2020 2020 2020 2020  sion),.         
-0001c810: 2020 2020 2020 2075 7469 6c2e 5374 6174         util.Stat
-0001c820: 6973 7469 6373 5761 726e 696e 672c 0a20  isticsWarning,. 
-0001c830: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0001c840: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001c850: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
-0001c860: 726f 7570 5f65 6e67 696e 652e 696e 7365  roup_engine.inse
-0001c870: 7274 5f73 7472 6561 6d28 0a20 2020 2020  rt_stream(.     
-0001c880: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-0001c890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c8a0: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
-0001c8b0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0001c8c0: 2020 2020 7175 6572 795f 6e61 6d65 2c0a      query_name,.
-0001c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8e0: 6f75 7470 7574 5f6d 6f64 652c 0a20 2020  output_mode,.   
-0001c8f0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-0001c900: 6974 5f74 6572 6d69 6e61 7469 6f6e 2c0a  it_termination,.
-0001c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c920: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
-0001c930: 2020 2020 2020 2020 2063 6865 636b 706f           checkpo
-0001c940: 696e 745f 6469 722c 0a20 2020 2020 2020  int_dir,.       
-0001c950: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-0001c960: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
-0001c970: 2020 2020 290a 0a20 2020 2064 6566 2063      )..    def c
-0001c980: 6f6d 6d69 745f 6465 7461 696c 7328 0a20  ommit_details(. 
-0001c990: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0001c9a0: 2020 2020 2077 616c 6c63 6c6f 636b 5f74       wallclock_t
-0001c9b0: 696d 653a 204f 7074 696f 6e61 6c5b 556e  ime: Optional[Un
-0001c9c0: 696f 6e5b 7374 722c 2069 6e74 2c20 6461  ion[str, int, da
-0001c9d0: 7465 7469 6d65 2c20 6461 7465 5d5d 203d  tetime, date]] =
-0001c9e0: 204e 6f6e 652c 0a20 2020 2020 2020 206c   None,.        l
-0001c9f0: 696d 6974 3a20 4f70 7469 6f6e 616c 5b69  imit: Optional[i
-0001ca00: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-0001ca10: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-0001ca20: 7472 6965 7665 7320 636f 6d6d 6974 2074  trieves commit t
-0001ca30: 696d 656c 696e 6520 666f 7220 7468 6973  imeline for this
-0001ca40: 2066 6561 7475 7265 2067 726f 7570 2e20   feature group. 
-0001ca50: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-0001ca60: 6f6e 6c79 2062 6520 7573 6564 0a20 2020  only be used.   
-0001ca70: 2020 2020 206f 6e20 7469 6d65 2074 7261       on time tra
-0001ca80: 7665 6c20 656e 6162 6c65 6420 6665 6174  vel enabled feat
-0001ca90: 7572 6520 6772 6f75 7073 0a0a 2020 2020  ure groups..    
-0001caa0: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
-0001cab0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-0001cac0: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-0001cad0: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
-0001cae0: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
-0001caf0: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
-0001cb00: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
-0001cb10: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
-0001cb20: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
-0001cb30: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-0001cb40: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
-0001cb50: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-0001cb60: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
-0001cb70: 2020 2020 2020 636f 6d6d 6974 5f64 6574        commit_det
-0001cb80: 6169 6c73 203d 2066 672e 636f 6d6d 6974  ails = fg.commit
-0001cb90: 5f64 6574 6169 6c73 2829 0a20 2020 2020  _details().     
-0001cba0: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-0001cbb0: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
-0001cbc0: 2020 2020 2020 2020 2020 2020 7761 6c6c              wall
-0001cbd0: 636c 6f63 6b5f 7469 6d65 3a20 436f 6d6d  clock_time: Comm
-0001cbe0: 6974 2064 6574 6169 6c73 2061 7320 6f66  it details as of
-0001cbf0: 2073 7065 6369 6669 6320 706f 696e 7420   specific point 
-0001cc00: 696e 2074 696d 652e 2044 6566 6175 6c74  in time. Default
-0001cc10: 7320 746f 2060 4e6f 6e65 602e 0a20 2020  s to `None`..   
-0001cc20: 2020 2020 2020 2020 2020 2020 2020 5374                St
-0001cc30: 7269 6e67 7320 7368 6f75 6c64 2062 6520  rings should be 
-0001cc40: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
-0001cc50: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-0001cc60: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
-0001cc70: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
-0001cc80: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
-0001cc90: 483a 254d 602c 0a20 2020 2020 2020 2020  H:%M`,.         
-0001cca0: 2020 2020 2020 2060 2559 2d25 6d2d 2564         `%Y-%m-%d
-0001ccb0: 2025 483a 254d 3a25 5360 2c20 6f72 2060   %H:%M:%S`, or `
-0001ccc0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-0001ccd0: 532e 2566 602e 0a20 2020 2020 2020 2020  S.%f`..         
-0001cce0: 2020 206c 696d 6974 3a20 4e75 6d62 6572     limit: Number
-0001ccf0: 206f 6620 636f 6d6d 6974 7320 746f 2072   of commits to r
-0001cd00: 6574 7269 6576 652e 2044 6566 6175 6c74  etrieve. Default
-0001cd10: 7320 746f 2060 4e6f 6e65 602e 0a0a 2020  s to `None`...  
-0001cd20: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
-0001cd30: 2020 2020 2020 2020 2020 2020 6044 6963              `Dic
-0001cd40: 745b 7374 722c 2044 6963 745b 7374 722c  t[str, Dict[str,
-0001cd50: 2073 7472 5d5d 602e 2044 6963 7469 6f6e   str]]`. Diction
-0001cd60: 6172 7920 6f62 6a65 6374 206f 6620 636f  ary object of co
-0001cd70: 6d6d 6974 206d 6574 6164 6174 6120 7469  mmit metadata ti
-0001cd80: 6d65 6c69 6e65 2c20 7768 6572 6520 4b65  meline, where Ke
-0001cd90: 7920 6973 2063 6f6d 6d69 7420 6964 2061  y is commit id a
-0001cda0: 6e64 2076 616c 7565 0a20 2020 2020 2020  nd value.       
-0001cdb0: 2020 2020 2069 7320 6044 6963 745b 7374       is `Dict[st
-0001cdc0: 722c 2073 7472 5d60 2077 6974 6820 6b65  r, str]` with ke
-0001cdd0: 7920 7661 6c75 6520 7061 6972 7320 6f66  y value pairs of
-0001cde0: 2064 6174 6520 636f 6d6d 6974 7465 6420   date committed 
-0001cdf0: 6f6e 2c20 6e75 6d62 6572 206f 6620 726f  on, number of ro
-0001ce00: 7773 2075 7064 6174 6564 2c20 696e 7365  ws updated, inse
-0001ce10: 7274 6564 2061 6e64 2064 656c 6574 6564  rted and deleted
-0001ce20: 2e0a 0a20 2020 2020 2020 2023 2052 6169  ...        # Rai
-0001ce30: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-0001ce40: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
-0001ce50: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
-0001ce60: 7272 6f72 602e 0a20 2020 2020 2020 2020  rror`..         
-0001ce70: 2020 2060 6873 6673 2e63 6c69 656e 742e     `hsfs.client.
-0001ce80: 6578 6365 7074 696f 6e73 2e46 6561 7475  exceptions.Featu
-0001ce90: 7265 5374 6f72 6545 7863 6570 7469 6f6e  reStoreException
-0001cea0: 602e 2049 6620 7468 6520 6665 6174 7572  `. If the featur
-0001ceb0: 6520 6772 6f75 7020 646f 6573 206e 6f74  e group does not
-0001cec0: 2068 6176 6520 6048 5544 4960 2074 696d   have `HUDI` tim
-0001ced0: 6520 7472 6176 656c 2066 6f72 6d61 740a  e travel format.
-0001cee0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001cef0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001cf00: 5f66 6561 7475 7265 5f67 726f 7570 5f65  _feature_group_e
-0001cf10: 6e67 696e 652e 636f 6d6d 6974 5f64 6574  ngine.commit_det
-0001cf20: 6169 6c73 2873 656c 662c 2077 616c 6c63  ails(self, wallc
-0001cf30: 6c6f 636b 5f74 696d 652c 206c 696d 6974  lock_time, limit
-0001cf40: 290a 0a20 2020 2064 6566 2063 6f6d 6d69  )..    def commi
-0001cf50: 745f 6465 6c65 7465 5f72 6563 6f72 6428  t_delete_record(
-0001cf60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0001cf70: 2020 2020 2020 2064 656c 6574 655f 6466         delete_df
-0001cf80: 3a20 5479 7065 5661 7228 2270 7973 7061  : TypeVar("pyspa
-0001cf90: 726b 2e73 716c 2e44 6174 6146 7261 6d65  rk.sql.DataFrame
-0001cfa0: 2229 2c20 2023 206e 6f71 613a 2046 3832  "),  # noqa: F82
-0001cfb0: 310a 2020 2020 2020 2020 7772 6974 655f  1.        write_
-0001cfc0: 6f70 7469 6f6e 733a 204f 7074 696f 6e61  options: Optiona
-0001cfd0: 6c5b 4469 6374 5b41 6e79 2c20 416e 795d  l[Dict[Any, Any]
-0001cfe0: 5d20 3d20 7b7d 2c0a 2020 2020 293a 0a20  ] = {},.    ):. 
-0001cff0: 2020 2020 2020 2022 2222 4472 6f70 7320         """Drops 
-0001d000: 7265 636f 7264 7320 7072 6573 656e 7420  records present 
-0001d010: 696e 2074 6865 2070 726f 7669 6465 6420  in the provided 
-0001d020: 4461 7461 4672 616d 6520 616e 6420 636f  DataFrame and co
-0001d030: 6d6d 6974 7320 6974 2061 7320 7570 6461  mmits it as upda
-0001d040: 7465 2074 6f20 7468 6973 0a20 2020 2020  te to this.     
-0001d050: 2020 2046 6561 7475 7265 2067 726f 7570     Feature group
-0001d060: 2e20 5468 6973 206d 6574 686f 6420 6361  . This method ca
-0001d070: 6e20 6f6e 6c79 2062 6520 7573 6564 206f  n only be used o
-0001d080: 6e20 6665 6174 7572 6520 6772 6f75 7073  n feature groups
-0001d090: 2073 746f 7265 6420 6173 2048 5544 4920   stored as HUDI 
-0001d0a0: 6f72 2044 454c 5441 2e0a 0a20 2020 2020  or DELTA...     
-0001d0b0: 2020 2023 2041 7267 756d 656e 7473 0a20     # Arguments. 
-0001d0c0: 2020 2020 2020 2020 2020 2064 656c 6574             delet
-0001d0d0: 655f 6466 3a20 6461 7461 4672 616d 6520  e_df: dataFrame 
-0001d0e0: 636f 6e74 6169 6e69 6e67 2072 6563 6f72  containing recor
-0001d0f0: 6473 2074 6f20 6265 2064 656c 6574 6564  ds to be deleted
-0001d100: 2e0a 2020 2020 2020 2020 2020 2020 7772  ..            wr
-0001d110: 6974 655f 6f70 7469 6f6e 733a 2055 7365  ite_options: Use
-0001d120: 7220 7072 6f76 6964 6564 2077 7269 7465  r provided write
-0001d130: 206f 7074 696f 6e73 2e20 4465 6661 756c   options. Defaul
-0001d140: 7473 2074 6f20 607b 7d60 2e0a 0a20 2020  ts to `{}`...   
-0001d150: 2020 2020 2023 2052 6169 7365 730a 2020       # Raises.  
-0001d160: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
-0001d170: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
-0001d180: 732e 5265 7374 4150 4945 7272 6f72 602e  s.RestAPIError`.
-0001d190: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001d1a0: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-0001d1b0: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
-0001d1c0: 636f 6d6d 6974 5f64 656c 6574 6528 7365  commit_delete(se
-0001d1d0: 6c66 2c20 6465 6c65 7465 5f64 662c 2077  lf, delete_df, w
-0001d1e0: 7269 7465 5f6f 7074 696f 6e73 290a 0a20  rite_options).. 
-0001d1f0: 2020 2064 6566 2061 735f 6f66 280a 2020     def as_of(.  
-0001d200: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0001d210: 2020 2020 7761 6c6c 636c 6f63 6b5f 7469      wallclock_ti
-0001d220: 6d65 3a20 4f70 7469 6f6e 616c 5b55 6e69  me: Optional[Uni
-0001d230: 6f6e 5b73 7472 2c20 696e 742c 2064 6174  on[str, int, dat
-0001d240: 6574 696d 652c 2064 6174 655d 5d20 3d20  etime, date]] = 
-0001d250: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
-0001d260: 636c 7564 655f 756e 7469 6c3a 204f 7074  clude_until: Opt
-0001d270: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-0001d280: 2069 6e74 2c20 6461 7465 7469 6d65 2c20   int, datetime, 
-0001d290: 6461 7465 5d5d 203d 204e 6f6e 652c 0a20  date]] = None,. 
-0001d2a0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0001d2b0: 2247 6574 2051 7565 7279 206f 626a 6563  "Get Query objec
-0001d2c0: 7420 746f 2072 6574 7269 6576 6520 616c  t to retrieve al
-0001d2d0: 6c20 6665 6174 7572 6573 206f 6620 7468  l features of th
-0001d2e0: 6520 6772 6f75 7020 6174 2061 2070 6f69  e group at a poi
-0001d2f0: 6e74 2069 6e20 7468 6520 7061 7374 2e0a  nt in the past..
-0001d300: 0a20 2020 2020 2020 2054 6869 7320 6d65  .        This me
-0001d310: 7468 6f64 2073 656c 6563 7473 2061 6c6c  thod selects all
-0001d320: 2066 6561 7475 7265 7320 696e 2074 6865   features in the
-0001d330: 2066 6561 7475 7265 2067 726f 7570 2061   feature group a
-0001d340: 6e64 2072 6574 7572 6e73 2061 2051 7565  nd returns a Que
-0001d350: 7279 206f 626a 6563 740a 2020 2020 2020  ry object.      
-0001d360: 2020 6174 2074 6865 2073 7065 6369 6669    at the specifi
-0001d370: 6564 2070 6f69 6e74 2069 6e20 7469 6d65  ed point in time
-0001d380: 2e20 4f70 7469 6f6e 616c 6c79 2c20 636f  . Optionally, co
-0001d390: 6d6d 6974 7320 6265 666f 7265 2061 2073  mmits before a s
-0001d3a0: 7065 6369 6669 6564 2070 6f69 6e74 2069  pecified point i
-0001d3b0: 6e20 7469 6d65 2063 616e 2062 650a 2020  n time can be.  
-0001d3c0: 2020 2020 2020 6578 636c 7564 6564 2066        excluded f
-0001d3d0: 726f 6d20 7468 6520 7175 6572 792e 2054  rom the query. T
-0001d3e0: 6865 2051 7565 7279 2063 616e 2074 6865  he Query can the
-0001d3f0: 6e20 6569 7468 6572 2062 6520 7265 6164  n either be read
-0001d400: 2069 6e74 6f20 6120 4461 7461 6672 616d   into a Datafram
-0001d410: 650a 2020 2020 2020 2020 6f72 2075 7365  e.        or use
-0001d420: 6420 6675 7274 6865 7220 746f 2070 6572  d further to per
-0001d430: 666f 726d 206a 6f69 6e73 206f 7220 636f  form joins or co
-0001d440: 6e73 7472 7563 7420 6120 7472 6169 6e69  nstruct a traini
-0001d450: 6e67 2064 6174 6173 6574 2e0a 0a20 2020  ng dataset...   
-0001d460: 2020 2020 2021 2121 2065 7861 6d70 6c65       !!! example
-0001d470: 2022 5265 6164 696e 6720 6665 6174 7572   "Reading featur
-0001d480: 6573 2061 7420 6120 7370 6563 6966 6963  es at a specific
-0001d490: 2070 6f69 6e74 2069 6e20 7469 6d65 3a22   point in time:"
-0001d4a0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-0001d4b0: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
-0001d4c0: 2020 2023 2063 6f6e 6e65 6374 2074 6f20     # connect to 
-0001d4d0: 7468 6520 4665 6174 7572 6520 5374 6f72  the Feature Stor
-0001d4e0: 650a 2020 2020 2020 2020 2020 2020 6673  e.            fs
-0001d4f0: 203d 202e 2e2e 0a0a 2020 2020 2020 2020   = .....        
-0001d500: 2020 2020 2320 6765 7420 7468 6520 4665      # get the Fe
-0001d510: 6174 7572 6520 4772 6f75 7020 696e 7374  ature Group inst
-0001d520: 616e 6365 0a20 2020 2020 2020 2020 2020  ance.           
-0001d530: 2066 6720 3d20 6673 2e67 6574 5f6f 725f   fg = fs.get_or_
-0001d540: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
-0001d550: 726f 7570 282e 2e2e 290a 0a20 2020 2020  roup(...)..     
-0001d560: 2020 2020 2020 2023 2067 6574 2064 6174         # get dat
-0001d570: 6120 6174 2061 2073 7065 6369 6669 6320  a at a specific 
-0001d580: 706f 696e 7420 696e 2074 696d 6520 616e  point in time an
-0001d590: 6420 7368 6f77 2069 740a 2020 2020 2020  d show it.      
-0001d5a0: 2020 2020 2020 6667 2e61 735f 6f66 2822        fg.as_of("
-0001d5b0: 3230 3230 2d31 302d 3230 2030 373a 3334  2020-10-20 07:34
-0001d5c0: 3a31 3122 292e 7265 6164 2829 2e73 686f  :11").read().sho
-0001d5d0: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-0001d5e0: 6060 600a 0a20 2020 2020 2020 2021 2121  ```..        !!!
-0001d5f0: 2065 7861 6d70 6c65 2022 5265 6164 696e   example "Readin
-0001d600: 6720 636f 6d6d 6974 7320 696e 6372 656d  g commits increm
-0001d610: 656e 7461 6c6c 7920 6265 7477 6565 6e20  entally between 
-0001d620: 7370 6563 6966 6965 6420 706f 696e 7473  specified points
-0001d630: 2069 6e20 7469 6d65 3a22 0a20 2020 2020   in time:".     
-0001d640: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-0001d650: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-0001d660: 6173 5f6f 6628 2232 3032 302d 3130 2d32  as_of("2020-10-2
-0001d670: 3020 3037 3a33 343a 3131 222c 2065 7863  0 07:34:11", exc
-0001d680: 6c75 6465 5f75 6e74 696c 3d22 3230 3230  lude_until="2020
-0001d690: 2d31 302d 3139 2030 373a 3334 3a31 3122  -10-19 07:34:11"
-0001d6a0: 292e 7265 6164 2829 2e73 686f 7728 290a  ).read().show().
-0001d6b0: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
-0001d6c0: 0a20 2020 2020 2020 2054 6865 2066 6972  .        The fir
-0001d6d0: 7374 2070 6172 616d 6574 6572 2069 7320  st parameter is 
-0001d6e0: 696e 636c 7573 6976 6520 7768 696c 6520  inclusive while 
-0001d6f0: 7468 6520 6c61 7474 6572 2069 7320 6578  the latter is ex
-0001d700: 636c 7573 6976 652e 0a20 2020 2020 2020  clusive..       
-0001d710: 2054 6861 7420 6d65 616e 732c 2069 6e20   That means, in 
-0001d720: 6f72 6465 7220 746f 2071 7565 7279 2061  order to query a
-0001d730: 2073 696e 676c 6520 636f 6d6d 6974 2c20   single commit, 
-0001d740: 796f 7520 6e65 6564 2074 6f20 7175 6572  you need to quer
-0001d750: 7920 7468 6174 2063 6f6d 6d69 7420 7469  y that commit ti
-0001d760: 6d65 0a20 2020 2020 2020 2061 6e64 2065  me.        and e
-0001d770: 7863 6c75 6465 2065 7665 7279 7468 696e  xclude everythin
-0001d780: 6720 6a75 7374 2062 6566 6f72 6520 7468  g just before th
-0001d790: 6520 636f 6d6d 6974 2e0a 0a20 2020 2020  e commit...     
-0001d7a0: 2020 2021 2121 2065 7861 6d70 6c65 2022     !!! example "
-0001d7b0: 5265 6164 696e 6720 6f6e 6c79 2074 6865  Reading only the
-0001d7c0: 2063 6861 6e67 6573 2066 726f 6d20 6120   changes from a 
-0001d7d0: 7369 6e67 6c65 2063 6f6d 6d69 7422 0a20  single commit". 
-0001d7e0: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
-0001d7f0: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
-0001d800: 2066 672e 6173 5f6f 6628 2232 3032 302d   fg.as_of("2020-
-0001d810: 3130 2d32 3020 3037 3a33 313a 3338 222c  10-20 07:31:38",
-0001d820: 2065 7863 6c75 6465 5f75 6e74 696c 3d22   exclude_until="
-0001d830: 3230 3230 2d31 302d 3230 2030 373a 3331  2020-10-20 07:31
-0001d840: 3a33 3722 292e 7265 6164 2829 2e73 686f  :37").read().sho
-0001d850: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-0001d860: 6060 600a 0a20 2020 2020 2020 2057 6865  ```..        Whe
-0001d870: 6e20 6e6f 2077 616c 6c63 6c6f 636b 5f74  n no wallclock_t
-0001d880: 696d 6520 6973 2067 6976 656e 2c20 7468  ime is given, th
-0001d890: 6520 6c61 7465 7374 2073 7461 7465 206f  e latest state o
-0001d8a0: 6620 6665 6174 7572 6573 2069 7320 7265  f features is re
-0001d8b0: 7475 726e 6564 2e20 4f70 7469 6f6e 616c  turned. Optional
-0001d8c0: 6c79 2c20 636f 6d6d 6974 7320 6265 666f  ly, commits befo
-0001d8d0: 7265 0a20 2020 2020 2020 2061 2073 7065  re.        a spe
-0001d8e0: 6369 6669 6564 2070 6f69 6e74 2069 6e20  cified point in 
-0001d8f0: 7469 6d65 2063 616e 2073 7469 6c6c 2062  time can still b
-0001d900: 6520 6578 636c 7564 6564 2e0a 0a20 2020  e excluded...   
-0001d910: 2020 2020 2021 2121 2065 7861 6d70 6c65       !!! example
-0001d920: 2022 5265 6164 696e 6720 7468 6520 6c61   "Reading the la
-0001d930: 7465 7374 2073 7461 7465 206f 6620 6665  test state of fe
-0001d940: 6174 7572 6573 2c20 6578 636c 7564 696e  atures, excludin
-0001d950: 6720 636f 6d6d 6974 7320 6265 666f 7265  g commits before
-0001d960: 2061 2073 7065 6369 6669 6564 2070 6f69   a specified poi
-0001d970: 6e74 2069 6e20 7469 6d65 3a22 0a20 2020  nt in time:".   
-0001d980: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
-0001d990: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
-0001d9a0: 672e 6173 5f6f 6628 4e6f 6e65 2c20 6578  g.as_of(None, ex
-0001d9b0: 636c 7564 655f 756e 7469 6c3d 2232 3032  clude_until="202
-0001d9c0: 302d 3130 2d32 3020 3037 3a33 313a 3338  0-10-20 07:31:38
-0001d9d0: 2229 2e72 6561 6428 292e 7368 6f77 2829  ").read().show()
-0001d9e0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-0001d9f0: 0a0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
-0001da00: 6861 7420 7468 6520 696e 7465 7276 616c  hat the interval
-0001da10: 2077 696c 6c20 6265 2061 7070 6c69 6564   will be applied
-0001da20: 2074 6f20 616c 6c20 6a6f 696e 7320 696e   to all joins in
-0001da30: 2074 6865 2071 7565 7279 2e0a 2020 2020   the query..    
-0001da40: 2020 2020 4966 2079 6f75 2077 616e 7420      If you want 
-0001da50: 746f 2071 7565 7279 2064 6966 6665 7265  to query differe
-0001da60: 6e74 2069 6e74 6572 7661 6c73 2066 6f72  nt intervals for
-0001da70: 2064 6966 6665 7265 6e74 2066 6561 7475   different featu
-0001da80: 7265 2067 726f 7570 7320 696e 0a20 2020  re groups in.   
-0001da90: 2020 2020 2074 6865 2071 7565 7279 2c20       the query, 
-0001daa0: 796f 7520 6861 7665 2074 6f20 6170 706c  you have to appl
-0001dab0: 7920 7468 656d 2069 6e20 6120 6e65 7374  y them in a nest
-0001dac0: 6564 2066 6173 6869 6f6e 3a0a 2020 2020  ed fashion:.    
-0001dad0: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
-0001dae0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-0001daf0: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-0001db00: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
-0001db10: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
-0001db20: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
-0001db30: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
-0001db40: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
-0001db50: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
-0001db60: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-0001db70: 6667 3120 3d20 6673 2e67 6574 5f6f 725f  fg1 = fs.get_or_
-0001db80: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
-0001db90: 726f 7570 282e 2e2e 290a 2020 2020 2020  roup(...).      
-0001dba0: 2020 2020 2020 6667 3220 3d20 6673 2e67        fg2 = fs.g
-0001dbb0: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-0001dbc0: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
-0001dbd0: 0a20 2020 2020 2020 2020 2020 2066 6731  .            fg1
-0001dbe0: 2e73 656c 6563 745f 616c 6c28 292e 6173  .select_all().as
-0001dbf0: 5f6f 6628 2232 3032 302d 3130 2d32 3022  _of("2020-10-20"
-0001dc00: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
-0001dc10: 2232 3032 302d 3130 2d31 3922 290a 2020  "2020-10-19").  
-0001dc20: 2020 2020 2020 2020 2020 2020 2020 2e6a                .j
-0001dc30: 6f69 6e28 6667 322e 7365 6c65 6374 5f61  oin(fg2.select_a
-0001dc40: 6c6c 2829 2e61 735f 6f66 2822 3230 3230  ll().as_of("2020
-0001dc50: 2d31 302d 3230 222c 2065 7863 6c75 6465  -10-20", exclude
-0001dc60: 5f75 6e74 696c 3d22 3230 3230 2d31 302d  _until="2020-10-
-0001dc70: 3139 2229 290a 2020 2020 2020 2020 2020  19")).          
-0001dc80: 2020 6060 600a 0a20 2020 2020 2020 2049    ```..        I
-0001dc90: 6620 696e 7374 6561 6420 796f 7520 6170  f instead you ap
-0001dca0: 706c 7920 616e 6f74 6865 7220 6061 735f  ply another `as_
-0001dcb0: 6f66 6020 7365 6c65 6374 696f 6e20 6166  of` selection af
-0001dcc0: 7465 7220 7468 6520 6a6f 696e 2c20 616c  ter the join, al
-0001dcd0: 6c0a 2020 2020 2020 2020 6a6f 696e 6564  l.        joined
-0001dce0: 2066 6561 7475 7265 2067 726f 7570 7320   feature groups 
-0001dcf0: 7769 6c6c 2062 6520 7175 6572 6965 6420  will be queried 
-0001dd00: 7769 7468 2074 6869 7320 696e 7465 7276  with this interv
-0001dd10: 616c 3a0a 2020 2020 2020 2020 2121 2120  al:.        !!! 
-0001dd20: 6578 616d 706c 650a 2020 2020 2020 2020  example.        
-0001dd30: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
-0001dd40: 2020 2020 2020 2020 2020 6667 312e 7365            fg1.se
-0001dd50: 6c65 6374 5f61 6c6c 2829 2e61 735f 6f66  lect_all().as_of
-0001dd60: 2822 3230 3230 2d31 302d 3230 222c 2065  ("2020-10-20", e
-0001dd70: 7863 6c75 6465 5f75 6e74 696c 3d22 3230  xclude_until="20
-0001dd80: 3230 2d31 302d 3139 2229 2020 2320 6173  20-10-19")  # as
-0001dd90: 5f6f 6620 6973 206e 6f74 2061 7070 6c69  _of is not appli
-0001dda0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
-0001ddb0: 2020 202e 6a6f 696e 2866 6732 2e73 656c     .join(fg2.sel
-0001ddc0: 6563 745f 616c 6c28 292e 6173 5f6f 6628  ect_all().as_of(
-0001ddd0: 2232 3032 302d 3130 2d32 3022 2c20 6578  "2020-10-20", ex
-0001dde0: 636c 7564 655f 756e 7469 6c3d 2232 3032  clude_until="202
-0001ddf0: 302d 3130 2d31 3522 2929 2020 2320 6173  0-10-15"))  # as
-0001de00: 5f6f 6620 6973 206e 6f74 2061 7070 6c69  _of is not appli
-0001de10: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
-0001de20: 2020 202e 6173 5f6f 6628 2232 3032 302d     .as_of("2020-
-0001de30: 3130 2d32 3022 2c20 6578 636c 7564 655f  10-20", exclude_
-0001de40: 756e 7469 6c3d 2232 3032 302d 3130 2d31  until="2020-10-1
-0001de50: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
-0001de60: 6060 600a 0a20 2020 2020 2020 2021 2121  ```..        !!!
-0001de70: 2077 6172 6e69 6e67 0a20 2020 2020 2020   warning.       
-0001de80: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
-0001de90: 6f6e 206f 6e6c 7920 776f 726b 7320 666f  on only works fo
-0001dea0: 7220 6665 6174 7572 6520 6772 6f75 7073  r feature groups
-0001deb0: 2077 6974 6820 7469 6d65 5f74 7261 7665   with time_trave
-0001dec0: 6c5f 666f 726d 6174 3d27 4855 4449 272e  l_format='HUDI'.
-0001ded0: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
-0001dee0: 726e 696e 670a 2020 2020 2020 2020 2020  rning.          
-0001def0: 2020 4578 636c 7564 696e 6720 636f 6d6d    Excluding comm
-0001df00: 6974 7320 7669 6120 6578 636c 7564 655f  its via exclude_
-0001df10: 756e 7469 6c20 6973 206f 6e6c 7920 706f  until is only po
-0001df20: 7373 6962 6c65 2077 6974 6869 6e20 7468  ssible within th
-0001df30: 6520 7261 6e67 6520 6f66 2074 6865 2048  e range of the H
-0001df40: 7564 6920 6163 7469 7665 2074 696d 656c  udi active timel
-0001df50: 696e 652e 0a20 2020 2020 2020 2020 2020  ine..           
-0001df60: 2042 7920 6465 6661 756c 742c 2048 7564   By default, Hud
-0001df70: 6920 6b65 6570 7320 7468 6520 6c61 7374  i keeps the last
-0001df80: 2032 3020 746f 2033 3020 636f 6d6d 6974   20 to 30 commit
-0001df90: 7320 696e 2074 6865 2061 6374 6976 6520  s in the active 
-0001dfa0: 7469 6d65 6c69 6e65 2e0a 2020 2020 2020  timeline..      
-0001dfb0: 2020 2020 2020 4966 2079 6f75 206e 6565        If you nee
-0001dfc0: 6420 746f 206b 6565 7020 6120 6c6f 6e67  d to keep a long
-0001dfd0: 6572 2061 6374 6976 6520 7469 6d65 6c69  er active timeli
-0001dfe0: 6e65 2c20 796f 7520 6361 6e20 6f76 6572  ne, you can over
-0001dff0: 7772 6974 6520 7468 6520 6f70 7469 6f6e  write the option
-0001e000: 733a 0a20 2020 2020 2020 2020 2020 2060  s:.            `
-0001e010: 686f 6f64 6965 2e6b 6565 702e 6d69 6e2e  hoodie.keep.min.
-0001e020: 636f 6d6d 6974 7360 2061 6e64 2060 686f  commits` and `ho
-0001e030: 6f64 6965 2e6b 6565 702e 6d61 782e 636f  odie.keep.max.co
-0001e040: 6d6d 6974 7360 0a20 2020 2020 2020 2020  mmits`.         
-0001e050: 2020 2077 6865 6e20 6361 6c6c 696e 6720     when calling 
-0001e060: 7468 6520 6069 6e73 6572 7428 2960 206d  the `insert()` m
-0001e070: 6574 686f 642e 0a0a 2020 2020 2020 2020  ethod...        
-0001e080: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
-0001e090: 2020 2020 2020 2020 7761 6c6c 636c 6f63          wallcloc
-0001e0a0: 6b5f 7469 6d65 3a20 5265 6164 2064 6174  k_time: Read dat
-0001e0b0: 6120 6173 206f 6620 7468 6973 2070 6f69  a as of this poi
-0001e0c0: 6e74 2069 6e20 7469 6d65 2e20 5374 7269  nt in time. Stri
-0001e0d0: 6e67 7320 7368 6f75 6c64 2062 6520 666f  ngs should be fo
-0001e0e0: 726d 6174 7465 6420 696e 206f 6e65 206f  rmatted in one o
-0001e0f0: 6620 7468 650a 2020 2020 2020 2020 2020  f the.          
-0001e100: 2020 2020 2020 666f 6c6c 6f77 696e 6720        following 
-0001e110: 666f 726d 6174 7320 6025 592d 256d 2d25  formats `%Y-%m-%
-0001e120: 6460 2c20 6025 592d 256d 2d25 6420 2548  d`, `%Y-%m-%d %H
-0001e130: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
-0001e140: 254d 602c 206f 7220 6025 592d 256d 2d25  %M`, or `%Y-%m-%
-0001e150: 6420 2548 3a25 4d3a 2553 602e 0a20 2020  d %H:%M:%S`..   
-0001e160: 2020 2020 2020 2020 2065 7863 6c75 6465           exclude
-0001e170: 5f75 6e74 696c 3a20 4578 636c 7564 6520  _until: Exclude 
-0001e180: 636f 6d6d 6974 7320 756e 7469 6c20 7468  commits until th
-0001e190: 6973 2070 6f69 6e74 2069 6e20 7469 6d65  is point in time
-0001e1a0: 2e20 5374 7269 6e67 2073 686f 756c 6420  . String should 
-0001e1b0: 6265 2066 6f72 6d61 7474 6564 2069 6e20  be formatted in 
-0001e1c0: 6f6e 6520 6f66 2074 6865 0a20 2020 2020  one of the.     
-0001e1d0: 2020 2020 2020 2020 2020 2066 6f6c 6c6f             follo
-0001e1e0: 7769 6e67 2066 6f72 6d61 7473 2060 2559  wing formats `%Y
-0001e1f0: 2d25 6d2d 2564 602c 2060 2559 2d25 6d2d  -%m-%d`, `%Y-%m-
-0001e200: 2564 2025 4860 2c20 6025 592d 256d 2d25  %d %H`, `%Y-%m-%
-0001e210: 6420 2548 3a25 4d60 2c20 6f72 2060 2559  d %H:%M`, or `%Y
-0001e220: 2d25 6d2d 2564 2025 483a 254d 3a25 5360  -%m-%d %H:%M:%S`
-0001e230: 2e0a 0a20 2020 2020 2020 2023 2052 6574  ...        # Ret
-0001e240: 7572 6e73 0a20 2020 2020 2020 2020 2020  urns.           
-0001e250: 2060 5175 6572 7960 2e20 5468 6520 7175   `Query`. The qu
-0001e260: 6572 7920 6f62 6a65 6374 2077 6974 6820  ery object with 
-0001e270: 7468 6520 6170 706c 6965 6420 7469 6d65  the applied time
-0001e280: 2074 7261 7665 6c20 636f 6e64 6974 696f   travel conditio
-0001e290: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
-0001e2a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001e2b0: 6c66 2e73 656c 6563 745f 616c 6c28 292e  lf.select_all().
-0001e2c0: 6173 5f6f 6628 0a20 2020 2020 2020 2020  as_of(.         
-0001e2d0: 2020 2077 616c 6c63 6c6f 636b 5f74 696d     wallclock_tim
-0001e2e0: 653d 7761 6c6c 636c 6f63 6b5f 7469 6d65  e=wallclock_time
-0001e2f0: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
-0001e300: 6578 636c 7564 655f 756e 7469 6c0a 2020  exclude_until.  
-0001e310: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0001e320: 2067 6574 5f73 7461 7469 7374 6963 735f   get_statistics_
-0001e330: 6279 5f63 6f6d 6d69 745f 7769 6e64 6f77  by_commit_window
-0001e340: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0001e350: 2020 2020 2020 2020 6672 6f6d 5f63 6f6d          from_com
-0001e360: 6d69 745f 7469 6d65 3a20 4f70 7469 6f6e  mit_time: Option
-0001e370: 616c 5b55 6e69 6f6e 5b73 7472 2c20 696e  al[Union[str, in
-0001e380: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
-0001e390: 655d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  e]] = None,.    
-0001e3a0: 2020 2020 746f 5f63 6f6d 6d69 745f 7469      to_commit_ti
-0001e3b0: 6d65 3a20 4f70 7469 6f6e 616c 5b55 6e69  me: Optional[Uni
-0001e3c0: 6f6e 5b73 7472 2c20 696e 742c 2064 6174  on[str, int, dat
-0001e3d0: 6574 696d 652c 2064 6174 655d 5d20 3d20  etime, date]] = 
-0001e3e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6665  None,.        fe
-0001e3f0: 6174 7572 655f 6e61 6d65 733a 204f 7074  ature_names: Opt
-0001e400: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-0001e410: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0001e420: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-0001e430: 6e73 2074 6865 2073 7461 7469 7374 6963  ns the statistic
-0001e440: 7320 636f 6d70 7574 6564 206f 6e20 6120  s computed on a 
-0001e450: 7370 6563 6966 6963 2063 6f6d 6d69 7420  specific commit 
-0001e460: 7769 6e64 6f77 2066 6f72 2074 6869 7320  window for this 
-0001e470: 6665 6174 7572 6520 6772 6f75 702e 2049  feature group. I
-0001e480: 6620 7469 6d65 2074 7261 7665 6c20 6973  f time travel is
-0001e490: 206e 6f74 2065 6e61 626c 6564 2c20 6974   not enabled, it
-0001e4a0: 2072 6169 7365 7320 616e 2065 7863 6570   raises an excep
-0001e4b0: 7469 6f6e 2e0a 0a20 2020 2020 2020 2049  tion...        I
-0001e4c0: 6620 6066 726f 6d5f 636f 6d6d 6974 5f74  f `from_commit_t
-0001e4d0: 696d 6560 2069 7320 604e 6f6e 6560 2c20  ime` is `None`, 
-0001e4e0: 7468 6520 636f 6d6d 6974 2077 696e 646f  the commit windo
-0001e4f0: 7720 7374 6172 7473 2066 726f 6d20 7468  w starts from th
-0001e500: 6520 6669 7273 7420 636f 6d6d 6974 2e0a  e first commit..
-0001e510: 2020 2020 2020 2020 4966 2060 746f 5f63          If `to_c
-0001e520: 6f6d 6d69 745f 7469 6d65 6020 6973 2060  ommit_time` is `
-0001e530: 4e6f 6e65 602c 2074 6865 2063 6f6d 6d69  None`, the commi
-0001e540: 7420 7769 6e64 6f77 2065 6e64 7320 6174  t window ends at
-0001e550: 2074 6865 206c 6173 7420 636f 6d6d 6974   the last commit
-0001e560: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-0001e570: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-0001e580: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-0001e590: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
-0001e5a0: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
-0001e5b0: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
-0001e5c0: 2020 2020 6673 203d 202e 2e2e 0a20 2020      fs = ....   
-0001e5d0: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
-0001e5e0: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
-0001e5f0: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
-0001e600: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
-0001e610: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-0001e620: 7572 655f 6772 6f75 7028 2e2e 2e29 0a20  ure_group(...). 
-0001e630: 2020 2020 2020 2020 2020 2066 675f 7374             fg_st
-0001e640: 6174 6973 7469 6373 203d 2066 672e 6765  atistics = fg.ge
-0001e650: 745f 7374 6174 6973 7469 6373 5f62 795f  t_statistics_by_
-0001e660: 636f 6d6d 6974 5f77 696e 646f 7728 6672  commit_window(fr
-0001e670: 6f6d 5f63 6f6d 6d69 745f 7469 6d65 3d4e  om_commit_time=N
-0001e680: 6f6e 652c 2074 6f5f 636f 6d6d 6974 5f74  one, to_commit_t
-0001e690: 696d 653d 4e6f 6e65 290a 2020 2020 2020  ime=None).      
-0001e6a0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-0001e6b0: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
-0001e6c0: 2020 2020 2020 2020 2020 746f 5f63 6f6d            to_com
-0001e6d0: 6d69 745f 7469 6d65 3a20 4461 7465 2061  mit_time: Date a
-0001e6e0: 6e64 2074 696d 6520 6f66 2074 6865 206c  nd time of the l
-0001e6f0: 6173 7420 636f 6d6d 6974 206f 6620 7468  ast commit of th
-0001e700: 6520 7769 6e64 6f77 2e20 4465 6661 756c  e window. Defaul
-0001e710: 7473 2074 6f20 604e 6f6e 6560 2e20 5374  ts to `None`. St
-0001e720: 7269 6e67 7320 7368 6f75 6c64 0a20 2020  rings should.   
-0001e730: 2020 2020 2020 2020 2020 2020 2062 6520               be 
-0001e740: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
-0001e750: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-0001e760: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
-0001e770: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
-0001e780: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
-0001e790: 483a 254d 602c 2060 2559 2d25 6d2d 2564  H:%M`, `%Y-%m-%d
-0001e7a0: 2025 483a 254d 3a25 5360 2c0a 2020 2020   %H:%M:%S`,.    
-0001e7b0: 2020 2020 2020 2020 2020 2020 6f72 2060              or `
-0001e7c0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-0001e7d0: 532e 2566 602e 0a20 2020 2020 2020 2020  S.%f`..         
-0001e7e0: 2020 2066 726f 6d5f 636f 6d6d 6974 5f74     from_commit_t
-0001e7f0: 696d 653a 2044 6174 6520 616e 6420 7469  ime: Date and ti
-0001e800: 6d65 206f 6620 7468 6520 6669 7273 7420  me of the first 
-0001e810: 636f 6d6d 6974 206f 6620 7468 6520 7769  commit of the wi
-0001e820: 6e64 6f77 2e20 4465 6661 756c 7473 2074  ndow. Defaults t
-0001e830: 6f20 604e 6f6e 6560 2e20 5374 7269 6e67  o `None`. String
-0001e840: 7320 7368 6f75 6c64 0a20 2020 2020 2020  s should.       
-0001e850: 2020 2020 2020 2020 2062 6520 666f 726d           be form
-0001e860: 6174 7465 6420 696e 206f 6e65 206f 6620  atted in one of 
-0001e870: 7468 6520 666f 6c6c 6f77 696e 6720 666f  the following fo
-0001e880: 726d 6174 7320 6025 592d 256d 2d25 6460  rmats `%Y-%m-%d`
-0001e890: 2c20 6025 592d 256d 2d25 6420 2548 602c  , `%Y-%m-%d %H`,
-0001e8a0: 2060 2559 2d25 6d2d 2564 2025 483a 254d   `%Y-%m-%d %H:%M
-0001e8b0: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
-0001e8c0: 254d 3a25 5360 2c0a 2020 2020 2020 2020  %M:%S`,.        
-0001e8d0: 2020 2020 2020 2020 6f72 2060 2559 2d25          or `%Y-%
-0001e8e0: 6d2d 2564 2025 483a 254d 3a25 532e 2566  m-%d %H:%M:%S.%f
-0001e8f0: 602e 0a20 2020 2020 2020 2020 2020 2066  `..            f
-0001e900: 6561 7475 7265 5f6e 616d 6573 3a20 4c69  eature_names: Li
-0001e910: 7374 206f 6620 6665 6174 7572 6520 6e61  st of feature na
-0001e920: 6d65 7320 6f66 2077 6869 6368 2073 7461  mes of which sta
-0001e930: 7469 7374 6963 7320 6172 6520 7265 7472  tistics are retr
-0001e940: 6965 7665 642e 0a20 2020 2020 2020 2023  ieved..        #
-0001e950: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0001e960: 2020 2020 2060 5374 6174 6973 7469 6373       `Statistics
-0001e970: 602e 2053 7461 7469 7374 6963 7320 6f62  `. Statistics ob
-0001e980: 6a65 6374 2e0a 2020 2020 2020 2020 2320  ject..        # 
-0001e990: 5261 6973 6573 0a20 2020 2020 2020 2020  Raises.         
-0001e9a0: 2020 2060 6873 6673 2e63 6c69 656e 742e     `hsfs.client.
-0001e9b0: 6578 6365 7074 696f 6e73 2e52 6573 7441  exceptions.RestA
-0001e9c0: 5049 4572 726f 7260 2e0a 2020 2020 2020  PIError`..      
-0001e9d0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0001e9e0: 206e 6f74 2073 656c 662e 5f69 735f 7469   not self._is_ti
-0001e9f0: 6d65 5f74 7261 7665 6c5f 656e 6162 6c65  me_travel_enable
-0001ea00: 6428 293a 0a20 2020 2020 2020 2020 2020  d():.           
-0001ea10: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001ea20: 7228 2254 696d 6520 7472 6176 656c 2069  r("Time travel i
-0001ea30: 7320 6e6f 7420 656e 6162 6c65 6420 666f  s not enabled fo
-0001ea40: 7220 7468 6973 2066 6561 7475 7265 2067  r this feature g
-0001ea50: 726f 7570 2229 0a20 2020 2020 2020 2072  roup").        r
-0001ea60: 6574 7572 6e20 7365 6c66 2e5f 7374 6174  eturn self._stat
-0001ea70: 6973 7469 6373 5f65 6e67 696e 652e 6765  istics_engine.ge
-0001ea80: 745f 6279 5f74 696d 655f 7769 6e64 6f77  t_by_time_window
-0001ea90: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-0001eaa0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-0001eab0: 7374 6172 745f 636f 6d6d 6974 5f74 696d  start_commit_tim
-0001eac0: 653d 6672 6f6d 5f63 6f6d 6d69 745f 7469  e=from_commit_ti
-0001ead0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0001eae0: 656e 645f 636f 6d6d 6974 5f74 696d 653d  end_commit_time=
-0001eaf0: 746f 5f63 6f6d 6d69 745f 7469 6d65 2c0a  to_commit_time,.
-0001eb00: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-0001eb10: 7572 655f 6e61 6d65 733d 6665 6174 7572  ure_names=featur
-0001eb20: 655f 6e61 6d65 732c 0a20 2020 2020 2020  e_names,.       
-0001eb30: 2029 0a0a 2020 2020 6465 6620 636f 6d70   )..    def comp
-0001eb40: 7574 655f 7374 6174 6973 7469 6373 280a  ute_statistics(.
-0001eb50: 2020 2020 2020 2020 7365 6c66 2c20 7761          self, wa
-0001eb60: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
-0001eb70: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-0001eb80: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
-0001eb90: 2064 6174 655d 5d20 3d20 4e6f 6e65 0a20   date]] = None. 
-0001eba0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0001ebb0: 2252 6563 6f6d 7075 7465 2074 6865 2073  "Recompute the s
-0001ebc0: 7461 7469 7374 6963 7320 666f 7220 7468  tatistics for th
-0001ebd0: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
-0001ebe0: 616e 6420 7361 7665 2074 6865 6d20 746f  and save them to
-0001ebf0: 2074 6865 0a20 2020 2020 2020 2066 6561   the.        fea
-0001ec00: 7475 7265 2073 746f 7265 2e0a 0a20 2020  ture store...   
-0001ec10: 2020 2020 2053 7461 7469 7374 6963 7320       Statistics 
-0001ec20: 6172 6520 6f6e 6c79 2063 6f6d 7075 7465  are only compute
-0001ec30: 6420 666f 7220 6461 7461 2069 6e20 7468  d for data in th
-0001ec40: 6520 6f66 666c 696e 6520 7374 6f72 6167  e offline storag
-0001ec50: 6520 6f66 2074 6865 2066 6561 7475 7265  e of the feature
-0001ec60: 0a20 2020 2020 2020 2067 726f 7570 2e0a  .        group..
-0001ec70: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-0001ec80: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-0001ec90: 2077 616c 6c63 6c6f 636b 5f74 696d 653a   wallclock_time:
-0001eca0: 2049 6620 7370 6563 6966 6965 6420 7769   If specified wi
-0001ecb0: 6c6c 2072 6563 6f6d 7075 7465 2073 7461  ll recompute sta
-0001ecc0: 7469 7374 6963 7320 6f6e 0a20 2020 2020  tistics on.     
-0001ecd0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-0001ece0: 7265 2067 726f 7570 2061 7320 6f66 2073  re group as of s
-0001ecf0: 7065 6369 6669 6320 706f 696e 7420 696e  pecific point in
-0001ed00: 2074 696d 652e 2049 6620 6e6f 7420 7370   time. If not sp
-0001ed10: 6563 6966 6965 6420 7468 656e 2077 696c  ecified then wil
-0001ed20: 6c20 636f 6d70 7574 6520 7374 6174 6973  l compute statis
-0001ed30: 7469 6373 0a20 2020 2020 2020 2020 2020  tics.           
-0001ed40: 2020 2020 2061 7320 6f66 206d 6f73 7420       as of most 
-0001ed50: 7265 6365 6e74 2074 696d 6520 6f66 2074  recent time of t
-0001ed60: 6869 7320 6665 6174 7572 6520 6772 6f75  his feature grou
-0001ed70: 702e 2044 6566 6175 6c74 7320 746f 2060  p. Defaults to `
-0001ed80: 4e6f 6e65 602e 2053 7472 696e 6773 2073  None`. Strings s
-0001ed90: 686f 756c 640a 2020 2020 2020 2020 2020  hould.          
-0001eda0: 2020 2020 2020 6265 2066 6f72 6d61 7474        be formatt
-0001edb0: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
-0001edc0: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
-0001edd0: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
-0001ede0: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
-0001edf0: 592d 256d 2d25 6420 2548 3a25 4d60 2c20  Y-%m-%d %H:%M`, 
-0001ee00: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-0001ee10: 2553 602c 0a20 2020 2020 2020 2020 2020  %S`,.           
-0001ee20: 2020 2020 206f 7220 6025 592d 256d 2d25       or `%Y-%m-%
-0001ee30: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
-0001ee40: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-0001ee50: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
-0001ee60: 5374 6174 6973 7469 6373 602e 2054 6865  Statistics`. The
-0001ee70: 2073 7461 7469 7374 6963 7320 6d65 7461   statistics meta
-0001ee80: 6461 7461 206f 626a 6563 742e 0a0a 2020  data object...  
-0001ee90: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
-0001eea0: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
-0001eeb0: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
-0001eec0: 6e73 2e52 6573 7441 5049 4572 726f 7260  ns.RestAPIError`
-0001eed0: 2e20 556e 6162 6c65 2074 6f20 7065 7273  . Unable to pers
-0001eee0: 6973 7420 7468 6520 7374 6174 6973 7469  ist the statisti
-0001eef0: 6373 2e0a 2020 2020 2020 2020 2222 220a  cs..        """.
-0001ef00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001ef10: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-0001ef20: 672e 656e 6162 6c65 643a 0a20 2020 2020  g.enabled:.     
-0001ef30: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0001ef40: 6973 5f74 696d 655f 7472 6176 656c 5f65  is_time_travel_e
-0001ef50: 6e61 626c 6564 2829 206f 7220 7761 6c6c  nabled() or wall
-0001ef60: 636c 6f63 6b5f 7469 6d65 2069 7320 6e6f  clock_time is no
-0001ef70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0001ef80: 2020 2020 2020 2020 7761 6c6c 636c 6f63          wallcloc
-0001ef90: 6b5f 7469 6d65 203d 2077 616c 6c63 6c6f  k_time = wallclo
-0001efa0: 636b 5f74 696d 6520 6f72 2064 6174 6574  ck_time or datet
-0001efb0: 696d 652e 6e6f 7728 290a 2020 2020 2020  ime.now().      
-0001efc0: 2020 2020 2020 2020 2020 2320 5265 7472            # Retr
-0001efd0: 6965 7665 2066 6720 636f 6d6d 6974 2069  ieve fg commit i
-0001efe0: 6420 7265 6c61 7465 6420 746f 2074 6869  d related to thi
-0001eff0: 7320 7761 6c6c 2063 6c6f 636b 2074 696d  s wall clock tim
-0001f000: 6520 616e 6420 7265 636f 6d70 7574 6520  e and recompute 
-0001f010: 7374 6174 6973 7469 6373 2e20 4974 2077  statistics. It w
-0001f020: 696c 6c20 7468 726f 770a 2020 2020 2020  ill throw.      
-0001f030: 2020 2020 2020 2020 2020 2320 6578 6365            # exce
-0001f040: 7074 696f 6e20 6966 2069 7473 206e 6f74  ption if its not
-0001f050: 2074 696d 6520 7472 6176 656c 2065 6e61   time travel ena
-0001f060: 626c 6564 2066 6561 7475 7265 2067 726f  bled feature gro
-0001f070: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
-0001f080: 2020 2020 6667 5f63 6f6d 6d69 745f 6964      fg_commit_id
-0001f090: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-0001f0a0: 2020 2020 2020 2020 2063 6f6d 6d69 745f           commit_
-0001f0b0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-0001f0c0: 2020 2020 2020 2066 6f72 2063 6f6d 6d69         for commi
-0001f0d0: 745f 6964 2069 6e20 7365 6c66 2e5f 6665  t_id in self._fe
-0001f0e0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-0001f0f0: 6e65 2e63 6f6d 6d69 745f 6465 7461 696c  ne.commit_detail
-0001f100: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-0001f110: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-0001f120: 2077 616c 6c63 6c6f 636b 5f74 696d 652c   wallclock_time,
-0001f130: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-0001f140: 2020 2020 2020 2029 2e6b 6579 7328 290a         ).keys().
-0001f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f160: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
-0001f170: 2020 2020 2072 6567 6973 7465 7265 645f       registered_
-0001f180: 7374 6174 7320 3d20 7365 6c66 2e67 6574  stats = self.get
-0001f190: 5f73 7461 7469 7374 6963 735f 6279 5f63  _statistics_by_c
-0001f1a0: 6f6d 6d69 745f 7769 6e64 6f77 280a 2020  ommit_window(.  
-0001f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f1c0: 2020 746f 5f63 6f6d 6d69 745f 7469 6d65    to_commit_time
-0001f1d0: 3d66 675f 636f 6d6d 6974 5f69 640a 2020  =fg_commit_id.  
-0001f1e0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f200: 6966 2072 6567 6973 7465 7265 645f 7374  if registered_st
-0001f210: 6174 7320 6973 206e 6f74 204e 6f6e 6520  ats is not None 
-0001f220: 616e 6420 7365 6c66 2e5f 6172 655f 7374  and self._are_st
-0001f230: 6174 6973 7469 6373 5f6d 6973 7369 6e67  atistics_missing
-0001f240: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001f250: 2020 2020 2020 7265 6769 7374 6572 6564        registered
-0001f260: 5f73 7461 7473 0a20 2020 2020 2020 2020  _stats.         
-0001f270: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-0001f280: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001f290: 6769 7374 6572 6564 5f73 7461 7473 203d  gistered_stats =
-0001f2a0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0001f2b0: 2020 2020 2020 2320 446f 6e27 7420 7265        # Don't re
-0001f2c0: 6164 2074 6865 2064 6174 6166 7261 6d65  ad the dataframe
-0001f2d0: 2068 6572 652c 2074 6f20 6176 6f69 6420   here, to avoid 
-0001f2e0: 7472 6967 6765 7269 6e67 2061 2072 6561  triggering a rea
-0001f2f0: 6420 6f70 6572 6174 696f 6e0a 2020 2020  d operation.    
-0001f300: 2020 2020 2020 2020 2020 2020 2320 666f              # fo
-0001f310: 7220 7468 6520 5079 7468 6f6e 2065 6e67  r the Python eng
-0001f320: 696e 652e 2054 6865 2050 7974 686f 6e20  ine. The Python 
-0001f330: 656e 6769 6e65 2069 7320 676f 696e 6720  engine is going 
-0001f340: 746f 2073 6574 7570 2061 2053 7061 726b  to setup a Spark
-0001f350: 204a 6f62 0a20 2020 2020 2020 2020 2020   Job.           
-0001f360: 2020 2020 2023 2074 6f20 7570 6461 7465       # to update
-0001f370: 2074 6865 2073 7461 7469 7374 6963 732e   the statistics.
-0001f380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f390: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-0001f3a0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001f3b0: 6769 7374 6572 6564 5f73 7461 7473 0a20  gistered_stats. 
-0001f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f3d0: 2020 206f 7220 7365 6c66 2e5f 7374 6174     or self._stat
-0001f3e0: 6973 7469 6373 5f65 6e67 696e 652e 636f  istics_engine.co
-0001f3f0: 6d70 7574 655f 616e 645f 7361 7665 5f73  mpute_and_save_s
-0001f400: 7461 7469 7374 6963 7328 0a20 2020 2020  tatistics(.     
-0001f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f420: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0001f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f440: 2066 6561 7475 7265 5f67 726f 7570 5f63   feature_group_c
-0001f450: 6f6d 6d69 745f 6964 3d66 675f 636f 6d6d  ommit_id=fg_comm
-0001f460: 6974 5f69 642c 0a20 2020 2020 2020 2020  it_id,.         
-0001f470: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001f480: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001f490: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-0001f4a0: 7065 7228 292e 636f 6d70 7574 655f 7374  per().compute_st
-0001f4b0: 6174 6973 7469 6373 2829 0a0a 2020 2020  atistics()..    
-0001f4c0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-0001f4d0: 2064 6566 2066 726f 6d5f 7265 7370 6f6e   def from_respon
-0001f4e0: 7365 5f6a 736f 6e28 636c 732c 206a 736f  se_json(cls, jso
-0001f4f0: 6e5f 6469 6374 293a 0a20 2020 2020 2020  n_dict):.       
-0001f500: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
-0001f510: 6420 3d20 6875 6d70 732e 6465 6361 6d65  d = humps.decame
-0001f520: 6c69 7a65 286a 736f 6e5f 6469 6374 290a  lize(json_dict).
-0001f530: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0001f540: 7461 6e63 6528 6a73 6f6e 5f64 6563 616d  tance(json_decam
-0001f550: 656c 697a 6564 2c20 6469 6374 293a 0a20  elized, dict):. 
-0001f560: 2020 2020 2020 2020 2020 2069 6620 2274             if "t
-0001f570: 7970 6522 2069 6e20 6a73 6f6e 5f64 6563  ype" in json_dec
-0001f580: 616d 656c 697a 6564 3a0a 2020 2020 2020  amelized:.      
-0001f590: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
-0001f5a0: 6563 616d 656c 697a 6564 5b22 7374 7265  ecamelized["stre
-0001f5b0: 616d 225d 203d 2028 0a20 2020 2020 2020  am"] = (.       
-0001f5c0: 2020 2020 2020 2020 2020 2020 206a 736f               jso
-0001f5d0: 6e5f 6465 6361 6d65 6c69 7a65 645b 2274  n_decamelized["t
-0001f5e0: 7970 6522 5d20 3d3d 2022 7374 7265 616d  ype"] == "stream
-0001f5f0: 4665 6174 7572 6547 726f 7570 4454 4f22  FeatureGroupDTO"
-0001f600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f610: 2029 0a20 2020 2020 2020 2020 2020 205f   ).            _
-0001f620: 203d 206a 736f 6e5f 6465 6361 6d65 6c69   = json_decameli
-0001f630: 7a65 642e 706f 7028 2274 7970 6522 2c20  zed.pop("type", 
-0001f640: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
-0001f650: 2020 6a73 6f6e 5f64 6563 616d 656c 697a    json_decameliz
-0001f660: 6564 2e70 6f70 2822 7661 6c69 6461 7469  ed.pop("validati
-0001f670: 6f6e 5f74 7970 6522 2c20 4e6f 6e65 290a  on_type", None).
-0001f680: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-0001f690: 656d 6265 6464 696e 675f 696e 6465 7822  embedding_index"
-0001f6a0: 2069 6e20 6a73 6f6e 5f64 6563 616d 656c   in json_decamel
-0001f6b0: 697a 6564 3a0a 2020 2020 2020 2020 2020  ized:.          
-0001f6c0: 2020 2020 2020 6a73 6f6e 5f64 6563 616d        json_decam
-0001f6d0: 656c 697a 6564 5b22 656d 6265 6464 696e  elized["embeddin
-0001f6e0: 675f 696e 6465 7822 5d20 3d20 456d 6265  g_index"] = Embe
-0001f6f0: 6464 696e 6749 6e64 6578 2e66 726f 6d5f  ddingIndex.from_
-0001f700: 6a73 6f6e 5f72 6573 706f 6e73 6528 0a20  json_response(. 
-0001f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f720: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
-0001f730: 7a65 645b 2265 6d62 6564 6469 6e67 5f69  zed["embedding_i
-0001f740: 6e64 6578 225d 0a20 2020 2020 2020 2020  ndex"].         
-0001f750: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001f760: 2020 2020 2072 6574 7572 6e20 636c 7328       return cls(
-0001f770: 2a2a 6a73 6f6e 5f64 6563 616d 656c 697a  **json_decameliz
-0001f780: 6564 290a 2020 2020 2020 2020 666f 7220  ed).        for 
-0001f790: 6667 2069 6e20 6a73 6f6e 5f64 6563 616d  fg in json_decam
-0001f7a0: 656c 697a 6564 3a0a 2020 2020 2020 2020  elized:.        
-0001f7b0: 2020 2020 6966 2022 7479 7065 2220 696e      if "type" in
-0001f7c0: 2066 673a 0a20 2020 2020 2020 2020 2020   fg:.           
-0001f7d0: 2020 2020 2066 675b 2273 7472 6561 6d22       fg["stream"
-0001f7e0: 5d20 3d20 6667 5b22 7479 7065 225d 203d  ] = fg["type"] =
-0001f7f0: 3d20 2273 7472 6561 6d46 6561 7475 7265  = "streamFeature
-0001f800: 4772 6f75 7044 544f 220a 2020 2020 2020  GroupDTO".      
-0001f810: 2020 2020 2020 5f20 3d20 6667 2e70 6f70        _ = fg.pop
-0001f820: 2822 7479 7065 222c 204e 6f6e 6529 0a20  ("type", None). 
-0001f830: 2020 2020 2020 2020 2020 2066 672e 706f             fg.po
-0001f840: 7028 2276 616c 6964 6174 696f 6e5f 7479  p("validation_ty
-0001f850: 7065 222c 204e 6f6e 6529 0a20 2020 2020  pe", None).     
-0001f860: 2020 2020 2020 2069 6620 2265 6d62 6564         if "embed
-0001f870: 6469 6e67 5f69 6e64 6578 2220 696e 2066  ding_index" in f
-0001f880: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0001f890: 2020 2066 675b 2265 6d62 6564 6469 6e67     fg["embedding
-0001f8a0: 5f69 6e64 6578 225d 203d 2045 6d62 6564  _index"] = Embed
-0001f8b0: 6469 6e67 496e 6465 782e 6672 6f6d 5f6a  dingIndex.from_j
-0001f8c0: 736f 6e5f 7265 7370 6f6e 7365 280a 2020  son_response(.  
-0001f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f8e0: 2020 6667 5b22 656d 6265 6464 696e 675f    fg["embedding_
-0001f8f0: 696e 6465 7822 5d0a 2020 2020 2020 2020  index"].        
-0001f900: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001f910: 2020 7265 7475 726e 205b 636c 7328 2a2a    return [cls(**
-0001f920: 6667 2920 666f 7220 6667 2069 6e20 6a73  fg) for fg in js
-0001f930: 6f6e 5f64 6563 616d 656c 697a 6564 5d0a  on_decamelized].
-0001f940: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
-0001f950: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
-0001f960: 6f6e 2873 656c 662c 206a 736f 6e5f 6469  on(self, json_di
-0001f970: 6374 293a 0a20 2020 2020 2020 206a 736f  ct):.        jso
-0001f980: 6e5f 6465 6361 6d65 6c69 7a65 6420 3d20  n_decamelized = 
-0001f990: 6875 6d70 732e 6465 6361 6d65 6c69 7a65  humps.decamelize
-0001f9a0: 286a 736f 6e5f 6469 6374 290a 2020 2020  (json_dict).    
-0001f9b0: 2020 2020 6a73 6f6e 5f64 6563 616d 656c      json_decamel
-0001f9c0: 697a 6564 5b22 7374 7265 616d 225d 203d  ized["stream"] =
-0001f9d0: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
-0001f9e0: 645b 2274 7970 6522 5d20 3d3d 2022 7374  d["type"] == "st
-0001f9f0: 7265 616d 4665 6174 7572 6547 726f 7570  reamFeatureGroup
-0001fa00: 4454 4f22 0a20 2020 2020 2020 205f 203d  DTO".        _ =
-0001fa10: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
-0001fa20: 642e 706f 7028 2274 7970 6522 290a 2020  d.pop("type").  
-0001fa30: 2020 2020 2020 6966 2022 656d 6265 6464        if "embedd
-0001fa40: 696e 675f 696e 6465 7822 2069 6e20 6a73  ing_index" in js
-0001fa50: 6f6e 5f64 6563 616d 656c 697a 6564 3a0a  on_decamelized:.
-0001fa60: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
-0001fa70: 5f64 6563 616d 656c 697a 6564 5b22 656d  _decamelized["em
-0001fa80: 6265 6464 696e 675f 696e 6465 7822 5d20  bedding_index"] 
-0001fa90: 3d20 456d 6265 6464 696e 6749 6e64 6578  = EmbeddingIndex
-0001faa0: 2e66 726f 6d5f 6a73 6f6e 5f72 6573 706f  .from_json_respo
-0001fab0: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
-0001fac0: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
-0001fad0: 6c69 7a65 645b 2265 6d62 6564 6469 6e67  lized["embedding
-0001fae0: 5f69 6e64 6578 225d 0a20 2020 2020 2020  _index"].       
-0001faf0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0001fb00: 656c 662e 5f5f 696e 6974 5f5f 282a 2a6a  elf.__init__(**j
-0001fb10: 736f 6e5f 6465 6361 6d65 6c69 7a65 6429  son_decamelized)
-0001fb20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001fb30: 7365 6c66 0a0a 2020 2020 6465 6620 6a73  self..    def js
-0001fb40: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
-0001fb50: 2020 2222 2247 6574 2073 7065 6369 6669    """Get specifi
-0001fb60: 6320 4665 6174 7572 6520 4772 6f75 7020  c Feature Group 
-0001fb70: 6d65 7461 6461 7461 2069 6e20 6a73 6f6e  metadata in json
-0001fb80: 2066 6f72 6d61 742e 0a0a 2020 2020 2020   format...      
-0001fb90: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
-0001fba0: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
-0001fbb0: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
-0001fbc0: 6667 2e6a 736f 6e28 290a 2020 2020 2020  fg.json().      
-0001fbd0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-0001fbe0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0001fbf0: 7475 726e 206a 736f 6e2e 6475 6d70 7328  turn json.dumps(
-0001fc00: 7365 6c66 2c20 636c 733d 7574 696c 2e46  self, cls=util.F
-0001fc10: 6561 7475 7265 5374 6f72 6545 6e63 6f64  eatureStoreEncod
-0001fc20: 6572 290a 0a20 2020 2064 6566 2074 6f5f  er)..    def to_
-0001fc30: 6469 6374 2873 656c 6629 3a0a 2020 2020  dict(self):.    
-0001fc40: 2020 2020 2222 2247 6574 2073 7472 7563      """Get struc
-0001fc50: 7475 7265 6420 696e 666f 2061 626f 7574  tured info about
-0001fc60: 2073 7065 6369 6669 6320 4665 6174 7572   specific Featur
-0001fc70: 6520 4772 6f75 7020 696e 2070 7974 686f  e Group in pytho
-0001fc80: 6e20 6469 6374 696f 6e61 7279 2066 6f72  n dictionary for
-0001fc90: 6d61 742e 0a0a 2020 2020 2020 2020 2121  mat...        !!
-0001fca0: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
-0001fcb0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-0001fcc0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-0001fcd0: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
-0001fce0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
-0001fcf0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
-0001fd00: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-0001fd10: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
-0001fd20: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-0001fd30: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
-0001fd40: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-0001fd50: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
-0001fd60: 2e29 0a0a 2020 2020 2020 2020 2020 2020  .)..            
-0001fd70: 6667 2e74 6f5f 6469 6374 2829 0a20 2020  fg.to_dict().   
-0001fd80: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
-0001fd90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001fda0: 2066 675f 6d65 7461 5f64 6963 7420 3d20   fg_meta_dict = 
-0001fdb0: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-0001fdc0: 6422 3a20 7365 6c66 2e5f 6964 2c0a 2020  d": self._id,.  
-0001fdd0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-0001fde0: 3a20 7365 6c66 2e5f 6e61 6d65 2c0a 2020  : self._name,.  
-0001fdf0: 2020 2020 2020 2020 2020 2276 6572 7369            "versi
-0001fe00: 6f6e 223a 2073 656c 662e 5f76 6572 7369  on": self._versi
-0001fe10: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-0001fe20: 2264 6573 6372 6970 7469 6f6e 223a 2073  "description": s
-0001fe30: 656c 662e 5f64 6573 6372 6970 7469 6f6e  elf._description
-0001fe40: 2c0a 2020 2020 2020 2020 2020 2020 226f  ,.            "o
-0001fe50: 6e6c 696e 6545 6e61 626c 6564 223a 2073  nlineEnabled": s
-0001fe60: 656c 662e 5f6f 6e6c 696e 655f 656e 6162  elf._online_enab
-0001fe70: 6c65 642c 0a20 2020 2020 2020 2020 2020  led,.           
-0001fe80: 2022 7469 6d65 5472 6176 656c 466f 726d   "timeTravelForm
-0001fe90: 6174 223a 2073 656c 662e 5f74 696d 655f  at": self._time_
-0001fea0: 7472 6176 656c 5f66 6f72 6d61 742c 0a20  travel_format,. 
-0001feb0: 2020 2020 2020 2020 2020 2022 6665 6174             "feat
-0001fec0: 7572 6573 223a 2073 656c 662e 5f66 6561  ures": self._fea
-0001fed0: 7475 7265 732c 0a20 2020 2020 2020 2020  tures,.         
-0001fee0: 2020 2022 6665 6174 7572 6573 746f 7265     "featurestore
-0001fef0: 4964 223a 2073 656c 662e 5f66 6561 7475  Id": self._featu
-0001ff00: 7265 5f73 746f 7265 5f69 642c 0a20 2020  re_store_id,.   
-0001ff10: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-0001ff20: 2022 6361 6368 6564 4665 6174 7572 6567   "cachedFeatureg
-0001ff30: 726f 7570 4454 4f22 0a20 2020 2020 2020  roupDTO".       
-0001ff40: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0001ff50: 2e5f 7374 7265 616d 0a20 2020 2020 2020  ._stream.       
-0001ff60: 2020 2020 2065 6c73 6520 2273 7472 6561       else "strea
-0001ff70: 6d46 6561 7475 7265 4772 6f75 7044 544f  mFeatureGroupDTO
-0001ff80: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0001ff90: 7374 6174 6973 7469 6373 436f 6e66 6967  statisticsConfig
-0001ffa0: 223a 2073 656c 662e 5f73 7461 7469 7374  ": self._statist
-0001ffb0: 6963 735f 636f 6e66 6967 2c0a 2020 2020  ics_config,.    
-0001ffc0: 2020 2020 2020 2020 2265 7665 6e74 5469          "eventTi
-0001ffd0: 6d65 223a 2073 656c 662e 6576 656e 745f  me": self.event_
-0001ffe0: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
-0001fff0: 2020 2265 7870 6563 7461 7469 6f6e 5375    "expectationSu
-00020000: 6974 6522 3a20 7365 6c66 2e5f 6578 7065  ite": self._expe
-00020010: 6374 6174 696f 6e5f 7375 6974 652c 0a20  ctation_suite,. 
-00020020: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
-00020030: 6e74 7322 3a20 7365 6c66 2e5f 7061 7265  nts": self._pare
-00020040: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
-00020050: 2022 746f 7069 634e 616d 6522 3a20 7365   "topicName": se
-00020060: 6c66 2e74 6f70 6963 5f6e 616d 652c 0a20  lf.topic_name,. 
-00020070: 2020 2020 2020 2020 2020 2022 6e6f 7469             "noti
-00020080: 6669 6361 7469 6f6e 546f 7069 634e 616d  ficationTopicNam
-00020090: 6522 3a20 7365 6c66 2e6e 6f74 6966 6963  e": self.notific
-000200a0: 6174 696f 6e5f 746f 7069 635f 6e61 6d65  ation_topic_name
-000200b0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-000200c0: 6570 7265 6361 7465 6422 3a20 7365 6c66  eprecated": self
-000200d0: 2e64 6570 7265 6361 7465 642c 0a20 2020  .deprecated,.   
-000200e0: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
-000200f0: 6620 7365 6c66 2e65 6d62 6564 6469 6e67  f self.embedding
-00020100: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
-00020110: 2020 2020 6667 5f6d 6574 615f 6469 6374      fg_meta_dict
-00020120: 5b22 656d 6265 6464 696e 6749 6e64 6578  ["embeddingIndex
-00020130: 225d 203d 2073 656c 662e 656d 6265 6464  "] = self.embedd
-00020140: 696e 675f 696e 6465 780a 2020 2020 2020  ing_index.      
-00020150: 2020 6966 2073 656c 662e 5f73 7472 6561    if self._strea
-00020160: 6d3a 0a20 2020 2020 2020 2020 2020 2066  m:.            f
-00020170: 675f 6d65 7461 5f64 6963 745b 2264 656c  g_meta_dict["del
-00020180: 7461 5374 7265 616d 6572 4a6f 6243 6f6e  taStreamerJobCon
-00020190: 6622 5d20 3d20 7365 6c66 2e5f 6465 6c74  f"] = self._delt
-000201a0: 6173 7472 6561 6d65 725f 6a6f 6263 6f6e  astreamer_jobcon
-000201b0: 660a 2020 2020 2020 2020 7265 7475 726e  f.        return
-000201c0: 2066 675f 6d65 7461 5f64 6963 740a 0a20   fg_meta_dict.. 
-000201d0: 2020 2064 6566 205f 6765 745f 7461 626c     def _get_tabl
-000201e0: 655f 6e61 6d65 2873 656c 6629 3a0a 2020  e_name(self):.  
-000201f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00020200: 662e 6665 6174 7572 655f 7374 6f72 655f  f.feature_store_
-00020210: 6e61 6d65 202b 2022 2e22 202b 2073 656c  name + "." + sel
-00020220: 662e 6765 745f 6667 5f6e 616d 6528 290a  f.get_fg_name().
-00020230: 0a20 2020 2064 6566 205f 6973 5f74 696d  .    def _is_tim
-00020240: 655f 7472 6176 656c 5f65 6e61 626c 6564  e_travel_enabled
-00020250: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00020260: 2222 2257 6865 7468 6572 2074 696d 652d  """Whether time-
-00020270: 7472 6176 656c 2069 7320 656e 6162 6c65  travel is enable
-00020280: 6420 6f72 206e 6f74 2222 220a 2020 2020  d or not""".    
-00020290: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
-000202a0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-000202b0: 696d 655f 7472 6176 656c 5f66 6f72 6d61  ime_travel_forma
-000202c0: 7420 6973 206e 6f74 204e 6f6e 650a 2020  t is not None.  
-000202d0: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-000202e0: 6c66 2e5f 7469 6d65 5f74 7261 7665 6c5f  lf._time_travel_
-000202f0: 666f 726d 6174 2e75 7070 6572 2829 203d  format.upper() =
-00020300: 3d20 2248 5544 4922 0a20 2020 2020 2020  = "HUDI".       
-00020310: 2029 0a0a 2020 2020 4070 726f 7065 7274   )..    @propert
-00020320: 790a 2020 2020 6465 6620 6964 2873 656c  y.    def id(sel
-00020330: 6629 3a0a 2020 2020 2020 2020 2222 2246  f):.        """F
-00020340: 6561 7475 7265 2067 726f 7570 2069 642e  eature group id.
-00020350: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00020360: 726e 2073 656c 662e 5f69 640a 0a20 2020  rn self._id..   
-00020370: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00020380: 6566 2064 6573 6372 6970 7469 6f6e 2873  ef description(s
-00020390: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000203a0: 2244 6573 6372 6970 7469 6f6e 206f 6620  "Description of 
-000203b0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-000203c0: 7020 636f 6e74 656e 7473 2e22 2222 0a20  p contents.""". 
-000203d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000203e0: 6c66 2e5f 6465 7363 7269 7074 696f 6e0a  lf._description.
-000203f0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00020400: 2020 2064 6566 2074 696d 655f 7472 6176     def time_trav
-00020410: 656c 5f66 6f72 6d61 7428 7365 6c66 293a  el_format(self):
-00020420: 0a20 2020 2020 2020 2022 2222 5365 7474  .        """Sett
-00020430: 696e 6720 6f66 2074 6865 2066 6561 7475  ing of the featu
-00020440: 7265 2067 726f 7570 2074 696d 6520 7472  re group time tr
-00020450: 6176 656c 2066 6f72 6d61 742e 2222 220a  avel format.""".
-00020460: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00020470: 656c 662e 5f74 696d 655f 7472 6176 656c  elf._time_travel
-00020480: 5f66 6f72 6d61 740a 0a20 2020 2040 7072  _format..    @pr
-00020490: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
-000204a0: 6172 7469 7469 6f6e 5f6b 6579 2873 656c  artition_key(sel
-000204b0: 6629 3a0a 2020 2020 2020 2020 2222 224c  f):.        """L
-000204c0: 6973 7420 6f66 2066 6561 7475 7265 7320  ist of features 
-000204d0: 6275 696c 6469 6e67 2074 6865 2070 6172  building the par
-000204e0: 7469 7469 6f6e 206b 6579 2e22 2222 0a20  tition key.""". 
-000204f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00020500: 6c66 2e5f 7061 7274 6974 696f 6e5f 6b65  lf._partition_ke
-00020510: 790a 0a20 2020 2040 7072 6f70 6572 7479  y..    @property
-00020520: 0a20 2020 2064 6566 2068 7564 695f 7072  .    def hudi_pr
-00020530: 6563 6f6d 6269 6e65 5f6b 6579 2873 656c  ecombine_key(sel
-00020540: 6629 3a0a 2020 2020 2020 2020 2222 2246  f):.        """F
-00020550: 6561 7475 7265 206e 616d 6520 7468 6174  eature name that
-00020560: 2069 7320 7468 6520 6875 6469 2070 7265   is the hudi pre
-00020570: 636f 6d62 696e 6520 6b65 792e 2222 220a  combine key.""".
-00020580: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00020590: 656c 662e 5f68 7564 695f 7072 6563 6f6d  elf._hudi_precom
-000205a0: 6269 6e65 5f6b 6579 0a0a 2020 2020 4070  bine_key..    @p
-000205b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000205c0: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-000205d0: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
-000205e0: 2020 2222 224e 616d 6520 6f66 2074 6865    """Name of the
-000205f0: 2066 6561 7475 7265 2073 746f 7265 2069   feature store i
-00020600: 6e20 7768 6963 6820 7468 6520 6665 6174  n which the feat
-00020610: 7572 6520 6772 6f75 7020 6973 206c 6f63  ure group is loc
-00020620: 6174 6564 2e22 2222 0a20 2020 2020 2020  ated.""".       
-00020630: 2072 6574 7572 6e20 7365 6c66 2e5f 6665   return self._fe
-00020640: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
-00020650: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00020660: 2020 2020 6465 6620 6372 6561 746f 7228      def creator(
-00020670: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00020680: 2222 5573 6572 6e61 6d65 206f 6620 7468  ""Username of th
-00020690: 6520 6372 6561 746f 722e 2222 220a 2020  e creator.""".  
-000206a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000206b0: 662e 5f63 7265 6174 6f72 0a0a 2020 2020  f._creator..    
-000206c0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-000206d0: 6620 6372 6561 7465 6428 7365 6c66 293a  f created(self):
-000206e0: 0a20 2020 2020 2020 2022 2222 5469 6d65  .        """Time
-000206f0: 7374 616d 7020 7768 656e 2074 6865 2066  stamp when the f
-00020700: 6561 7475 7265 2067 726f 7570 2077 6173  eature group was
-00020710: 2063 7265 6174 6564 2e22 2222 0a20 2020   created.""".   
-00020720: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00020730: 2e5f 6372 6561 7465 640a 0a20 2020 2040  ._created..    @
-00020740: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00020750: 2073 7472 6561 6d28 7365 6c66 293a 0a20   stream(self):. 
-00020760: 2020 2020 2020 2022 2222 5768 6574 6865         """Whethe
-00020770: 7220 746f 2065 6e61 626c 6520 7265 616c  r to enable real
-00020780: 2074 696d 6520 7374 7265 616d 2077 7269   time stream wri
-00020790: 7469 6e67 2063 6170 6162 696c 6974 6965  ting capabilitie
-000207a0: 732e 2222 220a 2020 2020 2020 2020 7265  s.""".        re
-000207b0: 7475 726e 2073 656c 662e 5f73 7472 6561  turn self._strea
-000207c0: 6d0a 0a20 2020 2040 7072 6f70 6572 7479  m..    @property
-000207d0: 0a20 2020 2064 6566 2070 6172 656e 7473  .    def parents
-000207e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000207f0: 2222 2250 6172 656e 7420 6665 6174 7572  """Parent featur
-00020800: 6520 6772 6f75 7073 2061 7320 6f72 6967  e groups as orig
-00020810: 696e 206f 6620 7468 6520 6461 7461 2069  in of the data i
-00020820: 6e20 7468 6520 6375 7272 656e 7420 6665  n the current fe
-00020830: 6174 7572 6520 6772 6f75 702e 0a20 2020  ature group..   
-00020840: 2020 2020 2054 6869 7320 6973 2070 6172       This is par
-00020850: 7420 6f66 2065 7870 6c69 6369 7420 7072  t of explicit pr
-00020860: 6f76 656e 616e 6365 2222 220a 2020 2020  ovenance""".    
-00020870: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00020880: 5f70 6172 656e 7473 0a0a 2020 2020 4070  _parents..    @p
-00020890: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000208a0: 6d61 7465 7269 616c 697a 6174 696f 6e5f  materialization_
-000208b0: 6a6f 6228 7365 6c66 293a 0a20 2020 2020  job(self):.     
-000208c0: 2020 2022 2222 4765 7420 7468 6520 4a6f     """Get the Jo
-000208d0: 6220 6f62 6a65 6374 2072 6566 6572 656e  b object referen
-000208e0: 6365 2066 6f72 2074 6865 206d 6174 6572  ce for the mater
-000208f0: 6961 6c69 7a61 7469 6f6e 206a 6f62 2066  ialization job f
-00020900: 6f72 2074 6869 730a 2020 2020 2020 2020  or this.        
-00020910: 4665 6174 7572 6520 4772 6f75 702e 2222  Feature Group.""
-00020920: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00020930: 662e 5f6d 6174 6572 6961 6c69 7a61 7469  f._materializati
-00020940: 6f6e 5f6a 6f62 2069 7320 6e6f 7420 4e6f  on_job is not No
-00020950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00020960: 7265 7475 726e 2073 656c 662e 5f6d 6174  return self._mat
-00020970: 6572 6961 6c69 7a61 7469 6f6e 5f6a 6f62  erialization_job
-00020980: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00020990: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-000209a0: 7265 5f67 726f 7570 5f6e 616d 6520 3d20  re_group_name = 
-000209b0: 7574 696c 2e66 6561 7475 7265 5f67 726f  util.feature_gro
-000209c0: 7570 5f6e 616d 6528 7365 6c66 290a 2020  up_name(self).  
-000209d0: 2020 2020 2020 2020 2020 6a6f 625f 7375            job_su
-000209e0: 6666 6978 5f6c 6973 7420 3d20 5b22 6d61  ffix_list = ["ma
-000209f0: 7465 7269 616c 697a 6174 696f 6e22 2c20  terialization", 
-00020a00: 2262 6163 6b66 696c 6c22 5d0a 2020 2020  "backfill"].    
-00020a10: 2020 2020 2020 2020 666f 7220 6a6f 625f          for job_
-00020a20: 7375 6666 6978 2069 6e20 6a6f 625f 7375  suffix in job_su
-00020a30: 6666 6978 5f6c 6973 743a 0a20 2020 2020  ffix_list:.     
-00020a40: 2020 2020 2020 2020 2020 206a 6f62 5f6e             job_n
-00020a50: 616d 6520 3d20 227b 7d5f 6f66 666c 696e  ame = "{}_offlin
-00020a60: 655f 6667 5f7b 7d22 2e66 6f72 6d61 7428  e_fg_{}".format(
-00020a70: 6665 6174 7572 655f 6772 6f75 705f 6e61  feature_group_na
-00020a80: 6d65 2c20 6a6f 625f 7375 6666 6978 290a  me, job_suffix).
-00020a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020aa0: 666f 7220 5f20 696e 2072 616e 6765 2833  for _ in range(3
-00020ab0: 293a 2020 2320 7265 7472 7920 7374 6172  ):  # retry star
-00020ac0: 7469 6e67 206a 6f62 0a20 2020 2020 2020  ting job.       
-00020ad0: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00020ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00020af0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00020b00: 6d61 7465 7269 616c 697a 6174 696f 6e5f  materialization_
-00020b10: 6a6f 6220 3d20 6a6f 625f 6170 692e 4a6f  job = job_api.Jo
-00020b20: 6241 7069 2829 2e67 6574 286a 6f62 5f6e  bApi().get(job_n
-00020b30: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00020b40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00020b50: 7572 6e20 7365 6c66 2e5f 6d61 7465 7269  urn self._materi
-00020b60: 616c 697a 6174 696f 6e5f 6a6f 620a 2020  alization_job.  
-00020b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b80: 2020 6578 6365 7074 2052 6573 7441 5049    except RestAPI
-00020b90: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00020ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020bb0: 2020 2020 6966 2065 2e72 6573 706f 6e73      if e.respons
-00020bc0: 652e 7374 6174 7573 5f63 6f64 6520 3d3d  e.status_code ==
-00020bd0: 2034 3034 3a0a 2020 2020 2020 2020 2020   404:.          
-00020be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020bf0: 2020 6966 2065 2e72 6573 706f 6e73 652e    if e.response.
-00020c00: 6a73 6f6e 2829 2e67 6574 2822 6572 726f  json().get("erro
-00020c10: 7243 6f64 6522 2c20 2222 2920 3d3d 2031  rCode", "") == 1
-00020c20: 3330 3030 393a 0a20 2020 2020 2020 2020  30009:.         
-00020c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c40: 2020 2020 2020 2062 7265 616b 2020 2320         break  # 
-00020c50: 6e6f 206e 6565 6420 746f 2072 6574 7279  no need to retry
-00020c60: 2c20 7369 6e63 6520 6e6f 2073 7563 6820  , since no such 
-00020c70: 6a6f 6220 6578 6973 7473 0a20 2020 2020  job exists.     
-00020c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00020cc0: 652e 736c 6565 7028 3129 2020 2320 6261  e.sleep(1)  # ba
-00020cd0: 636b 6f66 6620 616e 6420 7468 656e 2072  ckoff and then r
-00020ce0: 6574 7279 0a20 2020 2020 2020 2020 2020  etry.           
-00020cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d00: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00020d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d20: 2020 2020 2020 7261 6973 6520 650a 2020        raise e.  
-00020d30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00020d40: 4665 6174 7572 6553 746f 7265 4578 6365  FeatureStoreExce
-00020d50: 7074 696f 6e28 224e 6f20 6d61 7465 7269  ption("No materi
-00020d60: 616c 697a 6174 696f 6e20 6a6f 6220 7761  alization job wa
-00020d70: 7320 666f 756e 6422 290a 0a20 2020 2040  s found")..    @
-00020d80: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00020d90: 2073 7461 7469 7374 6963 7328 7365 6c66   statistics(self
-00020da0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00020db0: 7420 7468 6520 6c61 7465 7374 2063 6f6d  t the latest com
-00020dc0: 7075 7465 6420 7374 6174 6973 7469 6373  puted statistics
-00020dd0: 2066 6f72 2074 6865 2077 686f 6c65 2066   for the whole f
-00020de0: 6561 7475 7265 2067 726f 7570 2e22 2222  eature group."""
-00020df0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00020e00: 2e5f 6973 5f74 696d 655f 7472 6176 656c  ._is_time_travel
-00020e10: 5f65 6e61 626c 6564 2829 3a0a 2020 2020  _enabled():.    
-00020e20: 2020 2020 2020 2020 2320 7265 7472 6965          # retrie
-00020e30: 7665 2074 6865 206c 6174 6573 7473 2073  ve the latests s
-00020e40: 7461 7469 7374 6963 7320 636f 6d70 7574  tatistics comput
-00020e50: 6564 206f 6e20 7468 6520 7768 6f6c 6520  ed on the whole 
-00020e60: 4665 6174 7572 6520 4772 6f75 702c 2069  Feature Group, i
-00020e70: 6e63 6c75 6469 6e67 2061 6c6c 2074 6865  ncluding all the
-00020e80: 2063 6f6d 6d69 7473 2e0a 2020 2020 2020   commits..      
-00020e90: 2020 2020 2020 6e6f 7720 3d20 7574 696c        now = util
-00020ea0: 2e63 6f6e 7665 7274 5f65 7665 6e74 5f74  .convert_event_t
-00020eb0: 696d 655f 746f 5f74 696d 6573 7461 6d70  ime_to_timestamp
-00020ec0: 2864 6174 6574 696d 652e 6e6f 7728 2929  (datetime.now())
-00020ed0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00020ee0: 7572 6e20 7365 6c66 2e5f 7374 6174 6973  urn self._statis
-00020ef0: 7469 6373 5f65 6e67 696e 652e 6765 745f  tics_engine.get_
-00020f00: 6279 5f74 696d 655f 7769 6e64 6f77 280a  by_time_window(.
-00020f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f20: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00020f30: 2020 2020 2020 7374 6172 745f 636f 6d6d        start_comm
-00020f40: 6974 5f74 696d 653d 4e6f 6e65 2c0a 2020  it_time=None,.  
-00020f50: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00020f60: 645f 636f 6d6d 6974 5f74 696d 653d 6e6f  d_commit_time=no
-00020f70: 772c 0a20 2020 2020 2020 2020 2020 2029  w,.            )
-00020f80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00020f90: 7375 7065 7228 292e 7374 6174 6973 7469  super().statisti
-00020fa0: 6373 0a0a 2020 2020 4064 6573 6372 6970  cs..    @descrip
-00020fb0: 7469 6f6e 2e73 6574 7465 720a 2020 2020  tion.setter.    
-00020fc0: 6465 6620 6465 7363 7269 7074 696f 6e28  def description(
-00020fd0: 7365 6c66 2c20 6e65 775f 6465 7363 7269  self, new_descri
-00020fe0: 7074 696f 6e29 3a0a 2020 2020 2020 2020  ption):.        
-00020ff0: 7365 6c66 2e5f 6465 7363 7269 7074 696f  self._descriptio
-00021000: 6e20 3d20 6e65 775f 6465 7363 7269 7074  n = new_descript
-00021010: 696f 6e0a 0a20 2020 2040 7469 6d65 5f74  ion..    @time_t
-00021020: 7261 7665 6c5f 666f 726d 6174 2e73 6574  ravel_format.set
-00021030: 7465 720a 2020 2020 6465 6620 7469 6d65  ter.    def time
-00021040: 5f74 7261 7665 6c5f 666f 726d 6174 2873  _travel_format(s
-00021050: 656c 662c 206e 6577 5f74 696d 655f 7472  elf, new_time_tr
-00021060: 6176 656c 5f66 6f72 6d61 7429 3a0a 2020  avel_format):.  
-00021070: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
-00021080: 5f74 7261 7665 6c5f 666f 726d 6174 203d  _travel_format =
-00021090: 206e 6577 5f74 696d 655f 7472 6176 656c   new_time_travel
-000210a0: 5f66 6f72 6d61 740a 0a20 2020 2040 7061  _format..    @pa
-000210b0: 7274 6974 696f 6e5f 6b65 792e 7365 7474  rtition_key.sett
-000210c0: 6572 0a20 2020 2064 6566 2070 6172 7469  er.    def parti
-000210d0: 7469 6f6e 5f6b 6579 2873 656c 662c 206e  tion_key(self, n
-000210e0: 6577 5f70 6172 7469 7469 6f6e 5f6b 6579  ew_partition_key
-000210f0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00021100: 5f70 6172 7469 7469 6f6e 5f6b 6579 203d  _partition_key =
-00021110: 205b 706b 2e6c 6f77 6572 2829 2066 6f72   [pk.lower() for
-00021120: 2070 6b20 696e 206e 6577 5f70 6172 7469   pk in new_parti
-00021130: 7469 6f6e 5f6b 6579 5d0a 0a20 2020 2040  tion_key]..    @
-00021140: 6875 6469 5f70 7265 636f 6d62 696e 655f  hudi_precombine_
-00021150: 6b65 792e 7365 7474 6572 0a20 2020 2064  key.setter.    d
-00021160: 6566 2068 7564 695f 7072 6563 6f6d 6269  ef hudi_precombi
-00021170: 6e65 5f6b 6579 2873 656c 662c 2068 7564  ne_key(self, hud
-00021180: 695f 7072 6563 6f6d 6269 6e65 5f6b 6579  i_precombine_key
-00021190: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000211a0: 5f68 7564 695f 7072 6563 6f6d 6269 6e65  _hudi_precombine
-000211b0: 5f6b 6579 203d 2068 7564 695f 7072 6563  _key = hudi_prec
-000211c0: 6f6d 6269 6e65 5f6b 6579 2e6c 6f77 6572  ombine_key.lower
-000211d0: 2829 0a0a 2020 2020 4073 7472 6561 6d2e  ()..    @stream.
-000211e0: 7365 7474 6572 0a20 2020 2064 6566 2073  setter.    def s
-000211f0: 7472 6561 6d28 7365 6c66 2c20 7374 7265  tream(self, stre
-00021200: 616d 293a 0a20 2020 2020 2020 2073 656c  am):.        sel
-00021210: 662e 5f73 7472 6561 6d20 3d20 7374 7265  f._stream = stre
-00021220: 616d 0a0a 2020 2020 4070 6172 656e 7473  am..    @parents
-00021230: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00021240: 7061 7265 6e74 7328 7365 6c66 2c20 6e65  parents(self, ne
-00021250: 775f 7061 7265 6e74 7329 3a0a 2020 2020  w_parents):.    
-00021260: 2020 2020 7365 6c66 2e5f 7061 7265 6e74      self._parent
-00021270: 7320 3d20 6e65 775f 7061 7265 6e74 730a  s = new_parents.
-00021280: 0a0a 636c 6173 7320 4578 7465 726e 616c  ..class External
-00021290: 4665 6174 7572 6547 726f 7570 2846 6561  FeatureGroup(Fea
-000212a0: 7475 7265 4772 6f75 7042 6173 6529 3a0a  tureGroupBase):.
-000212b0: 2020 2020 4558 5445 524e 414c 5f46 4541      EXTERNAL_FEA
-000212c0: 5455 5245 5f47 524f 5550 203d 2022 4f4e  TURE_GROUP = "ON
-000212d0: 5f44 454d 414e 445f 4645 4154 5552 455f  _DEMAND_FEATURE_
-000212e0: 4752 4f55 5022 0a20 2020 2045 4e54 4954  GROUP".    ENTIT
-000212f0: 595f 5459 5045 203d 2022 6665 6174 7572  Y_TYPE = "featur
-00021300: 6567 726f 7570 7322 0a0a 2020 2020 6465  egroups"..    de
-00021310: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00021320: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00021330: 2020 7374 6f72 6167 655f 636f 6e6e 6563    storage_connec
-00021340: 746f 722c 0a20 2020 2020 2020 2071 7565  tor,.        que
-00021350: 7279 3d4e 6f6e 652c 0a20 2020 2020 2020  ry=None,.       
-00021360: 2064 6174 615f 666f 726d 6174 3d4e 6f6e   data_format=Non
-00021370: 652c 0a20 2020 2020 2020 2070 6174 683d  e,.        path=
-00021380: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f70  None,.        op
-00021390: 7469 6f6e 733d 7b7d 2c0a 2020 2020 2020  tions={},.      
-000213a0: 2020 6e61 6d65 3d4e 6f6e 652c 0a20 2020    name=None,.   
-000213b0: 2020 2020 2076 6572 7369 6f6e 3d4e 6f6e       version=Non
-000213c0: 652c 0a20 2020 2020 2020 2064 6573 6372  e,.        descr
-000213d0: 6970 7469 6f6e 3d4e 6f6e 652c 0a20 2020  iption=None,.   
-000213e0: 2020 2020 2070 7269 6d61 7279 5f6b 6579       primary_key
-000213f0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2066  =None,.        f
-00021400: 6561 7475 7265 7374 6f72 655f 6964 3d4e  eaturestore_id=N
-00021410: 6f6e 652c 0a20 2020 2020 2020 2066 6561  one,.        fea
-00021420: 7475 7265 7374 6f72 655f 6e61 6d65 3d4e  turestore_name=N
-00021430: 6f6e 652c 0a20 2020 2020 2020 2063 7265  one,.        cre
-00021440: 6174 6564 3d4e 6f6e 652c 0a20 2020 2020  ated=None,.     
-00021450: 2020 2063 7265 6174 6f72 3d4e 6f6e 652c     creator=None,
-00021460: 0a20 2020 2020 2020 2069 643d 4e6f 6e65  .        id=None
-00021470: 2c0a 2020 2020 2020 2020 6665 6174 7572  ,.        featur
-00021480: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
-00021490: 206c 6f63 6174 696f 6e3d 4e6f 6e65 2c0a   location=None,.
-000214a0: 2020 2020 2020 2020 7374 6174 6973 7469          statisti
-000214b0: 6373 5f63 6f6e 6669 673d 4e6f 6e65 2c0a  cs_config=None,.
-000214c0: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
-000214d0: 6d65 3d4e 6f6e 652c 0a20 2020 2020 2020  me=None,.       
-000214e0: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-000214f0: 7465 3d4e 6f6e 652c 0a20 2020 2020 2020  te=None,.       
-00021500: 206f 6e6c 696e 655f 656e 6162 6c65 643d   online_enabled=
-00021510: 4661 6c73 652c 0a20 2020 2020 2020 2068  False,.        h
-00021520: 7265 663d 4e6f 6e65 2c0a 2020 2020 2020  ref=None,.      
-00021530: 2020 6f6e 6c69 6e65 5f74 6f70 6963 5f6e    online_topic_n
-00021540: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
-00021550: 2020 746f 7069 635f 6e61 6d65 3d4e 6f6e    topic_name=Non
-00021560: 652c 0a20 2020 2020 2020 206e 6f74 6966  e,.        notif
-00021570: 6963 6174 696f 6e5f 746f 7069 635f 6e61  ication_topic_na
-00021580: 6d65 3d4e 6f6e 652c 0a20 2020 2020 2020  me=None,.       
-00021590: 2073 7069 6e65 3d46 616c 7365 2c0a 2020   spine=False,.  
-000215a0: 2020 2020 2020 6465 7072 6563 6174 6564        deprecated
-000215b0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-000215c0: 2a2a 6b77 6172 6773 2c0a 2020 2020 293a  **kwargs,.    ):
-000215d0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-000215e0: 2e5f 5f69 6e69 745f 5f28 0a20 2020 2020  .__init__(.     
-000215f0: 2020 2020 2020 206e 616d 652c 0a20 2020         name,.   
-00021600: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
-00021610: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
-00021620: 6174 7572 6573 746f 7265 5f69 642c 0a20  aturestore_id,. 
-00021630: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-00021640: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00021650: 2065 7665 6e74 5f74 696d 653d 6576 656e   event_time=even
-00021660: 745f 7469 6d65 2c0a 2020 2020 2020 2020  t_time,.        
-00021670: 2020 2020 6f6e 6c69 6e65 5f65 6e61 626c      online_enabl
-00021680: 6564 3d6f 6e6c 696e 655f 656e 6162 6c65  ed=online_enable
-00021690: 642c 0a20 2020 2020 2020 2020 2020 2069  d,.            i
-000216a0: 643d 6964 2c0a 2020 2020 2020 2020 2020  d=id,.          
-000216b0: 2020 6578 7065 6374 6174 696f 6e5f 7375    expectation_su
-000216c0: 6974 653d 6578 7065 6374 6174 696f 6e5f  ite=expectation_
-000216d0: 7375 6974 652c 0a20 2020 2020 2020 2020  suite,.         
-000216e0: 2020 206f 6e6c 696e 655f 746f 7069 635f     online_topic_
-000216f0: 6e61 6d65 3d6f 6e6c 696e 655f 746f 7069  name=online_topi
-00021700: 635f 6e61 6d65 2c0a 2020 2020 2020 2020  c_name,.        
-00021710: 2020 2020 746f 7069 635f 6e61 6d65 3d74      topic_name=t
-00021720: 6f70 6963 5f6e 616d 652c 0a20 2020 2020  opic_name,.     
-00021730: 2020 2020 2020 206e 6f74 6966 6963 6174         notificat
-00021740: 696f 6e5f 746f 7069 635f 6e61 6d65 3d6e  ion_topic_name=n
-00021750: 6f74 6966 6963 6174 696f 6e5f 746f 7069  otification_topi
-00021760: 635f 6e61 6d65 2c0a 2020 2020 2020 2020  c_name,.        
-00021770: 2020 2020 6465 7072 6563 6174 6564 3d64      deprecated=d
-00021780: 6570 7265 6361 7465 642c 0a20 2020 2020  eprecated,.     
-00021790: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
-000217a0: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
-000217b0: 655f 6e61 6d65 203d 2066 6561 7475 7265  e_name = feature
-000217c0: 7374 6f72 655f 6e61 6d65 0a20 2020 2020  store_name.     
-000217d0: 2020 2073 656c 662e 5f64 6573 6372 6970     self._descrip
-000217e0: 7469 6f6e 203d 2064 6573 6372 6970 7469  tion = descripti
-000217f0: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
-00021800: 5f63 7265 6174 6564 203d 2063 7265 6174  _created = creat
-00021810: 6564 0a20 2020 2020 2020 2073 656c 662e  ed.        self.
-00021820: 5f63 7265 6174 6f72 203d 2075 7365 722e  _creator = user.
-00021830: 5573 6572 2e66 726f 6d5f 7265 7370 6f6e  User.from_respon
-00021840: 7365 5f6a 736f 6e28 6372 6561 746f 7229  se_json(creator)
-00021850: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
-00021860: 7565 7279 203d 2071 7565 7279 0a20 2020  uery = query.   
-00021870: 2020 2020 2073 656c 662e 5f64 6174 615f       self._data_
-00021880: 666f 726d 6174 203d 2064 6174 615f 666f  format = data_fo
-00021890: 726d 6174 2e75 7070 6572 2829 2069 6620  rmat.upper() if 
-000218a0: 6461 7461 5f66 6f72 6d61 7420 656c 7365  data_format else
-000218b0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-000218c0: 6c66 2e5f 7061 7468 203d 2070 6174 680a  lf._path = path.
-000218d0: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-000218e0: 6561 7475 7265 7320 3d20 5b0a 2020 2020  eatures = [.    
-000218f0: 2020 2020 2020 2020 6665 6174 7572 652e          feature.
-00021900: 4665 6174 7572 652e 6672 6f6d 5f72 6573  Feature.from_res
-00021910: 706f 6e73 655f 6a73 6f6e 2866 6561 7429  ponse_json(feat)
-00021920: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
-00021930: 6561 742c 2064 6963 7429 2065 6c73 6520  eat, dict) else 
-00021940: 6665 6174 0a20 2020 2020 2020 2020 2020  feat.           
-00021950: 2066 6f72 2066 6561 7420 696e 2028 6665   for feat in (fe
-00021960: 6174 7572 6573 206f 7220 5b5d 290a 2020  atures or []).  
-00021970: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
-00021980: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
-00021990: 726f 7570 5f65 6e67 696e 6520 3d20 280a  roup_engine = (.
-000219a0: 2020 2020 2020 2020 2020 2020 6578 7465              exte
-000219b0: 726e 616c 5f66 6561 7475 7265 5f67 726f  rnal_feature_gro
-000219c0: 7570 5f65 6e67 696e 652e 4578 7465 726e  up_engine.Extern
-000219d0: 616c 4665 6174 7572 6547 726f 7570 456e  alFeatureGroupEn
-000219e0: 6769 6e65 2866 6561 7475 7265 7374 6f72  gine(featurestor
-000219f0: 655f 6964 290a 2020 2020 2020 2020 290a  e_id).        ).
-00021a00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00021a10: 2e5f 6964 3a0a 2020 2020 2020 2020 2020  ._id:.          
-00021a20: 2020 2320 476f 7420 6672 6f6d 2048 6f70    # Got from Hop
-00021a30: 7377 6f72 6b73 2c20 6465 7365 7269 616c  sworks, deserial
-00021a40: 697a 6520 6665 6174 7572 6573 2061 6e64  ize features and
-00021a50: 2073 746f 7261 6765 2063 6f6e 6e65 6374   storage connect
-00021a60: 6f72 0a20 2020 2020 2020 2020 2020 2073  or.            s
-00021a70: 656c 662e 5f66 6561 7475 7265 7320 3d20  elf._features = 
-00021a80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00021a90: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00021aa0: 2020 2020 2020 2020 6665 6174 7572 652e          feature.
-00021ab0: 4665 6174 7572 652e 6672 6f6d 5f72 6573  Feature.from_res
-00021ac0: 706f 6e73 655f 6a73 6f6e 2866 6561 7429  ponse_json(feat)
-00021ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021ae0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00021af0: 6365 2866 6561 742c 2064 6963 7429 0a20  ce(feat, dict). 
-00021b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b10: 2020 2065 6c73 6520 6665 6174 0a20 2020     else feat.   
-00021b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b30: 2066 6f72 2066 6561 7420 696e 2066 6561   for feat in fea
-00021b40: 7475 7265 730a 2020 2020 2020 2020 2020  tures.          
-00021b50: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00021b60: 2020 2020 2020 2020 6966 2066 6561 7475          if featu
-00021b70: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
-00021b80: 2020 2020 656c 7365 204e 6f6e 650a 2020      else None.  
-00021b90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00021ba0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-00021bb0: 6d61 7279 5f6b 6579 203d 2028 0a20 2020  mary_key = (.   
-00021bc0: 2020 2020 2020 2020 2020 2020 205b 6665               [fe
-00021bd0: 6174 2e6e 616d 6520 666f 7220 6665 6174  at.name for feat
-00021be0: 2069 6e20 7365 6c66 2e5f 6665 6174 7572   in self._featur
-00021bf0: 6573 2069 6620 6665 6174 2e70 7269 6d61  es if feat.prima
-00021c00: 7279 2069 7320 5472 7565 5d0a 2020 2020  ry is True].    
-00021c10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00021c20: 656c 662e 5f66 6561 7475 7265 730a 2020  elf._features.  
-00021c30: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00021c40: 7365 205b 5d0a 2020 2020 2020 2020 2020  se [].          
-00021c50: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00021c60: 7365 6c66 2e73 7461 7469 7374 6963 735f  self.statistics_
-00021c70: 636f 6e66 6967 203d 2073 7461 7469 7374  config = statist
-00021c80: 6963 735f 636f 6e66 6967 0a0a 2020 2020  ics_config..    
-00021c90: 2020 2020 2020 2020 7365 6c66 2e5f 6f70          self._op
-00021ca0: 7469 6f6e 7320 3d20 280a 2020 2020 2020  tions = (.      
-00021cb0: 2020 2020 2020 2020 2020 7b6f 7074 696f            {optio
-00021cc0: 6e5b 226e 616d 6522 5d3a 206f 7074 696f  n["name"]: optio
-00021cd0: 6e5b 2276 616c 7565 225d 2066 6f72 206f  n["value"] for o
-00021ce0: 7074 696f 6e20 696e 206f 7074 696f 6e73  ption in options
-00021cf0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00021d00: 2020 6966 206f 7074 696f 6e73 0a20 2020    if options.   
-00021d10: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00021d20: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-00021d30: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-00021d40: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00021d50: 656c 662e 7072 696d 6172 795f 6b65 7920  elf.primary_key 
-00021d60: 3d20 7072 696d 6172 795f 6b65 790a 2020  = primary_key.  
-00021d70: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00021d80: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
-00021d90: 203d 2073 7461 7469 7374 6963 735f 636f   = statistics_co
-00021da0: 6e66 6967 0a20 2020 2020 2020 2020 2020  nfig.           
-00021db0: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
-00021dc0: 3d20 6665 6174 7572 6573 0a20 2020 2020  = features.     
-00021dd0: 2020 2020 2020 2073 656c 662e 5f6f 7074         self._opt
-00021de0: 696f 6e73 203d 206f 7074 696f 6e73 0a0a  ions = options..
-00021df0: 2020 2020 2020 2020 6966 2073 746f 7261          if stora
-00021e00: 6765 5f63 6f6e 6e65 6374 6f72 2069 7320  ge_connector is 
-00021e10: 6e6f 7420 4e6f 6e65 2061 6e64 2069 7369  not None and isi
-00021e20: 6e73 7461 6e63 6528 7374 6f72 6167 655f  nstance(storage_
-00021e30: 636f 6e6e 6563 746f 722c 2064 6963 7429  connector, dict)
-00021e40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00021e50: 6c66 2e5f 7374 6f72 6167 655f 636f 6e6e  lf._storage_conn
-00021e60: 6563 746f 7220 3d20 7363 2e53 746f 7261  ector = sc.Stora
-00021e70: 6765 436f 6e6e 6563 746f 722e 6672 6f6d  geConnector.from
-00021e80: 5f72 6573 706f 6e73 655f 6a73 6f6e 280a  _response_json(.
-00021e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ea0: 7374 6f72 6167 655f 636f 6e6e 6563 746f  storage_connecto
-00021eb0: 720a 2020 2020 2020 2020 2020 2020 290a  r.            ).
-00021ec0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00021ed0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00021ee0: 7374 6f72 6167 655f 636f 6e6e 6563 746f  storage_connecto
-00021ef0: 7220 3d20 7374 6f72 6167 655f 636f 6e6e  r = storage_conn
-00021f00: 6563 746f 720a 0a20 2020 2020 2020 2073  ector..        s
-00021f10: 656c 662e 5f68 7265 6620 3d20 6872 6566  elf._href = href
-00021f20: 0a0a 2020 2020 6465 6620 7361 7665 2873  ..    def save(s
-00021f30: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00021f40: 2250 6572 7369 7374 2074 6865 206d 6574  "Persist the met
-00021f50: 6164 6174 6120 666f 7220 7468 6973 2065  adata for this e
-00021f60: 7874 6572 6e61 6c20 6665 6174 7572 6520  xternal feature 
-00021f70: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
-00021f80: 5769 7468 6f75 7420 6361 6c6c 696e 6720  Without calling 
-00021f90: 7468 6973 206d 6574 686f 642c 2079 6f75  this method, you
-00021fa0: 7220 6665 6174 7572 6520 6772 6f75 7020  r feature group 
-00021fb0: 7769 6c6c 206f 6e6c 7920 6578 6973 740a  will only exist.
-00021fc0: 2020 2020 2020 2020 696e 2079 6f75 7220          in your 
-00021fd0: 5079 7468 6f6e 204b 6572 6e65 6c2c 2062  Python Kernel, b
-00021fe0: 7574 206e 6f74 2069 6e20 486f 7073 776f  ut not in Hopswo
-00021ff0: 726b 732e 0a0a 2020 2020 2020 2020 6060  rks...        ``
-00022000: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00022010: 7175 6572 7920 3d20 2253 454c 4543 5420  query = "SELECT 
-00022020: 2a20 4652 4f4d 2073 616c 6573 220a 0a20  * FROM sales".. 
-00022030: 2020 2020 2020 2066 6720 3d20 6665 6174         fg = feat
-00022040: 7572 655f 7374 6f72 652e 6372 6561 7465  ure_store.create
-00022050: 5f65 7874 6572 6e61 6c5f 6665 6174 7572  _external_featur
-00022060: 655f 6772 6f75 7028 6e61 6d65 3d22 7361  e_group(name="sa
-00022070: 6c65 7322 2c0a 2020 2020 2020 2020 2020  les",.          
-00022080: 2020 7665 7273 696f 6e3d 312c 0a20 2020    version=1,.   
-00022090: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-000220a0: 7469 6f6e 3d22 5068 7973 6963 616c 2073  tion="Physical s
-000220b0: 686f 7020 7361 6c65 7320 6665 6174 7572  hop sales featur
-000220c0: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
-000220d0: 2071 7565 7279 3d71 7565 7279 2c0a 2020   query=query,.  
-000220e0: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-000220f0: 655f 636f 6e6e 6563 746f 723d 636f 6e6e  e_connector=conn
-00022100: 6563 746f 722c 0a20 2020 2020 2020 2020  ector,.         
-00022110: 2020 2070 7269 6d61 7279 5f6b 6579 3d5b     primary_key=[
-00022120: 2773 735f 7374 6f72 655f 736b 275d 2c0a  'ss_store_sk'],.
-00022130: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00022140: 745f 7469 6d65 3d27 7361 6c65 5f64 6174  t_time='sale_dat
-00022150: 6527 0a20 2020 2020 2020 2029 0a0a 2020  e'.        )..  
-00022160: 2020 2020 2020 6667 2e73 6176 6528 290a        fg.save().
-00022170: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00022180: 2020 2020 7365 6c66 2e5f 6665 6174 7572      self._featur
-00022190: 655f 6772 6f75 705f 656e 6769 6e65 2e73  e_group_engine.s
-000221a0: 6176 6528 7365 6c66 290a 2020 2020 2020  ave(self).      
-000221b0: 2020 7365 6c66 2e5f 636f 6465 5f65 6e67    self._code_eng
-000221c0: 696e 652e 7361 7665 5f63 6f64 6528 7365  ine.save_code(se
-000221d0: 6c66 290a 0a20 2020 2020 2020 2069 6620  lf)..        if 
-000221e0: 7365 6c66 2e73 7461 7469 7374 6963 735f  self.statistics_
-000221f0: 636f 6e66 6967 2e65 6e61 626c 6564 3a0a  config.enabled:.
-00022200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00022210: 2e5f 7374 6174 6973 7469 6373 5f65 6e67  ._statistics_eng
-00022220: 696e 652e 636f 6d70 7574 655f 616e 645f  ine.compute_and_
-00022230: 7361 7665 5f73 7461 7469 7374 6963 7328  save_statistics(
-00022240: 7365 6c66 290a 0a20 2020 2064 6566 2069  self)..    def i
-00022250: 6e73 6572 7428 0a20 2020 2020 2020 2073  nsert(.        s
-00022260: 656c 662c 0a20 2020 2020 2020 2066 6561  elf,.        fea
-00022270: 7475 7265 733a 2055 6e69 6f6e 5b0a 2020  tures: Union[.  
-00022280: 2020 2020 2020 2020 2020 7064 2e44 6174            pd.Dat
-00022290: 6146 7261 6d65 2c0a 2020 2020 2020 2020  aFrame,.        
-000222a0: 2020 2020 5479 7065 5661 7228 2270 7973      TypeVar("pys
-000222b0: 7061 726b 2e73 716c 2e44 6174 6146 7261  park.sql.DataFra
-000222c0: 6d65 2229 2c20 2023 206e 6f71 613a 2046  me"),  # noqa: F
-000222d0: 3832 310a 2020 2020 2020 2020 2020 2020  821.            
-000222e0: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
-000222f0: 2e52 4444 2229 2c20 2023 206e 6f71 613a  .RDD"),  # noqa:
-00022300: 2046 3832 310a 2020 2020 2020 2020 2020   F821.          
-00022310: 2020 6e70 2e6e 6461 7272 6179 2c0a 2020    np.ndarray,.  
-00022320: 2020 2020 2020 2020 2020 4c69 7374 5b6c            List[l
-00022330: 6973 745d 2c0a 2020 2020 2020 2020 5d2c  ist],.        ],
-00022340: 0a20 2020 2020 2020 2077 7269 7465 5f6f  .        write_o
-00022350: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
-00022360: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
-00022370: 203d 207b 7d2c 0a20 2020 2020 2020 2076   = {},.        v
-00022380: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
-00022390: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
-000223a0: 5b73 7472 2c20 416e 795d 5d20 3d20 7b7d  [str, Any]] = {}
-000223b0: 2c0a 2020 2020 2020 2020 7361 7665 5f63  ,.        save_c
-000223c0: 6f64 653a 204f 7074 696f 6e61 6c5b 626f  ode: Optional[bo
-000223d0: 6f6c 5d20 3d20 5472 7565 2c0a 2020 2020  ol] = True,.    
-000223e0: 2020 2020 7761 6974 3a20 626f 6f6c 203d      wait: bool =
-000223f0: 2046 616c 7365 2c0a 2020 2020 2920 2d3e   False,.    ) ->
-00022400: 2054 7570 6c65 5b4f 7074 696f 6e61 6c5b   Tuple[Optional[
-00022410: 4a6f 625d 2c20 4f70 7469 6f6e 616c 5b56  Job], Optional[V
-00022420: 616c 6964 6174 696f 6e52 6570 6f72 745d  alidationReport]
-00022430: 5d3a 0a20 2020 2020 2020 2022 2222 496e  ]:.        """In
-00022440: 7365 7274 2074 6865 2064 6174 6166 7261  sert the datafra
-00022450: 6d65 2066 6561 7475 7265 2076 616c 7565  me feature value
-00022460: 7320 4f4e 4c59 2069 6e20 7468 6520 6f6e  s ONLY in the on
-00022470: 6c69 6e65 2066 6561 7475 7265 2073 746f  line feature sto
-00022480: 7265 2e0a 0a20 2020 2020 2020 2045 7874  re...        Ext
-00022490: 6572 6e61 6c20 4665 6174 7572 6520 4772  ernal Feature Gr
-000224a0: 6f75 7073 2063 6f6e 7461 696e 7320 6d65  oups contains me
-000224b0: 7461 6461 7461 2061 626f 7574 2066 6561  tadata about fea
-000224c0: 7475 7265 2064 6174 6120 696e 2061 6e20  ture data in an 
-000224d0: 6578 7465 726e 616c 2073 746f 7261 6765  external storage
-000224e0: 2073 7973 7465 6d2e 0a20 2020 2020 2020   system..       
-000224f0: 2045 7874 6572 6e61 6c20 7374 6f72 6167   External storag
-00022500: 6520 7379 7374 656d 2061 7265 2075 7375  e system are usu
-00022510: 616c 6c79 206f 6666 6c69 6e65 2c20 6d65  ally offline, me
-00022520: 616e 696e 6720 6665 6174 7572 6520 7661  aning feature va
-00022530: 6c75 6573 2063 616e 6e6f 7420 6265 2072  lues cannot be r
-00022540: 6574 7269 6576 6564 2069 6e20 7265 616c  etrieved in real
-00022550: 2d74 696d 652e 0a20 2020 2020 2020 2049  -time..        I
-00022560: 6e20 6f72 6465 7220 746f 2075 7365 2074  n order to use t
-00022570: 6865 2066 6561 7475 7265 2076 616c 7565  he feature value
-00022580: 7320 666f 7220 7265 616c 2d74 696d 6520  s for real-time 
-00022590: 7573 652d 6361 7365 732c 2079 6f75 2063  use-cases, you c
-000225a0: 616e 2069 6e73 6572 7420 7468 656d 0a20  an insert them. 
-000225b0: 2020 2020 2020 2069 6e20 486f 7073 6f77         in Hopsow
-000225c0: 6f72 6b73 204f 6e6c 696e 6520 4665 6174  orks Online Feat
-000225d0: 7572 6520 5374 6f72 6520 7669 6120 7468  ure Store via th
-000225e0: 6973 206d 6574 686f 642e 0a0a 2020 2020  is method...    
-000225f0: 2020 2020 5468 6520 4f6e 6c69 6e65 2046      The Online F
-00022600: 6561 7475 7265 2053 746f 7265 2068 6173  eature Store has
-00022610: 2061 2073 696e 676c 652d 656e 7472 7920   a single-entry 
-00022620: 7065 7220 7072 696d 6172 7920 6b65 7920  per primary key 
-00022630: 7661 6c75 652c 206d 6561 696e 696e 6720  value, meaining 
-00022640: 7468 6174 2070 726f 7669 6469 6e67 2061  that providing a
-00022650: 206e 6577 2076 616c 7565 2077 6974 680a   new value with.
-00022660: 2020 2020 2020 2020 666f 7220 6120 6769          for a gi
-00022670: 7665 6e20 7072 696d 6172 7920 6b65 7920  ven primary key 
-00022680: 7769 6c6c 206f 7665 7277 7269 7465 2074  will overwrite t
-00022690: 6865 2065 7869 7374 696e 6720 7661 6c75  he existing valu
-000226a0: 652e 204e 6f20 7265 636f 7264 206f 6620  e. No record of 
-000226b0: 7468 6520 7072 6576 696f 7573 2076 616c  the previous val
-000226c0: 7565 2069 7320 6b65 7074 2e0a 0a20 2020  ue is kept...   
-000226d0: 2020 2020 2021 2121 2065 7861 6d70 6c65       !!! example
-000226e0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-000226f0: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
-00022700: 2020 2023 2063 6f6e 6e65 6374 2074 6f20     # connect to 
-00022710: 7468 6520 4665 6174 7572 6520 5374 6f72  the Feature Stor
-00022720: 650a 2020 2020 2020 2020 2020 2020 6673  e.            fs
-00022730: 203d 202e 2e2e 0a0a 2020 2020 2020 2020   = .....        
-00022740: 2020 2020 2320 6765 7420 7468 6520 4578      # get the Ex
-00022750: 7465 726e 616c 2046 6561 7475 7265 2047  ternal Feature G
-00022760: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-00022770: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
-00022780: 732e 6765 745f 6665 6174 7572 655f 6772  s.get_feature_gr
-00022790: 6f75 7028 6e61 6d65 3d22 6578 7465 726e  oup(name="extern
-000227a0: 616c 5f73 616c 6573 5f72 6563 6f72 6473  al_sales_records
-000227b0: 222c 2076 6572 7369 6f6e 3d31 290a 0a20  ", version=1).. 
-000227c0: 2020 2020 2020 2020 2020 2023 2067 6574             # get
-000227d0: 2074 6865 2066 6561 7475 7265 2076 616c   the feature val
-000227e0: 7565 732c 2065 2e67 2072 6561 6469 6e67  ues, e.g reading
-000227f0: 2066 726f 6d20 6373 7620 6669 6c65 7320   from csv files 
-00022800: 696e 2061 2053 3320 6275 636b 6574 0a20  in a S3 bucket. 
-00022810: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-00022820: 7265 5f76 616c 7565 7320 3d20 2e2e 2e0a  re_values = ....
-00022830: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00022840: 6e73 6572 7420 7468 6520 6665 6174 7572  nsert the featur
-00022850: 6520 7661 6c75 6573 2069 6e20 7468 6520  e values in the 
-00022860: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
-00022870: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
-00022880: 2066 672e 696e 7365 7274 2866 6561 7475   fg.insert(featu
-00022890: 7265 5f76 616c 7565 7329 0a20 2020 2020  re_values).     
-000228a0: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-000228b0: 2020 2020 2121 2120 4e6f 7465 0a20 2020      !!! Note.   
-000228c0: 2020 2020 2020 2020 2044 6174 6120 5661           Data Va
-000228d0: 6c69 6461 7469 6f6e 2076 6961 2047 7265  lidation via Gre
-000228e0: 6174 2045 7870 6563 7461 7469 6f6e 2069  at Expectation i
-000228f0: 7320 7375 7070 6f72 7465 6420 6966 2079  s supported if y
-00022900: 6f75 2068 6176 6520 6174 7461 6368 6564  ou have attached
-00022910: 2061 6e20 6578 7065 6374 6174 696f 6e20   an expectation 
-00022920: 7375 6974 6520 746f 0a20 2020 2020 2020  suite to.       
-00022930: 2020 2020 2079 6f75 7220 4578 7465 726e       your Extern
-00022940: 616c 2046 6561 7475 7265 2047 726f 7570  al Feature Group
-00022950: 2e20 486f 7765 7665 722c 2061 7320 6f70  . However, as op
-00022960: 706f 7365 6420 746f 2072 6567 756c 6172  posed to regular
-00022970: 2046 6561 7475 7265 2047 726f 7570 732c   Feature Groups,
-00022980: 2074 6869 7320 6361 6e20 6c65 6164 2074   this can lead t
-00022990: 6f0a 2020 2020 2020 2020 2020 2020 6469  o.            di
-000229a0: 7363 7265 7061 6e63 6965 7320 6265 7477  screpancies betw
-000229b0: 6565 6e20 7468 6520 6461 7461 2069 6e20  een the data in 
-000229c0: 7468 6520 6578 7465 726e 616c 2073 746f  the external sto
-000229d0: 7261 6765 2073 7973 7465 6d20 616e 6420  rage system and 
-000229e0: 7468 6520 6f6e 6c69 6e65 2066 6561 7475  the online featu
-000229f0: 7265 2073 746f 7265 2e0a 0a20 2020 2020  re store...     
-00022a00: 2020 2023 2041 7267 756d 656e 7473 0a20     # Arguments. 
-00022a10: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-00022a20: 7265 733a 2044 6174 6146 7261 6d65 2c20  res: DataFrame, 
-00022a30: 5244 442c 204e 6461 7272 6179 2c20 6c69  RDD, Ndarray, li
-00022a40: 7374 2e20 4665 6174 7572 6573 2074 6f20  st. Features to 
-00022a50: 6265 2073 6176 6564 2e0a 2020 2020 2020  be saved..      
-00022a60: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
-00022a70: 6f6e 733a 2041 6464 6974 696f 6e61 6c20  ons: Additional 
-00022a80: 7772 6974 6520 6f70 7469 6f6e 7320 6173  write options as
-00022a90: 206b 6579 2d76 616c 7565 2070 6169 7273   key-value pairs
-00022aa0: 2c20 6465 6661 756c 7473 2074 6f20 607b  , defaults to `{
-00022ab0: 7d60 2e0a 2020 2020 2020 2020 2020 2020  }`..            
-00022ac0: 2020 2020 5768 656e 2075 7369 6e67 2074      When using t
-00022ad0: 6865 2060 7079 7468 6f6e 6020 656e 6769  he `python` engi
-00022ae0: 6e65 2c20 7772 6974 655f 6f70 7469 6f6e  ne, write_option
-00022af0: 7320 6361 6e20 636f 6e74 6169 6e20 7468  s can contain th
-00022b00: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00022b10: 2020 666f 6c6c 6f77 696e 6720 656e 7472    following entr
-00022b20: 6965 733a 0a20 2020 2020 2020 2020 2020  ies:.           
-00022b30: 2020 2020 202a 206b 6579 2060 6b61 666b       * key `kafk
-00022b40: 615f 7072 6f64 7563 6572 5f63 6f6e 6669  a_producer_confi
-00022b50: 6760 2061 6e64 2076 616c 7565 2061 6e20  g` and value an 
-00022b60: 6f62 6a65 6374 206f 6620 7479 7065 205b  object of type [
-00022b70: 7072 6f70 6572 7469 6573 5d28 6874 7470  properties](http
-00022b80: 733a 2f2f 646f 6373 2e63 6f6e 666c 7565  s://docs.conflue
-00022b90: 6e74 2e69 6f2f 706c 6174 666f 726d 2f63  nt.io/platform/c
-00022ba0: 7572 7265 6e74 2f63 6c69 656e 7473 2f6c  urrent/clients/l
-00022bb0: 6962 7264 6b61 666b 612f 6874 6d6c 2f6d  ibrdkafka/html/m
-00022bc0: 645f 434f 4e46 4947 5552 4154 494f 4e2e  d_CONFIGURATION.
-00022bd0: 6874 6d6c 6e29 0a20 2020 2020 2020 2020  htmln).         
-00022be0: 2020 2020 2020 2020 2075 7365 6420 746f           used to
-00022bf0: 2063 6f6e 6669 6775 7265 2074 6865 204b   configure the K
-00022c00: 6166 6b61 2063 6c69 656e 742e 2054 6f20  afka client. To 
-00022c10: 6f70 7469 6d69 7a65 2066 6f72 2074 6872  optimize for thr
-00022c20: 6f75 6768 7075 7420 696e 2068 6967 6820  oughput in high 
-00022c30: 6c61 7465 6e63 7920 636f 6e6e 6563 7469  latency connecti
-00022c40: 6f6e 2063 6f6e 7369 6465 720a 2020 2020  on consider.    
-00022c50: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00022c60: 616e 6769 6e67 205b 7072 6f64 7563 6572  anging [producer
-00022c70: 2070 726f 7065 7274 6965 735d 2868 7474   properties](htt
-00022c80: 7073 3a2f 2f64 6f63 732e 636f 6e66 6c75  ps://docs.conflu
-00022c90: 656e 742e 696f 2f63 6c6f 7564 2f63 7572  ent.io/cloud/cur
-00022ca0: 7265 6e74 2f63 6c69 656e 742d 6170 7073  rent/client-apps
-00022cb0: 2f6f 7074 696d 697a 696e 672f 7468 726f  /optimizing/thro
-00022cc0: 7567 6870 7574 2e68 746d 6c23 7072 6f64  ughput.html#prod
-00022cd0: 7563 6572 292e 0a20 2020 2020 2020 2020  ucer)..         
-00022ce0: 2020 2020 2020 202a 206b 6579 2060 696e         * key `in
-00022cf0: 7465 726e 616c 5f6b 6166 6b61 6020 616e  ternal_kafka` an
-00022d00: 6420 7661 6c75 6520 6054 7275 6560 206f  d value `True` o
-00022d10: 7220 6046 616c 7365 6020 696e 2063 6173  r `False` in cas
-00022d20: 6520 796f 7520 6573 7461 626c 6973 6865  e you establishe
-00022d30: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00022d40: 2020 2020 636f 6e6e 6563 7469 7669 7479      connectivity
-00022d50: 2066 726f 6d20 796f 7520 5079 7468 6f6e   from you Python
-00022d60: 2065 6e76 6972 6f6e 6d65 6e74 2074 6f20   environment to 
-00022d70: 7468 6520 696e 7465 726e 616c 2061 6476  the internal adv
-00022d80: 6572 7469 7365 640a 2020 2020 2020 2020  ertised.        
-00022d90: 2020 2020 2020 2020 2020 6c69 7374 656e            listen
-00022da0: 6572 7320 6f66 2074 6865 2048 6f70 7377  ers of the Hopsw
-00022db0: 6f72 6b73 204b 6166 6b61 2043 6c75 7374  orks Kafka Clust
-00022dc0: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
-00022dd0: 6046 616c 7365 6020 616e 640a 2020 2020  `False` and.    
-00022de0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00022df0: 6c6c 2075 7365 2065 7874 6572 6e61 6c20  ll use external 
-00022e00: 6c69 7374 656e 6572 7320 7768 656e 2063  listeners when c
-00022e10: 6f6e 6e65 6374 696e 6720 6672 6f6d 206f  onnecting from o
-00022e20: 7574 7369 6465 206f 6620 486f 7073 776f  utside of Hopswo
-00022e30: 726b 732e 0a20 2020 2020 2020 2020 2020  rks..           
-00022e40: 2076 616c 6964 6174 696f 6e5f 6f70 7469   validation_opti
-00022e50: 6f6e 733a 2041 6464 6974 696f 6e61 6c20  ons: Additional 
-00022e60: 7661 6c69 6461 7469 6f6e 206f 7074 696f  validation optio
-00022e70: 6e73 2061 7320 6b65 792d 7661 6c75 6520  ns as key-value 
-00022e80: 7061 6972 732c 2064 6566 6175 6c74 7320  pairs, defaults 
-00022e90: 746f 2060 7b7d 602e 0a20 2020 2020 2020  to `{}`..       
-00022ea0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-00022eb0: 7275 6e5f 7661 6c69 6461 7469 6f6e 6020  run_validation` 
-00022ec0: 626f 6f6c 6561 6e20 7661 6c75 652c 2073  boolean value, s
-00022ed0: 6574 2074 6f20 6046 616c 7365 6020 746f  et to `False` to
-00022ee0: 2073 6b69 7020 7661 6c69 6461 7469 6f6e   skip validation
-00022ef0: 2074 656d 706f 7261 7269 6c79 206f 6e20   temporarily on 
-00022f00: 696e 6765 7374 696f 6e2e 0a20 2020 2020  ingestion..     
-00022f10: 2020 2020 2020 2020 2020 202a 206b 6579             * key
-00022f20: 2060 7361 7665 5f72 6570 6f72 7460 2062   `save_report` b
-00022f30: 6f6f 6c65 616e 2076 616c 7565 2c20 7365  oolean value, se
-00022f40: 7420 746f 2060 4661 6c73 6560 2074 6f20  t to `False` to 
-00022f50: 736b 6970 2075 706c 6f61 6420 6f66 2074  skip upload of t
-00022f60: 6865 2076 616c 6964 6174 696f 6e20 7265  he validation re
-00022f70: 706f 7274 2074 6f20 486f 7073 776f 726b  port to Hopswork
-00022f80: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00022f90: 2020 202a 206b 6579 2060 6765 5f76 616c     * key `ge_val
-00022fa0: 6964 6174 655f 6b77 6172 6773 6020 6120  idate_kwargs` a 
-00022fb0: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
-00022fc0: 696e 696e 6720 6b77 6172 6773 2066 6f72  ining kwargs for
-00022fd0: 2074 6865 2076 616c 6964 6174 6520 6d65   the validate me
-00022fe0: 7468 6f64 206f 6620 4772 6561 7420 4578  thod of Great Ex
-00022ff0: 7065 6374 6174 696f 6e73 2e0a 2020 2020  pectations..    
-00023000: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
-00023010: 7920 6066 6574 6368 5f65 7870 6563 7461  y `fetch_expecta
-00023020: 7469 6f6e 5f73 7569 7465 6020 6120 626f  tion_suite` a bo
-00023030: 6f6c 6561 6e20 7661 6c75 652c 2062 7920  olean value, by 
-00023040: 6465 6661 756c 7420 6054 7275 6560 2c20  default `True`, 
-00023050: 746f 2063 6f6e 7472 6f6c 2077 6865 7468  to control wheth
-00023060: 6572 2074 6865 2065 7870 6563 7461 7469  er the expectati
-00023070: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00023080: 2020 2020 2020 7375 6974 6520 6f66 2074        suite of t
-00023090: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-000230a0: 2073 686f 756c 6420 6265 2066 6574 6368   should be fetch
-000230b0: 6564 2062 6566 6f72 6520 6576 6572 7920  ed before every 
-000230c0: 696e 7365 7274 2e0a 2020 2020 2020 2020  insert..        
-000230d0: 2020 2020 7361 7665 5f63 6f64 653a 2057      save_code: W
-000230e0: 6865 6e20 7275 6e6e 696e 6720 4853 4653  hen running HSFS
-000230f0: 206f 6e20 486f 7073 776f 726b 7320 6f72   on Hopsworks or
-00023100: 2044 6174 6162 7269 636b 732c 2048 5346   Databricks, HSF
-00023110: 5320 6361 6e20 7361 7665 2074 6865 2063  S can save the c
-00023120: 6f64 652f 6e6f 7465 626f 6f6b 2075 7365  ode/notebook use
-00023130: 6420 746f 2063 7265 6174 650a 2020 2020  d to create.    
-00023140: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00023150: 6665 6174 7572 6520 6772 6f75 7020 6f72  feature group or
-00023160: 2075 7365 6420 746f 2069 6e73 6572 7420   used to insert 
-00023170: 6461 7461 2074 6f20 6974 2e20 5768 656e  data to it. When
-00023180: 2063 616c 6c69 6e67 2074 6865 2060 696e   calling the `in
-00023190: 7365 7274 6020 6d65 7468 6f64 2072 6570  sert` method rep
-000231a0: 6561 7465 646c 790a 2020 2020 2020 2020  eatedly.        
-000231b0: 2020 2020 2020 2020 7769 7468 2073 6d61          with sma
-000231c0: 6c6c 2062 6174 6368 6573 206f 6620 6461  ll batches of da
-000231d0: 7461 2c20 7468 6973 2063 616e 2073 6c6f  ta, this can slo
-000231e0: 7720 646f 776e 2074 6865 2077 7269 7465  w down the write
-000231f0: 732e 2055 7365 2074 6869 7320 6f70 7469  s. Use this opti
-00023200: 6f6e 2074 6f20 7475 726e 206f 6666 2073  on to turn off s
-00023210: 6176 696e 670a 2020 2020 2020 2020 2020  aving.          
-00023220: 2020 2020 2020 636f 6465 2e20 4465 6661        code. Defa
-00023230: 756c 7473 2074 6f20 6054 7275 6560 2e0a  ults to `True`..
-00023240: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-00023250: 6e73 0a20 2020 2020 2020 2020 2020 2054  ns.            T
-00023260: 7570 6c65 2860 4a6f 6260 2c20 6056 616c  uple(`Job`, `Val
-00023270: 6964 6174 696f 6e52 6570 6f72 7460 2920  idationReport`) 
-00023280: 5468 6520 7661 6c69 6461 7469 6f6e 2072  The validation r
-00023290: 6570 6f72 7420 6966 2076 616c 6964 6174  eport if validat
-000232a0: 696f 6e20 6973 2065 6e61 626c 6564 2e0a  ion is enabled..
-000232b0: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
-000232c0: 730a 2020 2020 2020 2020 2020 2020 6068  s.            `h
-000232d0: 7366 732e 636c 6965 6e74 2e65 7863 6570  sfs.client.excep
-000232e0: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
-000232f0: 6f72 602e 2065 2e67 2066 6169 6c20 746f  or`. e.g fail to
-00023300: 2063 7265 6174 6520 6665 6174 7572 6520   create feature 
-00023310: 6772 6f75 702c 2064 6174 6166 7261 6d65  group, dataframe
-00023320: 2073 6368 656d 6120 646f 6573 206e 6f74   schema does not
-00023330: 206d 6174 6368 0a20 2020 2020 2020 2020   match.         
-00023340: 2020 2020 2020 2065 7869 7374 696e 6720         existing 
-00023350: 6665 6174 7572 6520 6772 6f75 7020 7363  feature group sc
-00023360: 6865 6d61 2c20 6574 632e 0a20 2020 2020  hema, etc..     
-00023370: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
-00023380: 656e 742e 6578 6365 7074 696f 6e73 2e44  ent.exceptions.D
-00023390: 6174 6156 616c 6964 6174 696f 6e45 7863  ataValidationExc
-000233a0: 6570 7469 6f6e 602e 2049 6620 6461 7461  eption`. If data
-000233b0: 2076 616c 6964 6174 696f 6e20 6661 696c   validation fail
-000233c0: 7320 616e 6420 7468 6520 6578 7065 6374  s and the expect
-000233d0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-000233e0: 2020 2020 2020 7375 6974 6520 6076 616c        suite `val
-000233f0: 6964 6174 696f 6e5f 696e 6765 7374 696f  idation_ingestio
-00023400: 6e5f 706f 6c69 6379 6020 6973 2073 6574  n_policy` is set
-00023410: 2074 6f20 6053 5452 4943 5460 2e20 4461   to `STRICT`. Da
-00023420: 7461 2069 7320 4e4f 5420 696e 6765 7374  ta is NOT ingest
-00023430: 6564 2e0a 0a20 2020 2020 2020 2022 2222  ed...        """
-00023440: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
-00023450: 5f64 6174 6166 7261 6d65 203d 2065 6e67  _dataframe = eng
-00023460: 696e 652e 6765 745f 696e 7374 616e 6365  ine.get_instance
-00023470: 2829 2e63 6f6e 7665 7274 5f74 6f5f 6465  ().convert_to_de
-00023480: 6661 756c 745f 6461 7461 6672 616d 6528  fault_dataframe(
-00023490: 6665 6174 7572 6573 290a 0a20 2020 2020  features)..     
-000234a0: 2020 2069 6620 7772 6974 655f 6f70 7469     if write_opti
-000234b0: 6f6e 7320 6973 204e 6f6e 653a 0a20 2020  ons is None:.   
-000234c0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-000234d0: 7074 696f 6e73 203d 207b 7d0a 2020 2020  ptions = {}.    
-000234e0: 2020 2020 6966 2022 7761 6974 5f66 6f72      if "wait_for
-000234f0: 5f6a 6f62 2220 6e6f 7420 696e 2077 7269  _job" not in wri
-00023500: 7465 5f6f 7074 696f 6e73 3a0a 2020 2020  te_options:.    
-00023510: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-00023520: 7469 6f6e 735b 2277 6169 745f 666f 725f  tions["wait_for_
-00023530: 6a6f 6222 5d20 3d20 7761 6974 0a0a 2020  job"] = wait..  
-00023540: 2020 2020 2020 6a6f 622c 2067 655f 7265        job, ge_re
-00023550: 706f 7274 203d 2073 656c 662e 5f66 6561  port = self._fea
-00023560: 7475 7265 5f67 726f 7570 5f65 6e67 696e  ture_group_engin
-00023570: 652e 696e 7365 7274 280a 2020 2020 2020  e.insert(.      
-00023580: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00023590: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
-000235a0: 6461 7461 6672 616d 653d 6665 6174 7572  dataframe=featur
-000235b0: 655f 6461 7461 6672 616d 652c 0a20 2020  e_dataframe,.   
-000235c0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-000235d0: 7074 696f 6e73 3d77 7269 7465 5f6f 7074  ptions=write_opt
-000235e0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-000235f0: 2020 7661 6c69 6461 7469 6f6e 5f6f 7074    validation_opt
-00023600: 696f 6e73 3d7b 2273 6176 655f 7265 706f  ions={"save_repo
-00023610: 7274 223a 2054 7275 652c 202a 2a76 616c  rt": True, **val
-00023620: 6964 6174 696f 6e5f 6f70 7469 6f6e 737d  idation_options}
-00023630: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00023640: 2020 2020 2069 6620 7361 7665 5f63 6f64       if save_cod
-00023650: 6520 616e 6420 280a 2020 2020 2020 2020  e and (.        
-00023660: 2020 2020 6765 5f72 6570 6f72 7420 6973      ge_report is
-00023670: 204e 6f6e 6520 6f72 2067 655f 7265 706f   None or ge_repo
-00023680: 7274 2e69 6e67 6573 7469 6f6e 5f72 6573  rt.ingestion_res
-00023690: 756c 7420 3d3d 2022 494e 4745 5354 4544  ult == "INGESTED
-000236a0: 220a 2020 2020 2020 2020 293a 0a20 2020  ".        ):.   
-000236b0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-000236c0: 6f64 655f 656e 6769 6e65 2e73 6176 655f  ode_engine.save_
-000236d0: 636f 6465 2873 656c 6629 0a0a 2020 2020  code(self)..    
-000236e0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-000236f0: 6973 7469 6373 5f63 6f6e 6669 672e 656e  istics_config.en
-00023700: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
-00023710: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-00023720: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00023730: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00023740: 2020 2020 2020 2020 2253 7461 7469 7374          "Statist
-00023750: 6963 7320 6172 6520 6e6f 7420 636f 6d70  ics are not comp
-00023760: 7574 6564 2066 6f72 2069 6e73 6572 7469  uted for inserti
-00023770: 6f6e 2074 6f20 6f6e 6c69 6e65 2065 6e61  on to online ena
-00023780: 626c 6564 2065 7874 6572 6e61 6c20 6665  bled external fe
-00023790: 6174 7572 6520 6772 6f75 7020 607b 7d60  ature group `{}`
-000237a0: 2c20 7769 7468 2076 6572 7369 6f6e 220a  , with version".
-000237b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237c0: 2020 2020 2220 607b 7d60 2e20 4361 6c6c      " `{}`. Call
-000237d0: 2060 636f 6d70 7574 655f 7374 6174 6973   `compute_statis
-000237e0: 7469 6373 6020 6578 706c 6963 6974 6c79  tics` explicitly
-000237f0: 2074 6f20 636f 6d70 7574 6520 7374 6174   to compute stat
-00023800: 6973 7469 6373 206f 7665 7220 7468 6520  istics over the 
-00023810: 6461 7461 2069 6e20 7468 6520 6578 7465  data in the exte
-00023820: 726e 616c 2073 746f 7261 6765 2073 7973  rnal storage sys
-00023830: 7465 6d2e 220a 2020 2020 2020 2020 2020  tem.".          
-00023840: 2020 2020 2020 292e 666f 726d 6174 2873        ).format(s
-00023850: 656c 662e 5f6e 616d 652c 2073 656c 662e  elf._name, self.
-00023860: 5f76 6572 7369 6f6e 292c 0a20 2020 2020  _version),.     
-00023870: 2020 2020 2020 2020 2020 2075 7469 6c2e             util.
-00023880: 5374 6f72 6167 6557 6172 6e69 6e67 2c0a  StorageWarning,.
-00023890: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000238a0: 2020 2020 2020 2072 6574 7572 6e20 280a         return (.
-000238b0: 2020 2020 2020 2020 2020 2020 6a6f 622c              job,
-000238c0: 0a20 2020 2020 2020 2020 2020 2067 655f  .            ge_
-000238d0: 7265 706f 7274 2e74 6f5f 6765 5f74 7970  report.to_ge_typ
-000238e0: 6528 2920 6966 2067 655f 7265 706f 7274  e() if ge_report
-000238f0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00023900: 6520 4e6f 6e65 2c0a 2020 2020 2020 2020  e None,.        
-00023910: 290a 0a20 2020 2064 6566 2072 6561 6428  )..    def read(
-00023920: 0a20 2020 2020 2020 2073 656c 662c 2064  .        self, d
-00023930: 6174 6166 7261 6d65 5f74 7970 653a 204f  ataframe_type: O
-00023940: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-00023950: 6465 6661 756c 7422 2c20 6f6e 6c69 6e65  default", online
-00023960: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-00023970: 203d 2046 616c 7365 0a20 2020 2029 3a0a   = False.    ):.
-00023980: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
-00023990: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-000239a0: 2061 7320 6120 4461 7461 4672 616d 652e   as a DataFrame.
-000239b0: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
-000239c0: 616d 706c 650a 2020 2020 2020 2020 2020  ample.          
-000239d0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-000239e0: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
-000239f0: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
-00023a00: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
-00023a10: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
-00023a20: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
-00023a30: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
-00023a40: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
-00023a50: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
-00023a60: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-00023a70: 7572 655f 6772 6f75 7028 2e2e 2e29 0a0a  ure_group(...)..
-00023a80: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-00023a90: 2066 672e 7265 6164 2829 0a20 2020 2020   fg.read().     
-00023aa0: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-00023ab0: 2020 2020 2121 2120 7761 726e 696e 6720      !!! warning 
-00023ac0: 2245 6e67 696e 6520 5375 7070 6f72 7422  "Engine Support"
-00023ad0: 0a20 2020 2020 2020 2020 2020 202a 2a53  .            **S
-00023ae0: 7061 726b 206f 6e6c 792a 2a0a 0a20 2020  park only**..   
-00023af0: 2020 2020 2020 2020 2052 6561 6469 6e67           Reading
-00023b00: 2061 6e20 4578 7465 726e 616c 2046 6561   an External Fea
-00023b10: 7475 7265 2047 726f 7570 2064 6972 6563  ture Group direc
-00023b20: 746c 7920 696e 746f 2061 2050 616e 6461  tly into a Panda
-00023b30: 7320 4461 7461 6672 616d 6520 7573 696e  s Dataframe usin
-00023b40: 670a 2020 2020 2020 2020 2020 2020 5079  g.            Py
-00023b50: 7468 6f6e 2f50 616e 6461 7320 6173 2045  thon/Pandas as E
-00023b60: 6e67 696e 6520 6973 206e 6f74 2073 7570  ngine is not sup
-00023b70: 706f 7274 6564 2c20 686f 7765 7665 722c  ported, however,
-00023b80: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00023b90: 0a20 2020 2020 2020 2020 2020 2051 7565  .            Que
-00023ba0: 7279 2041 5049 2074 6f20 6372 6561 7465  ry API to create
-00023bb0: 2046 6561 7475 7265 2056 6965 7773 2f54   Feature Views/T
-00023bc0: 7261 696e 696e 6720 4461 7461 2063 6f6e  raining Data con
-00023bd0: 7461 696e 696e 6720 4578 7465 726e 616c  taining External
-00023be0: 0a20 2020 2020 2020 2020 2020 2046 6561  .            Fea
-00023bf0: 7475 7265 2047 726f 7570 732e 0a0a 2020  ture Groups...  
-00023c00: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
-00023c10: 730a 2020 2020 2020 2020 2020 2020 6461  s.            da
-00023c20: 7461 6672 616d 655f 7479 7065 3a20 7374  taframe_type: st
-00023c30: 722c 206f 7074 696f 6e61 6c2e 2050 6f73  r, optional. Pos
-00023c40: 7369 626c 6520 7661 6c75 6573 2061 7265  sible values are
-00023c50: 2060 2264 6566 6175 6c74 2260 2c20 6022   `"default"`, `"
-00023c60: 7370 6172 6b22 602c 0a20 2020 2020 2020  spark"`,.       
-00023c70: 2020 2020 2020 2020 2060 2270 616e 6461           `"panda
-00023c80: 7322 602c 2060 226e 756d 7079 2260 206f  s"`, `"numpy"` o
-00023c90: 7220 6022 7079 7468 6f6e 2260 2c20 6465  r `"python"`, de
-00023ca0: 6661 756c 7473 2074 6f20 6022 6465 6661  faults to `"defa
-00023cb0: 756c 7422 602e 0a20 2020 2020 2020 2020  ult"`..         
-00023cc0: 2020 206f 6e6c 696e 653a 2062 6f6f 6c2c     online: bool,
-00023cd0: 206f 7074 696f 6e61 6c2e 2049 6620 6054   optional. If `T
-00023ce0: 7275 6560 2072 6561 6420 6672 6f6d 206f  rue` read from o
-00023cf0: 6e6c 696e 6520 6665 6174 7572 6520 7374  nline feature st
-00023d00: 6f72 652c 2064 6566 6175 6c74 730a 2020  ore, defaults.  
-00023d10: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00023d20: 2060 4661 6c73 6560 2e0a 0a20 2020 2020   `False`...     
-00023d30: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-00023d40: 2020 2020 2020 2020 2060 4461 7461 4672           `DataFr
-00023d50: 616d 6560 3a20 5468 6520 7370 6172 6b20  ame`: The spark 
-00023d60: 6461 7461 6672 616d 6520 636f 6e74 6169  dataframe contai
-00023d70: 6e69 6e67 2074 6865 2066 6561 7475 7265  ning the feature
-00023d80: 2064 6174 612e 0a20 2020 2020 2020 2020   data..         
-00023d90: 2020 2060 7079 7370 6172 6b2e 4461 7461     `pyspark.Data
-00023da0: 4672 616d 6560 2e20 4120 5370 6172 6b20  Frame`. A Spark 
-00023db0: 4461 7461 4672 616d 652e 0a20 2020 2020  DataFrame..     
-00023dc0: 2020 2020 2020 2060 7061 6e64 6173 2e44         `pandas.D
-00023dd0: 6174 6146 7261 6d65 602e 2041 2050 616e  ataFrame`. A Pan
-00023de0: 6461 7320 4461 7461 4672 616d 652e 0a20  das DataFrame.. 
-00023df0: 2020 2020 2020 2020 2020 2060 6e75 6d70             `nump
-00023e00: 792e 6e64 6172 7261 7960 2e20 4120 7477  y.ndarray`. A tw
-00023e10: 6f2d 6469 6d65 6e73 696f 6e61 6c20 4e75  o-dimensional Nu
-00023e20: 6d70 7920 6172 7261 792e 0a20 2020 2020  mpy array..     
-00023e30: 2020 2020 2020 2060 6c69 7374 602e 2041         `list`. A
-00023e40: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
-00023e50: 2050 7974 686f 6e20 6c69 7374 2e0a 0a20   Python list... 
-00023e60: 2020 2020 2020 2023 2052 6169 7365 730a         # Raises.
-00023e70: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
-00023e80: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
-00023e90: 6f6e 732e 5265 7374 4150 4945 7272 6f72  ons.RestAPIError
-00023ea0: 602e 0a20 2020 2020 2020 2022 2222 0a0a  `..        """..
-00023eb0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-00023ec0: 2020 2020 2020 2020 2065 6e67 696e 652e           engine.
-00023ed0: 6765 745f 7479 7065 2829 203d 3d20 2270  get_type() == "p
-00023ee0: 7974 686f 6e22 0a20 2020 2020 2020 2020  ython".         
-00023ef0: 2020 2061 6e64 206e 6f74 206f 6e6c 696e     and not onlin
-00023f00: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
-00023f10: 6420 6e6f 7420 656e 6769 6e65 2e67 6574  d not engine.get
-00023f20: 5f69 6e73 7461 6e63 6528 292e 6973 5f66  _instance().is_f
-00023f30: 6c79 696e 6764 7563 6b5f 7175 6572 795f  lyingduck_query_
-00023f40: 7375 7070 6f72 7465 6428 0a20 2020 2020  supported(.     
-00023f50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00023f60: 7365 6c65 6374 5f61 6c6c 2829 0a20 2020  select_all().   
-00023f70: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00023f80: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00023f90: 2020 7261 6973 6520 4665 6174 7572 6553    raise FeatureS
-00023fa0: 746f 7265 4578 6365 7074 696f 6e28 0a20  toreException(. 
-00023fb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00023fc0: 5265 6164 696e 6720 616e 2045 7874 6572  Reading an Exter
-00023fd0: 6e61 6c20 4665 6174 7572 6520 4772 6f75  nal Feature Grou
-00023fe0: 7020 6469 7265 6374 6c79 2069 6e74 6f20  p directly into 
-00023ff0: 6120 5061 6e64 6173 2044 6174 6166 7261  a Pandas Datafra
-00024000: 6d65 2075 7369 6e67 2022 0a20 2020 2020  me using ".     
-00024010: 2020 2020 2020 2020 2020 202b 2022 5079             + "Py
-00024020: 7468 6f6e 2f50 616e 6461 7320 6173 2045  thon/Pandas as E
-00024030: 6e67 696e 6520 6672 6f6d 2074 6865 2065  ngine from the e
-00024040: 7874 6572 6e61 6c20 7374 6f72 6167 6520  xternal storage 
-00024050: 7379 7374 656d 2022 0a20 2020 2020 2020  system ".       
-00024060: 2020 2020 2020 2020 202b 2022 6973 206e           + "is n
-00024070: 6f74 2073 7570 706f 7274 6564 2c20 686f  ot supported, ho
-00024080: 7765 7665 722c 2069 6620 7468 6520 6665  wever, if the fe
-00024090: 6174 7572 6520 6772 6f75 7020 6973 206f  ature group is o
-000240a0: 6e6c 696e 6520 656e 6162 6c65 642c 2079  nline enabled, y
-000240b0: 6f75 2063 616e 2072 6561 6420 220a 2020  ou can read ".  
-000240c0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000240d0: 2266 726f 6d20 6f6e 6c69 6e65 2073 746f  "from online sto
-000240e0: 7261 6765 206f 7220 796f 7520 6361 6e20  rage or you can 
-000240f0: 7573 6520 7468 6520 220a 2020 2020 2020  use the ".      
-00024100: 2020 2020 2020 2020 2020 2b20 2251 7565            + "Que
-00024110: 7279 2041 5049 2074 6f20 6372 6561 7465  ry API to create
-00024120: 2046 6561 7475 7265 2056 6965 7773 2f54   Feature Views/T
-00024130: 7261 696e 696e 6720 4461 7461 2063 6f6e  raining Data con
-00024140: 7461 696e 696e 6720 4578 7465 726e 616c  taining External
-00024150: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00024160: 2020 202b 2022 4665 6174 7572 6520 4772     + "Feature Gr
-00024170: 6f75 7073 2e22 0a20 2020 2020 2020 2020  oups.".         
-00024180: 2020 2029 0a20 2020 2020 2020 2065 6e67     ).        eng
-00024190: 696e 652e 6765 745f 696e 7374 616e 6365  ine.get_instance
-000241a0: 2829 2e73 6574 5f6a 6f62 5f67 726f 7570  ().set_job_group
-000241b0: 280a 2020 2020 2020 2020 2020 2020 2246  (.            "F
-000241c0: 6574 6368 696e 6720 4665 6174 7572 6520  etching Feature 
-000241d0: 6772 6f75 7022 2c0a 2020 2020 2020 2020  group",.        
-000241e0: 2020 2020 2247 6574 7469 6e67 2066 6561      "Getting fea
-000241f0: 7475 7265 2067 726f 7570 3a20 7b7d 2066  ture group: {} f
-00024200: 726f 6d20 7468 6520 6665 6174 7572 6573  rom the features
-00024210: 746f 7265 207b 7d22 2e66 6f72 6d61 7428  tore {}".format(
-00024220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024230: 2073 656c 662e 5f6e 616d 652c 2073 656c   self._name, sel
-00024240: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
-00024250: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00024260: 2020 292c 0a20 2020 2020 2020 2029 0a20    ),.        ). 
-00024270: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00024280: 6c66 2e73 656c 6563 745f 616c 6c28 292e  lf.select_all().
-00024290: 7265 6164 2864 6174 6166 7261 6d65 5f74  read(dataframe_t
-000242a0: 7970 653d 6461 7461 6672 616d 655f 7479  ype=dataframe_ty
-000242b0: 7065 2c20 6f6e 6c69 6e65 3d6f 6e6c 696e  pe, online=onlin
-000242c0: 6529 0a0a 2020 2020 6465 6620 7368 6f77  e)..    def show
-000242d0: 2873 656c 662c 206e 293a 0a20 2020 2020  (self, n):.     
-000242e0: 2020 2022 2222 5368 6f77 2074 6865 2066     """Show the f
-000242f0: 6972 7374 206e 2072 6f77 7320 6f66 2074  irst n rows of t
-00024300: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00024310: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-00024320: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-00024330: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00024340: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
-00024350: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
-00024360: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
-00024370: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
-00024380: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-00024390: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
-000243a0: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
-000243b0: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
-000243c0: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-000243d0: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
-000243e0: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-000243f0: 7368 6f77 2835 290a 2020 2020 2020 2020  show(5).        
-00024400: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00024410: 2222 220a 2020 2020 2020 2020 656e 6769  """.        engi
-00024420: 6e65 2e67 6574 5f69 6e73 7461 6e63 6528  ne.get_instance(
-00024430: 292e 7365 745f 6a6f 625f 6772 6f75 7028  ).set_job_group(
-00024440: 0a20 2020 2020 2020 2020 2020 2022 4665  .            "Fe
-00024450: 7463 6869 6e67 2046 6561 7475 7265 2067  tching Feature g
-00024460: 726f 7570 222c 0a20 2020 2020 2020 2020  roup",.         
-00024470: 2020 2022 4765 7474 696e 6720 6665 6174     "Getting feat
-00024480: 7572 6520 6772 6f75 703a 207b 7d20 6672  ure group: {} fr
-00024490: 6f6d 2074 6865 2066 6561 7475 7265 7374  om the featurest
-000244a0: 6f72 6520 7b7d 222e 666f 726d 6174 280a  ore {}".format(.
-000244b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000244c0: 7365 6c66 2e5f 6e61 6d65 2c20 7365 6c66  self._name, self
-000244d0: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
-000244e0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-000244f0: 2029 2c0a 2020 2020 2020 2020 290a 2020   ),.        ).  
-00024500: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00024510: 662e 7365 6c65 6374 5f61 6c6c 2829 2e73  f.select_all().s
-00024520: 686f 7728 6e29 0a0a 2020 2020 4063 6c61  how(n)..    @cla
-00024530: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00024540: 2066 726f 6d5f 7265 7370 6f6e 7365 5f6a   from_response_j
-00024550: 736f 6e28 636c 732c 206a 736f 6e5f 6469  son(cls, json_di
-00024560: 6374 293a 0a20 2020 2020 2020 206a 736f  ct):.        jso
-00024570: 6e5f 6465 6361 6d65 6c69 7a65 6420 3d20  n_decamelized = 
-00024580: 6875 6d70 732e 6465 6361 6d65 6c69 7a65  humps.decamelize
-00024590: 286a 736f 6e5f 6469 6374 290a 2020 2020  (json_dict).    
-000245a0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000245b0: 6528 6a73 6f6e 5f64 6563 616d 656c 697a  e(json_decameliz
-000245c0: 6564 2c20 6469 6374 293a 0a20 2020 2020  ed, dict):.     
-000245d0: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
-000245e0: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
-000245f0: 2274 7970 6522 2c20 4e6f 6e65 290a 2020  "type", None).  
-00024600: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00024610: 2063 6c73 282a 2a6a 736f 6e5f 6465 6361   cls(**json_deca
-00024620: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
-00024630: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
-00024640: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
-00024650: 2020 2020 2020 2020 205f 203d 2066 672e           _ = fg.
-00024660: 706f 7028 2274 7970 6522 2c20 4e6f 6e65  pop("type", None
-00024670: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00024680: 205b 636c 7328 2a2a 6667 2920 666f 7220   [cls(**fg) for 
-00024690: 6667 2069 6e20 6a73 6f6e 5f64 6563 616d  fg in json_decam
-000246a0: 656c 697a 6564 5d0a 0a20 2020 2064 6566  elized]..    def
-000246b0: 2075 7064 6174 655f 6672 6f6d 5f72 6573   update_from_res
-000246c0: 706f 6e73 655f 6a73 6f6e 2873 656c 662c  ponse_json(self,
-000246d0: 206a 736f 6e5f 6469 6374 293a 0a20 2020   json_dict):.   
-000246e0: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
-000246f0: 6c69 7a65 6420 3d20 6875 6d70 732e 6465  lized = humps.de
-00024700: 6361 6d65 6c69 7a65 286a 736f 6e5f 6469  camelize(json_di
-00024710: 6374 290a 2020 2020 2020 2020 6966 2022  ct).        if "
-00024720: 7479 7065 2220 696e 206a 736f 6e5f 6465  type" in json_de
-00024730: 6361 6d65 6c69 7a65 643a 0a20 2020 2020  camelized:.     
-00024740: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
-00024750: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
-00024760: 2274 7970 6522 290a 2020 2020 2020 2020  "type").        
-00024770: 7365 6c66 2e5f 5f69 6e69 745f 5f28 2a2a  self.__init__(**
-00024780: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00024790: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000247a0: 2073 656c 660a 0a20 2020 2064 6566 206a   self..    def j
-000247b0: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
-000247c0: 2020 2072 6574 7572 6e20 6a73 6f6e 2e64     return json.d
-000247d0: 756d 7073 2873 656c 662c 2063 6c73 3d75  umps(self, cls=u
-000247e0: 7469 6c2e 4665 6174 7572 6553 746f 7265  til.FeatureStore
-000247f0: 456e 636f 6465 7229 0a0a 2020 2020 6465  Encoder)..    de
-00024800: 6620 746f 5f64 6963 7428 7365 6c66 293a  f to_dict(self):
-00024810: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00024820: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-00024830: 6422 3a20 7365 6c66 2e5f 6964 2c0a 2020  d": self._id,.  
-00024840: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00024850: 3a20 7365 6c66 2e5f 6e61 6d65 2c0a 2020  : self._name,.  
-00024860: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00024870: 6970 7469 6f6e 223a 2073 656c 662e 5f64  iption": self._d
-00024880: 6573 6372 6970 7469 6f6e 2c0a 2020 2020  escription,.    
-00024890: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-000248a0: 223a 2073 656c 662e 5f76 6572 7369 6f6e  ": self._version
-000248b0: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
-000248c0: 6561 7475 7265 7322 3a20 7365 6c66 2e5f  eatures": self._
-000248d0: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
-000248e0: 2020 2020 2020 2266 6561 7475 7265 7374        "featurest
-000248f0: 6f72 6549 6422 3a20 7365 6c66 2e5f 6665  oreId": self._fe
-00024900: 6174 7572 655f 7374 6f72 655f 6964 2c0a  ature_store_id,.
-00024910: 2020 2020 2020 2020 2020 2020 2271 7565              "que
-00024920: 7279 223a 2073 656c 662e 5f71 7565 7279  ry": self._query
-00024930: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-00024940: 6174 6146 6f72 6d61 7422 3a20 7365 6c66  ataFormat": self
-00024950: 2e5f 6461 7461 5f66 6f72 6d61 742c 0a20  ._data_format,. 
-00024960: 2020 2020 2020 2020 2020 2022 7061 7468             "path
-00024970: 223a 2073 656c 662e 5f70 6174 682c 0a20  ": self._path,. 
-00024980: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
-00024990: 6f6e 7322 3a20 5b7b 226e 616d 6522 3a20  ons": [{"name": 
-000249a0: 6b2c 2022 7661 6c75 6522 3a20 767d 2066  k, "value": v} f
-000249b0: 6f72 206b 2c20 7620 696e 2073 656c 662e  or k, v in self.
-000249c0: 5f6f 7074 696f 6e73 2e69 7465 6d73 2829  _options.items()
-000249d0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-000249e0: 2073 656c 662e 5f6f 7074 696f 6e73 0a20   self._options. 
-000249f0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00024a00: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00024a10: 2020 2273 746f 7261 6765 436f 6e6e 6563    "storageConnec
-00024a20: 746f 7222 3a20 7365 6c66 2e5f 7374 6f72  tor": self._stor
-00024a30: 6167 655f 636f 6e6e 6563 746f 722e 746f  age_connector.to
-00024a40: 5f64 6963 7428 292c 0a20 2020 2020 2020  _dict(),.       
-00024a50: 2020 2020 2022 7479 7065 223a 2022 6f6e       "type": "on
-00024a60: 4465 6d61 6e64 4665 6174 7572 6567 726f  DemandFeaturegro
-00024a70: 7570 4454 4f22 2c0a 2020 2020 2020 2020  upDTO",.        
-00024a80: 2020 2020 2273 7461 7469 7374 6963 7343      "statisticsC
-00024a90: 6f6e 6669 6722 3a20 7365 6c66 2e5f 7374  onfig": self._st
-00024aa0: 6174 6973 7469 6373 5f63 6f6e 6669 672c  atistics_config,
-00024ab0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-00024ac0: 656e 7454 696d 6522 3a20 7365 6c66 2e5f  entTime": self._
-00024ad0: 6576 656e 745f 7469 6d65 2c0a 2020 2020  event_time,.    
-00024ae0: 2020 2020 2020 2020 2265 7870 6563 7461          "expecta
-00024af0: 7469 6f6e 5375 6974 6522 3a20 7365 6c66  tionSuite": self
-00024b00: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
-00024b10: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-00024b20: 2022 6f6e 6c69 6e65 456e 6162 6c65 6422   "onlineEnabled"
-00024b30: 3a20 7365 6c66 2e5f 6f6e 6c69 6e65 5f65  : self._online_e
-00024b40: 6e61 626c 6564 2c0a 2020 2020 2020 2020  nabled,.        
-00024b50: 2020 2020 2273 7069 6e65 223a 2046 616c      "spine": Fal
-00024b60: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00024b70: 2274 6f70 6963 4e61 6d65 223a 2073 656c  "topicName": sel
-00024b80: 662e 746f 7069 635f 6e61 6d65 2c0a 2020  f.topic_name,.  
-00024b90: 2020 2020 2020 2020 2020 226e 6f74 6966            "notif
-00024ba0: 6963 6174 696f 6e54 6f70 6963 4e61 6d65  icationTopicName
-00024bb0: 223a 2073 656c 662e 6e6f 7469 6669 6361  ": self.notifica
-00024bc0: 7469 6f6e 5f74 6f70 6963 5f6e 616d 652c  tion_topic_name,
-00024bd0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00024be0: 7072 6563 6174 6564 223a 2073 656c 662e  precated": self.
-00024bf0: 6465 7072 6563 6174 6564 2c0a 2020 2020  deprecated,.    
-00024c00: 2020 2020 7d0a 0a20 2020 2040 7072 6f70      }..    @prop
-00024c10: 6572 7479 0a20 2020 2064 6566 2069 6428  erty.    def id(
-00024c20: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00024c30: 6574 7572 6e20 7365 6c66 2e5f 6964 0a0a  eturn self._id..
-00024c40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00024c50: 2020 6465 6620 6465 7363 7269 7074 696f    def descriptio
-00024c60: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00024c70: 2072 6574 7572 6e20 7365 6c66 2e5f 6465   return self._de
-00024c80: 7363 7269 7074 696f 6e0a 0a20 2020 2040  scription..    @
-00024c90: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00024ca0: 2071 7565 7279 2873 656c 6629 3a0a 2020   query(self):.  
-00024cb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00024cc0: 662e 5f71 7565 7279 0a0a 2020 2020 4070  f._query..    @p
-00024cd0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00024ce0: 6461 7461 5f66 6f72 6d61 7428 7365 6c66  data_format(self
-00024cf0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00024d00: 6e20 7365 6c66 2e5f 6461 7461 5f66 6f72  n self._data_for
-00024d10: 6d61 740a 0a20 2020 2040 7072 6f70 6572  mat..    @proper
-00024d20: 7479 0a20 2020 2064 6566 2070 6174 6828  ty.    def path(
-00024d30: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00024d40: 6574 7572 6e20 7365 6c66 2e5f 7061 7468  eturn self._path
-00024d50: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00024d60: 2020 2020 6465 6620 6f70 7469 6f6e 7328      def options(
-00024d70: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00024d80: 6574 7572 6e20 7365 6c66 2e5f 6f70 7469  eturn self._opti
-00024d90: 6f6e 730a 0a20 2020 2040 7072 6f70 6572  ons..    @proper
-00024da0: 7479 0a20 2020 2064 6566 2073 746f 7261  ty.    def stora
-00024db0: 6765 5f63 6f6e 6e65 6374 6f72 2873 656c  ge_connector(sel
-00024dc0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00024dd0: 726e 2073 656c 662e 5f73 746f 7261 6765  rn self._storage
-00024de0: 5f63 6f6e 6e65 6374 6f72 0a0a 2020 2020  _connector..    
-00024df0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00024e00: 6620 6372 6561 746f 7228 7365 6c66 293a  f creator(self):
-00024e10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00024e20: 7365 6c66 2e5f 6372 6561 746f 720a 0a20  self._creator.. 
-00024e30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00024e40: 2064 6566 2063 7265 6174 6564 2873 656c   def created(sel
-00024e50: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00024e60: 726e 2073 656c 662e 5f63 7265 6174 6564  rn self._created
-00024e70: 0a0a 2020 2020 4064 6573 6372 6970 7469  ..    @descripti
-00024e80: 6f6e 2e73 6574 7465 720a 2020 2020 6465  on.setter.    de
-00024e90: 6620 6465 7363 7269 7074 696f 6e28 7365  f description(se
-00024ea0: 6c66 2c20 6e65 775f 6465 7363 7269 7074  lf, new_descript
-00024eb0: 696f 6e29 3a0a 2020 2020 2020 2020 7365  ion):.        se
-00024ec0: 6c66 2e5f 6465 7363 7269 7074 696f 6e20  lf._description 
-00024ed0: 3d20 6e65 775f 6465 7363 7269 7074 696f  = new_descriptio
-00024ee0: 6e0a 0a20 2020 2040 7072 6f70 6572 7479  n..    @property
-00024ef0: 0a20 2020 2064 6566 2066 6561 7475 7265  .    def feature
-00024f00: 5f73 746f 7265 5f6e 616d 6528 7365 6c66  _store_name(self
-00024f10: 293a 0a20 2020 2020 2020 2022 2222 4e61  ):.        """Na
-00024f20: 6d65 206f 6620 7468 6520 6665 6174 7572  me of the featur
-00024f30: 6520 7374 6f72 6520 696e 2077 6869 6368  e store in which
-00024f40: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00024f50: 7570 2069 7320 6c6f 6361 7465 642e 2222  up is located.""
-00024f60: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00024f70: 2073 656c 662e 5f66 6561 7475 7265 5f73   self._feature_s
-00024f80: 746f 7265 5f6e 616d 650a 0a0a 636c 6173  tore_name...clas
-00024f90: 7320 5370 696e 6547 726f 7570 2846 6561  s SpineGroup(Fea
-00024fa0: 7475 7265 4772 6f75 7042 6173 6529 3a0a  tureGroupBase):.
-00024fb0: 2020 2020 5350 494e 455f 4752 4f55 5020      SPINE_GROUP 
-00024fc0: 3d20 224f 4e5f 4445 4d41 4e44 5f46 4541  = "ON_DEMAND_FEA
-00024fd0: 5455 5245 5f47 524f 5550 220a 2020 2020  TURE_GROUP".    
-00024fe0: 454e 5449 5459 5f54 5950 4520 3d20 2266  ENTITY_TYPE = "f
-00024ff0: 6561 7475 7265 6772 6f75 7073 220a 0a20  eaturegroups".. 
-00025000: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00025010: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00025020: 2020 2020 2020 2073 746f 7261 6765 5f63         storage_c
-00025030: 6f6e 6e65 6374 6f72 3d4e 6f6e 652c 0a20  onnector=None,. 
-00025040: 2020 2020 2020 2071 7565 7279 3d4e 6f6e         query=Non
-00025050: 652c 0a20 2020 2020 2020 2064 6174 615f  e,.        data_
-00025060: 666f 726d 6174 3d4e 6f6e 652c 0a20 2020  format=None,.   
-00025070: 2020 2020 2070 6174 683d 4e6f 6e65 2c0a       path=None,.
-00025080: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
-00025090: 7b7d 2c0a 2020 2020 2020 2020 6e61 6d65  {},.        name
-000250a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2076  =None,.        v
-000250b0: 6572 7369 6f6e 3d4e 6f6e 652c 0a20 2020  ersion=None,.   
-000250c0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000250d0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2070  =None,.        p
-000250e0: 7269 6d61 7279 5f6b 6579 3d4e 6f6e 652c  rimary_key=None,
-000250f0: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
-00025100: 7374 6f72 655f 6964 3d4e 6f6e 652c 0a20  store_id=None,. 
-00025110: 2020 2020 2020 2066 6561 7475 7265 7374         featurest
-00025120: 6f72 655f 6e61 6d65 3d4e 6f6e 652c 0a20  ore_name=None,. 
-00025130: 2020 2020 2020 2063 7265 6174 6564 3d4e         created=N
-00025140: 6f6e 652c 0a20 2020 2020 2020 2063 7265  one,.        cre
-00025150: 6174 6f72 3d4e 6f6e 652c 0a20 2020 2020  ator=None,.     
-00025160: 2020 2069 643d 4e6f 6e65 2c0a 2020 2020     id=None,.    
-00025170: 2020 2020 6665 6174 7572 6573 3d4e 6f6e      features=Non
-00025180: 652c 0a20 2020 2020 2020 206c 6f63 6174  e,.        locat
-00025190: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
-000251a0: 2020 7374 6174 6973 7469 6373 5f63 6f6e    statistics_con
-000251b0: 6669 673d 4e6f 6e65 2c0a 2020 2020 2020  fig=None,.      
-000251c0: 2020 6576 656e 745f 7469 6d65 3d4e 6f6e    event_time=Non
-000251d0: 652c 0a20 2020 2020 2020 2065 7870 6563  e,.        expec
-000251e0: 7461 7469 6f6e 5f73 7569 7465 3d4e 6f6e  tation_suite=Non
-000251f0: 652c 0a20 2020 2020 2020 206f 6e6c 696e  e,.        onlin
-00025200: 655f 656e 6162 6c65 643d 4661 6c73 652c  e_enabled=False,
-00025210: 0a20 2020 2020 2020 2068 7265 663d 4e6f  .        href=No
-00025220: 6e65 2c0a 2020 2020 2020 2020 6f6e 6c69  ne,.        onli
-00025230: 6e65 5f74 6f70 6963 5f6e 616d 653d 4e6f  ne_topic_name=No
-00025240: 6e65 2c0a 2020 2020 2020 2020 746f 7069  ne,.        topi
-00025250: 635f 6e61 6d65 3d4e 6f6e 652c 0a20 2020  c_name=None,.   
-00025260: 2020 2020 2073 7069 6e65 3d54 7275 652c       spine=True,
-00025270: 0a20 2020 2020 2020 2064 6174 6166 7261  .        datafra
-00025280: 6d65 3d22 7370 696e 6522 2c0a 2020 2020  me="spine",.    
-00025290: 2020 2020 6465 7072 6563 6174 6564 3d46      deprecated=F
-000252a0: 616c 7365 2c0a 2020 2020 2020 2020 2a2a  alse,.        **
-000252b0: 6b77 6172 6773 2c0a 2020 2020 293a 0a20  kwargs,.    ):. 
-000252c0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-000252d0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000252e0: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
-000252f0: 2020 2020 2020 2076 6572 7369 6f6e 2c0a         version,.
-00025300: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00025310: 7572 6573 746f 7265 5f69 642c 0a20 2020  urestore_id,.   
-00025320: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
-00025330: 6e2c 0a20 2020 2020 2020 2020 2020 2065  n,.            e
-00025340: 7665 6e74 5f74 696d 653d 6576 656e 745f  vent_time=event_
-00025350: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
-00025360: 2020 6f6e 6c69 6e65 5f65 6e61 626c 6564    online_enabled
-00025370: 3d6f 6e6c 696e 655f 656e 6162 6c65 642c  =online_enabled,
-00025380: 0a20 2020 2020 2020 2020 2020 2069 643d  .            id=
-00025390: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-000253a0: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-000253b0: 653d 6578 7065 6374 6174 696f 6e5f 7375  e=expectation_su
-000253c0: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-000253d0: 206f 6e6c 696e 655f 746f 7069 635f 6e61   online_topic_na
-000253e0: 6d65 3d6f 6e6c 696e 655f 746f 7069 635f  me=online_topic_
-000253f0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00025400: 2020 746f 7069 635f 6e61 6d65 3d74 6f70    topic_name=top
-00025410: 6963 5f6e 616d 652c 0a20 2020 2020 2020  ic_name,.       
-00025420: 2020 2020 2064 6570 7265 6361 7465 643d       deprecated=
-00025430: 6465 7072 6563 6174 6564 2c0a 2020 2020  deprecated,.    
-00025440: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
-00025450: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
-00025460: 7265 5f6e 616d 6520 3d20 6665 6174 7572  re_name = featur
-00025470: 6573 746f 7265 5f6e 616d 650a 2020 2020  estore_name.    
-00025480: 2020 2020 7365 6c66 2e5f 6465 7363 7269      self._descri
-00025490: 7074 696f 6e20 3d20 6465 7363 7269 7074  ption = descript
-000254a0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
-000254b0: 2e5f 6372 6561 7465 6420 3d20 6372 6561  ._created = crea
-000254c0: 7465 640a 2020 2020 2020 2020 7365 6c66  ted.        self
-000254d0: 2e5f 6372 6561 746f 7220 3d20 7573 6572  ._creator = user
-000254e0: 2e55 7365 722e 6672 6f6d 5f72 6573 706f  .User.from_respo
-000254f0: 6e73 655f 6a73 6f6e 2863 7265 6174 6f72  nse_json(creator
-00025500: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00025510: 5f66 6561 7475 7265 7320 3d20 5b0a 2020  _features = [.  
-00025520: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00025530: 652e 4665 6174 7572 652e 6672 6f6d 5f72  e.Feature.from_r
-00025540: 6573 706f 6e73 655f 6a73 6f6e 2866 6561  esponse_json(fea
-00025550: 7429 2069 6620 6973 696e 7374 616e 6365  t) if isinstance
-00025560: 2866 6561 742c 2064 6963 7429 2065 6c73  (feat, dict) els
-00025570: 6520 6665 6174 0a20 2020 2020 2020 2020  e feat.         
-00025580: 2020 2066 6f72 2066 6561 7420 696e 2028     for feat in (
-00025590: 6665 6174 7572 6573 206f 7220 5b5d 290a  features or []).
-000255a0: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
-000255b0: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
-000255c0: 5f67 726f 7570 5f65 6e67 696e 6520 3d20  _group_engine = 
-000255d0: 7370 696e 655f 6772 6f75 705f 656e 6769  spine_group_engi
-000255e0: 6e65 2e53 7069 6e65 4772 6f75 7045 6e67  ne.SpineGroupEng
-000255f0: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
-00025600: 2066 6561 7475 7265 7374 6f72 655f 6964   featurestore_id
-00025610: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00025620: 2020 2020 6966 2073 656c 662e 5f69 643a      if self._id:
-00025630: 0a20 2020 2020 2020 2020 2020 2023 2047  .            # G
-00025640: 6f74 2066 726f 6d20 486f 7073 776f 726b  ot from Hopswork
-00025650: 732c 2064 6573 6572 6961 6c69 7a65 2066  s, deserialize f
-00025660: 6561 7475 7265 7320 616e 6420 7374 6f72  eatures and stor
-00025670: 6167 6520 636f 6e6e 6563 746f 720a 2020  age connector.  
-00025680: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00025690: 6665 6174 7572 6573 203d 2028 0a20 2020  features = (.   
-000256a0: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
-000256b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256c0: 2020 2066 6561 7475 7265 2e46 6561 7475     feature.Featu
-000256d0: 7265 2e66 726f 6d5f 7265 7370 6f6e 7365  re.from_response
-000256e0: 5f6a 736f 6e28 6665 6174 290a 2020 2020  _json(feat).    
-000256f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025700: 6966 2069 7369 6e73 7461 6e63 6528 6665  if isinstance(fe
-00025710: 6174 2c20 6469 6374 290a 2020 2020 2020  at, dict).      
-00025720: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00025730: 7365 2066 6561 740a 2020 2020 2020 2020  se feat.        
-00025740: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00025750: 6665 6174 2069 6e20 6665 6174 7572 6573  feat in features
-00025760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025770: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-00025780: 2020 2069 6620 6665 6174 7572 6573 0a20     if features. 
-00025790: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000257a0: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
-000257b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000257c0: 2020 2073 656c 662e 7072 696d 6172 795f     self.primary_
-000257d0: 6b65 7920 3d20 280a 2020 2020 2020 2020  key = (.        
-000257e0: 2020 2020 2020 2020 5b66 6561 742e 6e61          [feat.na
-000257f0: 6d65 2066 6f72 2066 6561 7420 696e 2073  me for feat in s
-00025800: 656c 662e 5f66 6561 7475 7265 7320 6966  elf._features if
-00025810: 2066 6561 742e 7072 696d 6172 7920 6973   feat.primary is
-00025820: 2054 7275 655d 0a20 2020 2020 2020 2020   True].         
-00025830: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00025840: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
-00025850: 2020 2020 2020 2020 2065 6c73 6520 5b5d           else []
-00025860: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00025870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00025880: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-00025890: 6720 3d20 7374 6174 6973 7469 6373 5f63  g = statistics_c
-000258a0: 6f6e 6669 670a 2020 2020 2020 2020 656c  onfig.        el
-000258b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000258c0: 7365 6c66 2e70 7269 6d61 7279 5f6b 6579  self.primary_key
-000258d0: 203d 2070 7269 6d61 7279 5f6b 6579 0a20   = primary_key. 
-000258e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000258f0: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-00025900: 6720 3d20 7374 6174 6973 7469 6373 5f63  g = statistics_c
-00025910: 6f6e 6669 670a 2020 2020 2020 2020 2020  onfig.          
-00025920: 2020 7365 6c66 2e5f 6665 6174 7572 6573    self._features
-00025930: 203d 2066 6561 7475 7265 730a 0a20 2020   = features..   
-00025940: 2020 2020 2073 656c 662e 5f68 7265 6620       self._href 
-00025950: 3d20 6872 6566 0a0a 2020 2020 2020 2020  = href..        
-00025960: 2320 6861 7320 746f 2068 6170 7065 6e20  # has to happen 
-00025970: 6c61 7374 202d 3e20 6665 6174 7572 6573  last -> features
-00025980: 2061 6e64 2069 6420 6172 6520 6e65 6564   and id are need
-00025990: 6564 2066 6f72 2073 6368 656d 6120 7665  ed for schema ve
-000259a0: 7269 6669 6361 7469 6f6e 0a20 2020 2020  rification.     
-000259b0: 2020 2023 2075 7365 2073 6574 7465 7220     # use setter 
-000259c0: 746f 2063 6f6e 7665 7274 2074 6f20 6465  to convert to de
-000259d0: 6661 756c 7420 6461 7461 6672 616d 6520  fault dataframe 
-000259e0: 7479 7065 2066 6f72 2065 6e67 696e 650a  type for engine.
-000259f0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
-00025a00: 6166 7261 6d65 203d 2064 6174 6166 7261  aframe = datafra
-00025a10: 6d65 0a0a 2020 2020 6465 6620 5f73 6176  me..    def _sav
-00025a20: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00025a30: 2022 2222 5065 7273 6973 7420 7468 6520   """Persist the 
-00025a40: 6d65 7461 6461 7461 2066 6f72 2074 6869  metadata for thi
-00025a50: 7320 7370 696e 6520 6772 6f75 702e 0a0a  s spine group...
-00025a60: 2020 2020 2020 2020 5769 7468 6f75 7420          Without 
-00025a70: 6361 6c6c 696e 6720 7468 6973 206d 6574  calling this met
-00025a80: 686f 642c 2079 6f75 7220 6665 6174 7572  hod, your featur
-00025a90: 6520 6772 6f75 7020 7769 6c6c 206f 6e6c  e group will onl
-00025aa0: 7920 6578 6973 740a 2020 2020 2020 2020  y exist.        
-00025ab0: 696e 2079 6f75 7220 5079 7468 6f6e 204b  in your Python K
-00025ac0: 6572 6e65 6c2c 2062 7574 206e 6f74 2069  ernel, but not i
-00025ad0: 6e20 486f 7073 776f 726b 732e 0a0a 2020  n Hopsworks...  
-00025ae0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00025af0: 2020 2020 2020 2020 7175 6572 7920 3d20          query = 
-00025b00: 2253 454c 4543 5420 2a20 4652 4f4d 2073  "SELECT * FROM s
-00025b10: 616c 6573 220a 0a20 2020 2020 2020 2066  ales"..        f
-00025b20: 6720 3d20 6665 6174 7572 655f 7374 6f72  g = feature_stor
-00025b30: 652e 6372 6561 7465 5f73 7069 6e65 5f67  e.create_spine_g
-00025b40: 726f 7570 286e 616d 653d 2273 616c 6573  roup(name="sales
-00025b50: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
-00025b60: 6572 7369 6f6e 3d31 2c0a 2020 2020 2020  ersion=1,.      
-00025b70: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00025b80: 6e3d 2250 6879 7369 6361 6c20 7368 6f70  n="Physical shop
-00025b90: 2073 616c 6573 2066 6561 7475 7265 7322   sales features"
-00025ba0: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
-00025bb0: 696d 6172 795f 6b65 793d 5b27 7373 5f73  imary_key=['ss_s
-00025bc0: 746f 7265 5f73 6b27 5d2c 0a20 2020 2020  tore_sk'],.     
-00025bd0: 2020 2020 2020 2065 7665 6e74 5f74 696d         event_tim
-00025be0: 653d 2773 616c 655f 6461 7465 272c 0a20  e='sale_date',. 
-00025bf0: 2020 2020 2020 2020 2020 2064 6174 6166             dataf
-00025c00: 7261 6d65 3d64 662c 0a20 2020 2020 2020  rame=df,.       
-00025c10: 2029 0a0a 2020 2020 2020 2020 6667 2e5f   )..        fg._
-00025c20: 7361 7665 2829 0a20 2020 2020 2020 2022  save().        "
-00025c30: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00025c40: 5f66 6561 7475 7265 5f67 726f 7570 5f65  _feature_group_e
-00025c50: 6e67 696e 652e 7361 7665 2873 656c 6629  ngine.save(self)
-00025c60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00025c70: 7365 6c66 0a0a 2020 2020 4070 726f 7065  self..    @prope
-00025c80: 7274 790a 2020 2020 6465 6620 6461 7461  rty.    def data
-00025c90: 6672 616d 6528 7365 6c66 293a 0a20 2020  frame(self):.   
-00025ca0: 2020 2020 2022 2222 5370 696e 6520 6461       """Spine da
-00025cb0: 7461 6672 616d 6520 7769 7468 2070 7269  taframe with pri
-00025cc0: 6d61 7279 206b 6579 2c20 6576 656e 7420  mary key, event 
-00025cd0: 7469 6d65 2061 6e64 0a20 2020 2020 2020  time and.       
-00025ce0: 206c 6162 656c 2063 6f6c 756d 6e20 746f   label column to
-00025cf0: 2075 7365 2066 6f72 2070 6f69 6e74 2069   use for point i
-00025d00: 6e20 7469 6d65 206a 6f69 6e20 7768 656e  n time join when
-00025d10: 2066 6574 6368 696e 6720 6665 6174 7572   fetching featur
-00025d20: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-00025d30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00025d40: 656c 662e 5f64 6174 6166 7261 6d65 0a0a  elf._dataframe..
-00025d50: 2020 2020 4064 6174 6166 7261 6d65 2e73      @dataframe.s
-00025d60: 6574 7465 720a 2020 2020 6465 6620 6461  etter.    def da
-00025d70: 7461 6672 616d 6528 7365 6c66 2c20 6461  taframe(self, da
-00025d80: 7461 6672 616d 6529 3a0a 2020 2020 2020  taframe):.      
-00025d90: 2020 2222 2255 7064 6174 6520 7468 6520    """Update the 
-00025da0: 7370 696e 6520 6461 7461 6672 616d 6520  spine dataframe 
-00025db0: 636f 6e74 6169 6e65 6420 696e 2074 6865  contained in the
-00025dc0: 2073 7069 6e65 2067 726f 7570 2e22 2222   spine group."""
-00025dd0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-00025de0: 6174 6166 7261 6d65 203d 2065 6e67 696e  ataframe = engin
-00025df0: 652e 6765 745f 696e 7374 616e 6365 2829  e.get_instance()
-00025e00: 2e63 6f6e 7665 7274 5f74 6f5f 6465 6661  .convert_to_defa
-00025e10: 756c 745f 6461 7461 6672 616d 6528 6461  ult_dataframe(da
-00025e20: 7461 6672 616d 6529 0a0a 2020 2020 2020  taframe)..      
-00025e30: 2020 2320 696e 2066 7320 7175 6572 7920    # in fs query 
-00025e40: 7468 6520 6665 6174 7572 6573 2061 7265  the features are
-00025e50: 206e 6f74 2073 656e 742c 2073 6f20 7468   not sent, so th
-00025e60: 656e 2064 6f6e 2774 2064 6f20 7661 6c69  en don't do vali
-00025e70: 6461 7469 6f6e 0a20 2020 2020 2020 2069  dation.        i
-00025e80: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-00025e90: 7365 6c66 2e5f 6964 2069 7320 6e6f 7420  self._id is not 
-00025ea0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00025eb0: 2061 6e64 2073 656c 662e 5f64 6174 6166   and self._dataf
-00025ec0: 7261 6d65 2069 7320 6e6f 7420 4e6f 6e65  rame is not None
-00025ed0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00025ee0: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
-00025ef0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00025f00: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00025f10: 2020 2064 6174 6166 7261 6d65 5f66 6561     dataframe_fea
-00025f20: 7475 7265 7320 3d20 656e 6769 6e65 2e67  tures = engine.g
-00025f30: 6574 5f69 6e73 7461 6e63 6528 292e 7061  et_instance().pa
-00025f40: 7273 655f 7363 6865 6d61 5f66 6561 7475  rse_schema_featu
-00025f50: 7265 5f67 726f 7570 280a 2020 2020 2020  re_group(.      
-00025f60: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00025f70: 6461 7461 6672 616d 650a 2020 2020 2020  dataframe.      
-00025f80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00025f90: 2020 2020 7365 6c66 2e5f 6665 6174 7572      self._featur
-00025fa0: 655f 6772 6f75 705f 656e 6769 6e65 2e5f  e_group_engine._
-00025fb0: 7665 7269 6679 5f73 6368 656d 615f 636f  verify_schema_co
-00025fc0: 6d70 6174 6962 696c 6974 7928 0a20 2020  mpatibility(.   
-00025fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00025fe0: 662e 5f66 6561 7475 7265 732c 2064 6174  f._features, dat
-00025ff0: 6166 7261 6d65 5f66 6561 7475 7265 730a  aframe_features.
-00026000: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00026010: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00026020: 2020 2020 6465 6620 6672 6f6d 5f72 6573      def from_res
-00026030: 706f 6e73 655f 6a73 6f6e 2863 6c73 2c20  ponse_json(cls, 
-00026040: 6a73 6f6e 5f64 6963 7429 3a0a 2020 2020  json_dict):.    
-00026050: 2020 2020 6a73 6f6e 5f64 6563 616d 656c      json_decamel
-00026060: 697a 6564 203d 2068 756d 7073 2e64 6563  ized = humps.dec
-00026070: 616d 656c 697a 6528 6a73 6f6e 5f64 6963  amelize(json_dic
-00026080: 7429 0a20 2020 2020 2020 2069 6620 6973  t).        if is
-00026090: 696e 7374 616e 6365 286a 736f 6e5f 6465  instance(json_de
-000260a0: 6361 6d65 6c69 7a65 642c 2064 6963 7429  camelized, dict)
-000260b0: 3a0a 2020 2020 2020 2020 2020 2020 5f20  :.            _ 
-000260c0: 3d20 6a73 6f6e 5f64 6563 616d 656c 697a  = json_decameliz
-000260d0: 6564 2e70 6f70 2822 7479 7065 222c 204e  ed.pop("type", N
-000260e0: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
-000260f0: 2072 6574 7572 6e20 636c 7328 2a2a 6a73   return cls(**js
-00026100: 6f6e 5f64 6563 616d 656c 697a 6564 290a  on_decamelized).
-00026110: 2020 2020 2020 2020 666f 7220 6667 2069          for fg i
-00026120: 6e20 6a73 6f6e 5f64 6563 616d 656c 697a  n json_decameliz
-00026130: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00026140: 5f20 3d20 6667 2e70 6f70 2822 7479 7065  _ = fg.pop("type
-00026150: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-00026160: 2072 6574 7572 6e20 5b63 6c73 282a 2a66   return [cls(**f
-00026170: 6729 2066 6f72 2066 6720 696e 206a 736f  g) for fg in jso
-00026180: 6e5f 6465 6361 6d65 6c69 7a65 645d 0a0a  n_decamelized]..
-00026190: 2020 2020 6465 6620 7570 6461 7465 5f66      def update_f
-000261a0: 726f 6d5f 7265 7370 6f6e 7365 5f6a 736f  rom_response_jso
-000261b0: 6e28 7365 6c66 2c20 6a73 6f6e 5f64 6963  n(self, json_dic
-000261c0: 7429 3a0a 2020 2020 2020 2020 6a73 6f6e  t):.        json
-000261d0: 5f64 6563 616d 656c 697a 6564 203d 2068  _decamelized = h
-000261e0: 756d 7073 2e64 6563 616d 656c 697a 6528  umps.decamelize(
-000261f0: 6a73 6f6e 5f64 6963 7429 0a20 2020 2020  json_dict).     
-00026200: 2020 2069 6620 2274 7970 6522 2069 6e20     if "type" in 
-00026210: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00026220: 3a0a 2020 2020 2020 2020 2020 2020 5f20  :.            _ 
-00026230: 3d20 6a73 6f6e 5f64 6563 616d 656c 697a  = json_decameliz
-00026240: 6564 2e70 6f70 2822 7479 7065 2229 0a20  ed.pop("type"). 
-00026250: 2020 2020 2020 2073 656c 662e 5f5f 696e         self.__in
-00026260: 6974 5f5f 282a 2a6a 736f 6e5f 6465 6361  it__(**json_deca
-00026270: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
-00026280: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-00026290: 2020 6465 6620 6a73 6f6e 2873 656c 6629    def json(self)
-000262a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000262b0: 206a 736f 6e2e 6475 6d70 7328 7365 6c66   json.dumps(self
-000262c0: 2c20 636c 733d 7574 696c 2e46 6561 7475  , cls=util.Featu
-000262d0: 7265 5374 6f72 6545 6e63 6f64 6572 290a  reStoreEncoder).
-000262e0: 0a20 2020 2064 6566 2074 6f5f 6469 6374  .    def to_dict
-000262f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00026300: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-00026310: 2020 2020 2022 6964 223a 2073 656c 662e       "id": self.
-00026320: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00026330: 2022 6e61 6d65 223a 2073 656c 662e 5f6e   "name": self._n
-00026340: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00026350: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00026360: 7365 6c66 2e5f 6465 7363 7269 7074 696f  self._descriptio
-00026370: 6e2c 0a20 2020 2020 2020 2020 2020 2022  n,.            "
-00026380: 7665 7273 696f 6e22 3a20 7365 6c66 2e5f  version": self._
-00026390: 7665 7273 696f 6e2c 0a20 2020 2020 2020  version,.       
-000263a0: 2020 2020 2022 6665 6174 7572 6573 223a       "features":
-000263b0: 2073 656c 662e 5f66 6561 7475 7265 732c   self._features,
-000263c0: 0a20 2020 2020 2020 2020 2020 2022 6665  .            "fe
-000263d0: 6174 7572 6573 746f 7265 4964 223a 2073  aturestoreId": s
-000263e0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
-000263f0: 7265 5f69 642c 0a20 2020 2020 2020 2020  re_id,.         
-00026400: 2020 2022 7479 7065 223a 2022 6f6e 4465     "type": "onDe
-00026410: 6d61 6e64 4665 6174 7572 6567 726f 7570  mandFeaturegroup
-00026420: 4454 4f22 2c0a 2020 2020 2020 2020 2020  DTO",.          
-00026430: 2020 2273 7461 7469 7374 6963 7343 6f6e    "statisticsCon
-00026440: 6669 6722 3a20 7365 6c66 2e5f 7374 6174  fig": self._stat
-00026450: 6973 7469 6373 5f63 6f6e 6669 672c 0a20  istics_config,. 
-00026460: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00026470: 7454 696d 6522 3a20 7365 6c66 2e5f 6576  tTime": self._ev
-00026480: 656e 745f 7469 6d65 2c0a 2020 2020 2020  ent_time,.      
-00026490: 2020 2020 2020 2273 7069 6e65 223a 2054        "spine": T
-000264a0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000264b0: 2022 746f 7069 634e 616d 6522 3a20 7365   "topicName": se
-000264c0: 6c66 2e74 6f70 6963 5f6e 616d 652c 0a20  lf.topic_name,. 
-000264d0: 2020 2020 2020 2020 2020 2022 6465 7072             "depr
-000264e0: 6563 6174 6564 223a 2073 656c 662e 6465  ecated": self.de
-000264f0: 7072 6563 6174 6564 2c0a 2020 2020 2020  precated,.      
-00026500: 2020 7d0a                                  }.
+00013b10: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+00013b20: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
+00013b30: 6365 2829 2e73 6574 5f6a 6f62 5f67 726f  ce().set_job_gro
+00013b40: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+00013b50: 2246 6574 6368 696e 6720 4665 6174 7572  "Fetching Featur
+00013b60: 6520 6772 6f75 7022 2c0a 2020 2020 2020  e group",.      
+00013b70: 2020 2020 2020 2247 6574 7469 6e67 2066        "Getting f
+00013b80: 6561 7475 7265 2067 726f 7570 3a20 7b7d  eature group: {}
+00013b90: 2066 726f 6d20 7468 6520 6665 6174 7572   from the featur
+00013ba0: 6573 746f 7265 207b 7d22 2e66 6f72 6d61  estore {}".forma
+00013bb0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00013bc0: 2020 2073 656c 662e 5f6e 616d 652c 2073     self._name, s
+00013bd0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
+00013be0: 7265 5f6e 616d 650a 2020 2020 2020 2020  re_name.        
+00013bf0: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
+00013c00: 0a20 2020 2020 2020 2069 6620 7761 6c6c  .        if wall
+00013c10: 636c 6f63 6b5f 7469 6d65 3a0a 2020 2020  clock_time:.    
+00013c20: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00013c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c40: 2073 656c 662e 7365 6c65 6374 5f61 6c6c   self.select_all
+00013c50: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00013c60: 2020 202e 6173 5f6f 6628 7761 6c6c 636c     .as_of(wallcl
+00013c70: 6f63 6b5f 7469 6d65 290a 2020 2020 2020  ock_time).      
+00013c80: 2020 2020 2020 2020 2020 2e72 6561 6428            .read(
+00013c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ca0: 2020 2020 206f 6e6c 696e 652c 0a20 2020       online,.   
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 2064 6174 6166 7261 6d65 5f74 7970 652c   dataframe_type,
+00013cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ce0: 2020 2020 2072 6561 645f 6f70 7469 6f6e       read_option
+00013cf0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00013d00: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00013d10: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+00013d20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013d30: 7572 6e20 7365 6c66 2e73 656c 6563 745f  urn self.select_
+00013d40: 616c 6c28 292e 7265 6164 280a 2020 2020  all().read(.    
+00013d50: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
+00013d60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00013d70: 2020 2020 6461 7461 6672 616d 655f 7479      dataframe_ty
+00013d80: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+00013d90: 2020 2020 7265 6164 5f6f 7074 696f 6e73      read_options
+00013da0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00013db0: 0a20 2020 2064 6566 2072 6561 645f 6368  .    def read_ch
+00013dc0: 616e 6765 7328 0a20 2020 2020 2020 2073  anges(.        s
+00013dd0: 656c 662c 0a20 2020 2020 2020 2073 7461  elf,.        sta
+00013de0: 7274 5f77 616c 6c63 6c6f 636b 5f74 696d  rt_wallclock_tim
+00013df0: 653a 2055 6e69 6f6e 5b73 7472 2c20 696e  e: Union[str, in
+00013e00: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
+00013e10: 655d 2c0a 2020 2020 2020 2020 656e 645f  e],.        end_
+00013e20: 7761 6c6c 636c 6f63 6b5f 7469 6d65 3a20  wallclock_time: 
+00013e30: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
+00013e40: 6461 7465 7469 6d65 2c20 6461 7465 5d2c  datetime, date],
+00013e50: 0a20 2020 2020 2020 2072 6561 645f 6f70  .        read_op
+00013e60: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+00013e70: 6469 6374 5d20 3d20 7b7d 2c0a 2020 2020  dict] = {},.    
+00013e80: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00013e90: 6164 7320 7570 6461 7465 7320 6f66 2074  ads updates of t
+00013ea0: 6869 7320 6665 6174 7572 6520 7468 6174  his feature that
+00013eb0: 206f 6363 7572 7265 6420 6265 7477 6565   occurred betwee
+00013ec0: 6e20 7370 6563 6966 6965 6420 706f 696e  n specified poin
+00013ed0: 7473 2069 6e20 7469 6d65 2e0a 0a20 2020  ts in time...   
+00013ee0: 2020 2020 2021 2121 2077 6172 6e69 6e67       !!! warning
+00013ef0: 2022 4465 7072 6563 6174 6564 220a 2020   "Deprecated".  
+00013f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f10: 2020 6072 6561 645f 6368 616e 6765 7360    `read_changes`
+00013f20: 206d 6574 686f 6420 6973 2064 6570 7265   method is depre
+00013f30: 6361 7465 642e 2055 7365 0a20 2020 2020  cated. Use.     
+00013f40: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00013f50: 6173 5f6f 6628 656e 645f 7761 6c6c 636c  as_of(end_wallcl
+00013f60: 6f63 6b5f 7469 6d65 2c20 6578 636c 7564  ock_time, exclud
+00013f70: 655f 756e 7469 6c3d 7374 6172 745f 7761  e_until=start_wa
+00013f80: 6c6c 636c 6f63 6b5f 7469 6d65 292e 7265  llclock_time).re
+00013f90: 6164 2872 6561 645f 6f70 7469 6f6e 733d  ad(read_options=
+00013fa0: 7265 6164 5f6f 7074 696f 6e73 2960 0a20  read_options)`. 
+00013fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fc0: 2020 2069 6e73 7465 6164 2e0a 0a20 2020     instead...   
+00013fd0: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+00013fe0: 6f6e 206f 6e6c 7920 776f 726b 7320 6f6e  on only works on
+00013ff0: 2066 6561 7475 7265 2067 726f 7570 7320   feature groups 
+00014000: 7769 7468 2060 4855 4449 6020 7469 6d65  with `HUDI` time
+00014010: 2074 7261 7665 6c20 666f 726d 6174 2e0a   travel format..
+00014020: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
+00014030: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00014040: 2073 7461 7274 5f77 616c 6c63 6c6f 636b   start_wallclock
+00014050: 5f74 696d 653a 2053 7461 7274 2074 696d  _time: Start tim
+00014060: 6520 6f66 2074 6865 2074 696d 6520 7472  e of the time tr
+00014070: 6176 656c 2071 7565 7279 2e20 5374 7269  avel query. Stri
+00014080: 6e67 7320 7368 6f75 6c64 2062 6520 666f  ngs should be fo
+00014090: 726d 6174 7465 6420 696e 206f 6e65 206f  rmatted in one o
+000140a0: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+000140b0: 666f 726d 6174 7320 6025 592d 256d 2d25  formats `%Y-%m-%
+000140c0: 6460 2c20 6025 592d 256d 2d25 6420 2548  d`, `%Y-%m-%d %H
+000140d0: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
+000140e0: 254d 602c 0a20 2020 2020 2020 2020 2020  %M`,.           
+000140f0: 2020 2020 2060 2559 2d25 6d2d 2564 2025       `%Y-%m-%d %
+00014100: 483a 254d 3a25 5360 2c20 6f72 2060 2559  H:%M:%S`, or `%Y
+00014110: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
+00014120: 2566 602e 0a20 2020 2020 2020 2020 2020  %f`..           
+00014130: 2065 6e64 5f77 616c 6c63 6c6f 636b 5f74   end_wallclock_t
+00014140: 696d 653a 2045 6e64 2074 696d 6520 6f66  ime: End time of
+00014150: 2074 6865 2074 696d 6520 7472 6176 656c   the time travel
+00014160: 2071 7565 7279 2e20 5374 7269 6e67 7320   query. Strings 
+00014170: 7368 6f75 6c64 2062 6520 666f 726d 6174  should be format
+00014180: 7465 6420 696e 206f 6e65 206f 6620 7468  ted in one of th
+00014190: 6520 666f 6c6c 6f77 696e 6720 666f 726d  e following form
+000141a0: 6174 7320 6025 592d 256d 2d25 6460 2c20  ats `%Y-%m-%d`, 
+000141b0: 6025 592d 256d 2d25 6420 2548 602c 2060  `%Y-%m-%d %H`, `
+000141c0: 2559 2d25 6d2d 2564 2025 483a 254d 602c  %Y-%m-%d %H:%M`,
+000141d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141e0: 2060 2559 2d25 6d2d 2564 2025 483a 254d   `%Y-%m-%d %H:%M
+000141f0: 3a25 5360 2c20 6f72 2060 2559 2d25 6d2d  :%S`, or `%Y-%m-
+00014200: 2564 2025 483a 254d 3a25 532e 2566 602e  %d %H:%M:%S.%f`.
+00014210: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00014220: 645f 6f70 7469 6f6e 733a 2041 6464 6974  d_options: Addit
+00014230: 696f 6e61 6c20 6f70 7469 6f6e 7320 6173  ional options as
+00014240: 206b 6579 2f76 616c 7565 2070 6169 7273   key/value pairs
+00014250: 2074 6f20 7061 7373 2074 6f20 7468 6520   to pass to the 
+00014260: 6578 6563 7574 696f 6e20 656e 6769 6e65  execution engine
+00014270: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014280: 2020 466f 7220 7370 6172 6b20 656e 6769    For spark engi
+00014290: 6e65 3a20 4469 6374 696f 6e61 7279 206f  ne: Dictionary o
+000142a0: 6620 7265 6164 206f 7074 696f 6e73 2066  f read options f
+000142b0: 6f72 2053 7061 726b 2e0a 2020 2020 2020  or Spark..      
+000142c0: 2020 2020 2020 2020 2020 466f 7220 7079            For py
+000142d0: 7468 6f6e 2065 6e67 696e 653a 0a20 2020  thon engine:.   
+000142e0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+000142f0: 6579 2060 2268 6976 655f 636f 6e66 6967  ey `"hive_config
+00014300: 2260 2074 6f20 7061 7373 2061 2064 6963  "` to pass a dic
+00014310: 7469 6f6e 6172 7920 6f66 2068 6976 6520  tionary of hive 
+00014320: 6f72 2074 657a 2063 6f6e 6669 6775 7261  or tez configura
+00014330: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
+00014340: 2020 2020 2020 2020 2046 6f72 2065 7861           For exa
+00014350: 6d70 6c65 3a20 607b 2268 6976 655f 636f  mple: `{"hive_co
+00014360: 6e66 6967 223a 207b 2268 6976 652e 7465  nfig": {"hive.te
+00014370: 7a2e 6370 752e 7663 6f72 6573 223a 2032  z.cpu.vcores": 2
+00014380: 2c20 2274 657a 2e67 726f 7570 696e 672e  , "tez.grouping.
+00014390: 7370 6c69 742d 636f 756e 7422 3a20 2233  split-count": "3
+000143a0: 227d 7d60 0a20 2020 2020 2020 2020 2020  "}}`.           
+000143b0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+000143c0: 2060 7b7d 602e 0a0a 2020 2020 2020 2020   `{}`...        
+000143d0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
+000143e0: 2020 2020 2020 6044 6174 6146 7261 6d65        `DataFrame
+000143f0: 602e 2054 6865 2073 7061 726b 2064 6174  `. The spark dat
+00014400: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
+00014410: 6720 7468 6520 696e 6372 656d 656e 7461  g the incrementa
+00014420: 6c20 6368 616e 6765 7320 6f66 0a20 2020  l changes of.   
+00014430: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00014440: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+00014450: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
+00014460: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
+00014470: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
+00014480: 7441 5049 4572 726f 7260 2e20 204e 6f20  tAPIError`.  No 
+00014490: 6461 7461 2069 7320 6176 6169 6c61 626c  data is availabl
+000144a0: 6520 666f 7220 6665 6174 7572 6520 6772  e for feature gr
+000144b0: 6f75 7020 7769 7468 2074 6869 7320 636f  oup with this co
+000144c0: 6d6d 6974 2064 6174 652e 0a20 2020 2020  mmit date..     
+000144d0: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+000144e0: 656e 742e 6578 6365 7074 696f 6e73 2e46  ent.exceptions.F
+000144f0: 6561 7475 7265 5374 6f72 6545 7863 6570  eatureStoreExcep
+00014500: 7469 6f6e 602e 2049 6620 7468 6520 6665  tion`. If the fe
+00014510: 6174 7572 6520 6772 6f75 7020 646f 6573  ature group does
+00014520: 206e 6f74 2068 6176 6520 6048 5544 4960   not have `HUDI`
+00014530: 2074 696d 6520 7472 6176 656c 2066 6f72   time travel for
+00014540: 6d61 740a 2020 2020 2020 2020 2222 220a  mat.        """.
+00014550: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00014560: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00014570: 662e 7365 6c65 6374 5f61 6c6c 2829 0a20  f.select_all(). 
+00014580: 2020 2020 2020 2020 2020 202e 7075 6c6c             .pull
+00014590: 5f63 6861 6e67 6573 2873 7461 7274 5f77  _changes(start_w
+000145a0: 616c 6c63 6c6f 636b 5f74 696d 652c 2065  allclock_time, e
+000145b0: 6e64 5f77 616c 6c63 6c6f 636b 5f74 696d  nd_wallclock_tim
+000145c0: 6529 0a20 2020 2020 2020 2020 2020 202e  e).            .
+000145d0: 7265 6164 2846 616c 7365 2c20 2264 6566  read(False, "def
+000145e0: 6175 6c74 222c 2072 6561 645f 6f70 7469  ault", read_opti
+000145f0: 6f6e 7329 0a20 2020 2020 2020 2029 0a0a  ons).        )..
+00014600: 2020 2020 6465 6620 6669 6e64 5f6e 6569      def find_nei
+00014610: 6768 626f 7273 280a 2020 2020 2020 2020  ghbors(.        
+00014620: 7365 6c66 2c0a 2020 2020 2020 2020 656d  self,.        em
+00014630: 6265 6464 696e 673a 204c 6973 745b 556e  bedding: List[Un
+00014640: 696f 6e5b 696e 742c 2066 6c6f 6174 5d5d  ion[int, float]]
+00014650: 2c0a 2020 2020 2020 2020 636f 6c3a 204f  ,.        col: O
+00014660: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00014670: 6f6e 652c 0a20 2020 2020 2020 206b 3a20  one,.        k: 
+00014680: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00014690: 3130 2c0a 2020 2020 2020 2020 6669 6c74  10,.        filt
+000146a0: 6572 3a20 4f70 7469 6f6e 616c 5b55 6e69  er: Optional[Uni
+000146b0: 6f6e 5b46 696c 7465 722c 204c 6f67 6963  on[Filter, Logic
+000146c0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+000146d0: 2020 206d 696e 5f73 636f 7265 3a20 4f70     min_score: Op
+000146e0: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
+000146f0: 302c 0a20 2020 2029 202d 3e20 4c69 7374  0,.    ) -> List
+00014700: 5b54 7570 6c65 5b66 6c6f 6174 2c20 4c69  [Tuple[float, Li
+00014710: 7374 5b41 6e79 5d5d 5d3a 0a20 2020 2020  st[Any]]]:.     
+00014720: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
+00014730: 696e 6473 2074 6865 206e 6561 7265 7374  inds the nearest
+00014740: 206e 6569 6768 626f 7273 2066 6f72 2061   neighbors for a
+00014750: 2067 6976 656e 2065 6d62 6564 6469 6e67   given embedding
+00014760: 2069 6e20 7468 6520 7665 6374 6f72 2064   in the vector d
+00014770: 6174 6162 6173 652e 0a0a 2020 2020 2020  atabase...      
+00014780: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
+00014790: 2020 2020 2020 2020 2020 656d 6265 6464            embedd
+000147a0: 696e 673a 2054 6865 2074 6172 6765 7420  ing: The target 
+000147b0: 656d 6265 6464 696e 6720 666f 7220 7768  embedding for wh
+000147c0: 6963 6820 6e65 6967 6862 6f72 7320 6172  ich neighbors ar
+000147d0: 6520 746f 2062 6520 666f 756e 642e 0a20  e to be found.. 
+000147e0: 2020 2020 2020 2020 2020 2063 6f6c 3a20             col: 
+000147f0: 5468 6520 636f 6c75 6d6e 206e 616d 6520  The column name 
+00014800: 7573 6564 2074 6f20 636f 6d70 7574 6520  used to compute 
+00014810: 7369 6d69 6c61 7269 7479 2073 636f 7265  similarity score
+00014820: 2e20 5265 7175 6972 6564 206f 6e6c 7920  . Required only 
+00014830: 6966 2074 6865 7265 0a20 2020 2020 2020  if there.       
+00014840: 2020 2020 2061 7265 206d 756c 7469 706c       are multipl
+00014850: 6520 656d 6265 6464 696e 6773 2028 6f70  e embeddings (op
+00014860: 7469 6f6e 616c 292e 0a20 2020 2020 2020  tional)..       
+00014870: 2020 2020 206b 3a20 5468 6520 6e75 6d62       k: The numb
+00014880: 6572 206f 6620 6e65 6172 6573 7420 6e65  er of nearest ne
+00014890: 6967 6862 6f72 7320 746f 2072 6574 7269  ighbors to retri
+000148a0: 6576 6520 2864 6566 6175 6c74 2069 7320  eve (default is 
+000148b0: 3130 292e 0a20 2020 2020 2020 2020 2020  10)..           
+000148c0: 2066 696c 7465 723a 2041 2066 696c 7465   filter: A filte
+000148d0: 7220 6578 7072 6573 7369 6f6e 2074 6f20  r expression to 
+000148e0: 7265 7374 7269 6374 2074 6865 2073 6561  restrict the sea
+000148f0: 7263 6820 7370 6163 6520 286f 7074 696f  rch space (optio
+00014900: 6e61 6c29 2e0a 2020 2020 2020 2020 2020  nal)..          
+00014910: 2020 6d69 6e5f 7363 6f72 653a 2054 6865    min_score: The
+00014920: 206d 696e 696d 756d 2073 696d 696c 6172   minimum similar
+00014930: 6974 7920 7363 6f72 6520 666f 7220 6e65  ity score for ne
+00014940: 6967 6862 6f72 7320 746f 2062 6520 636f  ighbors to be co
+00014950: 6e73 6964 6572 6564 2028 6465 6661 756c  nsidered (defaul
+00014960: 7420 6973 2030 292e 0a0a 2020 2020 2020  t is 0)...      
+00014970: 2020 2320 5265 7475 726e 730a 2020 2020    # Returns.    
+00014980: 2020 2020 2020 2020 4120 6c69 7374 206f          A list o
+00014990: 6620 7475 706c 6573 2072 6570 7265 7365  f tuples represe
+000149a0: 6e74 696e 6720 7468 6520 6e65 6172 6573  nting the neares
+000149b0: 7420 6e65 6967 6862 6f72 732e 0a20 2020  t neighbors..   
+000149c0: 2020 2020 2020 2020 2045 6163 6820 7475           Each tu
+000149d0: 706c 6520 636f 6e74 6169 6e73 3a20 6028  ple contains: `(
+000149e0: 5468 6520 7369 6d69 6c61 7269 7479 2073  The similarity s
+000149f0: 636f 7265 2c20 4120 6c69 7374 206f 6620  core, A list of 
+00014a00: 6665 6174 7572 6520 7661 6c75 6573 2960  feature values)`
+00014a10: 0a0a 2020 2020 2020 2020 2121 2120 4578  ..        !!! Ex
+00014a20: 616d 706c 650a 2020 2020 2020 2020 2020  ample.          
+00014a30: 2020 6060 600a 2020 2020 2020 2020 2020    ```.          
+00014a40: 2020 656d 6265 6464 696e 675f 696e 6465    embedding_inde
+00014a50: 7820 3d20 456d 6265 6464 696e 6749 6e64  x = EmbeddingInd
+00014a60: 6578 2829 0a20 2020 2020 2020 2020 2020  ex().           
+00014a70: 2065 6d62 6564 6469 6e67 5f69 6e64 6578   embedding_index
+00014a80: 2e61 6464 5f65 6d62 6564 6469 6e67 286e  .add_embedding(n
+00014a90: 616d 653d 2275 7365 725f 7665 6374 6f72  ame="user_vector
+00014aa0: 222c 2064 696d 656e 7369 6f6e 3d33 290a  ", dimension=3).
+00014ab0: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
+00014ac0: 2066 732e 6372 6561 7465 5f66 6561 7475   fs.create_featu
+00014ad0: 7265 5f67 726f 7570 280a 2020 2020 2020  re_group(.      
+00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014af0: 2020 6e61 6d65 3d27 6169 725f 7175 616c    name='air_qual
+00014b00: 6974 7927 2c0a 2020 2020 2020 2020 2020  ity',.          
+00014b10: 2020 2020 2020 2020 2020 2020 2020 656d                em
+00014b20: 6265 6464 696e 675f 696e 6465 7820 3d20  bedding_index = 
+00014b30: 656d 6265 6464 696e 675f 696e 6465 782c  embedding_index,
+00014b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014b50: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
+00014b60: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
+00014b70: 2020 2020 2020 2020 2020 2020 7072 696d              prim
+00014b80: 6172 795f 6b65 793d 5b27 6964 3127 5d2c  ary_key=['id1'],
+00014b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014ba0: 2020 2020 2020 2020 206f 6e6c 696e 655f           online_
+00014bb0: 656e 6162 6c65 643d 5472 7565 2c0a 2020  enabled=True,.  
+00014bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bd0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00014be0: 6667 2e69 6e73 6572 7428 6461 7461 290a  fg.insert(data).
+00014bf0: 2020 2020 2020 2020 2020 2020 6667 2e66              fg.f
+00014c00: 696e 645f 6e65 6967 6862 6f72 7328 0a20  ind_neighbors(. 
+00014c10: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00014c20: 302e 312c 2030 2e32 2c20 302e 335d 2c0a  0.1, 0.2, 0.3],.
+00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c40: 6b3d 352c 0a20 2020 2020 2020 2020 2020  k=5,.           
+00014c50: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00014c60: 2320 6170 706c 7920 6669 6c74 6572 0a20  # apply filter. 
+00014c70: 2020 2020 2020 2020 2020 2066 672e 6669             fg.fi
+00014c80: 6e64 5f6e 6569 6768 626f 7273 280a 2020  nd_neighbors(.  
+00014c90: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
+00014ca0: 2e31 2c20 302e 322c 2030 2e33 5d2c 0a20  .1, 0.2, 0.3],. 
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00014cc0: 3d35 2c0a 2020 2020 2020 2020 2020 2020  =5,.            
+00014cd0: 2020 2020 6669 6c74 6572 3d28 6667 2e69      filter=(fg.i
+00014ce0: 6431 203e 2031 3029 2026 2028 6667 2e69  d1 > 10) & (fg.i
+00014cf0: 6431 203c 2033 3029 0a20 2020 2020 2020  d1 < 30).       
+00014d00: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014d10: 2020 2060 6060 0a20 2020 2020 2020 2022     ```.        "
+00014d20: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00014d30: 6c66 2e5f 7665 6374 6f72 5f64 625f 636c  lf._vector_db_cl
+00014d40: 6965 6e74 2069 7320 4e6f 6e65 2061 6e64  ient is None and
+00014d50: 2073 656c 662e 5f65 6d62 6564 6469 6e67   self._embedding
+00014d60: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
+00014d70: 2020 2020 7365 6c66 2e5f 7665 6374 6f72      self._vector
+00014d80: 5f64 625f 636c 6965 6e74 203d 2056 6563  _db_client = Vec
+00014d90: 746f 7244 6243 6c69 656e 7428 7365 6c66  torDbClient(self
+00014da0: 2e73 656c 6563 745f 616c 6c28 2929 0a20  .select_all()). 
+00014db0: 2020 2020 2020 2072 6573 756c 7473 203d         results =
+00014dc0: 2073 656c 662e 5f76 6563 746f 725f 6462   self._vector_db
+00014dd0: 5f63 6c69 656e 742e 6669 6e64 5f6e 6569  _client.find_nei
+00014de0: 6768 626f 7273 280a 2020 2020 2020 2020  ghbors(.        
+00014df0: 2020 2020 656d 6265 6464 696e 672c 0a20      embedding,. 
+00014e00: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+00014e10: 7265 3d28 7365 6c66 2e5f 5f67 6574 6174  re=(self.__getat
+00014e20: 7472 5f5f 2863 6f6c 2920 6966 2063 6f6c  tr__(col) if col
+00014e30: 2065 6c73 6520 4e6f 6e65 292c 0a20 2020   else None),.   
+00014e40: 2020 2020 2020 2020 206b 3d6b 2c0a 2020           k=k,.  
+00014e50: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00014e60: 3d66 696c 7465 722c 0a20 2020 2020 2020  =filter,.       
+00014e70: 2020 2020 206d 696e 5f73 636f 7265 3d6d       min_score=m
+00014e80: 696e 5f73 636f 7265 2c0a 2020 2020 2020  in_score,.      
+00014e90: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+00014ea0: 726e 205b 0a20 2020 2020 2020 2020 2020  rn [.           
+00014eb0: 2028 7265 7375 6c74 5b30 5d2c 205b 7265   (result[0], [re
+00014ec0: 7375 6c74 5b31 5d5b 662e 6e61 6d65 5d20  sult[1][f.name] 
+00014ed0: 666f 7220 6620 696e 2073 656c 662e 6665  for f in self.fe
+00014ee0: 6174 7572 6573 5d29 0a20 2020 2020 2020  atures]).       
+00014ef0: 2020 2020 2066 6f72 2072 6573 756c 7420       for result 
+00014f00: 696e 2072 6573 756c 7473 0a20 2020 2020  in results.     
+00014f10: 2020 205d 0a0a 2020 2020 6465 6620 7368     ]..    def sh
+00014f20: 6f77 2873 656c 662c 206e 3a20 696e 742c  ow(self, n: int,
+00014f30: 206f 6e6c 696e 653a 204f 7074 696f 6e61   online: Optiona
+00014f40: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 6529  l[bool] = False)
+00014f50: 3a0a 2020 2020 2020 2020 2222 2253 686f  :.        """Sho
+00014f60: 7720 7468 6520 6669 7273 7420 606e 6020  w the first `n` 
+00014f70: 726f 7773 206f 6620 7468 6520 6665 6174  rows of the feat
+00014f80: 7572 6520 6772 6f75 702e 0a0a 2020 2020  ure group...    
+00014f90: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
+00014fa0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+00014fb0: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+00014fc0: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
+00014fd0: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
+00014fe0: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
+00014ff0: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
+00015000: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
+00015010: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
+00015020: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+00015030: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
+00015040: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+00015050: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
+00015060: 2020 2020 2020 2320 6d61 6b65 2061 2071        # make a q
+00015070: 7565 7279 2061 6e64 2073 686f 7720 746f  uery and show to
+00015080: 7020 3520 726f 7773 0a20 2020 2020 2020  p 5 rows.       
+00015090: 2020 2020 2066 672e 7365 6c65 6374 285b       fg.select([
+000150a0: 2764 6174 6527 2c27 7765 656b 6c79 5f73  'date','weekly_s
+000150b0: 616c 6573 272c 2769 735f 686f 6c69 6461  ales','is_holida
+000150c0: 7927 5d29 2e73 686f 7728 3529 0a20 2020  y']).show(5).   
+000150d0: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
+000150e0: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
+000150f0: 730a 2020 2020 2020 2020 2020 2020 6e3a  s.            n:
+00015100: 2069 6e74 2e20 4e75 6d62 6572 206f 6620   int. Number of 
+00015110: 726f 7773 2074 6f20 7368 6f77 2e0a 2020  rows to show..  
+00015120: 2020 2020 2020 2020 2020 6f6e 6c69 6e65            online
+00015130: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00015140: 2e20 4966 2060 5472 7565 6020 7265 6164  . If `True` read
+00015150: 2066 726f 6d20 6f6e 6c69 6e65 2066 6561   from online fea
+00015160: 7475 7265 2073 746f 7265 2c20 6465 6661  ture store, defa
+00015170: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
+00015180: 2020 2020 2074 6f20 6046 616c 7365 602e       to `False`.
+00015190: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000151a0: 2020 2020 2065 6e67 696e 652e 6765 745f       engine.get_
+000151b0: 696e 7374 616e 6365 2829 2e73 6574 5f6a  instance().set_j
+000151c0: 6f62 5f67 726f 7570 280a 2020 2020 2020  ob_group(.      
+000151d0: 2020 2020 2020 2246 6574 6368 696e 6720        "Fetching 
+000151e0: 4665 6174 7572 6520 6772 6f75 7022 2c0a  Feature group",.
+000151f0: 2020 2020 2020 2020 2020 2020 2247 6574              "Get
+00015200: 7469 6e67 2066 6561 7475 7265 2067 726f  ting feature gro
+00015210: 7570 3a20 7b7d 2066 726f 6d20 7468 6520  up: {} from the 
+00015220: 6665 6174 7572 6573 746f 7265 207b 7d22  featurestore {}"
+00015230: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00015240: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
+00015250: 616d 652c 2073 656c 662e 5f66 6561 7475  ame, self._featu
+00015260: 7265 5f73 746f 7265 5f6e 616d 650a 2020  re_store_name.  
+00015270: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00015280: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00015290: 6620 6f6e 6c69 6e65 2061 6e64 2073 656c  f online and sel
+000152a0: 662e 656d 6265 6464 696e 675f 696e 6465  f.embedding_inde
+000152b0: 783a 0a20 2020 2020 2020 2020 2020 2069  x:.            i
+000152c0: 6620 7365 6c66 2e5f 7665 6374 6f72 5f64  f self._vector_d
+000152d0: 625f 636c 6965 6e74 2069 7320 4e6f 6e65  b_client is None
+000152e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000152f0: 2020 7365 6c66 2e5f 7665 6374 6f72 5f64    self._vector_d
+00015300: 625f 636c 6965 6e74 203d 2056 6563 746f  b_client = Vecto
+00015310: 7244 6243 6c69 656e 7428 7365 6c66 2e73  rDbClient(self.s
+00015320: 656c 6563 745f 616c 6c28 2929 0a20 2020  elect_all()).   
+00015330: 2020 2020 2020 2020 2072 6573 756c 7473           results
+00015340: 203d 2073 656c 662e 5f76 6563 746f 725f   = self._vector_
+00015350: 6462 5f63 6c69 656e 742e 7265 6164 280a  db_client.read(.
+00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015370: 7365 6c66 2e69 642c 0a20 2020 2020 2020  self.id,.       
+00015380: 2020 2020 2020 2020 207b 7d2c 0a20 2020           {},.   
+00015390: 2020 2020 2020 2020 2020 2020 2070 6b3d               pk=
+000153a0: 7365 6c66 2e65 6d62 6564 6469 6e67 5f69  self.embedding_i
+000153b0: 6e64 6578 2e63 6f6c 5f70 7265 6669 7820  ndex.col_prefix 
+000153c0: 2b20 7365 6c66 2e70 7269 6d61 7279 5f6b  + self.primary_k
+000153d0: 6579 5b30 5d2c 0a20 2020 2020 2020 2020  ey[0],.         
+000153e0: 2020 2020 2020 2069 6e64 6578 5f6e 616d         index_nam
+000153f0: 653d 7365 6c66 2e65 6d62 6564 6469 6e67  e=self.embedding
+00015400: 5f69 6e64 6578 2e69 6e64 6578 5f6e 616d  _index.index_nam
+00015410: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00015420: 2020 206e 3d6e 2c0a 2020 2020 2020 2020     n=n,.        
+00015430: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00015440: 2020 7265 7475 726e 205b 5b72 6573 756c    return [[resul
+00015450: 745b 662e 6e61 6d65 5d20 666f 7220 6620  t[f.name] for f 
+00015460: 696e 2073 656c 662e 6665 6174 7572 6573  in self.features
+00015470: 5d20 666f 7220 7265 7375 6c74 2069 6e20  ] for result in 
+00015480: 7265 7375 6c74 735d 0a20 2020 2020 2020  results].       
+00015490: 2072 6574 7572 6e20 7365 6c66 2e73 656c   return self.sel
+000154a0: 6563 745f 616c 6c28 292e 7368 6f77 286e  ect_all().show(n
+000154b0: 2c20 6f6e 6c69 6e65 290a 0a20 2020 2064  , online)..    d
+000154c0: 6566 2073 6176 6528 0a20 2020 2020 2020  ef save(.       
+000154d0: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+000154e0: 6561 7475 7265 733a 2055 6e69 6f6e 5b0a  eatures: Union[.
+000154f0: 2020 2020 2020 2020 2020 2020 7064 2e44              pd.D
+00015500: 6174 6146 7261 6d65 2c0a 2020 2020 2020  ataFrame,.      
+00015510: 2020 2020 2020 5479 7065 5661 7228 2270        TypeVar("p
+00015520: 7973 7061 726b 2e73 716c 2e44 6174 6146  yspark.sql.DataF
+00015530: 7261 6d65 2229 2c20 2023 206e 6f71 613a  rame"),  # noqa:
+00015540: 2046 3832 310a 2020 2020 2020 2020 2020   F821.          
+00015550: 2020 5479 7065 5661 7228 2270 7973 7061    TypeVar("pyspa
+00015560: 726b 2e52 4444 2229 2c20 2023 206e 6f71  rk.RDD"),  # noq
+00015570: 613a 2046 3832 310a 2020 2020 2020 2020  a: F821.        
+00015580: 2020 2020 6e70 2e6e 6461 7272 6179 2c0a      np.ndarray,.
+00015590: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+000155a0: 5b66 6561 7475 7265 2e46 6561 7475 7265  [feature.Feature
+000155b0: 5d2c 0a20 2020 2020 2020 205d 203d 204e  ],.        ] = N
+000155c0: 6f6e 652c 0a20 2020 2020 2020 2077 7269  one,.        wri
+000155d0: 7465 5f6f 7074 696f 6e73 3a20 4f70 7469  te_options: Opti
+000155e0: 6f6e 616c 5b44 6963 745b 416e 792c 2041  onal[Dict[Any, A
+000155f0: 6e79 5d5d 203d 207b 7d2c 0a20 2020 2020  ny]] = {},.     
+00015600: 2020 2076 616c 6964 6174 696f 6e5f 6f70     validation_op
+00015610: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+00015620: 4469 6374 5b41 6e79 2c20 416e 795d 5d20  Dict[Any, Any]] 
+00015630: 3d20 7b7d 2c0a 2020 2020 2020 2020 7761  = {},.        wa
+00015640: 6974 3a20 626f 6f6c 203d 2046 616c 7365  it: bool = False
+00015650: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00015660: 2022 2222 5065 7273 6973 7420 7468 6520   """Persist the 
+00015670: 6d65 7461 6461 7461 2061 6e64 206d 6174  metadata and mat
+00015680: 6572 6961 6c69 7a65 2074 6865 2066 6561  erialize the fea
+00015690: 7475 7265 2067 726f 7570 2074 6f20 7468  ture group to th
+000156a0: 6520 6665 6174 7572 6520 7374 6f72 652e  e feature store.
+000156b0: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
+000156c0: 726e 696e 6720 2243 6861 6e67 6564 2069  rning "Changed i
+000156d0: 6e20 332e 332e 3022 0a20 2020 2020 2020  n 3.3.0".       
+000156e0: 2020 2020 2060 696e 7365 7274 6020 616e       `insert` an
+000156f0: 6420 6073 6176 6560 206d 6574 686f 6473  d `save` methods
+00015700: 2061 7265 206e 6f77 2061 7379 6e63 2062   are now async b
+00015710: 7920 6465 6661 756c 7420 696e 206e 6f6e  y default in non
+00015720: 2d73 7061 726b 2063 6c69 656e 7473 2e0a  -spark clients..
+00015730: 2020 2020 2020 2020 2020 2020 546f 2061              To a
+00015740: 6368 6965 7665 2074 6865 206f 6c64 2062  chieve the old b
+00015750: 6568 6176 696f 7572 2c20 7365 7420 6077  ehaviour, set `w
+00015760: 6169 7460 2061 7267 756d 656e 7420 746f  ait` argument to
+00015770: 2060 5472 7565 602e 0a0a 2020 2020 2020   `True`...      
+00015780: 2020 4361 6c6c 696e 6720 6073 6176 6560    Calling `save`
+00015790: 2063 7265 6174 6573 2074 6865 206d 6574   creates the met
+000157a0: 6164 6174 6120 666f 7220 7468 6520 6665  adata for the fe
+000157b0: 6174 7572 6520 6772 6f75 7020 696e 2074  ature group in t
+000157c0: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
+000157d0: 2e0a 2020 2020 2020 2020 4966 2061 2044  ..        If a D
+000157e0: 6174 6146 7261 6d65 2c20 5244 4420 6f72  ataFrame, RDD or
+000157f0: 204e 6461 7272 6179 2069 7320 7072 6f76   Ndarray is prov
+00015800: 6964 6564 2c20 7468 6520 6461 7461 2069  ided, the data i
+00015810: 7320 7772 6974 7465 6e20 746f 2074 6865  s written to the
+00015820: 0a20 2020 2020 2020 206f 6e6c 696e 652f  .        online/
+00015830: 6f66 666c 696e 6520 6665 6174 7572 6520  offline feature 
+00015840: 7374 6f72 6520 6173 2073 7065 6369 6669  store as specifi
+00015850: 6564 2e0a 2020 2020 2020 2020 4279 2064  ed..        By d
+00015860: 6566 6175 6c74 2c20 7468 6973 2077 7269  efault, this wri
+00015870: 7465 7320 7468 6520 6665 6174 7572 6520  tes the feature 
+00015880: 6772 6f75 7020 746f 2074 6865 206f 6666  group to the off
+00015890: 6c69 6e65 2073 746f 7261 6765 2c20 616e  line storage, an
+000158a0: 6420 6966 0a20 2020 2020 2020 2060 6f6e  d if.        `on
+000158b0: 6c69 6e65 5f65 6e61 626c 6564 6020 666f  line_enabled` fo
+000158c0: 7220 7468 6520 6665 6174 7572 6520 6772  r the feature gr
+000158d0: 6f75 702c 2061 6c73 6f20 746f 2074 6865  oup, also to the
+000158e0: 206f 6e6c 696e 6520 6665 6174 7572 6520   online feature 
+000158f0: 7374 6f72 652e 0a20 2020 2020 2020 2054  store..        T
+00015900: 6865 2060 6665 6174 7572 6573 6020 6461  he `features` da
+00015910: 7461 6672 616d 6520 6361 6e20 6265 2061  taframe can be a
+00015920: 2053 7061 726b 2044 6174 6146 7261 6d65   Spark DataFrame
+00015930: 206f 7220 5244 442c 2061 2050 616e 6461   or RDD, a Panda
+00015940: 7320 4461 7461 4672 616d 652c 0a20 2020  s DataFrame,.   
+00015950: 2020 2020 206f 7220 6120 7477 6f2d 6469       or a two-di
+00015960: 6d65 6e73 696f 6e61 6c20 4e75 6d70 7920  mensional Numpy 
+00015970: 6172 7261 7920 6f72 2061 2074 776f 2d64  array or a two-d
+00015980: 696d 656e 7369 6f6e 616c 2050 7974 686f  imensional Pytho
+00015990: 6e20 6e65 7374 6564 206c 6973 742e 0a20  n nested list.. 
+000159a0: 2020 2020 2020 2023 2041 7267 756d 656e         # Argumen
+000159b0: 7473 0a20 2020 2020 2020 2020 2020 2066  ts.            f
+000159c0: 6561 7475 7265 733a 2044 6174 6146 7261  eatures: DataFra
+000159d0: 6d65 2c20 5244 442c 204e 6461 7272 6179  me, RDD, Ndarray
+000159e0: 206f 7220 6120 6c69 7374 206f 6620 6665   or a list of fe
+000159f0: 6174 7572 6573 2e20 4665 6174 7572 6573  atures. Features
+00015a00: 2074 6f20 6265 2073 6176 6564 2e0a 2020   to be saved..  
+00015a10: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00015a20: 6973 2061 7267 756d 656e 7420 6973 206f  is argument is o
+00015a30: 7074 696f 6e61 6c20 6966 2074 6865 2066  ptional if the f
+00015a40: 6561 7475 7265 206c 6973 7420 6973 2070  eature list is p
+00015a50: 726f 7669 6465 6420 696e 2074 6865 2063  rovided in the c
+00015a60: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+00015a70: 6f75 7020 6f72 0a20 2020 2020 2020 2020  oup or.         
+00015a80: 2020 2020 2020 2069 6e20 7468 6520 6765         in the ge
+00015a90: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
+00015aa0: 7572 655f 6772 6f75 7020 6d65 7468 6f64  ure_group method
+00015ab0: 2069 6e76 6f6b 6174 696f 6e2e 0a20 2020   invokation..   
+00015ac0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
+00015ad0: 7074 696f 6e73 3a20 4164 6469 7469 6f6e  ptions: Addition
+00015ae0: 616c 2077 7269 7465 206f 7074 696f 6e73  al write options
+00015af0: 2061 7320 6b65 792d 7661 6c75 6520 7061   as key-value pa
+00015b00: 6972 732c 2064 6566 6175 6c74 7320 746f  irs, defaults to
+00015b10: 2060 7b7d 602e 0a20 2020 2020 2020 2020   `{}`..         
+00015b20: 2020 2020 2020 2057 6865 6e20 7573 696e         When usin
+00015b30: 6720 7468 6520 6070 7974 686f 6e60 2065  g the `python` e
+00015b40: 6e67 696e 652c 2077 7269 7465 5f6f 7074  ngine, write_opt
+00015b50: 696f 6e73 2063 616e 2063 6f6e 7461 696e  ions can contain
+00015b60: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00015b70: 2020 2020 2066 6f6c 6c6f 7769 6e67 2065       following e
+00015b80: 6e74 7269 6573 3a0a 2020 2020 2020 2020  ntries:.        
+00015b90: 2020 2020 2020 2020 2a20 6b65 7920 6073          * key `s
+00015ba0: 7061 726b 6020 616e 6420 7661 6c75 6520  park` and value 
+00015bb0: 616e 206f 626a 6563 7420 6f66 2074 7970  an object of typ
+00015bc0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00015bd0: 2020 5b68 7366 732e 636f 7265 2e6a 6f62    [hsfs.core.job
+00015be0: 5f63 6f6e 6669 6775 7261 7469 6f6e 2e4a  _configuration.J
+00015bf0: 6f62 436f 6e66 6967 7572 6174 696f 6e5d  obConfiguration]
+00015c00: 282e 2e2f 6a6f 625f 636f 6e66 6967 7572  (../job_configur
+00015c10: 6174 696f 6e29 0a20 2020 2020 2020 2020  ation).         
+00015c20: 2020 2020 2020 2020 2074 6f20 636f 6e66           to conf
+00015c30: 6967 7572 6520 7468 6520 486f 7073 776f  igure the Hopswo
+00015c40: 726b 7320 4a6f 6220 7573 6564 2074 6f20  rks Job used to 
+00015c50: 7772 6974 6520 6461 7461 2069 6e74 6f20  write data into 
+00015c60: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00015c70: 2020 2020 2020 6665 6174 7572 6520 6772        feature gr
+00015c80: 6f75 702e 0a20 2020 2020 2020 2020 2020  oup..           
+00015c90: 2020 2020 202a 206b 6579 2060 7761 6974       * key `wait
+00015ca0: 5f66 6f72 5f6a 6f62 6020 616e 6420 7661  _for_job` and va
+00015cb0: 6c75 6520 6054 7275 6560 206f 7220 6046  lue `True` or `F
+00015cc0: 616c 7365 6020 746f 2063 6f6e 6669 6775  alse` to configu
+00015cd0: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+00015ce0: 2020 2020 2077 6865 7468 6572 206f 7220       whether or 
+00015cf0: 6e6f 7420 746f 2074 6865 2073 6176 6520  not to the save 
+00015d00: 6361 6c6c 2073 686f 756c 6420 7265 7475  call should retu
+00015d10: 726e 206f 6e6c 790a 2020 2020 2020 2020  rn only.        
+00015d20: 2020 2020 2020 2020 2020 6166 7465 7220            after 
+00015d30: 7468 6520 486f 7073 776f 726b 7320 4a6f  the Hopsworks Jo
+00015d40: 6220 6861 7320 6669 6e69 7368 6564 2e20  b has finished. 
+00015d50: 4279 2064 6566 6175 6c74 2069 7420 646f  By default it do
+00015d60: 6573 206e 6f74 2077 6169 742e 0a20 2020  es not wait..   
+00015d70: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+00015d80: 6579 2060 7374 6172 745f 6f66 666c 696e  ey `start_offlin
+00015d90: 655f 6261 636b 6669 6c6c 6020 616e 6420  e_backfill` and 
+00015da0: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
+00015db0: 6046 616c 7365 6020 746f 2063 6f6e 6669  `False` to confi
+00015dc0: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
+00015dd0: 2020 2020 2020 2077 6865 7468 6572 206f         whether o
+00015de0: 7220 6e6f 7420 746f 2073 7461 7274 2074  r not to start t
+00015df0: 6865 206d 6174 6572 6961 6c69 7a61 7469  he materializati
+00015e00: 6f6e 206a 6f62 2074 6f20 7772 6974 6520  on job to write 
+00015e10: 6461 7461 2074 6f20 7468 6520 6f66 666c  data to the offl
+00015e20: 696e 650a 2020 2020 2020 2020 2020 2020  ine.            
+00015e30: 2020 2020 2020 7374 6f72 6167 652e 2060        storage. `
+00015e40: 7374 6172 745f 6f66 666c 696e 655f 6261  start_offline_ba
+00015e50: 636b 6669 6c6c 6020 6973 2064 6570 7265  ckfill` is depre
+00015e60: 6361 7465 642e 2055 7365 2060 7374 6172  cated. Use `star
+00015e70: 745f 6f66 666c 696e 655f 6d61 7465 7269  t_offline_materi
+00015e80: 616c 697a 6174 696f 6e60 2069 6e73 7465  alization` inste
+00015e90: 6164 2e0a 2020 2020 2020 2020 2020 2020  ad..            
+00015ea0: 2020 2020 2a20 6b65 7920 6073 7461 7274      * key `start
+00015eb0: 5f6f 6666 6c69 6e65 5f6d 6174 6572 6961  _offline_materia
+00015ec0: 6c69 7a61 7469 6f6e 6020 616e 6420 7661  lization` and va
+00015ed0: 6c75 6520 6054 7275 6560 206f 7220 6046  lue `True` or `F
+00015ee0: 616c 7365 6020 746f 2063 6f6e 6669 6775  alse` to configu
+00015ef0: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+00015f00: 2020 2020 2077 6865 7468 6572 206f 7220       whether or 
+00015f10: 6e6f 7420 746f 2073 7461 7274 2074 6865  not to start the
+00015f20: 206d 6174 6572 6961 6c69 7a61 7469 6f6e   materialization
+00015f30: 206a 6f62 2074 6f20 7772 6974 6520 6461   job to write da
+00015f40: 7461 2074 6f20 7468 6520 6f66 666c 696e  ta to the offlin
+00015f50: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00015f60: 2020 2020 7374 6f72 6167 652e 2042 7920      storage. By 
+00015f70: 6465 6661 756c 7420 7468 6520 6d61 7465  default the mate
+00015f80: 7269 616c 697a 6174 696f 6e20 6a6f 6220  rialization job 
+00015f90: 6765 7473 2073 7461 7274 6564 2069 6d6d  gets started imm
+00015fa0: 6564 6961 7465 6c79 2e0a 2020 2020 2020  ediately..      
+00015fb0: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+00015fc0: 606b 6166 6b61 5f70 726f 6475 6365 725f  `kafka_producer_
+00015fd0: 636f 6e66 6967 6020 616e 6420 7661 6c75  config` and valu
+00015fe0: 6520 616e 206f 626a 6563 7420 6f66 2074  e an object of t
+00015ff0: 7970 6520 5b70 726f 7065 7274 6965 735d  ype [properties]
+00016000: 2868 7474 7073 3a2f 2f64 6f63 732e 636f  (https://docs.co
+00016010: 6e66 6c75 656e 742e 696f 2f70 6c61 7466  nfluent.io/platf
+00016020: 6f72 6d2f 6375 7272 656e 742f 636c 6965  orm/current/clie
+00016030: 6e74 732f 6c69 6272 646b 6166 6b61 2f68  nts/librdkafka/h
+00016040: 746d 6c2f 6d64 5f43 4f4e 4649 4755 5241  tml/md_CONFIGURA
+00016050: 5449 4f4e 2e68 746d 6c6e 290a 2020 2020  TION.htmln).    
+00016060: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00016070: 6564 2074 6f20 636f 6e66 6967 7572 6520  ed to configure 
+00016080: 7468 6520 4b61 666b 6120 636c 6965 6e74  the Kafka client
+00016090: 2e20 546f 206f 7074 696d 697a 6520 666f  . To optimize fo
+000160a0: 7220 7468 726f 7567 6870 7574 2069 6e20  r throughput in 
+000160b0: 6869 6768 206c 6174 656e 6379 2063 6f6e  high latency con
+000160c0: 6e65 6374 696f 6e2c 2063 6f6e 7369 6465  nection, conside
+000160d0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+000160e0: 2020 2020 6368 616e 6769 6e67 2074 6865      changing the
+000160f0: 205b 7072 6f64 7563 6572 2070 726f 7065   [producer prope
+00016100: 7274 6965 735d 2868 7474 7073 3a2f 2f64  rties](https://d
+00016110: 6f63 732e 636f 6e66 6c75 656e 742e 696f  ocs.confluent.io
+00016120: 2f63 6c6f 7564 2f63 7572 7265 6e74 2f63  /cloud/current/c
+00016130: 6c69 656e 742d 6170 7073 2f6f 7074 696d  lient-apps/optim
+00016140: 697a 696e 672f 7468 726f 7567 6870 7574  izing/throughput
+00016150: 2e68 746d 6c23 7072 6f64 7563 6572 292e  .html#producer).
+00016160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016170: 202a 206b 6579 2060 696e 7465 726e 616c   * key `internal
+00016180: 5f6b 6166 6b61 6020 616e 6420 7661 6c75  _kafka` and valu
+00016190: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
+000161a0: 7365 6020 696e 2063 6173 6520 796f 7520  se` in case you 
+000161b0: 6573 7461 626c 6973 6865 640a 2020 2020  established.    
+000161c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000161d0: 6e6e 6563 7469 7669 7479 2066 726f 6d20  nnectivity from 
+000161e0: 796f 7520 5079 7468 6f6e 2065 6e76 6972  you Python envir
+000161f0: 6f6e 6d65 6e74 2074 6f20 7468 6520 696e  onment to the in
+00016200: 7465 726e 616c 2061 6476 6572 7469 7365  ternal advertise
+00016210: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00016220: 2020 2020 6c69 7374 656e 6572 7320 6f66      listeners of
+00016230: 2074 6865 2048 6f70 7377 6f72 6b73 204b   the Hopsworks K
+00016240: 6166 6b61 2043 6c75 7374 6572 2e20 4465  afka Cluster. De
+00016250: 6661 756c 7473 2074 6f20 6046 616c 7365  faults to `False
+00016260: 6020 616e 640a 2020 2020 2020 2020 2020  ` and.          
+00016270: 2020 2020 2020 2020 7769 6c6c 2075 7365          will use
+00016280: 2065 7874 6572 6e61 6c20 6c69 7374 656e   external listen
+00016290: 6572 7320 7768 656e 2063 6f6e 6e65 6374  ers when connect
+000162a0: 696e 6720 6672 6f6d 206f 7574 7369 6465  ing from outside
+000162b0: 206f 6620 486f 7073 776f 726b 732e 0a20   of Hopsworks.. 
+000162c0: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+000162d0: 6174 696f 6e5f 6f70 7469 6f6e 733a 2041  ation_options: A
+000162e0: 6464 6974 696f 6e61 6c20 7661 6c69 6461  dditional valida
+000162f0: 7469 6f6e 206f 7074 696f 6e73 2061 7320  tion options as 
+00016300: 6b65 792d 7661 6c75 6520 7061 6972 732c  key-value pairs,
+00016310: 2064 6566 6175 6c74 7320 746f 2060 7b7d   defaults to `{}
+00016320: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
+00016330: 2020 202a 206b 6579 2060 7275 6e5f 7661     * key `run_va
+00016340: 6c69 6461 7469 6f6e 6020 626f 6f6c 6561  lidation` boolea
+00016350: 6e20 7661 6c75 652c 2073 6574 2074 6f20  n value, set to 
+00016360: 6046 616c 7365 6020 746f 2073 6b69 7020  `False` to skip 
+00016370: 7661 6c69 6461 7469 6f6e 2074 656d 706f  validation tempo
+00016380: 7261 7269 6c79 206f 6e20 696e 6765 7374  rarily on ingest
+00016390: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+000163a0: 2020 2020 202a 206b 6579 2060 7361 7665       * key `save
+000163b0: 5f72 6570 6f72 7460 2062 6f6f 6c65 616e  _report` boolean
+000163c0: 2076 616c 7565 2c20 7365 7420 746f 2060   value, set to `
+000163d0: 4661 6c73 6560 2074 6f20 736b 6970 2075  False` to skip u
+000163e0: 706c 6f61 6420 6f66 2074 6865 2076 616c  pload of the val
+000163f0: 6964 6174 696f 6e20 7265 706f 7274 2074  idation report t
+00016400: 6f20 486f 7073 776f 726b 732e 0a20 2020  o Hopsworks..   
+00016410: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+00016420: 6579 2060 6765 5f76 616c 6964 6174 655f  ey `ge_validate_
+00016430: 6b77 6172 6773 6020 6120 6469 6374 696f  kwargs` a dictio
+00016440: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00016450: 6b77 6172 6773 2066 6f72 2074 6865 2076  kwargs for the v
+00016460: 616c 6964 6174 6520 6d65 7468 6f64 206f  alidate method o
+00016470: 6620 4772 6561 7420 4578 7065 6374 6174  f Great Expectat
+00016480: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+00016490: 2020 7761 6974 3a20 5761 6974 2066 6f72    wait: Wait for
+000164a0: 206a 6f62 2074 6f20 6669 6e69 7368 2062   job to finish b
+000164b0: 6566 6f72 6520 7265 7475 726e 696e 672c  efore returning,
+000164c0: 2064 6566 6175 6c74 7320 746f 2060 4661   defaults to `Fa
+000164d0: 6c73 6560 2e0a 2020 2020 2020 2020 2020  lse`..          
+000164e0: 2020 2020 2020 5368 6f72 7463 7574 2066        Shortcut f
+000164f0: 6f72 2072 6561 645f 6f70 7469 6f6e 7320  or read_options 
+00016500: 607b 2277 6169 745f 666f 725f 6a6f 6222  `{"wait_for_job"
+00016510: 3a20 4661 6c73 657d 602e 0a0a 2020 2020  : False}`...    
+00016520: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00016530: 2020 2020 2020 2020 2020 604a 6f62 603a            `Job`:
+00016540: 2057 6865 6e20 7573 696e 6720 7468 6520   When using the 
+00016550: 6070 7974 686f 6e60 2065 6e67 696e 652c  `python` engine,
+00016560: 2069 7420 7265 7475 726e 7320 7468 6520   it returns the 
+00016570: 486f 7073 776f 726b 7320 4a6f 620a 2020  Hopsworks Job.  
+00016580: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00016590: 6174 2077 6173 206c 6175 6e63 6865 6420  at was launched 
+000165a0: 746f 2069 6e67 6573 7420 7468 6520 6665  to ingest the fe
+000165b0: 6174 7572 6520 6772 6f75 7020 6461 7461  ature group data
+000165c0: 2e0a 0a20 2020 2020 2020 2023 2052 6169  ...        # Rai
+000165d0: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
+000165e0: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
+000165f0: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
+00016600: 7272 6f72 602e 2055 6e61 626c 6520 746f  rror`. Unable to
+00016610: 2063 7265 6174 6520 6665 6174 7572 6520   create feature 
+00016620: 6772 6f75 702e 0a20 2020 2020 2020 2022  group..        "
+00016630: 2222 0a20 2020 2020 2020 2069 6620 2866  "".        if (f
+00016640: 6561 7475 7265 7320 6973 204e 6f6e 6520  eatures is None 
+00016650: 616e 6420 6c65 6e28 7365 6c66 2e5f 6665  and len(self._fe
+00016660: 6174 7572 6573 2920 3e20 3029 206f 7220  atures) > 0) or 
+00016670: 280a 2020 2020 2020 2020 2020 2020 6973  (.            is
+00016680: 696e 7374 616e 6365 2866 6561 7475 7265  instance(feature
+00016690: 732c 204c 6973 7429 0a20 2020 2020 2020  s, List).       
+000166a0: 2020 2020 2061 6e64 206c 656e 2866 6561       and len(fea
+000166b0: 7475 7265 7329 203e 2030 0a20 2020 2020  tures) > 0.     
+000166c0: 2020 2020 2020 2061 6e64 2061 6c6c 285b         and all([
+000166d0: 6973 696e 7374 616e 6365 2866 2c20 6665  isinstance(f, fe
+000166e0: 6174 7572 652e 4665 6174 7572 6529 2066  ature.Feature) f
+000166f0: 6f72 2066 2069 6e20 6665 6174 7572 6573  or f in features
+00016700: 5d29 0a20 2020 2020 2020 2029 3a0a 2020  ]).        ):.  
+00016710: 2020 2020 2020 2020 2020 2320 5468 6973            # This
+00016720: 2069 7320 646f 6e65 2066 6f72 2063 6f6d   is done for com
+00016730: 7061 7469 6269 6c69 7479 2e20 5573 6572  patibility. User
+00016740: 7320 6361 6e20 7370 6563 6966 7920 7468  s can specify th
+00016750: 6520 6665 6174 7572 6520 6c69 7374 2069  e feature list i
+00016760: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
+00016770: 2020 2320 2867 6574 5f6f 725f 2963 7265    # (get_or_)cre
+00016780: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+00016790: 702e 2055 7365 7273 2063 616e 2061 6c73  p. Users can als
+000167a0: 6f20 7072 6f76 6964 6520 7468 6520 6665  o provide the fe
+000167b0: 6174 7572 6520 6c69 7374 2069 6e20 7468  ature list in th
+000167c0: 6520 7361 7665 2829 2e0a 2020 2020 2020  e save()..      
+000167d0: 2020 2020 2020 2320 5468 6f75 6768 2069        # Though i
+000167e0: 7427 7320 616e 206f 7074 696f 6e61 6c20  t's an optional 
+000167f0: 7061 7261 6d65 7465 722e 0a20 2020 2020  parameter..     
+00016800: 2020 2020 2020 2023 2046 6f72 2063 6f6e         # For con
+00016810: 7369 7374 656e 6379 2072 6561 736f 6e73  sistency reasons
+00016820: 2069 6620 7468 6520 7573 6572 2073 7065   if the user spe
+00016830: 6369 6679 2062 6f74 6820 7468 6520 6665  cify both the fe
+00016840: 6174 7572 6520 6c69 7374 2069 6e20 7468  ature list in th
+00016850: 6520 2867 6574 5f6f 725f 2963 7265 6174  e (get_or_)creat
+00016860: 655f 6665 6174 7572 655f 6772 6f75 700a  e_feature_group.
+00016870: 2020 2020 2020 2020 2020 2020 2320 616e              # an
+00016880: 6420 696e 2074 6865 2060 7361 7665 2829  d in the `save()
+00016890: 6020 6361 6c6c 2c20 7468 656e 2074 6865  ` call, then the
+000168a0: 2028 6765 745f 6f72 5f29 6372 6561 7465   (get_or_)create
+000168b0: 5f66 6561 7475 7265 5f67 726f 7570 2077  _feature_group w
+000168c0: 696e 732e 0a20 2020 2020 2020 2020 2020  ins..           
+000168d0: 2023 2054 6869 7320 6973 2063 6f6e 7369   # This is consi
+000168e0: 7374 656e 7420 7769 7468 2074 6865 2062  stent with the b
+000168f0: 6568 6176 696f 7220 6f66 2074 6865 2069  ehavior of the i
+00016900: 6e73 6572 7420 6d65 7468 6f64 2077 6865  nsert method whe
+00016910: 7265 2074 6865 2066 6561 7475 7265 206c  re the feature l
+00016920: 6973 7420 7769 6e73 206f 7665 7220 7468  ist wins over th
+00016930: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
+00016940: 6461 7461 6672 616d 6520 7374 7275 6374  dataframe struct
+00016950: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
+00016960: 7365 6c66 2e5f 6665 6174 7572 6573 203d  self._features =
+00016970: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
+00016980: 6966 206c 656e 2873 656c 662e 5f66 6561  if len(self._fea
+00016990: 7475 7265 7329 203e 2030 2065 6c73 6520  tures) > 0 else 
+000169a0: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
+000169b0: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
+000169c0: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
+000169d0: 7361 7665 5f66 6561 7475 7265 5f67 726f  save_feature_gro
+000169e0: 7570 5f6d 6574 6164 6174 6128 0a20 2020  up_metadata(.   
+000169f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016a00: 662c 204e 6f6e 652c 2077 7269 7465 5f6f  f, None, write_o
+00016a10: 7074 696f 6e73 0a20 2020 2020 2020 2020  ptions.         
+00016a20: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00016a30: 2020 7265 7475 726e 204e 6f6e 652c 204e    return None, N
+00016a40: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
+00016a50: 6665 6174 7572 6573 2069 7320 4e6f 6e65  features is None
+00016a60: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00016a70: 6973 6520 4665 6174 7572 6553 746f 7265  ise FeatureStore
+00016a80: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+00016a90: 2020 2020 2020 2020 2020 2022 4665 6174             "Feat
+00016aa0: 7572 6520 6c69 7374 206e 6f74 2070 726f  ure list not pro
+00016ab0: 7669 6465 6420 696e 2074 6865 2063 7265  vided in the cre
+00016ac0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+00016ad0: 7020 6f72 2067 6574 5f6f 725f 6372 6561  p or get_or_crea
+00016ae0: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+00016af0: 2069 6e76 6f6b 6174 696f 6e73 2e22 0a20   invokations.". 
+00016b00: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00016b10: 2022 2050 6c65 6173 6520 7072 6f76 6964   " Please provid
+00016b20: 6520 6120 6c69 7374 206f 6620 6665 6174  e a list of feat
+00016b30: 7572 6573 206f 7220 6120 4461 7461 6672  ures or a Datafr
+00016b40: 616d 6522 0a20 2020 2020 2020 2020 2020  ame".           
+00016b50: 2029 0a0a 2020 2020 2020 2020 6665 6174   )..        feat
+00016b60: 7572 655f 6461 7461 6672 616d 6520 3d20  ure_dataframe = 
+00016b70: 656e 6769 6e65 2e67 6574 5f69 6e73 7461  engine.get_insta
+00016b80: 6e63 6528 292e 636f 6e76 6572 745f 746f  nce().convert_to
+00016b90: 5f64 6566 6175 6c74 5f64 6174 6166 7261  _default_datafra
+00016ba0: 6d65 2866 6561 7475 7265 7329 0a0a 2020  me(features)..  
+00016bb0: 2020 2020 2020 7573 6572 5f76 6572 7369        user_versi
+00016bc0: 6f6e 203d 2073 656c 662e 5f76 6572 7369  on = self._versi
+00016bd0: 6f6e 0a0a 2020 2020 2020 2020 6966 2077  on..        if w
+00016be0: 7269 7465 5f6f 7074 696f 6e73 2069 7320  rite_options is 
+00016bf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016c00: 2020 7772 6974 655f 6f70 7469 6f6e 7320    write_options 
+00016c10: 3d20 7b7d 0a20 2020 2020 2020 2069 6620  = {}.        if 
+00016c20: 2277 6169 745f 666f 725f 6a6f 6222 206e  "wait_for_job" n
+00016c30: 6f74 2069 6e20 7772 6974 655f 6f70 7469  ot in write_opti
+00016c40: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00016c50: 2077 7269 7465 5f6f 7074 696f 6e73 5b22   write_options["
+00016c60: 7761 6974 5f66 6f72 5f6a 6f62 225d 203d  wait_for_job"] =
+00016c70: 2077 6169 740a 0a20 2020 2020 2020 2023   wait..        #
+00016c80: 2066 675f 6a6f 6220 6973 2075 7365 6420   fg_job is used 
+00016c90: 6f6e 6c79 2069 6620 7468 6520 7079 7468  only if the pyth
+00016ca0: 6f6e 2065 6e67 696e 6520 6973 2075 7365  on engine is use
+00016cb0: 640a 2020 2020 2020 2020 6667 5f6a 6f62  d.        fg_job
+00016cc0: 2c20 6765 5f72 6570 6f72 7420 3d20 7365  , ge_report = se
+00016cd0: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+00016ce0: 705f 656e 6769 6e65 2e73 6176 6528 0a20  p_engine.save(. 
+00016cf0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00016d00: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
+00016d10: 6d65 2c20 7772 6974 655f 6f70 7469 6f6e  me, write_option
+00016d20: 732c 2076 616c 6964 6174 696f 6e5f 6f70  s, validation_op
+00016d30: 7469 6f6e 730a 2020 2020 2020 2020 290a  tions.        ).
+00016d40: 2020 2020 2020 2020 6966 2067 655f 7265          if ge_re
+00016d50: 706f 7274 2069 7320 4e6f 6e65 206f 7220  port is None or 
+00016d60: 6765 5f72 6570 6f72 742e 696e 6765 7374  ge_report.ingest
+00016d70: 696f 6e5f 7265 7375 6c74 203d 3d20 2249  ion_result == "I
+00016d80: 4e47 4553 5445 4422 3a0a 2020 2020 2020  NGESTED":.      
+00016d90: 2020 2020 2020 7365 6c66 2e5f 636f 6465        self._code
+00016da0: 5f65 6e67 696e 652e 7361 7665 5f63 6f64  _engine.save_cod
+00016db0: 6528 7365 6c66 290a 0a20 2020 2020 2020  e(self)..       
+00016dc0: 2069 6620 7365 6c66 2e73 7461 7469 7374   if self.statist
+00016dd0: 6963 735f 636f 6e66 6967 2e65 6e61 626c  ics_config.enabl
+00016de0: 6564 2061 6e64 2065 6e67 696e 652e 6765  ed and engine.ge
+00016df0: 745f 7479 7065 2829 2e73 7461 7274 7377  t_type().startsw
+00016e00: 6974 6828 2273 7061 726b 2229 3a0a 2020  ith("spark"):.  
+00016e10: 2020 2020 2020 2020 2020 2320 4f6e 6c79            # Only
+00016e20: 2063 6f6d 7075 7465 2073 7461 7469 7374   compute statist
+00016e30: 6963 7320 6966 2074 6865 2065 6e67 696e  ics if the engin
+00016e40: 6520 6973 2053 7061 726b 2e0a 2020 2020  e is Spark..    
+00016e50: 2020 2020 2020 2020 2320 466f 7220 5079          # For Py
+00016e60: 7468 6f6e 2065 6e67 696e 652c 2074 6865  thon engine, the
+00016e70: 2063 6f6d 7075 7461 7469 6f6e 2068 6170   computation hap
+00016e80: 7065 6e73 2069 6e20 7468 6520 486f 7073  pens in the Hops
+00016e90: 776f 726b 7320 6170 706c 6963 6174 696f  works applicatio
+00016ea0: 6e0a 2020 2020 2020 2020 2020 2020 7365  n.            se
+00016eb0: 6c66 2e5f 7374 6174 6973 7469 6373 5f65  lf._statistics_e
+00016ec0: 6e67 696e 652e 636f 6d70 7574 655f 616e  ngine.compute_an
+00016ed0: 645f 7361 7665 5f73 7461 7469 7374 6963  d_save_statistic
+00016ee0: 7328 7365 6c66 2c20 6665 6174 7572 655f  s(self, feature_
+00016ef0: 6461 7461 6672 616d 6529 0a20 2020 2020  dataframe).     
+00016f00: 2020 2069 6620 7573 6572 5f76 6572 7369     if user_versi
+00016f10: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00016f20: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+00016f30: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
+00016f40: 2020 2020 2020 2022 4e6f 2076 6572 7369         "No versi
+00016f50: 6f6e 2070 726f 7669 6465 6420 666f 7220  on provided for 
+00016f60: 6372 6561 7469 6e67 2066 6561 7475 7265  creating feature
+00016f70: 2067 726f 7570 2060 7b7d 602c 2069 6e63   group `{}`, inc
+00016f80: 7265 6d65 6e74 6564 2076 6572 7369 6f6e  remented version
+00016f90: 2074 6f20 607b 7d60 2e22 2e66 6f72 6d61   to `{}`.".forma
+00016fa0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00016fb0: 2020 2020 2020 2073 656c 662e 5f6e 616d         self._nam
+00016fc0: 652c 2073 656c 662e 5f76 6572 7369 6f6e  e, self._version
+00016fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016fe0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00016ff0: 2020 2020 7574 696c 2e56 6572 7369 6f6e      util.Version
+00017000: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
+00017010: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+00017020: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+00017030: 2020 2020 6667 5f6a 6f62 2c0a 2020 2020      fg_job,.    
+00017040: 2020 2020 2020 2020 6765 5f72 6570 6f72          ge_repor
+00017050: 742e 746f 5f67 655f 7479 7065 2829 2069  t.to_ge_type() i
+00017060: 6620 6765 5f72 6570 6f72 7420 6973 206e  f ge_report is n
+00017070: 6f74 204e 6f6e 6520 656c 7365 204e 6f6e  ot None else Non
+00017080: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
+00017090: 2020 6465 6620 696e 7365 7274 280a 2020    def insert(.  
+000170a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000170b0: 2020 2020 6665 6174 7572 6573 3a20 556e      features: Un
+000170c0: 696f 6e5b 0a20 2020 2020 2020 2020 2020  ion[.           
+000170d0: 2070 642e 4461 7461 4672 616d 652c 0a20   pd.DataFrame,. 
+000170e0: 2020 2020 2020 2020 2020 2054 7970 6556             TypeV
+000170f0: 6172 2822 7079 7370 6172 6b2e 7371 6c2e  ar("pyspark.sql.
+00017100: 4461 7461 4672 616d 6522 292c 2020 2320  DataFrame"),  # 
+00017110: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
+00017120: 2020 2020 2020 2054 7970 6556 6172 2822         TypeVar("
+00017130: 7079 7370 6172 6b2e 5244 4422 292c 2020  pyspark.RDD"),  
+00017140: 2320 6e6f 7161 3a20 4638 3231 0a20 2020  # noqa: F821.   
+00017150: 2020 2020 2020 2020 206e 702e 6e64 6172           np.ndar
+00017160: 7261 792c 0a20 2020 2020 2020 2020 2020  ray,.           
+00017170: 204c 6973 745b 6c69 7374 5d2c 0a20 2020   List[list],.   
+00017180: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017190: 6f76 6572 7772 6974 653a 204f 7074 696f  overwrite: Optio
+000171a0: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
+000171b0: 652c 0a20 2020 2020 2020 206f 7065 7261  e,.        opera
+000171c0: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b73  tion: Optional[s
+000171d0: 7472 5d20 3d20 2275 7073 6572 7422 2c0a  tr] = "upsert",.
+000171e0: 2020 2020 2020 2020 7374 6f72 6167 653a          storage:
+000171f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00017200: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
+00017210: 7269 7465 5f6f 7074 696f 6e73 3a20 4f70  rite_options: Op
+00017220: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00017230: 2041 6e79 5d5d 203d 207b 7d2c 0a20 2020   Any]] = {},.   
+00017240: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+00017250: 6f70 7469 6f6e 733a 204f 7074 696f 6e61  options: Optiona
+00017260: 6c5b 4469 6374 5b73 7472 2c20 416e 795d  l[Dict[str, Any]
+00017270: 5d20 3d20 7b7d 2c0a 2020 2020 2020 2020  ] = {},.        
+00017280: 7361 7665 5f63 6f64 653a 204f 7074 696f  save_code: Optio
+00017290: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
+000172a0: 2c0a 2020 2020 2020 2020 7761 6974 3a20  ,.        wait: 
+000172b0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+000172c0: 2020 2920 2d3e 2054 7570 6c65 5b4f 7074    ) -> Tuple[Opt
+000172d0: 696f 6e61 6c5b 4a6f 625d 2c20 4f70 7469  ional[Job], Opti
+000172e0: 6f6e 616c 5b56 616c 6964 6174 696f 6e52  onal[ValidationR
+000172f0: 6570 6f72 745d 5d3a 0a20 2020 2020 2020  eport]]:.       
+00017300: 2022 2222 5065 7273 6973 7420 7468 6520   """Persist the 
+00017310: 6d65 7461 6461 7461 2061 6e64 206d 6174  metadata and mat
+00017320: 6572 6961 6c69 7a65 2074 6865 2066 6561  erialize the fea
+00017330: 7475 7265 2067 726f 7570 2074 6f20 7468  ture group to th
+00017340: 6520 6665 6174 7572 6520 7374 6f72 650a  e feature store.
+00017350: 2020 2020 2020 2020 6f72 2069 6e73 6572          or inser
+00017360: 7420 6461 7461 2066 726f 6d20 6120 6461  t data from a da
+00017370: 7461 6672 616d 6520 696e 746f 2074 6865  taframe into the
+00017380: 2065 7869 7374 696e 6720 6665 6174 7572   existing featur
+00017390: 6520 6772 6f75 702e 0a0a 2020 2020 2020  e group...      
+000173a0: 2020 496e 6372 656d 656e 7461 6c6c 7920    Incrementally 
+000173b0: 696e 7365 7274 2064 6174 6120 746f 2061  insert data to a
+000173c0: 2066 6561 7475 7265 2067 726f 7570 206f   feature group o
+000173d0: 7220 6f76 6572 7772 6974 6520 616c 6c20  r overwrite all 
+000173e0: 6461 7461 2063 6f6e 7461 696e 6564 2069  data contained i
+000173f0: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
+00017400: 6f75 702e 2042 790a 2020 2020 2020 2020  oup. By.        
+00017410: 6465 6661 756c 742c 2074 6865 2064 6174  default, the dat
+00017420: 6120 6973 2069 6e73 6572 7465 6420 696e  a is inserted in
+00017430: 746f 2074 6865 206f 6666 6c69 6e65 2073  to the offline s
+00017440: 746f 7261 6765 2061 7320 7765 6c6c 2061  torage as well a
+00017450: 7320 7468 6520 6f6e 6c69 6e65 2073 746f  s the online sto
+00017460: 7261 6765 2069 6620 7468 6520 6665 6174  rage if the feat
+00017470: 7572 6520 6772 6f75 7020 6973 0a20 2020  ure group is.   
+00017480: 2020 2020 2060 6f6e 6c69 6e65 5f65 6e61       `online_ena
+00017490: 626c 6564 3d54 7275 6560 2e0a 0a20 2020  bled=True`...   
+000174a0: 2020 2020 2054 6865 2060 6665 6174 7572       The `featur
+000174b0: 6573 6020 6461 7461 6672 616d 6520 6361  es` dataframe ca
+000174c0: 6e20 6265 2061 2053 7061 726b 2044 6174  n be a Spark Dat
+000174d0: 6146 7261 6d65 206f 7220 5244 442c 2061  aFrame or RDD, a
+000174e0: 2050 616e 6461 7320 4461 7461 4672 616d   Pandas DataFram
+000174f0: 652c 0a20 2020 2020 2020 206f 7220 6120  e,.        or a 
+00017500: 7477 6f2d 6469 6d65 6e73 696f 6e61 6c20  two-dimensional 
+00017510: 4e75 6d70 7920 6172 7261 7920 6f72 2061  Numpy array or a
+00017520: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
+00017530: 2050 7974 686f 6e20 6e65 7374 6564 206c   Python nested l
+00017540: 6973 742e 0a20 2020 2020 2020 2049 6620  ist..        If 
+00017550: 7374 6174 6973 7469 6373 2061 7265 2065  statistics are e
+00017560: 6e61 626c 6564 2c20 7374 6174 6973 7469  nabled, statisti
+00017570: 6373 2061 7265 2072 6563 6f6d 7075 7465  cs are recompute
+00017580: 6420 666f 7220 7468 6520 656e 7469 7265  d for the entire
+00017590: 2066 6561 7475 7265 0a20 2020 2020 2020   feature.       
+000175a0: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
+000175b0: 4966 2066 6561 7475 7265 2067 726f 7570  If feature group
+000175c0: 2773 2074 696d 6520 7472 6176 656c 2066  's time travel f
+000175d0: 6f72 6d61 7420 6973 2060 4855 4449 6020  ormat is `HUDI` 
+000175e0: 7468 656e 2060 6f70 6572 6174 696f 6e60  then `operation`
+000175f0: 2061 7267 756d 656e 7420 6361 6e20 6265   argument can be
+00017600: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
+00017610: 6069 6e73 6572 7460 206f 7220 6075 7073  `insert` or `ups
+00017620: 6572 7460 2e0a 0a20 2020 2020 2020 2049  ert`...        I
+00017630: 6620 6665 6174 7572 6520 6772 6f75 7020  f feature group 
+00017640: 646f 6573 6e27 7420 6578 6973 7420 7468  doesn't exist th
+00017650: 6520 696e 7365 7274 206d 6574 686f 6420  e insert method 
+00017660: 7769 6c6c 2063 7265 6174 6520 7468 6520  will create the 
+00017670: 6e65 6365 7373 6172 7920 6d65 7461 6461  necessary metada
+00017680: 7461 2074 6865 2066 6972 7374 2074 696d  ta the first tim
+00017690: 6520 6974 2069 730a 2020 2020 2020 2020  e it is.        
+000176a0: 696e 766f 6b65 6420 616e 6420 7772 6974  invoked and writ
+000176b0: 6573 2074 6865 2073 7065 6369 6669 6564  es the specified
+000176c0: 2060 6665 6174 7572 6573 6020 6461 7461   `features` data
+000176d0: 6672 616d 6520 6173 2066 6561 7475 7265  frame as feature
+000176e0: 2067 726f 7570 2074 6f20 7468 6520 6f6e   group to the on
+000176f0: 6c69 6e65 2f6f 6666 6c69 6e65 2066 6561  line/offline fea
+00017700: 7475 7265 2073 746f 7265 2e0a 0a20 2020  ture store...   
+00017710: 2020 2020 2021 2121 2077 6172 6e69 6e67       !!! warning
+00017720: 2022 4368 616e 6765 6420 696e 2033 2e33   "Changed in 3.3
+00017730: 2e30 220a 2020 2020 2020 2020 2020 2020  .0".            
+00017740: 6069 6e73 6572 7460 2061 6e64 2060 7361  `insert` and `sa
+00017750: 7665 6020 6d65 7468 6f64 7320 6172 6520  ve` methods are 
+00017760: 6e6f 7720 6173 796e 6320 6279 2064 6566  now async by def
+00017770: 6175 6c74 2069 6e20 6e6f 6e2d 7370 6172  ault in non-spar
+00017780: 6b20 636c 6965 6e74 732e 0a20 2020 2020  k clients..     
+00017790: 2020 2020 2020 2054 6f20 6163 6869 6576         To achiev
+000177a0: 6520 7468 6520 6f6c 6420 6265 6861 7669  e the old behavi
+000177b0: 6f75 722c 2073 6574 2060 7761 6974 6020  our, set `wait` 
+000177c0: 6172 6775 6d65 6e74 2074 6f20 6054 7275  argument to `Tru
+000177d0: 6560 2e0a 0a20 2020 2020 2020 2021 2121  e`...        !!!
+000177e0: 2065 7861 6d70 6c65 2022 5570 7365 7274   example "Upsert
+000177f0: 206e 6577 2066 6561 7475 7265 2064 6174   new feature dat
+00017800: 6120 7769 7468 2074 696d 6520 7472 6176  a with time trav
+00017810: 656c 2066 6f72 6d61 7420 6048 5544 4960  el format `HUDI`
+00017820: 220a 2020 2020 2020 2020 2020 2020 6060  ".            ``
+00017830: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00017840: 2020 2020 2320 636f 6e6e 6563 7420 746f      # connect to
+00017850: 2074 6865 2046 6561 7475 7265 2053 746f   the Feature Sto
+00017860: 7265 0a20 2020 2020 2020 2020 2020 2066  re.            f
+00017870: 7320 3d20 2e2e 2e0a 0a20 2020 2020 2020  s = .....       
+00017880: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
+00017890: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
+000178a0: 7265 5f67 726f 7570 280a 2020 2020 2020  re_group(.      
+000178b0: 2020 2020 2020 2020 2020 6e61 6d65 3d27            name='
+000178c0: 6269 7463 6f69 6e5f 7072 6963 6527 2c0a  bitcoin_price',.
+000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178e0: 6465 7363 7269 7074 696f 6e3d 2742 6974  description='Bit
+000178f0: 636f 696e 2070 7269 6365 2061 6767 7265  coin price aggre
+00017900: 6761 7465 6420 666f 7220 6461 7973 272c  gated for days',
+00017910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017920: 2076 6572 7369 6f6e 3d31 2c0a 2020 2020   version=1,.    
+00017930: 2020 2020 2020 2020 2020 2020 7072 696d              prim
+00017940: 6172 795f 6b65 793d 5b27 756e 6978 275d  ary_key=['unix']
+00017950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017960: 2020 6f6e 6c69 6e65 5f65 6e61 626c 6564    online_enabled
+00017970: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00017980: 2020 2020 2020 2065 7665 6e74 5f74 696d         event_tim
+00017990: 653d 2775 6e69 7827 0a20 2020 2020 2020  e='unix'.       
+000179a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000179b0: 2020 2020 6667 2e69 6e73 6572 7428 6466      fg.insert(df
+000179c0: 5f62 6974 636f 696e 5f70 726f 6365 7373  _bitcoin_process
+000179d0: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
+000179e0: 6060 600a 0a20 2020 2020 2020 2021 2121  ```..        !!!
+000179f0: 2065 7861 6d70 6c65 2022 4173 796e 6320   example "Async 
+00017a00: 696e 7365 7274 220a 2020 2020 2020 2020  insert".        
+00017a10: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+00017a20: 2020 2020 2020 2020 2020 2320 636f 6e6e            # conn
+00017a30: 6563 7420 746f 2074 6865 2046 6561 7475  ect to the Featu
+00017a40: 7265 2053 746f 7265 0a20 2020 2020 2020  re Store.       
+00017a50: 2020 2020 2066 7320 3d20 2e2e 2e0a 0a20       fs = ..... 
+00017a60: 2020 2020 2020 2020 2020 2066 6731 203d             fg1 =
+00017a70: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+00017a80: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+00017a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017aa0: 206e 616d 653d 2766 6561 7475 7265 5f67   name='feature_g
+00017ab0: 726f 7570 5f6e 616d 6531 272c 0a20 2020  roup_name1',.   
+00017ac0: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00017ad0: 6372 6970 7469 6f6e 3d27 4465 7363 7269  cription='Descri
+00017ae0: 7074 696f 6e20 6f66 2074 6865 2066 6972  ption of the fir
+00017af0: 7374 2046 4727 2c0a 2020 2020 2020 2020  st FG',.        
+00017b00: 2020 2020 2020 2020 7665 7273 696f 6e3d          version=
+00017b10: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+00017b20: 2020 2070 7269 6d61 7279 5f6b 6579 3d5b     primary_key=[
+00017b30: 2775 6e69 7827 5d2c 0a20 2020 2020 2020  'unix'],.       
+00017b40: 2020 2020 2020 2020 206f 6e6c 696e 655f           online_
+00017b50: 656e 6162 6c65 643d 5472 7565 2c0a 2020  enabled=True,.  
+00017b60: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00017b70: 656e 745f 7469 6d65 3d27 756e 6978 270a  ent_time='unix'.
+00017b80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00017b90: 2020 2020 2020 2020 2020 2320 6173 796e            # asyn
+00017ba0: 6320 696e 7365 7274 696f 6e20 696e 206f  c insertion in o
+00017bb0: 7264 6572 206e 6f74 2074 6f20 7761 6974  rder not to wait
+00017bc0: 2074 696c 6c20 6669 6e69 7368 206f 6620   till finish of 
+00017bd0: 7468 6520 6a6f 620a 2020 2020 2020 2020  the job.        
+00017be0: 2020 2020 6667 2e69 6e73 6572 7428 6466      fg.insert(df
+00017bf0: 5f66 6f72 5f66 6731 2c20 7772 6974 655f  _for_fg1, write_
+00017c00: 6f70 7469 6f6e 733d 7b22 7761 6974 5f66  options={"wait_f
+00017c10: 6f72 5f6a 6f62 2220 3a20 4661 6c73 657d  or_job" : False}
+00017c20: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00017c30: 6732 203d 2066 732e 6765 745f 6f72 5f63  g2 = fs.get_or_c
+00017c40: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+00017c50: 6f75 7028 0a20 2020 2020 2020 2020 2020  oup(.           
+00017c60: 2020 2020 206e 616d 653d 2766 6561 7475       name='featu
+00017c70: 7265 5f67 726f 7570 5f6e 616d 6532 272c  re_group_name2',
+00017c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c90: 2064 6573 6372 6970 7469 6f6e 3d27 4465   description='De
+00017ca0: 7363 7269 7074 696f 6e20 6f66 2074 6865  scription of the
+00017cb0: 2073 6563 6f6e 6420 4647 272c 0a20 2020   second FG',.   
+00017cc0: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+00017cd0: 7369 6f6e 3d31 2c0a 2020 2020 2020 2020  sion=1,.        
+00017ce0: 2020 2020 2020 2020 7072 696d 6172 795f          primary_
+00017cf0: 6b65 793d 5b27 756e 6978 275d 2c0a 2020  key=['unix'],.  
+00017d00: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+00017d10: 6c69 6e65 5f65 6e61 626c 6564 3d54 7275  line_enabled=Tru
+00017d20: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00017d30: 2020 2065 7665 6e74 5f74 696d 653d 2775     event_time='u
+00017d40: 6e69 7827 0a20 2020 2020 2020 2020 2020  nix'.           
+00017d50: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
+00017d60: 672e 696e 7365 7274 2864 665f 666f 725f  g.insert(df_for_
+00017d70: 6667 3229 0a20 2020 2020 2020 2020 2020  fg2).           
+00017d80: 2060 6060 0a0a 2020 2020 2020 2020 2320   ```..        # 
+00017d90: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
+00017da0: 2020 2020 2020 6665 6174 7572 6573 3a20        features: 
+00017db0: 4461 7461 4672 616d 652c 2052 4444 2c20  DataFrame, RDD, 
+00017dc0: 4e64 6172 7261 792c 206c 6973 742e 2046  Ndarray, list. F
+00017dd0: 6561 7475 7265 7320 746f 2062 6520 7361  eatures to be sa
+00017de0: 7665 642e 0a20 2020 2020 2020 2020 2020  ved..           
+00017df0: 206f 7665 7277 7269 7465 3a20 4472 6f70   overwrite: Drop
+00017e00: 2061 6c6c 2064 6174 6120 696e 2074 6865   all data in the
+00017e10: 2066 6561 7475 7265 2067 726f 7570 2062   feature group b
+00017e20: 6566 6f72 650a 2020 2020 2020 2020 2020  efore.          
+00017e30: 2020 2020 2020 696e 7365 7274 696e 6720        inserting 
+00017e40: 6e65 7720 6461 7461 2e20 5468 6973 2064  new data. This d
+00017e50: 6f65 7320 6e6f 7420 6166 6665 6374 206d  oes not affect m
+00017e60: 6574 6164 6174 612c 2064 6566 6175 6c74  etadata, default
+00017e70: 7320 746f 2046 616c 7365 2e0a 2020 2020  s to False..    
+00017e80: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+00017e90: 6e3a 2041 7061 6368 6520 4875 6469 206f  n: Apache Hudi o
+00017ea0: 7065 7261 7469 6f6e 2074 7970 6520 6022  peration type `"
+00017eb0: 696e 7365 7274 2260 206f 7220 6022 7570  insert"` or `"up
+00017ec0: 7365 7274 2260 2e0a 2020 2020 2020 2020  sert"`..        
+00017ed0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+00017ee0: 2074 6f20 6022 7570 7365 7274 2260 2e0a   to `"upsert"`..
+00017ef0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+00017f00: 6167 653a 204f 7665 7277 7269 7465 2064  age: Overwrite d
+00017f10: 6566 6175 6c74 2062 6568 6176 696f 7572  efault behaviour
+00017f20: 2c20 7772 6974 6520 746f 206f 6666 6c69  , write to offli
+00017f30: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00017f40: 2020 2073 746f 7261 6765 206f 6e6c 7920     storage only 
+00017f50: 7769 7468 2060 226f 6666 6c69 6e65 2260  with `"offline"`
+00017f60: 206f 7220 6f6e 6c69 6e65 206f 6e6c 7920   or online only 
+00017f70: 7769 7468 2060 226f 6e6c 696e 6522 602c  with `"online"`,
+00017f80: 2064 6566 6175 6c74 730a 2020 2020 2020   defaults.      
+00017f90: 2020 2020 2020 2020 2020 746f 2060 4e6f            to `No
+00017fa0: 6e65 6020 2849 6620 7468 6520 7374 7265  ne` (If the stre
+00017fb0: 616d 696e 6720 4150 4973 2061 7265 2065  aming APIs are e
+00017fc0: 6e61 626c 6564 2c20 7370 6563 6966 7969  nabled, specifyi
+00017fd0: 6e67 2074 6865 2073 746f 7261 6765 206f  ng the storage o
+00017fe0: 7074 696f 6e20 6973 206e 6f74 2073 7570  ption is not sup
+00017ff0: 706f 7274 6564 292e 0a20 2020 2020 2020  ported)..       
+00018000: 2020 2020 2077 7269 7465 5f6f 7074 696f       write_optio
+00018010: 6e73 3a20 4164 6469 7469 6f6e 616c 2077  ns: Additional w
+00018020: 7269 7465 206f 7074 696f 6e73 2061 7320  rite options as 
+00018030: 6b65 792d 7661 6c75 6520 7061 6972 732c  key-value pairs,
+00018040: 2064 6566 6175 6c74 7320 746f 2060 7b7d   defaults to `{}
+00018050: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
+00018060: 2020 2057 6865 6e20 7573 696e 6720 7468     When using th
+00018070: 6520 6070 7974 686f 6e60 2065 6e67 696e  e `python` engin
+00018080: 652c 2077 7269 7465 5f6f 7074 696f 6e73  e, write_options
+00018090: 2063 616e 2063 6f6e 7461 696e 2074 6865   can contain the
+000180a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000180b0: 2066 6f6c 6c6f 7769 6e67 2065 6e74 7269   following entri
+000180c0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+000180d0: 2020 2020 2a20 6b65 7920 6073 7061 726b      * key `spark
+000180e0: 6020 616e 6420 7661 6c75 6520 616e 206f  ` and value an o
+000180f0: 626a 6563 7420 6f66 2074 7970 650a 2020  bject of type.  
+00018100: 2020 2020 2020 2020 2020 2020 2020 5b68                [h
+00018110: 7366 732e 636f 7265 2e6a 6f62 5f63 6f6e  sfs.core.job_con
+00018120: 6669 6775 7261 7469 6f6e 2e4a 6f62 436f  figuration.JobCo
+00018130: 6e66 6967 7572 6174 696f 6e5d 282e 2e2f  nfiguration](../
+00018140: 6a6f 625f 636f 6e66 6967 7572 6174 696f  job_configuratio
+00018150: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
+00018160: 2020 2020 2074 6f20 636f 6e66 6967 7572       to configur
+00018170: 6520 7468 6520 486f 7073 776f 726b 7320  e the Hopsworks 
+00018180: 4a6f 6220 7573 6564 2074 6f20 7772 6974  Job used to writ
+00018190: 6520 6461 7461 2069 6e74 6f20 7468 650a  e data into the.
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181b0: 2020 6665 6174 7572 6520 6772 6f75 702e    feature group.
+000181c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000181d0: 202a 206b 6579 2060 7761 6974 5f66 6f72   * key `wait_for
+000181e0: 5f6a 6f62 6020 616e 6420 7661 6c75 6520  _job` and value 
+000181f0: 6054 7275 6560 206f 7220 6046 616c 7365  `True` or `False
+00018200: 6020 746f 2063 6f6e 6669 6775 7265 0a20  ` to configure. 
+00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018220: 2077 6865 7468 6572 206f 7220 6e6f 7420   whether or not 
+00018230: 746f 2074 6865 2069 6e73 6572 7420 6361  to the insert ca
+00018240: 6c6c 2073 686f 756c 6420 7265 7475 726e  ll should return
+00018250: 206f 6e6c 790a 2020 2020 2020 2020 2020   only.          
+00018260: 2020 2020 2020 2020 6166 7465 7220 7468          after th
+00018270: 6520 486f 7073 776f 726b 7320 4a6f 6220  e Hopsworks Job 
+00018280: 6861 7320 6669 6e69 7368 6564 2e20 4279  has finished. By
+00018290: 2064 6566 6175 6c74 2069 7420 7761 6974   default it wait
+000182a0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+000182b0: 2020 202a 206b 6579 2060 7374 6172 745f     * key `start_
+000182c0: 6f66 666c 696e 655f 6261 636b 6669 6c6c  offline_backfill
+000182d0: 6020 616e 6420 7661 6c75 6520 6054 7275  ` and value `Tru
+000182e0: 6560 206f 7220 6046 616c 7365 6020 746f  e` or `False` to
+000182f0: 2063 6f6e 6669 6775 7265 0a20 2020 2020   configure.     
+00018300: 2020 2020 2020 2020 2020 2020 2077 6865               whe
+00018310: 7468 6572 206f 7220 6e6f 7420 746f 2073  ther or not to s
+00018320: 7461 7274 2074 6865 206d 6174 6572 6961  tart the materia
+00018330: 6c69 7a61 7469 6f6e 206a 6f62 2074 6f20  lization job to 
+00018340: 7772 6974 6520 6461 7461 2074 6f20 7468  write data to th
+00018350: 6520 6f66 666c 696e 650a 2020 2020 2020  e offline.      
+00018360: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+00018370: 6167 652e 2060 7374 6172 745f 6f66 666c  age. `start_offl
+00018380: 696e 655f 6261 636b 6669 6c6c 6020 6973  ine_backfill` is
+00018390: 2064 6570 7265 6361 7465 642e 2055 7365   deprecated. Use
+000183a0: 2060 7374 6172 745f 6f66 666c 696e 655f   `start_offline_
+000183b0: 6d61 7465 7269 616c 697a 6174 696f 6e60  materialization`
+000183c0: 2069 6e73 7465 6164 2e0a 2020 2020 2020   instead..      
+000183d0: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+000183e0: 6073 7461 7274 5f6f 6666 6c69 6e65 5f6d  `start_offline_m
+000183f0: 6174 6572 6961 6c69 7a61 7469 6f6e 6020  aterialization` 
+00018400: 616e 6420 7661 6c75 6520 6054 7275 6560  and value `True`
+00018410: 206f 7220 6046 616c 7365 6020 746f 2063   or `False` to c
+00018420: 6f6e 6669 6775 7265 0a20 2020 2020 2020  onfigure.       
+00018430: 2020 2020 2020 2020 2020 2077 6865 7468             wheth
+00018440: 6572 206f 7220 6e6f 7420 746f 2073 7461  er or not to sta
+00018450: 7274 2074 6865 206d 6174 6572 6961 6c69  rt the materiali
+00018460: 7a61 7469 6f6e 206a 6f62 2074 6f20 7772  zation job to wr
+00018470: 6974 6520 6461 7461 2074 6f20 7468 6520  ite data to the 
+00018480: 6f66 666c 696e 650a 2020 2020 2020 2020  offline.        
+00018490: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+000184a0: 652e 2042 7920 6465 6661 756c 7420 7468  e. By default th
+000184b0: 6520 6d61 7465 7269 616c 697a 6174 696f  e materializatio
+000184c0: 6e20 6a6f 6220 6765 7473 2073 7461 7274  n job gets start
+000184d0: 6564 2069 6d6d 6564 6961 7465 6c79 2e0a  ed immediately..
+000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184f0: 2a20 6b65 7920 606b 6166 6b61 5f70 726f  * key `kafka_pro
+00018500: 6475 6365 725f 636f 6e66 6967 6020 616e  ducer_config` an
+00018510: 6420 7661 6c75 6520 616e 206f 626a 6563  d value an objec
+00018520: 7420 6f66 2074 7970 6520 5b70 726f 7065  t of type [prope
+00018530: 7274 6965 735d 2868 7474 7073 3a2f 2f64  rties](https://d
+00018540: 6f63 732e 636f 6e66 6c75 656e 742e 696f  ocs.confluent.io
+00018550: 2f70 6c61 7466 6f72 6d2f 6375 7272 656e  /platform/curren
+00018560: 742f 636c 6965 6e74 732f 6c69 6272 646b  t/clients/librdk
+00018570: 6166 6b61 2f68 746d 6c2f 6d64 5f43 4f4e  afka/html/md_CON
+00018580: 4649 4755 5241 5449 4f4e 2e68 746d 6c6e  FIGURATION.htmln
+00018590: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000185a0: 2020 2020 7573 6564 2074 6f20 636f 6e66      used to conf
+000185b0: 6967 7572 6520 7468 6520 4b61 666b 6120  igure the Kafka 
+000185c0: 636c 6965 6e74 2e20 546f 206f 7074 696d  client. To optim
+000185d0: 697a 6520 666f 7220 7468 726f 7567 6870  ize for throughp
+000185e0: 7574 2069 6e20 6869 6768 206c 6174 656e  ut in high laten
+000185f0: 6379 2063 6f6e 6e65 6374 696f 6e20 636f  cy connection co
+00018600: 6e73 6964 6572 0a20 2020 2020 2020 2020  nsider.         
+00018610: 2020 2020 2020 2020 2063 6861 6e67 696e           changin
+00018620: 6720 5b70 726f 6475 6365 7220 7072 6f70  g [producer prop
+00018630: 6572 7469 6573 5d28 6874 7470 733a 2f2f  erties](https://
+00018640: 646f 6373 2e63 6f6e 666c 7565 6e74 2e69  docs.confluent.i
+00018650: 6f2f 636c 6f75 642f 6375 7272 656e 742f  o/cloud/current/
+00018660: 636c 6965 6e74 2d61 7070 732f 6f70 7469  client-apps/opti
+00018670: 6d69 7a69 6e67 2f74 6872 6f75 6768 7075  mizing/throughpu
+00018680: 742e 6874 6d6c 2370 726f 6475 6365 7229  t.html#producer)
+00018690: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000186a0: 2020 2a20 6b65 7920 6069 6e74 6572 6e61    * key `interna
+000186b0: 6c5f 6b61 666b 6160 2061 6e64 2076 616c  l_kafka` and val
+000186c0: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
+000186d0: 6c73 6560 2069 6e20 6361 7365 2079 6f75  lse` in case you
+000186e0: 2065 7374 6162 6c69 7368 6564 0a20 2020   established.   
+000186f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00018700: 6f6e 6e65 6374 6976 6974 7920 6672 6f6d  onnectivity from
+00018710: 2079 6f75 2050 7974 686f 6e20 656e 7669   you Python envi
+00018720: 726f 6e6d 656e 7420 746f 2074 6865 2069  ronment to the i
+00018730: 6e74 6572 6e61 6c20 6164 7665 7274 6973  nternal advertis
+00018740: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00018750: 2020 2020 206c 6973 7465 6e65 7273 206f       listeners o
+00018760: 6620 7468 6520 486f 7073 776f 726b 7320  f the Hopsworks 
+00018770: 4b61 666b 6120 436c 7573 7465 722e 2044  Kafka Cluster. D
+00018780: 6566 6175 6c74 7320 746f 2060 4661 6c73  efaults to `Fals
+00018790: 6560 2061 6e64 0a20 2020 2020 2020 2020  e` and.         
+000187a0: 2020 2020 2020 2020 2077 696c 6c20 7573           will us
+000187b0: 6520 6578 7465 726e 616c 206c 6973 7465  e external liste
+000187c0: 6e65 7273 2077 6865 6e20 636f 6e6e 6563  ners when connec
+000187d0: 7469 6e67 2066 726f 6d20 6f75 7473 6964  ting from outsid
+000187e0: 6520 6f66 2048 6f70 7377 6f72 6b73 2e0a  e of Hopsworks..
+000187f0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+00018800: 6461 7469 6f6e 5f6f 7074 696f 6e73 3a20  dation_options: 
+00018810: 4164 6469 7469 6f6e 616c 2076 616c 6964  Additional valid
+00018820: 6174 696f 6e20 6f70 7469 6f6e 7320 6173  ation options as
+00018830: 206b 6579 2d76 616c 7565 2070 6169 7273   key-value pairs
+00018840: 2c20 6465 6661 756c 7473 2074 6f20 607b  , defaults to `{
+00018850: 7d60 2e0a 2020 2020 2020 2020 2020 2020  }`..            
+00018860: 2020 2020 2a20 6b65 7920 6072 756e 5f76      * key `run_v
+00018870: 616c 6964 6174 696f 6e60 2062 6f6f 6c65  alidation` boole
+00018880: 616e 2076 616c 7565 2c20 7365 7420 746f  an value, set to
+00018890: 2060 4661 6c73 6560 2074 6f20 736b 6970   `False` to skip
+000188a0: 2076 616c 6964 6174 696f 6e20 7465 6d70   validation temp
+000188b0: 6f72 6172 696c 7920 6f6e 2069 6e67 6573  orarily on inges
+000188c0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+000188d0: 2020 2020 2020 2a20 6b65 7920 6073 6176        * key `sav
+000188e0: 655f 7265 706f 7274 6020 626f 6f6c 6561  e_report` boolea
+000188f0: 6e20 7661 6c75 652c 2073 6574 2074 6f20  n value, set to 
+00018900: 6046 616c 7365 6020 746f 2073 6b69 7020  `False` to skip 
+00018910: 7570 6c6f 6164 206f 6620 7468 6520 7661  upload of the va
+00018920: 6c69 6461 7469 6f6e 2072 6570 6f72 7420  lidation report 
+00018930: 746f 2048 6f70 7377 6f72 6b73 2e0a 2020  to Hopsworks..  
+00018940: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00018950: 6b65 7920 6067 655f 7661 6c69 6461 7465  key `ge_validate
+00018960: 5f6b 7761 7267 7360 2061 2064 6963 7469  _kwargs` a dicti
+00018970: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00018980: 206b 7761 7267 7320 666f 7220 7468 6520   kwargs for the 
+00018990: 7661 6c69 6461 7465 206d 6574 686f 6420  validate method 
+000189a0: 6f66 2047 7265 6174 2045 7870 6563 7461  of Great Expecta
+000189b0: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
+000189c0: 2020 2020 2020 202a 206b 6579 2060 6665         * key `fe
+000189d0: 7463 685f 6578 7065 6374 6174 696f 6e5f  tch_expectation_
+000189e0: 7375 6974 6560 2061 2062 6f6f 6c65 616e  suite` a boolean
+000189f0: 2076 616c 7565 2c20 6279 2064 6566 6175   value, by defau
+00018a00: 6c74 2060 5472 7565 602c 2074 6f20 636f  lt `True`, to co
+00018a10: 6e74 726f 6c20 7768 6574 6865 7220 7468  ntrol whether th
+00018a20: 6520 6578 7065 6374 6174 696f 6e0a 2020  e expectation.  
+00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a40: 2073 7569 7465 206f 6620 7468 6520 6665   suite of the fe
+00018a50: 6174 7572 6520 6772 6f75 7020 7368 6f75  ature group shou
+00018a60: 6c64 2062 6520 6665 7463 6865 6420 6265  ld be fetched be
+00018a70: 666f 7265 2065 7665 7279 2069 6e73 6572  fore every inser
+00018a80: 742e 0a20 2020 2020 2020 2020 2020 2073  t..            s
+00018a90: 6176 655f 636f 6465 3a20 5768 656e 2072  ave_code: When r
+00018aa0: 756e 6e69 6e67 2048 5346 5320 6f6e 2048  unning HSFS on H
+00018ab0: 6f70 7377 6f72 6b73 206f 7220 4461 7461  opsworks or Data
+00018ac0: 6272 6963 6b73 2c20 4853 4653 2063 616e  bricks, HSFS can
+00018ad0: 2073 6176 6520 7468 6520 636f 6465 2f6e   save the code/n
+00018ae0: 6f74 6562 6f6f 6b20 7573 6564 2074 6f20  otebook used to 
+00018af0: 6372 6561 7465 0a20 2020 2020 2020 2020  create.         
+00018b00: 2020 2020 2020 2074 6865 2066 6561 7475         the featu
+00018b10: 7265 2067 726f 7570 206f 7220 7573 6564  re group or used
+00018b20: 2074 6f20 696e 7365 7274 2064 6174 6120   to insert data 
+00018b30: 746f 2069 742e 2057 6865 6e20 6361 6c6c  to it. When call
+00018b40: 696e 6720 7468 6520 6069 6e73 6572 7460  ing the `insert`
+00018b50: 206d 6574 686f 6420 7265 7065 6174 6564   method repeated
+00018b60: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
+00018b70: 2020 2077 6974 6820 736d 616c 6c20 6261     with small ba
+00018b80: 7463 6865 7320 6f66 2064 6174 612c 2074  tches of data, t
+00018b90: 6869 7320 6361 6e20 736c 6f77 2064 6f77  his can slow dow
+00018ba0: 6e20 7468 6520 7772 6974 6573 2e20 5573  n the writes. Us
+00018bb0: 6520 7468 6973 206f 7074 696f 6e20 746f  e this option to
+00018bc0: 2074 7572 6e20 6f66 6620 7361 7669 6e67   turn off saving
+00018bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018be0: 2063 6f64 652e 2044 6566 6175 6c74 7320   code. Defaults 
+00018bf0: 746f 2060 5472 7565 602e 0a20 2020 2020  to `True`..     
+00018c00: 2020 2020 2020 2077 6169 743a 2057 6169         wait: Wai
+00018c10: 7420 666f 7220 6a6f 6220 746f 2066 696e  t for job to fin
+00018c20: 6973 6820 6265 666f 7265 2072 6574 7572  ish before retur
+00018c30: 6e69 6e67 2c20 6465 6661 756c 7473 2074  ning, defaults t
+00018c40: 6f20 6046 616c 7365 602e 0a20 2020 2020  o `False`..     
+00018c50: 2020 2020 2020 2020 2020 2053 686f 7274             Short
+00018c60: 6375 7420 666f 7220 7265 6164 5f6f 7074  cut for read_opt
+00018c70: 696f 6e73 2060 7b22 7761 6974 5f66 6f72  ions `{"wait_for
+00018c80: 5f6a 6f62 223a 2046 616c 7365 7d60 2e0a  _job": False}`..
+00018c90: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+00018ca0: 6e73 0a20 2020 2020 2020 2020 2020 2028  ns.            (
+00018cb0: 604a 6f62 602c 2060 5661 6c69 6461 7469  `Job`, `Validati
+00018cc0: 6f6e 5265 706f 7274 6029 2041 2074 7570  onReport`) A tup
+00018cd0: 6c65 2077 6974 6820 6a6f 6220 696e 666f  le with job info
+00018ce0: 726d 6174 696f 6e20 6966 2070 7974 686f  rmation if pytho
+00018cf0: 6e20 656e 6769 6e65 2069 7320 7573 6564  n engine is used
+00018d00: 2061 6e64 2074 6865 2076 616c 6964 6174   and the validat
+00018d10: 696f 6e20 7265 706f 7274 2069 6620 7661  ion report if va
+00018d20: 6c69 6461 7469 6f6e 2069 7320 656e 6162  lidation is enab
+00018d30: 6c65 642e 0a0a 2020 2020 2020 2020 2320  led...        # 
+00018d40: 5261 6973 6573 0a20 2020 2020 2020 2020  Raises.         
+00018d50: 2020 2060 6873 6673 2e63 6c69 656e 742e     `hsfs.client.
+00018d60: 6578 6365 7074 696f 6e73 2e52 6573 7441  exceptions.RestA
+00018d70: 5049 4572 726f 7260 2e20 652e 6720 6661  PIError`. e.g fa
+00018d80: 696c 2074 6f20 6372 6561 7465 2066 6561  il to create fea
+00018d90: 7475 7265 2067 726f 7570 2c20 6461 7461  ture group, data
+00018da0: 6672 616d 6520 7363 6865 6d61 2064 6f65  frame schema doe
+00018db0: 7320 6e6f 7420 6d61 7463 680a 2020 2020  s not match.    
+00018dc0: 2020 2020 2020 2020 2020 2020 6578 6973              exis
+00018dd0: 7469 6e67 2066 6561 7475 7265 2067 726f  ting feature gro
+00018de0: 7570 2073 6368 656d 612c 2065 7463 2e0a  up schema, etc..
+00018df0: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
+00018e00: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
+00018e10: 6f6e 732e 4461 7461 5661 6c69 6461 7469  ons.DataValidati
+00018e20: 6f6e 4578 6365 7074 696f 6e60 2e20 4966  onException`. If
+00018e30: 2064 6174 6120 7661 6c69 6461 7469 6f6e   data validation
+00018e40: 2066 6169 6c73 2061 6e64 2074 6865 2065   fails and the e
+00018e50: 7870 6563 7461 7469 6f6e 0a20 2020 2020  xpectation.     
+00018e60: 2020 2020 2020 2020 2020 2073 7569 7465             suite
+00018e70: 2060 7661 6c69 6461 7469 6f6e 5f69 6e67   `validation_ing
+00018e80: 6573 7469 6f6e 5f70 6f6c 6963 7960 2069  estion_policy` i
+00018e90: 7320 7365 7420 746f 2060 5354 5249 4354  s set to `STRICT
+00018ea0: 602e 2044 6174 6120 6973 204e 4f54 2069  `. Data is NOT i
+00018eb0: 6e67 6573 7465 642e 0a20 2020 2020 2020  ngested..       
+00018ec0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00018ed0: 7374 6f72 6167 6520 616e 6420 7365 6c66  storage and self
+00018ee0: 2e73 7472 6561 6d3a 0a20 2020 2020 2020  .stream:.       
+00018ef0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00018f00: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
+00018f10: 2020 2020 2253 7065 6369 6679 696e 6720      "Specifying 
+00018f20: 7468 6520 7374 6f72 6167 6520 6f70 7469  the storage opti
+00018f30: 6f6e 2069 7320 6e6f 7420 7375 7070 6f72  on is not suppor
+00018f40: 7465 6420 6966 2074 6865 2073 7472 6561  ted if the strea
+00018f50: 6d69 6e67 2041 5049 7320 6172 6520 656e  ming APIs are en
+00018f60: 6162 6c65 6422 0a20 2020 2020 2020 2020  abled".         
+00018f70: 2020 2029 0a0a 2020 2020 2020 2020 6665     )..        fe
+00018f80: 6174 7572 655f 6461 7461 6672 616d 6520  ature_dataframe 
+00018f90: 3d20 656e 6769 6e65 2e67 6574 5f69 6e73  = engine.get_ins
+00018fa0: 7461 6e63 6528 292e 636f 6e76 6572 745f  tance().convert_
+00018fb0: 746f 5f64 6566 6175 6c74 5f64 6174 6166  to_default_dataf
+00018fc0: 7261 6d65 2866 6561 7475 7265 7329 0a0a  rame(features)..
+00018fd0: 2020 2020 2020 2020 6966 2077 7269 7465          if write
+00018fe0: 5f6f 7074 696f 6e73 2069 7320 4e6f 6e65  _options is None
+00018ff0: 3a0a 2020 2020 2020 2020 2020 2020 7772  :.            wr
+00019000: 6974 655f 6f70 7469 6f6e 7320 3d20 7b7d  ite_options = {}
+00019010: 0a20 2020 2020 2020 2069 6620 2277 6169  .        if "wai
+00019020: 745f 666f 725f 6a6f 6222 206e 6f74 2069  t_for_job" not i
+00019030: 6e20 7772 6974 655f 6f70 7469 6f6e 733a  n write_options:
+00019040: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
+00019050: 7465 5f6f 7074 696f 6e73 5b22 7761 6974  te_options["wait
+00019060: 5f66 6f72 5f6a 6f62 225d 203d 2077 6169  _for_job"] = wai
+00019070: 740a 0a20 2020 2020 2020 206a 6f62 2c20  t..        job, 
+00019080: 6765 5f72 6570 6f72 7420 3d20 7365 6c66  ge_report = self
+00019090: 2e5f 6665 6174 7572 655f 6772 6f75 705f  ._feature_group_
+000190a0: 656e 6769 6e65 2e69 6e73 6572 7428 0a20  engine.insert(. 
+000190b0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+000190c0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
+000190d0: 7475 7265 5f64 6174 6166 7261 6d65 3d66  ture_dataframe=f
+000190e0: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+000190f0: 2c0a 2020 2020 2020 2020 2020 2020 6f76  ,.            ov
+00019100: 6572 7772 6974 653d 6f76 6572 7772 6974  erwrite=overwrit
+00019110: 652c 0a20 2020 2020 2020 2020 2020 206f  e,.            o
+00019120: 7065 7261 7469 6f6e 3d6f 7065 7261 7469  peration=operati
+00019130: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00019140: 7374 6f72 6167 653d 7374 6f72 6167 652e  storage=storage.
+00019150: 6c6f 7765 7228 2920 6966 2073 746f 7261  lower() if stora
+00019160: 6765 2069 7320 6e6f 7420 4e6f 6e65 2065  ge is not None e
+00019170: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
+00019180: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
+00019190: 6f6e 733d 7772 6974 655f 6f70 7469 6f6e  ons=write_option
+000191a0: 732c 0a20 2020 2020 2020 2020 2020 2076  s,.            v
+000191b0: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
+000191c0: 733d 7b22 7361 7665 5f72 6570 6f72 7422  s={"save_report"
+000191d0: 3a20 5472 7565 2c20 2a2a 7661 6c69 6461  : True, **valida
+000191e0: 7469 6f6e 5f6f 7074 696f 6e73 7d2c 0a20  tion_options},. 
+000191f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00019200: 2069 6620 7361 7665 5f63 6f64 6520 616e   if save_code an
+00019210: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
+00019220: 6765 5f72 6570 6f72 7420 6973 204e 6f6e  ge_report is Non
+00019230: 6520 6f72 2067 655f 7265 706f 7274 2e69  e or ge_report.i
+00019240: 6e67 6573 7469 6f6e 5f72 6573 756c 7420  ngestion_result 
+00019250: 3d3d 2022 494e 4745 5354 4544 220a 2020  == "INGESTED".  
+00019260: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00019270: 2020 2020 2073 656c 662e 5f63 6f64 655f       self._code_
+00019280: 656e 6769 6e65 2e73 6176 655f 636f 6465  engine.save_code
+00019290: 2873 656c 6629 0a0a 2020 2020 2020 2020  (self)..        
+000192a0: 6966 2065 6e67 696e 652e 6765 745f 7479  if engine.get_ty
+000192b0: 7065 2829 2e73 7461 7274 7377 6974 6828  pe().startswith(
+000192c0: 2273 7061 726b 2229 2061 6e64 206e 6f74  "spark") and not
+000192d0: 2073 656c 662e 7374 7265 616d 3a0a 2020   self.stream:.  
+000192e0: 2020 2020 2020 2020 2020 2320 416c 736f            # Also
+000192f0: 2c20 6f6e 6c79 2063 6f6d 7075 7465 2073  , only compute s
+00019300: 7461 7469 7374 6963 7320 6966 2073 7472  tatistics if str
+00019310: 6561 6d20 6973 2046 616c 7365 2e0a 2020  eam is False..  
+00019320: 2020 2020 2020 2020 2020 2320 6966 2054            # if T
+00019330: 7275 652c 2074 6865 2062 6163 6b66 696c  rue, the backfil
+00019340: 6c20 6a6f 6220 6861 7320 6e6f 7420 6265  l job has not be
+00019350: 656e 2074 7269 6767 6572 6564 2061 6e64  en triggered and
+00019360: 2074 6865 2064 6174 6120 6861 7320 6e6f   the data has no
+00019370: 7420 6265 656e 2069 6e73 6572 7465 6420  t been inserted 
+00019380: 2869 7427 7320 696e 204b 6166 6b61 290a  (it's in Kafka).
+00019390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000193a0: 2e63 6f6d 7075 7465 5f73 7461 7469 7374  .compute_statist
+000193b0: 6963 7328 290a 0a20 2020 2020 2020 2072  ics()..        r
+000193c0: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+000193d0: 2020 2020 6a6f 622c 0a20 2020 2020 2020      job,.       
+000193e0: 2020 2020 2067 655f 7265 706f 7274 2e74       ge_report.t
+000193f0: 6f5f 6765 5f74 7970 6528 2920 6966 2067  o_ge_type() if g
+00019400: 655f 7265 706f 7274 2069 7320 6e6f 7420  e_report is not 
+00019410: 4e6f 6e65 2065 6c73 6520 4e6f 6e65 2c0a  None else None,.
+00019420: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00019430: 6566 206d 756c 7469 5f70 6172 745f 696e  ef multi_part_in
+00019440: 7365 7274 280a 2020 2020 2020 2020 7365  sert(.        se
+00019450: 6c66 2c0a 2020 2020 2020 2020 6665 6174  lf,.        feat
+00019460: 7572 6573 3a20 556e 696f 6e5b 0a20 2020  ures: Union[.   
+00019470: 2020 2020 2020 2020 2070 642e 4461 7461           pd.Data
+00019480: 4672 616d 652c 0a20 2020 2020 2020 2020  Frame,.         
+00019490: 2020 2054 7970 6556 6172 2822 7079 7370     TypeVar("pysp
+000194a0: 6172 6b2e 7371 6c2e 4461 7461 4672 616d  ark.sql.DataFram
+000194b0: 6522 292c 2020 2320 6e6f 7161 3a20 4638  e"),  # noqa: F8
+000194c0: 3231 0a20 2020 2020 2020 2020 2020 2054  21.            T
+000194d0: 7970 6556 6172 2822 7079 7370 6172 6b2e  ypeVar("pyspark.
+000194e0: 5244 4422 292c 2020 2320 6e6f 7161 3a20  RDD"),  # noqa: 
+000194f0: 4638 3231 0a20 2020 2020 2020 2020 2020  F821.           
+00019500: 206e 702e 6e64 6172 7261 792c 0a20 2020   np.ndarray,.   
+00019510: 2020 2020 2020 2020 204c 6973 745b 6c69           List[li
+00019520: 7374 5d2c 0a20 2020 2020 2020 205d 203d  st],.        ] =
+00019530: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+00019540: 7665 7277 7269 7465 3a20 4f70 7469 6f6e  verwrite: Option
+00019550: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
+00019560: 2c0a 2020 2020 2020 2020 6f70 6572 6174  ,.        operat
+00019570: 696f 6e3a 204f 7074 696f 6e61 6c5b 7374  ion: Optional[st
+00019580: 725d 203d 2022 7570 7365 7274 222c 0a20  r] = "upsert",. 
+00019590: 2020 2020 2020 2073 746f 7261 6765 3a20         storage: 
+000195a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000195b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7772  None,.        wr
+000195c0: 6974 655f 6f70 7469 6f6e 733a 204f 7074  ite_options: Opt
+000195d0: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+000195e0: 416e 795d 5d20 3d20 7b7d 2c0a 2020 2020  Any]] = {},.    
+000195f0: 2020 2020 7661 6c69 6461 7469 6f6e 5f6f      validation_o
+00019600: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
+00019610: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00019620: 203d 207b 7d2c 0a20 2020 2029 202d 3e20   = {},.    ) -> 
+00019630: 556e 696f 6e5b 0a20 2020 2020 2020 2054  Union[.        T
+00019640: 7570 6c65 5b4f 7074 696f 6e61 6c5b 4a6f  uple[Optional[Jo
+00019650: 625d 2c20 4f70 7469 6f6e 616c 5b56 616c  b], Optional[Val
+00019660: 6964 6174 696f 6e52 6570 6f72 745d 5d2c  idationReport]],
+00019670: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00019680: 5f67 726f 7570 5f77 7269 7465 722e 4665  _group_writer.Fe
+00019690: 6174 7572 6547 726f 7570 5772 6974 6572  atureGroupWriter
+000196a0: 2c0a 2020 2020 5d3a 0a20 2020 2020 2020  ,.    ]:.       
+000196b0: 2022 2222 4765 7420 4665 6174 7572 6547   """Get FeatureG
+000196c0: 726f 7570 5772 6974 6572 2066 6f72 206f  roupWriter for o
+000196d0: 7074 696d 697a 6564 206d 756c 7469 2070  ptimized multi p
+000196e0: 6172 7420 696e 7365 7274 7320 6f72 2063  art inserts or c
+000196f0: 616c 6c20 7468 6973 206d 6574 686f 640a  all this method.
+00019700: 2020 2020 2020 2020 746f 2073 7461 7274          to start
+00019710: 206d 616e 7561 6c20 6d75 6c74 6920 7061   manual multi pa
+00019720: 7274 206f 7074 696d 697a 6564 2069 6e73  rt optimized ins
+00019730: 6572 7473 2e0a 0a20 2020 2020 2020 2049  erts...        I
+00019740: 6e20 7573 6520 6361 7365 7320 7768 6572  n use cases wher
+00019750: 6520 7665 7279 2073 6d61 6c6c 2062 6174  e very small bat
+00019760: 6368 6573 2028 3120 746f 2031 3030 3029  ches (1 to 1000)
+00019770: 2072 6f77 7320 7065 7220 4461 7461 6672   rows per Datafr
+00019780: 616d 6520 6e65 6564 0a20 2020 2020 2020  ame need.       
+00019790: 2074 6f20 6265 2077 7269 7474 656e 2074   to be written t
+000197a0: 6f20 7468 6520 6665 6174 7572 6520 7374  o the feature st
+000197b0: 6f72 6520 7265 7065 6174 6564 6c79 2c20  ore repeatedly, 
+000197c0: 6974 206d 6967 6874 2062 6520 696e 6566  it might be inef
+000197d0: 6669 6369 656e 7420 746f 2075 7365 0a20  ficient to use. 
+000197e0: 2020 2020 2020 2074 6865 2073 7461 6e64         the stand
+000197f0: 6172 6420 6066 6561 7475 7265 5f67 726f  ard `feature_gro
+00019800: 7570 2e69 6e73 6572 7428 2960 206d 6574  up.insert()` met
+00019810: 686f 6420 6173 2069 7420 7065 7266 6f72  hod as it perfor
+00019820: 6d73 2073 6f6d 6520 6261 636b 6772 6f75  ms some backgrou
+00019830: 6e64 0a20 2020 2020 2020 2061 6374 696f  nd.        actio
+00019840: 6e73 2074 6f20 7570 6461 7465 2074 6865  ns to update the
+00019850: 206d 6574 6164 6174 6120 6f66 2074 6865   metadata of the
+00019860: 2066 6561 7475 7265 2067 726f 7570 206f   feature group o
+00019870: 626a 6563 7420 6669 7273 742e 0a0a 2020  bject first...  
+00019880: 2020 2020 2020 466f 7220 7468 6573 6520        For these 
+00019890: 6361 7365 732c 2074 6865 2066 6561 7475  cases, the featu
+000198a0: 7265 2067 726f 7570 2070 726f 7669 6465  re group provide
+000198b0: 7320 7468 6520 606d 756c 7469 5f70 6172  s the `multi_par
+000198c0: 745f 696e 7365 7274 6020 4150 492c 0a20  t_insert` API,. 
+000198d0: 2020 2020 2020 2077 6869 6368 2069 7320         which is 
+000198e0: 6f70 7469 6d69 7a65 6420 666f 7220 7772  optimized for wr
+000198f0: 6974 696e 6720 6d61 6e79 2073 6d61 6c6c  iting many small
+00019900: 2044 6174 6166 7261 6d65 7320 6166 7465   Dataframes afte
+00019910: 7220 616e 6f74 6865 722e 0a0a 2020 2020  r another...    
+00019920: 2020 2020 5468 6572 6520 6172 6520 7477      There are tw
+00019930: 6f20 7761 7973 2074 6f20 7573 6520 7468  o ways to use th
+00019940: 6973 2041 5049 3a0a 2020 2020 2020 2020  is API:.        
+00019950: 2121 2120 6578 616d 706c 6520 2250 7974  !!! example "Pyt
+00019960: 686f 6e20 436f 6e74 6578 7420 4d61 6e61  hon Context Mana
+00019970: 6765 7222 0a20 2020 2020 2020 2020 2020  ger".           
+00019980: 2055 7369 6e67 2074 6865 2050 7974 686f   Using the Pytho
+00019990: 6e20 6077 6974 6860 2073 796e 7461 7820  n `with` syntax 
+000199a0: 796f 7520 6361 6e20 6163 7175 6972 6520  you can acquire 
+000199b0: 6120 4665 6174 7572 6547 726f 7570 5772  a FeatureGroupWr
+000199c0: 6974 6572 0a20 2020 2020 2020 2020 2020  iter.           
+000199d0: 206f 626a 6563 7420 7468 6174 2069 6d70   object that imp
+000199e0: 6c65 6d65 6e74 7320 7468 6520 7361 6d65  lements the same
+000199f0: 2060 6d75 6c74 695f 7061 7274 5f69 6e73   `multi_part_ins
+00019a00: 6572 7460 2041 5049 2e0a 2020 2020 2020  ert` API..      
+00019a10: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00019a20: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00019a30: 7572 655f 6772 6f75 7020 3d20 6673 2e67  ure_group = fs.g
+00019a40: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
+00019a50: 7475 7265 5f67 726f 7570 2822 6667 5f6e  ture_group("fg_n
+00019a60: 616d 6522 2c20 7665 7273 696f 6e3d 3129  ame", version=1)
+00019a70: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+00019a80: 7468 2066 6561 7475 7265 5f67 726f 7570  th feature_group
+00019a90: 2e6d 756c 7469 5f70 6172 745f 696e 7365  .multi_part_inse
+00019aa0: 7274 2829 2061 7320 7772 6974 6572 3a0a  rt() as writer:.
+00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ac0: 2320 7275 6e20 696e 7365 7274 7320 696e  # run inserts in
+00019ad0: 2061 206c 6f6f 703a 0a20 2020 2020 2020   a loop:.       
+00019ae0: 2020 2020 2020 2020 2077 6869 6c65 206c           while l
+00019af0: 6f6f 703a 0a20 2020 2020 2020 2020 2020  oop:.           
+00019b00: 2020 2020 2020 2020 2073 6d61 6c6c 5f62           small_b
+00019b10: 6174 6368 5f64 6620 3d20 2e2e 2e0a 2020  atch_df = ....  
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 2020 7772 6974 6572 2e69 6e73 6572 7428    writer.insert(
+00019b40: 736d 616c 6c5f 6261 7463 685f 6466 290a  small_batch_df).
+00019b50: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00019b60: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00019b70: 7772 6974 6572 2062 6174 6368 6573 2074  writer batches t
+00019b80: 6865 2073 6d61 6c6c 2044 6174 6166 7261  he small Datafra
+00019b90: 6d65 7320 616e 6420 7472 616e 736d 6974  mes and transmit
+00019ba0: 7320 7468 656d 2074 6f20 486f 7073 776f  s them to Hopswo
+00019bb0: 726b 730a 2020 2020 2020 2020 2020 2020  rks.            
+00019bc0: 6566 6669 6369 656e 746c 792e 0a20 2020  efficiently..   
+00019bd0: 2020 2020 2020 2020 2057 6865 6e20 6578           When ex
+00019be0: 6974 696e 6720 7468 6520 636f 6e74 6578  iting the contex
+00019bf0: 742c 2074 6865 2066 6561 7475 7265 2067  t, the feature g
+00019c00: 726f 7570 2077 7269 7465 7220 6973 2073  roup writer is s
+00019c10: 7572 6520 746f 2065 7869 740a 2020 2020  ure to exit.    
+00019c20: 2020 2020 2020 2020 6f6e 6c79 206f 6e63          only onc
+00019c30: 6520 616c 6c20 7468 6520 726f 7773 2068  e all the rows h
+00019c40: 6176 6520 6265 656e 2074 7261 6e73 6d69  ave been transmi
+00019c50: 7474 6564 2e0a 0a20 2020 2020 2020 2021  tted...        !
+00019c60: 2121 2065 7861 6d70 6c65 2022 4d75 6c74  !! example "Mult
+00019c70: 6920 7061 7274 2069 6e73 6572 7420 7769  i part insert wi
+00019c80: 7468 206d 616e 7561 6c20 636f 6e74 6578  th manual contex
+00019c90: 7420 6d61 6e61 6765 6d65 6e74 220a 2020  t management".  
+00019ca0: 2020 2020 2020 2020 2020 496e 7374 6561            Instea
+00019cb0: 6420 6f66 206c 6574 7469 6e67 2050 7974  d of letting Pyt
+00019cc0: 686f 6e20 6861 6e64 6c65 2074 6865 2065  hon handle the e
+00019cd0: 6e74 6572 696e 6720 616e 6420 6578 6974  ntering and exit
+00019ce0: 696e 6720 6f66 2074 6865 0a20 2020 2020  ing of the.     
+00019cf0: 2020 2020 2020 206d 756c 7469 2070 6172         multi par
+00019d00: 7420 696e 7365 7274 2063 6f6e 7465 7874  t insert context
+00019d10: 2c20 796f 7520 6361 6e20 7374 6172 7420  , you can start 
+00019d20: 616e 6420 6669 6e61 6c69 7a65 2074 6865  and finalize the
+00019d30: 2063 6f6e 7465 7874 0a20 2020 2020 2020   context.       
+00019d40: 2020 2020 206d 616e 7561 6c6c 792e 0a20       manually.. 
+00019d50: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
+00019d60: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
+00019d70: 2066 6561 7475 7265 5f67 726f 7570 203d   feature_group =
+00019d80: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+00019d90: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+00019da0: 2266 675f 6e61 6d65 222c 2076 6572 7369  "fg_name", versi
+00019db0: 6f6e 3d31 290a 0a20 2020 2020 2020 2020  on=1)..         
+00019dc0: 2020 2077 6869 6c65 206c 6f6f 703a 0a20     while loop:. 
+00019dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019de0: 6d61 6c6c 5f62 6174 6368 5f64 6620 3d20  mall_batch_df = 
+00019df0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00019e00: 2020 2020 6665 6174 7572 655f 6772 6f75      feature_grou
+00019e10: 702e 6d75 6c74 695f 7061 7274 5f69 6e73  p.multi_part_ins
+00019e20: 6572 7428 736d 616c 6c5f 6261 7463 685f  ert(small_batch_
+00019e30: 6466 290a 0a20 2020 2020 2020 2020 2020  df)..           
+00019e40: 2023 2049 4d50 4f52 5441 4e54 3a20 6669   # IMPORTANT: fi
+00019e50: 6e61 6c69 7a65 2074 6865 206d 756c 7469  nalize the multi
+00019e60: 2070 6172 7420 696e 7365 7274 2074 6f20   part insert to 
+00019e70: 6d61 6b65 2073 7572 6520 616c 6c20 726f  make sure all ro
+00019e80: 7773 0a20 2020 2020 2020 2020 2020 2023  ws.            #
+00019e90: 2068 6176 6520 6265 656e 2074 7261 6e73   have been trans
+00019ea0: 6d69 7474 6564 0a20 2020 2020 2020 2020  mitted.         
+00019eb0: 2020 2066 6561 7475 7265 5f67 726f 7570     feature_group
+00019ec0: 2e66 696e 616c 697a 655f 6d75 6c74 695f  .finalize_multi_
+00019ed0: 7061 7274 5f69 6e73 6572 7428 290a 2020  part_insert().  
+00019ee0: 2020 2020 2020 2020 2020 6060 600a 2020            ```.  
+00019ef0: 2020 2020 2020 2020 2020 4e6f 7465 2074            Note t
+00019f00: 6861 7420 7468 6520 6669 7273 7420 6361  hat the first ca
+00019f10: 6c6c 2074 6f20 606d 756c 7469 5f70 6172  ll to `multi_par
+00019f20: 745f 696e 7365 7274 6020 696e 6974 6961  t_insert` initia
+00019f30: 7465 7320 7468 6520 636f 6e74 6578 740a  tes the context.
+00019f40: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00019f50: 6265 2073 7572 6520 746f 2066 696e 616c  be sure to final
+00019f60: 697a 6520 6974 2e20 5468 6520 6066 696e  ize it. The `fin
+00019f70: 616c 697a 655f 6d75 6c74 695f 7061 7274  alize_multi_part
+00019f80: 5f69 6e73 6572 7460 2069 7320 610a 2020  _insert` is a.  
+00019f90: 2020 2020 2020 2020 2020 626c 6f63 6b69            blocki
+00019fa0: 6e67 2063 616c 6c20 7468 6174 2072 6574  ng call that ret
+00019fb0: 7572 6e73 206f 6e63 6520 616c 6c20 726f  urns once all ro
+00019fc0: 7773 2068 6176 6520 6265 656e 2074 7261  ws have been tra
+00019fd0: 6e73 6d69 7474 6564 2e0a 0a20 2020 2020  nsmitted...     
+00019fe0: 2020 2020 2020 204f 6e63 6520 796f 7520         Once you 
+00019ff0: 6172 6520 646f 6e65 2077 6974 6820 7468  are done with th
+0001a000: 6520 6d75 6c74 6920 7061 7274 2069 6e73  e multi part ins
+0001a010: 6572 742c 2069 7420 6973 2067 6f6f 6420  ert, it is good 
+0001a020: 7072 6163 7469 6365 2074 6f0a 2020 2020  practice to.    
+0001a030: 2020 2020 2020 2020 7374 6172 7420 7468          start th
+0001a040: 6520 6d61 7465 7269 616c 697a 6174 696f  e materializatio
+0001a050: 6e20 6a6f 6220 696e 206f 7264 6572 2074  n job in order t
+0001a060: 6f20 7772 6974 6520 7468 6520 6461 7461  o write the data
+0001a070: 2074 6f20 7468 6520 6f66 666c 696e 650a   to the offline.
+0001a080: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+0001a090: 6167 653a 0a20 2020 2020 2020 2020 2020  age:.           
+0001a0a0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+0001a0b0: 2020 2020 2020 2066 6561 7475 7265 5f67         feature_g
+0001a0c0: 726f 7570 2e6d 6174 6572 6961 6c69 7a61  roup.materializa
+0001a0d0: 7469 6f6e 5f6a 6f62 2e72 756e 2861 7761  tion_job.run(awa
+0001a0e0: 6974 5f74 6572 6d69 6e61 7469 6f6e 3d54  it_termination=T
+0001a0f0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0001a100: 2060 6060 0a0a 2020 2020 2020 2020 2320   ```..        # 
+0001a110: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
+0001a120: 2020 2020 2020 6665 6174 7572 6573 3a20        features: 
+0001a130: 4461 7461 4672 616d 652c 2052 4444 2c20  DataFrame, RDD, 
+0001a140: 4e64 6172 7261 792c 206c 6973 742e 2046  Ndarray, list. F
+0001a150: 6561 7475 7265 7320 746f 2062 6520 7361  eatures to be sa
+0001a160: 7665 642e 0a20 2020 2020 2020 2020 2020  ved..           
+0001a170: 206f 7665 7277 7269 7465 3a20 4472 6f70   overwrite: Drop
+0001a180: 2061 6c6c 2064 6174 6120 696e 2074 6865   all data in the
+0001a190: 2066 6561 7475 7265 2067 726f 7570 2062   feature group b
+0001a1a0: 6566 6f72 650a 2020 2020 2020 2020 2020  efore.          
+0001a1b0: 2020 2020 2020 696e 7365 7274 696e 6720        inserting 
+0001a1c0: 6e65 7720 6461 7461 2e20 5468 6973 2064  new data. This d
+0001a1d0: 6f65 7320 6e6f 7420 6166 6665 6374 206d  oes not affect m
+0001a1e0: 6574 6164 6174 612c 2064 6566 6175 6c74  etadata, default
+0001a1f0: 7320 746f 2046 616c 7365 2e0a 2020 2020  s to False..    
+0001a200: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+0001a210: 6e3a 2041 7061 6368 6520 4875 6469 206f  n: Apache Hudi o
+0001a220: 7065 7261 7469 6f6e 2074 7970 6520 6022  peration type `"
+0001a230: 696e 7365 7274 2260 206f 7220 6022 7570  insert"` or `"up
+0001a240: 7365 7274 2260 2e0a 2020 2020 2020 2020  sert"`..        
+0001a250: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+0001a260: 2074 6f20 6022 7570 7365 7274 2260 2e0a   to `"upsert"`..
+0001a270: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+0001a280: 6167 653a 204f 7665 7277 7269 7465 2064  age: Overwrite d
+0001a290: 6566 6175 6c74 2062 6568 6176 696f 7572  efault behaviour
+0001a2a0: 2c20 7772 6974 6520 746f 206f 6666 6c69  , write to offli
+0001a2b0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0001a2c0: 2020 2073 746f 7261 6765 206f 6e6c 7920     storage only 
+0001a2d0: 7769 7468 2060 226f 6666 6c69 6e65 2260  with `"offline"`
+0001a2e0: 206f 7220 6f6e 6c69 6e65 206f 6e6c 7920   or online only 
+0001a2f0: 7769 7468 2060 226f 6e6c 696e 6522 602c  with `"online"`,
+0001a300: 2064 6566 6175 6c74 730a 2020 2020 2020   defaults.      
+0001a310: 2020 2020 2020 2020 2020 746f 2060 4e6f            to `No
+0001a320: 6e65 602e 0a20 2020 2020 2020 2020 2020  ne`..           
+0001a330: 2077 7269 7465 5f6f 7074 696f 6e73 3a20   write_options: 
+0001a340: 4164 6469 7469 6f6e 616c 2077 7269 7465  Additional write
+0001a350: 206f 7074 696f 6e73 2061 7320 6b65 792d   options as key-
+0001a360: 7661 6c75 6520 7061 6972 732c 2064 6566  value pairs, def
+0001a370: 6175 6c74 7320 746f 2060 7b7d 602e 0a20  aults to `{}`.. 
+0001a380: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+0001a390: 6865 6e20 7573 696e 6720 7468 6520 6070  hen using the `p
+0001a3a0: 7974 686f 6e60 2065 6e67 696e 652c 2077  ython` engine, w
+0001a3b0: 7269 7465 5f6f 7074 696f 6e73 2063 616e  rite_options can
+0001a3c0: 2063 6f6e 7461 696e 2074 6865 0a20 2020   contain the.   
+0001a3d0: 2020 2020 2020 2020 2020 2020 2066 6f6c               fol
+0001a3e0: 6c6f 7769 6e67 2065 6e74 7269 6573 3a0a  lowing entries:.
+0001a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a400: 2a20 6b65 7920 6073 7061 726b 6020 616e  * key `spark` an
+0001a410: 6420 7661 6c75 6520 616e 206f 626a 6563  d value an objec
+0001a420: 7420 6f66 2074 7970 650a 2020 2020 2020  t of type.      
+0001a430: 2020 2020 2020 2020 2020 5b68 7366 732e            [hsfs.
+0001a440: 636f 7265 2e6a 6f62 5f63 6f6e 6669 6775  core.job_configu
+0001a450: 7261 7469 6f6e 2e4a 6f62 436f 6e66 6967  ration.JobConfig
+0001a460: 7572 6174 696f 6e5d 282e 2e2f 6a6f 625f  uration](../job_
+0001a470: 636f 6e66 6967 7572 6174 696f 6e29 0a20  configuration). 
+0001a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a490: 2074 6f20 636f 6e66 6967 7572 6520 7468   to configure th
+0001a4a0: 6520 486f 7073 776f 726b 7320 4a6f 6220  e Hopsworks Job 
+0001a4b0: 7573 6564 2074 6f20 7772 6974 6520 6461  used to write da
+0001a4c0: 7461 2069 6e74 6f20 7468 650a 2020 2020  ta into the.    
+0001a4d0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+0001a4e0: 6174 7572 6520 6772 6f75 702e 0a20 2020  ature group..   
+0001a4f0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0001a500: 6579 2060 7761 6974 5f66 6f72 5f6a 6f62  ey `wait_for_job
+0001a510: 6020 616e 6420 7661 6c75 6520 6054 7275  ` and value `Tru
+0001a520: 6560 206f 7220 6046 616c 7365 6020 746f  e` or `False` to
+0001a530: 2063 6f6e 6669 6775 7265 0a20 2020 2020   configure.     
+0001a540: 2020 2020 2020 2020 2020 2020 2077 6865               whe
+0001a550: 7468 6572 206f 7220 6e6f 7420 746f 2074  ther or not to t
+0001a560: 6865 2069 6e73 6572 7420 6361 6c6c 2073  he insert call s
+0001a570: 686f 756c 6420 7265 7475 726e 206f 6e6c  hould return onl
+0001a580: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+0001a590: 2020 2020 6166 7465 7220 7468 6520 486f      after the Ho
+0001a5a0: 7073 776f 726b 7320 4a6f 6220 6861 7320  psworks Job has 
+0001a5b0: 6669 6e69 7368 6564 2e20 4279 2064 6566  finished. By def
+0001a5c0: 6175 6c74 2069 7420 7761 6974 732e 0a20  ault it waits.. 
+0001a5d0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0001a5e0: 206b 6579 2060 7374 6172 745f 6f66 666c   key `start_offl
+0001a5f0: 696e 655f 6261 636b 6669 6c6c 6020 616e  ine_backfill` an
+0001a600: 6420 7661 6c75 6520 6054 7275 6560 206f  d value `True` o
+0001a610: 7220 6046 616c 7365 6020 746f 2063 6f6e  r `False` to con
+0001a620: 6669 6775 7265 0a20 2020 2020 2020 2020  figure.         
+0001a630: 2020 2020 2020 2020 2077 6865 7468 6572           whether
+0001a640: 206f 7220 6e6f 7420 746f 2073 7461 7274   or not to start
+0001a650: 2074 6865 206d 6174 6572 6961 6c69 7a61   the materializa
+0001a660: 7469 6f6e 206a 6f62 2074 6f20 7772 6974  tion job to writ
+0001a670: 6520 6461 7461 2074 6f20 7468 6520 6f66  e data to the of
+0001a680: 666c 696e 650a 2020 2020 2020 2020 2020  fline.          
+0001a690: 2020 2020 2020 2020 7374 6f72 6167 652e          storage.
+0001a6a0: 2060 7374 6172 745f 6f66 666c 696e 655f   `start_offline_
+0001a6b0: 6261 636b 6669 6c6c 6020 6973 2064 6570  backfill` is dep
+0001a6c0: 7265 6361 7465 642e 2055 7365 2060 7374  recated. Use `st
+0001a6d0: 6172 745f 6f66 666c 696e 655f 6d61 7465  art_offline_mate
+0001a6e0: 7269 616c 697a 6174 696f 6e60 2069 6e73  rialization` ins
+0001a6f0: 7465 6164 2e0a 2020 2020 2020 2020 2020  tead..          
+0001a700: 2020 2020 2020 2a20 6b65 7920 6073 7461        * key `sta
+0001a710: 7274 5f6f 6666 6c69 6e65 5f6d 6174 6572  rt_offline_mater
+0001a720: 6961 6c69 7a61 7469 6f6e 6020 616e 6420  ialization` and 
+0001a730: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
+0001a740: 6046 616c 7365 6020 746f 2063 6f6e 6669  `False` to confi
+0001a750: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
+0001a760: 2020 2020 2020 2077 6865 7468 6572 206f         whether o
+0001a770: 7220 6e6f 7420 746f 2073 7461 7274 2074  r not to start t
+0001a780: 6865 206d 6174 6572 6961 6c69 7a61 7469  he materializati
+0001a790: 6f6e 206a 6f62 2074 6f20 7772 6974 6520  on job to write 
+0001a7a0: 6461 7461 2074 6f20 7468 6520 6f66 666c  data to the offl
+0001a7b0: 696e 650a 2020 2020 2020 2020 2020 2020  ine.            
+0001a7c0: 2020 2020 2020 7374 6f72 6167 652e 2042        storage. B
+0001a7d0: 7920 6465 6661 756c 7420 7468 6520 6d61  y default the ma
+0001a7e0: 7465 7269 616c 697a 6174 696f 6e20 6a6f  terialization jo
+0001a7f0: 6220 646f 6573 206e 6f74 2067 6574 2073  b does not get s
+0001a800: 7461 7274 6564 2061 7574 6f6d 6174 6963  tarted automatic
+0001a810: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
+0001a820: 2020 2020 2020 2066 6f72 206d 756c 7469         for multi
+0001a830: 2070 6172 7420 696e 7365 7274 732e 0a20   part inserts.. 
+0001a840: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0001a850: 206b 6579 2060 6b61 666b 615f 7072 6f64   key `kafka_prod
+0001a860: 7563 6572 5f63 6f6e 6669 6760 2061 6e64  ucer_config` and
+0001a870: 2076 616c 7565 2061 6e20 6f62 6a65 6374   value an object
+0001a880: 206f 6620 7479 7065 205b 7072 6f70 6572   of type [proper
+0001a890: 7469 6573 5d28 6874 7470 733a 2f2f 646f  ties](https://do
+0001a8a0: 6373 2e63 6f6e 666c 7565 6e74 2e69 6f2f  cs.confluent.io/
+0001a8b0: 706c 6174 666f 726d 2f63 7572 7265 6e74  platform/current
+0001a8c0: 2f63 6c69 656e 7473 2f6c 6962 7264 6b61  /clients/librdka
+0001a8d0: 666b 612f 6874 6d6c 2f6d 645f 434f 4e46  fka/html/md_CONF
+0001a8e0: 4947 5552 4154 494f 4e2e 6874 6d6c 6e29  IGURATION.htmln)
+0001a8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a900: 2020 2075 7365 6420 746f 2063 6f6e 6669     used to confi
+0001a910: 6775 7265 2074 6865 204b 6166 6b61 2063  gure the Kafka c
+0001a920: 6c69 656e 742e 2054 6f20 6f70 7469 6d69  lient. To optimi
+0001a930: 7a65 2066 6f72 2074 6872 6f75 6768 7075  ze for throughpu
+0001a940: 7420 696e 2068 6967 6820 6c61 7465 6e63  t in high latenc
+0001a950: 7920 636f 6e6e 6563 7469 6f6e 2063 6f6e  y connection con
+0001a960: 7369 6465 720a 2020 2020 2020 2020 2020  sider.          
+0001a970: 2020 2020 2020 2020 6368 616e 6769 6e67          changing
+0001a980: 205b 7072 6f64 7563 6572 2070 726f 7065   [producer prope
+0001a990: 7274 6965 735d 2868 7474 7073 3a2f 2f64  rties](https://d
+0001a9a0: 6f63 732e 636f 6e66 6c75 656e 742e 696f  ocs.confluent.io
+0001a9b0: 2f63 6c6f 7564 2f63 7572 7265 6e74 2f63  /cloud/current/c
+0001a9c0: 6c69 656e 742d 6170 7073 2f6f 7074 696d  lient-apps/optim
+0001a9d0: 697a 696e 672f 7468 726f 7567 6870 7574  izing/throughput
+0001a9e0: 2e68 746d 6c23 7072 6f64 7563 6572 292e  .html#producer).
+0001a9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aa00: 202a 206b 6579 2060 696e 7465 726e 616c   * key `internal
+0001aa10: 5f6b 6166 6b61 6020 616e 6420 7661 6c75  _kafka` and valu
+0001aa20: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
+0001aa30: 7365 6020 696e 2063 6173 6520 796f 7520  se` in case you 
+0001aa40: 6573 7461 626c 6973 6865 640a 2020 2020  established.    
+0001aa50: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0001aa60: 6e6e 6563 7469 7669 7479 2066 726f 6d20  nnectivity from 
+0001aa70: 796f 7520 5079 7468 6f6e 2065 6e76 6972  you Python envir
+0001aa80: 6f6e 6d65 6e74 2074 6f20 7468 6520 696e  onment to the in
+0001aa90: 7465 726e 616c 2061 6476 6572 7469 7365  ternal advertise
+0001aaa0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0001aab0: 2020 2020 6c69 7374 656e 6572 7320 6f66      listeners of
+0001aac0: 2074 6865 2048 6f70 7377 6f72 6b73 204b   the Hopsworks K
+0001aad0: 6166 6b61 2043 6c75 7374 6572 2e20 4465  afka Cluster. De
+0001aae0: 6661 756c 7473 2074 6f20 6046 616c 7365  faults to `False
+0001aaf0: 6020 616e 640a 2020 2020 2020 2020 2020  ` and.          
+0001ab00: 2020 2020 2020 2020 7769 6c6c 2075 7365          will use
+0001ab10: 2065 7874 6572 6e61 6c20 6c69 7374 656e   external listen
+0001ab20: 6572 7320 7768 656e 2063 6f6e 6e65 6374  ers when connect
+0001ab30: 696e 6720 6672 6f6d 206f 7574 7369 6465  ing from outside
+0001ab40: 206f 6620 486f 7073 776f 726b 732e 0a20   of Hopsworks.. 
+0001ab50: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+0001ab60: 6174 696f 6e5f 6f70 7469 6f6e 733a 2041  ation_options: A
+0001ab70: 6464 6974 696f 6e61 6c20 7661 6c69 6461  dditional valida
+0001ab80: 7469 6f6e 206f 7074 696f 6e73 2061 7320  tion options as 
+0001ab90: 6b65 792d 7661 6c75 6520 7061 6972 732c  key-value pairs,
+0001aba0: 2064 6566 6175 6c74 7320 746f 2060 7b7d   defaults to `{}
+0001abb0: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
+0001abc0: 2020 202a 206b 6579 2060 7275 6e5f 7661     * key `run_va
+0001abd0: 6c69 6461 7469 6f6e 6020 626f 6f6c 6561  lidation` boolea
+0001abe0: 6e20 7661 6c75 652c 2073 6574 2074 6f20  n value, set to 
+0001abf0: 6046 616c 7365 6020 746f 2073 6b69 7020  `False` to skip 
+0001ac00: 7661 6c69 6461 7469 6f6e 2074 656d 706f  validation tempo
+0001ac10: 7261 7269 6c79 206f 6e20 696e 6765 7374  rarily on ingest
+0001ac20: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+0001ac30: 2020 2020 202a 206b 6579 2060 7361 7665       * key `save
+0001ac40: 5f72 6570 6f72 7460 2062 6f6f 6c65 616e  _report` boolean
+0001ac50: 2076 616c 7565 2c20 7365 7420 746f 2060   value, set to `
+0001ac60: 4661 6c73 6560 2074 6f20 736b 6970 2075  False` to skip u
+0001ac70: 706c 6f61 6420 6f66 2074 6865 2076 616c  pload of the val
+0001ac80: 6964 6174 696f 6e20 7265 706f 7274 2074  idation report t
+0001ac90: 6f20 486f 7073 776f 726b 732e 0a20 2020  o Hopsworks..   
+0001aca0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0001acb0: 6579 2060 6765 5f76 616c 6964 6174 655f  ey `ge_validate_
+0001acc0: 6b77 6172 6773 6020 6120 6469 6374 696f  kwargs` a dictio
+0001acd0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+0001ace0: 6b77 6172 6773 2066 6f72 2074 6865 2076  kwargs for the v
+0001acf0: 616c 6964 6174 6520 6d65 7468 6f64 206f  alidate method o
+0001ad00: 6620 4772 6561 7420 4578 7065 6374 6174  f Great Expectat
+0001ad10: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
+0001ad20: 2020 2020 2020 2a20 6b65 7920 6066 6574        * key `fet
+0001ad30: 6368 5f65 7870 6563 7461 7469 6f6e 5f73  ch_expectation_s
+0001ad40: 7569 7465 6020 6120 626f 6f6c 6561 6e20  uite` a boolean 
+0001ad50: 7661 6c75 652c 2062 7920 6465 6661 756c  value, by defaul
+0001ad60: 7420 6046 616c 7365 6020 666f 7220 6d75  t `False` for mu
+0001ad70: 6c74 6920 7061 7274 2069 6e73 6572 7473  lti part inserts
+0001ad80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ad90: 2020 2020 2074 6f20 636f 6e74 726f 6c20       to control 
+0001ada0: 7768 6574 6865 7220 7468 6520 6578 7065  whether the expe
+0001adb0: 6374 6174 696f 6e20 7375 6974 6520 6f66  ctation suite of
+0001adc0: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
+0001add0: 7570 2073 686f 756c 6420 6265 2066 6574  up should be fet
+0001ade0: 6368 6564 2062 6566 6f72 6520 6576 6572  ched before ever
+0001adf0: 7920 696e 7365 7274 2e0a 0a20 2020 2020  y insert...     
+0001ae00: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
+0001ae10: 2020 2020 2020 2020 2028 604a 6f62 602c           (`Job`,
+0001ae20: 2060 5661 6c69 6461 7469 6f6e 5265 706f   `ValidationRepo
+0001ae30: 7274 6029 2041 2074 7570 6c65 2077 6974  rt`) A tuple wit
+0001ae40: 6820 6a6f 6220 696e 666f 726d 6174 696f  h job informatio
+0001ae50: 6e20 6966 2070 7974 686f 6e20 656e 6769  n if python engi
+0001ae60: 6e65 2069 7320 7573 6564 2061 6e64 2074  ne is used and t
+0001ae70: 6865 2076 616c 6964 6174 696f 6e20 7265  he validation re
+0001ae80: 706f 7274 2069 6620 7661 6c69 6461 7469  port if validati
+0001ae90: 6f6e 2069 7320 656e 6162 6c65 642e 0a20  on is enabled.. 
+0001aea0: 2020 2020 2020 2020 2020 2060 4665 6174             `Feat
+0001aeb0: 7572 6547 726f 7570 5772 6974 6572 6020  ureGroupWriter` 
+0001aec0: 5768 656e 2075 7365 6420 6173 2061 2063  When used as a c
+0001aed0: 6f6e 7465 7874 206d 616e 6167 6572 2077  ontext manager w
+0001aee0: 6974 6820 5079 7468 6f6e 2060 7769 7468  ith Python `with
+0001aef0: 6020 7374 6174 656d 656e 742e 0a20 2020  ` statement..   
+0001af00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001af10: 2073 656c 662e 5f6d 756c 7469 5f70 6172   self._multi_par
+0001af20: 745f 696e 7365 7274 203d 2054 7275 650a  t_insert = True.
+0001af30: 2020 2020 2020 2020 6d75 6c74 695f 7061          multi_pa
+0001af40: 7274 5f77 7269 7465 7220 3d20 6665 6174  rt_writer = feat
+0001af50: 7572 655f 6772 6f75 705f 7772 6974 6572  ure_group_writer
+0001af60: 2e46 6561 7475 7265 4772 6f75 7057 7269  .FeatureGroupWri
+0001af70: 7465 7228 7365 6c66 290a 2020 2020 2020  ter(self).      
+0001af80: 2020 6966 2066 6561 7475 7265 7320 6973    if features is
+0001af90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001afa0: 2020 2072 6574 7572 6e20 6d75 6c74 695f     return multi_
+0001afb0: 7061 7274 5f77 7269 7465 720a 2020 2020  part_writer.    
+0001afc0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001afd0: 2020 2020 2020 2320 676f 2074 6872 6f75        # go throu
+0001afe0: 6768 2077 7269 7465 7220 746f 2061 766f  gh writer to avo
+0001aff0: 6964 2073 6574 7469 6e67 206d 756c 7469  id setting multi
+0001b000: 2069 6e73 6572 7420 6465 6661 756c 7473   insert defaults
+0001b010: 2061 6761 696e 0a20 2020 2020 2020 2020   again.         
+0001b020: 2020 2072 6574 7572 6e20 6d75 6c74 695f     return multi_
+0001b030: 7061 7274 5f77 7269 7465 722e 696e 7365  part_writer.inse
+0001b040: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+0001b050: 2020 2020 6665 6174 7572 6573 2c0a 2020      features,.  
+0001b060: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
+0001b070: 6572 7772 6974 652c 0a20 2020 2020 2020  erwrite,.       
+0001b080: 2020 2020 2020 2020 206f 7065 7261 7469           operati
+0001b090: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0001b0a0: 2020 2020 7374 6f72 6167 652c 0a20 2020      storage,.   
+0001b0b0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+0001b0c0: 7465 5f6f 7074 696f 6e73 2c0a 2020 2020  te_options,.    
+0001b0d0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+0001b0e0: 6461 7469 6f6e 5f6f 7074 696f 6e73 2c0a  dation_options,.
+0001b0f0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0001b100: 2020 2064 6566 2066 696e 616c 697a 655f     def finalize_
+0001b110: 6d75 6c74 695f 7061 7274 5f69 6e73 6572  multi_part_inser
+0001b120: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0001b130: 2022 2222 4669 6e61 6c69 7a65 7320 616e   """Finalizes an
+0001b140: 6420 6578 6974 7320 7468 6520 6d75 6c74  d exits the mult
+0001b150: 6920 7061 7274 2069 6e73 6572 7420 636f  i part insert co
+0001b160: 6e74 6578 7420 6f70 656e 6564 2062 7920  ntext opened by 
+0001b170: 606d 756c 7469 5f70 6172 745f 696e 7365  `multi_part_inse
+0001b180: 7274 600a 2020 2020 2020 2020 696e 2061  rt`.        in a
+0001b190: 2062 6c6f 636b 696e 6720 6661 7368 696f   blocking fashio
+0001b1a0: 6e20 6f6e 6365 2061 6c6c 2072 6f77 7320  n once all rows 
+0001b1b0: 6861 7665 2062 6565 6e20 7472 616e 736d  have been transm
+0001b1c0: 6974 7465 642e 0a0a 2020 2020 2020 2020  itted...        
+0001b1d0: 2121 2120 6578 616d 706c 6520 224d 756c  !!! example "Mul
+0001b1e0: 7469 2070 6172 7420 696e 7365 7274 2077  ti part insert w
+0001b1f0: 6974 6820 6d61 6e75 616c 2063 6f6e 7465  ith manual conte
+0001b200: 7874 206d 616e 6167 656d 656e 7422 0a20  xt management". 
+0001b210: 2020 2020 2020 2020 2020 2049 6e73 7465             Inste
+0001b220: 6164 206f 6620 6c65 7474 696e 6720 5079  ad of letting Py
+0001b230: 7468 6f6e 2068 616e 646c 6520 7468 6520  thon handle the 
+0001b240: 656e 7465 7269 6e67 2061 6e64 2065 7869  entering and exi
+0001b250: 7469 6e67 206f 6620 7468 650a 2020 2020  ting of the.    
+0001b260: 2020 2020 2020 2020 6d75 6c74 6920 7061          multi pa
+0001b270: 7274 2069 6e73 6572 7420 636f 6e74 6578  rt insert contex
+0001b280: 742c 2079 6f75 2063 616e 2073 7461 7274  t, you can start
+0001b290: 2061 6e64 2066 696e 616c 697a 6520 7468   and finalize th
+0001b2a0: 6520 636f 6e74 6578 740a 2020 2020 2020  e context.      
+0001b2b0: 2020 2020 2020 6d61 6e75 616c 6c79 2e0a        manually..
+0001b2c0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+0001b2d0: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+0001b2e0: 2020 6665 6174 7572 655f 6772 6f75 7020    feature_group 
+0001b2f0: 3d20 6673 2e67 6574 5f6f 725f 6372 6561  = fs.get_or_crea
+0001b300: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+0001b310: 2822 6667 5f6e 616d 6522 2c20 7665 7273  ("fg_name", vers
+0001b320: 696f 6e3d 3129 0a0a 2020 2020 2020 2020  ion=1)..        
+0001b330: 2020 2020 7768 696c 6520 6c6f 6f70 3a0a      while loop:.
+0001b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b350: 736d 616c 6c5f 6261 7463 685f 6466 203d  small_batch_df =
+0001b360: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+0001b370: 2020 2020 2066 6561 7475 7265 5f67 726f       feature_gro
+0001b380: 7570 2e6d 756c 7469 5f70 6172 745f 696e  up.multi_part_in
+0001b390: 7365 7274 2873 6d61 6c6c 5f62 6174 6368  sert(small_batch
+0001b3a0: 5f64 6629 0a0a 2020 2020 2020 2020 2020  _df)..          
+0001b3b0: 2020 2320 494d 504f 5254 414e 543a 2066    # IMPORTANT: f
+0001b3c0: 696e 616c 697a 6520 7468 6520 6d75 6c74  inalize the mult
+0001b3d0: 6920 7061 7274 2069 6e73 6572 7420 746f  i part insert to
+0001b3e0: 206d 616b 6520 7375 7265 2061 6c6c 2072   make sure all r
+0001b3f0: 6f77 730a 2020 2020 2020 2020 2020 2020  ows.            
+0001b400: 2320 6861 7665 2062 6565 6e20 7472 616e  # have been tran
+0001b410: 736d 6974 7465 640a 2020 2020 2020 2020  smitted.        
+0001b420: 2020 2020 6665 6174 7572 655f 6772 6f75      feature_grou
+0001b430: 702e 6669 6e61 6c69 7a65 5f6d 756c 7469  p.finalize_multi
+0001b440: 5f70 6172 745f 696e 7365 7274 2829 0a20  _part_insert(). 
+0001b450: 2020 2020 2020 2020 2020 2060 6060 0a20             ```. 
+0001b460: 2020 2020 2020 2020 2020 204e 6f74 6520             Note 
+0001b470: 7468 6174 2074 6865 2066 6972 7374 2063  that the first c
+0001b480: 616c 6c20 746f 2060 6d75 6c74 695f 7061  all to `multi_pa
+0001b490: 7274 5f69 6e73 6572 7460 2069 6e69 7469  rt_insert` initi
+0001b4a0: 6174 6573 2074 6865 2063 6f6e 7465 7874  ates the context
+0001b4b0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001b4c0: 2062 6520 7375 7265 2074 6f20 6669 6e61   be sure to fina
+0001b4d0: 6c69 7a65 2069 742e 2054 6865 2060 6669  lize it. The `fi
+0001b4e0: 6e61 6c69 7a65 5f6d 756c 7469 5f70 6172  nalize_multi_par
+0001b4f0: 745f 696e 7365 7274 6020 6973 2061 0a20  t_insert` is a. 
+0001b500: 2020 2020 2020 2020 2020 2062 6c6f 636b             block
+0001b510: 696e 6720 6361 6c6c 2074 6861 7420 7265  ing call that re
+0001b520: 7475 726e 7320 6f6e 6365 2061 6c6c 2072  turns once all r
+0001b530: 6f77 7320 6861 7665 2062 6565 6e20 7472  ows have been tr
+0001b540: 616e 736d 6974 7465 642e 0a20 2020 2020  ansmitted..     
+0001b550: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0001b560: 6620 7365 6c66 2e5f 6b61 666b 615f 7072  f self._kafka_pr
+0001b570: 6f64 7563 6572 2069 7320 6e6f 7420 4e6f  oducer is not No
+0001b580: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001b590: 7365 6c66 2e5f 6b61 666b 615f 7072 6f64  self._kafka_prod
+0001b5a0: 7563 6572 2e66 6c75 7368 2829 0a20 2020  ucer.flush().   
+0001b5b0: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
+0001b5c0: 6166 6b61 5f70 726f 6475 6365 7220 3d20  afka_producer = 
+0001b5d0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0001b5e0: 662e 5f66 6561 7475 7265 5f77 7269 7465  f._feature_write
+0001b5f0: 7273 203d 204e 6f6e 650a 2020 2020 2020  rs = None.      
+0001b600: 2020 7365 6c66 2e5f 7772 6974 6572 203d    self._writer =
+0001b610: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0001b620: 6c66 2e5f 6d75 6c74 695f 7061 7274 5f69  lf._multi_part_i
+0001b630: 6e73 6572 7420 3d20 4661 6c73 650a 0a20  nsert = False.. 
+0001b640: 2020 2064 6566 2069 6e73 6572 745f 7374     def insert_st
+0001b650: 7265 616d 280a 2020 2020 2020 2020 7365  ream(.        se
+0001b660: 6c66 2c0a 2020 2020 2020 2020 6665 6174  lf,.        feat
+0001b670: 7572 6573 3a20 5479 7065 5661 7228 2270  ures: TypeVar("p
+0001b680: 7973 7061 726b 2e73 716c 2e44 6174 6146  yspark.sql.DataF
+0001b690: 7261 6d65 2229 2c20 2023 206e 6f71 613a  rame"),  # noqa:
+0001b6a0: 2046 3832 310a 2020 2020 2020 2020 7175   F821.        qu
+0001b6b0: 6572 795f 6e61 6d65 3a20 4f70 7469 6f6e  ery_name: Option
+0001b6c0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0001b6d0: 2020 2020 2020 2020 6f75 7470 7574 5f6d          output_m
+0001b6e0: 6f64 653a 204f 7074 696f 6e61 6c5b 7374  ode: Optional[st
+0001b6f0: 725d 203d 2022 6170 7065 6e64 222c 0a20  r] = "append",. 
+0001b700: 2020 2020 2020 2061 7761 6974 5f74 6572         await_ter
+0001b710: 6d69 6e61 7469 6f6e 3a20 4f70 7469 6f6e  mination: Option
+0001b720: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
+0001b730: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
+0001b740: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
+0001b750: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001b760: 2063 6865 636b 706f 696e 745f 6469 723a   checkpoint_dir:
+0001b770: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0001b780: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
+0001b790: 7269 7465 5f6f 7074 696f 6e73 3a20 4f70  rite_options: Op
+0001b7a0: 7469 6f6e 616c 5b44 6963 745b 416e 792c  tional[Dict[Any,
+0001b7b0: 2041 6e79 5d5d 203d 207b 7d2c 0a20 2020   Any]] = {},.   
+0001b7c0: 2029 3a0a 2020 2020 2020 2020 2222 2249   ):.        """I
+0001b7d0: 6e67 6573 7420 6120 5370 6172 6b20 5374  ngest a Spark St
+0001b7e0: 7275 6374 7572 6564 2053 7472 6561 6d69  ructured Streami
+0001b7f0: 6e67 2044 6174 6166 7261 6d65 2074 6f20  ng Dataframe to 
+0001b800: 7468 6520 6f6e 6c69 6e65 2066 6561 7475  the online featu
+0001b810: 7265 2073 746f 7265 2e0a 0a20 2020 2020  re store...     
+0001b820: 2020 2054 6869 7320 6d65 7468 6f64 2063     This method c
+0001b830: 7265 6174 6573 2061 206c 6f6e 6720 7275  reates a long ru
+0001b840: 6e6e 696e 6720 5370 6172 6b20 5374 7265  nning Spark Stre
+0001b850: 616d 696e 6720 5175 6572 792c 2079 6f75  aming Query, you
+0001b860: 2063 616e 2063 6f6e 7472 6f6c 2074 6865   can control the
+0001b870: 0a20 2020 2020 2020 2074 6572 6d69 6e61  .        termina
+0001b880: 7469 6f6e 206f 6620 7468 6520 7175 6572  tion of the quer
+0001b890: 7920 7468 726f 7567 6820 7468 6520 6172  y through the ar
+0001b8a0: 6775 6d65 6e74 732e 0a0a 2020 2020 2020  guments...      
+0001b8b0: 2020 4974 2069 7320 706f 7373 6962 6c65    It is possible
+0001b8c0: 2074 6f20 7374 6f70 2074 6865 2072 6574   to stop the ret
+0001b8d0: 7572 6e65 6420 7175 6572 7920 7769 7468  urned query with
+0001b8e0: 2074 6865 2060 2e73 746f 7028 2960 2061   the `.stop()` a
+0001b8f0: 6e64 2063 6865 636b 2069 7473 0a20 2020  nd check its.   
+0001b900: 2020 2020 2073 7461 7475 7320 7769 7468       status with
+0001b910: 2060 2e69 7341 6374 6976 6560 2e0a 0a20   `.isActive`... 
+0001b920: 2020 2020 2020 2054 6f20 6765 7420 6120         To get a 
+0001b930: 6c69 7374 206f 6620 616c 6c20 6163 7469  list of all acti
+0001b940: 7665 2071 7565 7269 6573 2c20 7573 653a  ve queries, use:
+0001b950: 0a0a 2020 2020 2020 2020 6060 6070 7974  ..        ```pyt
+0001b960: 686f 6e0a 2020 2020 2020 2020 7371 6d20  hon.        sqm 
+0001b970: 3d20 7370 6172 6b2e 7374 7265 616d 730a  = spark.streams.
+0001b980: 0a20 2020 2020 2020 2023 2067 6574 2074  .        # get t
+0001b990: 6865 206c 6973 7420 6f66 2061 6374 6976  he list of activ
+0001b9a0: 6520 7374 7265 616d 696e 6720 7175 6572  e streaming quer
+0001b9b0: 6965 730a 2020 2020 2020 2020 5b71 2e6e  ies.        [q.n
+0001b9c0: 616d 6520 666f 7220 7120 696e 2073 716d  ame for q in sqm
+0001b9d0: 2e61 6374 6976 655d 0a20 2020 2020 2020  .active].       
+0001b9e0: 2060 6060 0a0a 2020 2020 2020 2020 2121   ```..        !!
+0001b9f0: 2120 7761 726e 696e 6720 2245 6e67 696e  ! warning "Engin
+0001ba00: 6520 5375 7070 6f72 7422 0a20 2020 2020  e Support".     
+0001ba10: 2020 2020 2020 202a 2a53 7061 726b 206f         **Spark o
+0001ba20: 6e6c 792a 2a0a 0a20 2020 2020 2020 2020  nly**..         
+0001ba30: 2020 2053 7472 6561 6d20 696e 6765 7374     Stream ingest
+0001ba40: 696f 6e20 7573 696e 6720 5061 6e64 6173  ion using Pandas
+0001ba50: 2f50 7974 686f 6e20 6173 2065 6e67 696e  /Python as engin
+0001ba60: 6520 6973 2063 7572 7265 6e74 6c79 206e  e is currently n
+0001ba70: 6f74 2073 7570 706f 7274 6564 2e0a 2020  ot supported..  
+0001ba80: 2020 2020 2020 2020 2020 5079 7468 6f6e            Python
+0001ba90: 2f50 616e 6461 7320 6861 7320 6e6f 206e  /Pandas has no n
+0001baa0: 6f74 696f 6e20 6f66 2073 7472 6561 6d69  otion of streami
+0001bab0: 6e67 2e0a 0a20 2020 2020 2020 2021 2121  ng...        !!!
+0001bac0: 2077 6172 6e69 6e67 2022 4461 7461 2056   warning "Data V
+0001bad0: 616c 6964 6174 696f 6e20 5375 7070 6f72  alidation Suppor
+0001bae0: 7422 0a20 2020 2020 2020 2020 2020 2060  t".            `
+0001baf0: 696e 7365 7274 5f73 7472 6561 6d60 2064  insert_stream` d
+0001bb00: 6f65 7320 6e6f 7420 7065 7266 6f72 6d20  oes not perform 
+0001bb10: 616e 7920 6461 7461 2076 616c 6964 6174  any data validat
+0001bb20: 696f 6e20 7573 696e 6720 4772 6561 7420  ion using Great 
+0001bb30: 4578 7065 6374 6174 696f 6e73 0a20 2020  Expectations.   
+0001bb40: 2020 2020 2020 2020 2065 7665 6e20 7768           even wh
+0001bb50: 656e 2061 2065 7870 6563 7461 7469 6f6e  en a expectation
+0001bb60: 2073 7569 7465 2069 7320 6174 7461 6368   suite is attach
+0001bb70: 6564 2e0a 0a20 2020 2020 2020 2023 2041  ed...        # A
+0001bb80: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+0001bb90: 2020 2020 2066 6561 7475 7265 733a 2046       features: F
+0001bba0: 6561 7475 7265 7320 696e 2053 7472 6561  eatures in Strea
+0001bbb0: 6d69 6e67 2044 6174 6166 7261 6d65 2074  ming Dataframe t
+0001bbc0: 6f20 6265 2073 6176 6564 2e0a 2020 2020  o be saved..    
+0001bbd0: 2020 2020 2020 2020 7175 6572 795f 6e61          query_na
+0001bbe0: 6d65 3a20 4974 2069 7320 706f 7373 6962  me: It is possib
+0001bbf0: 6c65 2074 6f20 6f70 7469 6f6e 616c 6c79  le to optionally
+0001bc00: 2073 7065 6369 6679 2061 206e 616d 6520   specify a name 
+0001bc10: 666f 7220 7468 6520 7175 6572 7920 746f  for the query to
+0001bc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bc30: 206d 616b 6520 6974 2065 6173 6965 7220   make it easier 
+0001bc40: 746f 2072 6563 6f67 6e69 7365 2069 6e20  to recognise in 
+0001bc50: 7468 6520 5370 6172 6b20 5549 2e20 4465  the Spark UI. De
+0001bc60: 6661 756c 7473 2074 6f20 604e 6f6e 6560  faults to `None`
+0001bc70: 2e0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+0001bc80: 7470 7574 5f6d 6f64 653a 2053 7065 6369  tput_mode: Speci
+0001bc90: 6669 6573 2068 6f77 2064 6174 6120 6f66  fies how data of
+0001bca0: 2061 2073 7472 6561 6d69 6e67 2044 6174   a streaming Dat
+0001bcb0: 6146 7261 6d65 2f44 6174 6173 6574 2069  aFrame/Dataset i
+0001bcc0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001bcd0: 2020 7772 6974 7465 6e20 746f 2061 2073    written to a s
+0001bce0: 7472 6561 6d69 6e67 2073 696e 6b2e 2028  treaming sink. (
+0001bcf0: 3129 2060 2261 7070 656e 6422 603a 204f  1) `"append"`: O
+0001bd00: 6e6c 7920 7468 6520 6e65 7720 726f 7773  nly the new rows
+0001bd10: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+0001bd20: 2020 2020 2020 2020 7374 7265 616d 696e          streamin
+0001bd30: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
+0001bd40: 7365 7420 7769 6c6c 2062 6520 7772 6974  set will be writ
+0001bd50: 7465 6e20 746f 2074 6865 2073 696e 6b2e  ten to the sink.
+0001bd60: 2028 3229 0a20 2020 2020 2020 2020 2020   (2).           
+0001bd70: 2020 2020 2060 2263 6f6d 706c 6574 6522       `"complete"
+0001bd80: 603a 2041 6c6c 2074 6865 2072 6f77 7320  `: All the rows 
+0001bd90: 696e 2074 6865 2073 7472 6561 6d69 6e67  in the streaming
+0001bda0: 2044 6174 6146 7261 6d65 2f44 6174 6173   DataFrame/Datas
+0001bdb0: 6574 2077 696c 6c20 6265 0a20 2020 2020  et will be.     
+0001bdc0: 2020 2020 2020 2020 2020 2077 7269 7474             writt
+0001bdd0: 656e 2074 6f20 7468 6520 7369 6e6b 2065  en to the sink e
+0001bde0: 7665 7279 2074 696d 6520 7468 6572 6520  very time there 
+0001bdf0: 6973 2073 6f6d 6520 7570 6461 7465 2e20  is some update. 
+0001be00: 2833 2920 6022 7570 6461 7465 2260 3a0a  (3) `"update"`:.
+0001be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be20: 6f6e 6c79 2074 6865 2072 6f77 7320 7468  only the rows th
+0001be30: 6174 2077 6572 6520 7570 6461 7465 6420  at were updated 
+0001be40: 696e 2074 6865 2073 7472 6561 6d69 6e67  in the streaming
+0001be50: 2044 6174 6146 7261 6d65 2f44 6174 6173   DataFrame/Datas
+0001be60: 6574 2077 696c 6c0a 2020 2020 2020 2020  et will.        
+0001be70: 2020 2020 2020 2020 6265 2077 7269 7474          be writt
+0001be80: 656e 2074 6f20 7468 6520 7369 6e6b 2065  en to the sink e
+0001be90: 7665 7279 2074 696d 6520 7468 6572 6520  very time there 
+0001bea0: 6172 6520 736f 6d65 2075 7064 6174 6573  are some updates
+0001beb0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bec0: 2020 4966 2074 6865 2071 7565 7279 2064    If the query d
+0001bed0: 6f65 736e e280 9974 2063 6f6e 7461 696e  oesn...t contain
+0001bee0: 2061 6767 7265 6761 7469 6f6e 732c 2069   aggregations, i
+0001bef0: 7420 7769 6c6c 2062 6520 6571 7569 7661  t will be equiva
+0001bf00: 6c65 6e74 2074 6f0a 2020 2020 2020 2020  lent to.        
+0001bf10: 2020 2020 2020 2020 6170 7065 6e64 206d          append m
+0001bf20: 6f64 652e 2044 6566 6175 6c74 7320 746f  ode. Defaults to
+0001bf30: 2060 2261 7070 656e 6422 602e 0a20 2020   `"append"`..   
+0001bf40: 2020 2020 2020 2020 2061 7761 6974 5f74           await_t
+0001bf50: 6572 6d69 6e61 7469 6f6e 3a20 5761 6974  ermination: Wait
+0001bf60: 7320 666f 7220 7468 6520 7465 726d 696e  s for the termin
+0001bf70: 6174 696f 6e20 6f66 2074 6869 7320 7175  ation of this qu
+0001bf80: 6572 792c 2065 6974 6865 7220 6279 0a20  ery, either by. 
+0001bf90: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+0001bfa0: 7565 7279 2e73 746f 7028 2920 6f72 2062  uery.stop() or b
+0001bfb0: 7920 616e 2065 7863 6570 7469 6f6e 2e20  y an exception. 
+0001bfc0: 4966 2074 6865 2071 7565 7279 2068 6173  If the query has
+0001bfd0: 2074 6572 6d69 6e61 7465 6420 7769 7468   terminated with
+0001bfe0: 2061 6e0a 2020 2020 2020 2020 2020 2020   an.            
+0001bff0: 2020 2020 6578 6365 7074 696f 6e2c 2074      exception, t
+0001c000: 6865 6e20 7468 6520 6578 6365 7074 696f  hen the exceptio
+0001c010: 6e20 7769 6c6c 2062 6520 7468 726f 776e  n will be thrown
+0001c020: 2e20 4966 2074 696d 656f 7574 2069 7320  . If timeout is 
+0001c030: 7365 742c 2069 740a 2020 2020 2020 2020  set, it.        
+0001c040: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+0001c050: 7768 6574 6865 7220 7468 6520 7175 6572  whether the quer
+0001c060: 7920 6861 7320 7465 726d 696e 6174 6564  y has terminated
+0001c070: 206f 7220 6e6f 7420 7769 7468 696e 2074   or not within t
+0001c080: 6865 2074 696d 656f 7574 0a20 2020 2020  he timeout.     
+0001c090: 2020 2020 2020 2020 2020 2073 6563 6f6e             secon
+0001c0a0: 6473 2e20 4465 6661 756c 7473 2074 6f20  ds. Defaults to 
+0001c0b0: 6046 616c 7365 602e 0a20 2020 2020 2020  `False`..       
+0001c0c0: 2020 2020 2074 696d 656f 7574 3a20 4f6e       timeout: On
+0001c0d0: 6c79 2072 656c 6576 616e 7420 696e 2063  ly relevant in c
+0001c0e0: 6f6d 6269 6e61 7469 6f6e 2077 6974 6820  ombination with 
+0001c0f0: 6061 7761 6974 5f74 6572 6d69 6e61 7469  `await_terminati
+0001c100: 6f6e 3d54 7275 6560 2e0a 2020 2020 2020  on=True`..      
+0001c110: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0001c120: 7473 2074 6f20 604e 6f6e 6560 2e0a 2020  ts to `None`..  
+0001c130: 2020 2020 2020 2020 2020 6368 6563 6b70            checkp
+0001c140: 6f69 6e74 5f64 6972 3a20 4368 6563 6b70  oint_dir: Checkp
+0001c150: 6f69 6e74 2064 6972 6563 746f 7279 206c  oint directory l
+0001c160: 6f63 6174 696f 6e2e 2054 6869 7320 7769  ocation. This wi
+0001c170: 6c6c 2062 6520 7573 6564 2074 6f20 6173  ll be used to as
+0001c180: 2061 2072 6566 6572 656e 6365 2074 6f0a   a reference to.
+0001c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1a0: 6672 6f6d 2077 6865 7265 2074 6f20 7265  from where to re
+0001c1b0: 7375 6d65 2074 6865 2073 7472 6561 6d69  sume the streami
+0001c1c0: 6e67 206a 6f62 2e20 4966 2060 4e6f 6e65  ng job. If `None
+0001c1d0: 6020 7468 656e 2068 7366 7320 7769 6c6c  ` then hsfs will
+0001c1e0: 2063 6f6e 7374 7275 6374 2061 730a 2020   construct as.  
+0001c1f0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+0001c200: 6e73 6572 745f 7374 7265 616d 5f22 202b  nsert_stream_" +
+0001c210: 206f 6e6c 696e 655f 746f 7069 635f 6e61   online_topic_na
+0001c220: 6d65 2e20 4465 6661 756c 7473 2074 6f20  me. Defaults to 
+0001c230: 604e 6f6e 6560 2e0a 2020 2020 2020 2020  `None`..        
+0001c240: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
+0001c250: 7469 6f6e 733a 2041 6464 6974 696f 6e61  tions: Additiona
+0001c260: 6c20 7772 6974 6520 6f70 7469 6f6e 7320  l write options 
+0001c270: 666f 7220 5370 6172 6b20 6173 206b 6579  for Spark as key
+0001c280: 2d76 616c 7565 2070 6169 7273 2e0a 2020  -value pairs..  
+0001c290: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0001c2a0: 6661 756c 7473 2074 6f20 607b 7d60 2e0a  faults to `{}`..
+0001c2b0: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+0001c2c0: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
+0001c2d0: 5374 7265 616d 696e 6751 7565 7279 603a  StreamingQuery`:
+0001c2e0: 2053 7061 726b 2053 7472 7563 7475 7265   Spark Structure
+0001c2f0: 6420 5374 7265 616d 696e 6720 5175 6572  d Streaming Quer
+0001c300: 7920 6f62 6a65 6374 2e0a 2020 2020 2020  y object..      
+0001c310: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0001c320: 2028 0a20 2020 2020 2020 2020 2020 206e   (.            n
+0001c330: 6f74 2065 6e67 696e 652e 6765 745f 696e  ot engine.get_in
+0001c340: 7374 616e 6365 2829 2e69 735f 7370 6172  stance().is_spar
+0001c350: 6b5f 6461 7461 6672 616d 6528 6665 6174  k_dataframe(feat
+0001c360: 7572 6573 290a 2020 2020 2020 2020 2020  ures).          
+0001c370: 2020 6f72 206e 6f74 2066 6561 7475 7265    or not feature
+0001c380: 732e 6973 5374 7265 616d 696e 670a 2020  s.isStreaming.  
+0001c390: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0001c3a0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+0001c3b0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0001c3c0: 2020 2020 2020 2246 6561 7475 7265 7320        "Features 
+0001c3d0: 6861 7665 2074 6f20 6265 2061 2073 7472  have to be a str
+0001c3e0: 6561 6d69 6e67 2074 7970 6520 7370 6172  eaming type spar
+0001c3f0: 6b20 6461 7461 6672 616d 652e 2055 7365  k dataframe. Use
+0001c400: 2060 696e 7365 7274 2829 6020 6d65 7468   `insert()` meth
+0001c410: 6f64 2069 6e73 7465 6164 2e22 0a20 2020  od instead.".   
+0001c420: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001c430: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001c440: 2020 2020 2023 206c 6f77 6572 2063 6173       # lower cas
+0001c450: 696e 6720 6665 6174 7572 6520 6e61 6d65  ing feature name
+0001c460: 730a 2020 2020 2020 2020 2020 2020 6665  s.            fe
+0001c470: 6174 7572 655f 6461 7461 6672 616d 6520  ature_dataframe 
+0001c480: 3d20 656e 6769 6e65 2e67 6574 5f69 6e73  = engine.get_ins
+0001c490: 7461 6e63 6528 292e 636f 6e76 6572 745f  tance().convert_
+0001c4a0: 746f 5f64 6566 6175 6c74 5f64 6174 6166  to_default_dataf
+0001c4b0: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
+0001c4c0: 2020 2020 2020 6665 6174 7572 6573 0a20        features. 
+0001c4d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001c4e0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0001c4f0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+0001c500: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+0001c510: 2020 2020 2020 2020 2020 2020 2020 2253                "S
+0001c520: 7472 6561 6d20 696e 6765 7374 696f 6e20  tream ingestion 
+0001c530: 666f 7220 6665 6174 7572 6520 6772 6f75  for feature grou
+0001c540: 7020 607b 7d60 2c20 7769 7468 2076 6572  p `{}`, with ver
+0001c550: 7369 6f6e 220a 2020 2020 2020 2020 2020  sion".          
+0001c560: 2020 2020 2020 2020 2020 2220 607b 7d60            " `{}`
+0001c570: 2077 696c 6c20 6e6f 7420 636f 6d70 7574   will not comput
+0001c580: 6520 7374 6174 6973 7469 6373 2e22 0a20  e statistics.". 
+0001c590: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001c5a0: 2e66 6f72 6d61 7428 7365 6c66 2e5f 6e61  .format(self._na
+0001c5b0: 6d65 2c20 7365 6c66 2e5f 7665 7273 696f  me, self._versio
+0001c5c0: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
+0001c5d0: 2020 2020 7574 696c 2e53 7461 7469 7374      util.Statist
+0001c5e0: 6963 7357 6172 6e69 6e67 2c0a 2020 2020  icsWarning,.    
+0001c5f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001c600: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001c610: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+0001c620: 705f 656e 6769 6e65 2e69 6e73 6572 745f  p_engine.insert_
+0001c630: 7374 7265 616d 280a 2020 2020 2020 2020  stream(.        
+0001c640: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0001c650: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+0001c660: 6174 7572 655f 6461 7461 6672 616d 652c  ature_dataframe,
+0001c670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c680: 2071 7565 7279 5f6e 616d 652c 0a20 2020   query_name,.   
+0001c690: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0001c6a0: 7075 745f 6d6f 6465 2c0a 2020 2020 2020  put_mode,.      
+0001c6b0: 2020 2020 2020 2020 2020 6177 6169 745f            await_
+0001c6c0: 7465 726d 696e 6174 696f 6e2c 0a20 2020  termination,.   
+0001c6d0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+0001c6e0: 656f 7574 2c0a 2020 2020 2020 2020 2020  eout,.          
+0001c6f0: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
+0001c700: 5f64 6972 2c0a 2020 2020 2020 2020 2020  _dir,.          
+0001c710: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
+0001c720: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+0001c730: 2029 0a0a 2020 2020 6465 6620 636f 6d6d   )..    def comm
+0001c740: 6974 5f64 6574 6169 6c73 280a 2020 2020  it_details(.    
+0001c750: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0001c760: 2020 7761 6c6c 636c 6f63 6b5f 7469 6d65    wallclock_time
+0001c770: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+0001c780: 5b73 7472 2c20 696e 742c 2064 6174 6574  [str, int, datet
+0001c790: 696d 652c 2064 6174 655d 5d20 3d20 4e6f  ime, date]] = No
+0001c7a0: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
+0001c7b0: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
+0001c7c0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0001c7d0: 2020 2020 2020 2020 2222 2252 6574 7269          """Retri
+0001c7e0: 6576 6573 2063 6f6d 6d69 7420 7469 6d65  eves commit time
+0001c7f0: 6c69 6e65 2066 6f72 2074 6869 7320 6665  line for this fe
+0001c800: 6174 7572 6520 6772 6f75 702e 2054 6869  ature group. Thi
+0001c810: 7320 6d65 7468 6f64 2063 616e 206f 6e6c  s method can onl
+0001c820: 7920 6265 2075 7365 640a 2020 2020 2020  y be used.      
+0001c830: 2020 6f6e 2074 696d 6520 7472 6176 656c    on time travel
+0001c840: 2065 6e61 626c 6564 2066 6561 7475 7265   enabled feature
+0001c850: 2067 726f 7570 730a 0a20 2020 2020 2020   groups..       
+0001c860: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+0001c870: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+0001c880: 6f6e 0a20 2020 2020 2020 2020 2020 2023  on.            #
+0001c890: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
+0001c8a0: 4665 6174 7572 6520 5374 6f72 650a 2020  Feature Store.  
+0001c8b0: 2020 2020 2020 2020 2020 6673 203d 202e            fs = .
+0001c8c0: 2e2e 0a0a 2020 2020 2020 2020 2020 2020  ....            
+0001c8d0: 2320 6765 7420 7468 6520 4665 6174 7572  # get the Featur
+0001c8e0: 6520 4772 6f75 7020 696e 7374 616e 6365  e Group instance
+0001c8f0: 0a20 2020 2020 2020 2020 2020 2066 6720  .            fg 
+0001c900: 3d20 6673 2e67 6574 5f6f 725f 6372 6561  = fs.get_or_crea
+0001c910: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+0001c920: 282e 2e2e 290a 0a20 2020 2020 2020 2020  (...)..         
+0001c930: 2020 2063 6f6d 6d69 745f 6465 7461 696c     commit_detail
+0001c940: 7320 3d20 6667 2e63 6f6d 6d69 745f 6465  s = fg.commit_de
+0001c950: 7461 696c 7328 290a 2020 2020 2020 2020  tails().        
+0001c960: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+0001c970: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
+0001c980: 2020 2020 2020 2020 2077 616c 6c63 6c6f           wallclo
+0001c990: 636b 5f74 696d 653a 2043 6f6d 6d69 7420  ck_time: Commit 
+0001c9a0: 6465 7461 696c 7320 6173 206f 6620 7370  details as of sp
+0001c9b0: 6563 6966 6963 2070 6f69 6e74 2069 6e20  ecific point in 
+0001c9c0: 7469 6d65 2e20 4465 6661 756c 7473 2074  time. Defaults t
+0001c9d0: 6f20 604e 6f6e 6560 2e0a 2020 2020 2020  o `None`..      
+0001c9e0: 2020 2020 2020 2020 2020 2053 7472 696e             Strin
+0001c9f0: 6773 2073 686f 756c 6420 6265 2066 6f72  gs should be for
+0001ca00: 6d61 7474 6564 2069 6e20 6f6e 6520 6f66  matted in one of
+0001ca10: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
+0001ca20: 6f72 6d61 7473 2060 2559 2d25 6d2d 2564  ormats `%Y-%m-%d
+0001ca30: 602c 2060 2559 2d25 6d2d 2564 2025 4860  `, `%Y-%m-%d %H`
+0001ca40: 2c20 6025 592d 256d 2d25 6420 2548 3a25  , `%Y-%m-%d %H:%
+0001ca50: 4d60 2c0a 2020 2020 2020 2020 2020 2020  M`,.            
+0001ca60: 2020 2020 6025 592d 256d 2d25 6420 2548      `%Y-%m-%d %H
+0001ca70: 3a25 4d3a 2553 602c 206f 7220 6025 592d  :%M:%S`, or `%Y-
+0001ca80: 256d 2d25 6420 2548 3a25 4d3a 2553 2e25  %m-%d %H:%M:%S.%
+0001ca90: 6660 2e0a 2020 2020 2020 2020 2020 2020  f`..            
+0001caa0: 6c69 6d69 743a 204e 756d 6265 7220 6f66  limit: Number of
+0001cab0: 2063 6f6d 6d69 7473 2074 6f20 7265 7472   commits to retr
+0001cac0: 6965 7665 2e20 4465 6661 756c 7473 2074  ieve. Defaults t
+0001cad0: 6f20 604e 6f6e 6560 2e0a 0a20 2020 2020  o `None`...     
+0001cae0: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
+0001caf0: 2020 2020 2020 2020 2060 4469 6374 5b73           `Dict[s
+0001cb00: 7472 2c20 4469 6374 5b73 7472 2c20 7374  tr, Dict[str, st
+0001cb10: 725d 5d60 2e20 4469 6374 696f 6e61 7279  r]]`. Dictionary
+0001cb20: 206f 626a 6563 7420 6f66 2063 6f6d 6d69   object of commi
+0001cb30: 7420 6d65 7461 6461 7461 2074 696d 656c  t metadata timel
+0001cb40: 696e 652c 2077 6865 7265 204b 6579 2069  ine, where Key i
+0001cb50: 7320 636f 6d6d 6974 2069 6420 616e 6420  s commit id and 
+0001cb60: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
+0001cb70: 2020 6973 2060 4469 6374 5b73 7472 2c20    is `Dict[str, 
+0001cb80: 7374 725d 6020 7769 7468 206b 6579 2076  str]` with key v
+0001cb90: 616c 7565 2070 6169 7273 206f 6620 6461  alue pairs of da
+0001cba0: 7465 2063 6f6d 6d69 7474 6564 206f 6e2c  te committed on,
+0001cbb0: 206e 756d 6265 7220 6f66 2072 6f77 7320   number of rows 
+0001cbc0: 7570 6461 7465 642c 2069 6e73 6572 7465  updated, inserte
+0001cbd0: 6420 616e 6420 6465 6c65 7465 642e 0a0a  d and deleted...
+0001cbe0: 2020 2020 2020 2020 2320 5261 6973 6573          # Raises
+0001cbf0: 0a20 2020 2020 2020 2020 2020 2060 6873  .            `hs
+0001cc00: 6673 2e63 6c69 656e 742e 6578 6365 7074  fs.client.except
+0001cc10: 696f 6e73 2e52 6573 7441 5049 4572 726f  ions.RestAPIErro
+0001cc20: 7260 2e0a 2020 2020 2020 2020 2020 2020  r`..            
+0001cc30: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
+0001cc40: 6570 7469 6f6e 732e 4665 6174 7572 6553  eptions.FeatureS
+0001cc50: 746f 7265 4578 6365 7074 696f 6e60 2e20  toreException`. 
+0001cc60: 4966 2074 6865 2066 6561 7475 7265 2067  If the feature g
+0001cc70: 726f 7570 2064 6f65 7320 6e6f 7420 6861  roup does not ha
+0001cc80: 7665 2060 4855 4449 6020 7469 6d65 2074  ve `HUDI` time t
+0001cc90: 7261 7665 6c20 666f 726d 6174 0a20 2020  ravel format.   
+0001cca0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001ccb0: 2072 6574 7572 6e20 7365 6c66 2e5f 6665   return self._fe
+0001ccc0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
+0001ccd0: 6e65 2e63 6f6d 6d69 745f 6465 7461 696c  ne.commit_detail
+0001cce0: 7328 7365 6c66 2c20 7761 6c6c 636c 6f63  s(self, wallcloc
+0001ccf0: 6b5f 7469 6d65 2c20 6c69 6d69 7429 0a0a  k_time, limit)..
+0001cd00: 2020 2020 6465 6620 636f 6d6d 6974 5f64      def commit_d
+0001cd10: 656c 6574 655f 7265 636f 7264 280a 2020  elete_record(.  
+0001cd20: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0001cd30: 2020 2020 6465 6c65 7465 5f64 663a 2054      delete_df: T
+0001cd40: 7970 6556 6172 2822 7079 7370 6172 6b2e  ypeVar("pyspark.
+0001cd50: 7371 6c2e 4461 7461 4672 616d 6522 292c  sql.DataFrame"),
+0001cd60: 2020 2320 6e6f 7161 3a20 4638 3231 0a20    # noqa: F821. 
+0001cd70: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
+0001cd80: 696f 6e73 3a20 4f70 7469 6f6e 616c 5b44  ions: Optional[D
+0001cd90: 6963 745b 416e 792c 2041 6e79 5d5d 203d  ict[Any, Any]] =
+0001cda0: 207b 7d2c 0a20 2020 2029 3a0a 2020 2020   {},.    ):.    
+0001cdb0: 2020 2020 2222 2244 726f 7073 2072 6563      """Drops rec
+0001cdc0: 6f72 6473 2070 7265 7365 6e74 2069 6e20  ords present in 
+0001cdd0: 7468 6520 7072 6f76 6964 6564 2044 6174  the provided Dat
+0001cde0: 6146 7261 6d65 2061 6e64 2063 6f6d 6d69  aFrame and commi
+0001cdf0: 7473 2069 7420 6173 2075 7064 6174 6520  ts it as update 
+0001ce00: 746f 2074 6869 730a 2020 2020 2020 2020  to this.        
+0001ce10: 4665 6174 7572 6520 6772 6f75 702e 2054  Feature group. T
+0001ce20: 6869 7320 6d65 7468 6f64 2063 616e 206f  his method can o
+0001ce30: 6e6c 7920 6265 2075 7365 6420 6f6e 2066  nly be used on f
+0001ce40: 6561 7475 7265 2067 726f 7570 7320 7374  eature groups st
+0001ce50: 6f72 6564 2061 7320 4855 4449 206f 7220  ored as HUDI or 
+0001ce60: 4445 4c54 412e 0a0a 2020 2020 2020 2020  DELTA...        
+0001ce70: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+0001ce80: 2020 2020 2020 2020 6465 6c65 7465 5f64          delete_d
+0001ce90: 663a 2064 6174 6146 7261 6d65 2063 6f6e  f: dataFrame con
+0001cea0: 7461 696e 696e 6720 7265 636f 7264 7320  taining records 
+0001ceb0: 746f 2062 6520 6465 6c65 7465 642e 0a20  to be deleted.. 
+0001cec0: 2020 2020 2020 2020 2020 2077 7269 7465             write
+0001ced0: 5f6f 7074 696f 6e73 3a20 5573 6572 2070  _options: User p
+0001cee0: 726f 7669 6465 6420 7772 6974 6520 6f70  rovided write op
+0001cef0: 7469 6f6e 732e 2044 6566 6175 6c74 7320  tions. Defaults 
+0001cf00: 746f 2060 7b7d 602e 0a0a 2020 2020 2020  to `{}`...      
+0001cf10: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
+0001cf20: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+0001cf30: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
+0001cf40: 6573 7441 5049 4572 726f 7260 2e0a 2020  estAPIError`..  
+0001cf50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001cf60: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
+0001cf70: 6772 6f75 705f 656e 6769 6e65 2e63 6f6d  group_engine.com
+0001cf80: 6d69 745f 6465 6c65 7465 2873 656c 662c  mit_delete(self,
+0001cf90: 2064 656c 6574 655f 6466 2c20 7772 6974   delete_df, writ
+0001cfa0: 655f 6f70 7469 6f6e 7329 0a0a 2020 2020  e_options)..    
+0001cfb0: 6465 6620 6173 5f6f 6628 0a20 2020 2020  def as_of(.     
+0001cfc0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0001cfd0: 2077 616c 6c63 6c6f 636b 5f74 696d 653a   wallclock_time:
+0001cfe0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0001cff0: 7374 722c 2069 6e74 2c20 6461 7465 7469  str, int, dateti
+0001d000: 6d65 2c20 6461 7465 5d5d 203d 204e 6f6e  me, date]] = Non
+0001d010: 652c 0a20 2020 2020 2020 2065 7863 6c75  e,.        exclu
+0001d020: 6465 5f75 6e74 696c 3a20 4f70 7469 6f6e  de_until: Option
+0001d030: 616c 5b55 6e69 6f6e 5b73 7472 2c20 696e  al[Union[str, in
+0001d040: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
+0001d050: 655d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  e]] = None,.    
+0001d060: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+0001d070: 7420 5175 6572 7920 6f62 6a65 6374 2074  t Query object t
+0001d080: 6f20 7265 7472 6965 7665 2061 6c6c 2066  o retrieve all f
+0001d090: 6561 7475 7265 7320 6f66 2074 6865 2067  eatures of the g
+0001d0a0: 726f 7570 2061 7420 6120 706f 696e 7420  roup at a point 
+0001d0b0: 696e 2074 6865 2070 6173 742e 0a0a 2020  in the past...  
+0001d0c0: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
+0001d0d0: 6420 7365 6c65 6374 7320 616c 6c20 6665  d selects all fe
+0001d0e0: 6174 7572 6573 2069 6e20 7468 6520 6665  atures in the fe
+0001d0f0: 6174 7572 6520 6772 6f75 7020 616e 6420  ature group and 
+0001d100: 7265 7475 726e 7320 6120 5175 6572 7920  returns a Query 
+0001d110: 6f62 6a65 6374 0a20 2020 2020 2020 2061  object.        a
+0001d120: 7420 7468 6520 7370 6563 6966 6965 6420  t the specified 
+0001d130: 706f 696e 7420 696e 2074 696d 652e 204f  point in time. O
+0001d140: 7074 696f 6e61 6c6c 792c 2063 6f6d 6d69  ptionally, commi
+0001d150: 7473 2062 6566 6f72 6520 6120 7370 6563  ts before a spec
+0001d160: 6966 6965 6420 706f 696e 7420 696e 2074  ified point in t
+0001d170: 696d 6520 6361 6e20 6265 0a20 2020 2020  ime can be.     
+0001d180: 2020 2065 7863 6c75 6465 6420 6672 6f6d     excluded from
+0001d190: 2074 6865 2071 7565 7279 2e20 5468 6520   the query. The 
+0001d1a0: 5175 6572 7920 6361 6e20 7468 656e 2065  Query can then e
+0001d1b0: 6974 6865 7220 6265 2072 6561 6420 696e  ither be read in
+0001d1c0: 746f 2061 2044 6174 6166 7261 6d65 0a20  to a Dataframe. 
+0001d1d0: 2020 2020 2020 206f 7220 7573 6564 2066         or used f
+0001d1e0: 7572 7468 6572 2074 6f20 7065 7266 6f72  urther to perfor
+0001d1f0: 6d20 6a6f 696e 7320 6f72 2063 6f6e 7374  m joins or const
+0001d200: 7275 6374 2061 2074 7261 696e 696e 6720  ruct a training 
+0001d210: 6461 7461 7365 742e 0a0a 2020 2020 2020  dataset...      
+0001d220: 2020 2121 2120 6578 616d 706c 6520 2252    !!! example "R
+0001d230: 6561 6469 6e67 2066 6561 7475 7265 7320  eading features 
+0001d240: 6174 2061 2073 7065 6369 6669 6320 706f  at a specific po
+0001d250: 696e 7420 696e 2074 696d 653a 220a 2020  int in time:".  
+0001d260: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
+0001d270: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
+0001d280: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
+0001d290: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
+0001d2a0: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
+0001d2b0: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
+0001d2c0: 2023 2067 6574 2074 6865 2046 6561 7475   # get the Featu
+0001d2d0: 7265 2047 726f 7570 2069 6e73 7461 6e63  re Group instanc
+0001d2e0: 650a 2020 2020 2020 2020 2020 2020 6667  e.            fg
+0001d2f0: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
+0001d300: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+0001d310: 7028 2e2e 2e29 0a0a 2020 2020 2020 2020  p(...)..        
+0001d320: 2020 2020 2320 6765 7420 6461 7461 2061      # get data a
+0001d330: 7420 6120 7370 6563 6966 6963 2070 6f69  t a specific poi
+0001d340: 6e74 2069 6e20 7469 6d65 2061 6e64 2073  nt in time and s
+0001d350: 686f 7720 6974 0a20 2020 2020 2020 2020  how it.         
+0001d360: 2020 2066 672e 6173 5f6f 6628 2232 3032     fg.as_of("202
+0001d370: 302d 3130 2d32 3020 3037 3a33 343a 3131  0-10-20 07:34:11
+0001d380: 2229 2e72 6561 6428 292e 7368 6f77 2829  ").read().show()
+0001d390: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+0001d3a0: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
+0001d3b0: 616d 706c 6520 2252 6561 6469 6e67 2063  ample "Reading c
+0001d3c0: 6f6d 6d69 7473 2069 6e63 7265 6d65 6e74  ommits increment
+0001d3d0: 616c 6c79 2062 6574 7765 656e 2073 7065  ally between spe
+0001d3e0: 6369 6669 6564 2070 6f69 6e74 7320 696e  cified points in
+0001d3f0: 2074 696d 653a 220a 2020 2020 2020 2020   time:".        
+0001d400: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+0001d410: 2020 2020 2020 2020 2020 6667 2e61 735f            fg.as_
+0001d420: 6f66 2822 3230 3230 2d31 302d 3230 2030  of("2020-10-20 0
+0001d430: 373a 3334 3a31 3122 2c20 6578 636c 7564  7:34:11", exclud
+0001d440: 655f 756e 7469 6c3d 2232 3032 302d 3130  e_until="2020-10
+0001d450: 2d31 3920 3037 3a33 343a 3131 2229 2e72  -19 07:34:11").r
+0001d460: 6561 6428 292e 7368 6f77 2829 0a20 2020  ead().show().   
+0001d470: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
+0001d480: 2020 2020 2020 5468 6520 6669 7273 7420        The first 
+0001d490: 7061 7261 6d65 7465 7220 6973 2069 6e63  parameter is inc
+0001d4a0: 6c75 7369 7665 2077 6869 6c65 2074 6865  lusive while the
+0001d4b0: 206c 6174 7465 7220 6973 2065 7863 6c75   latter is exclu
+0001d4c0: 7369 7665 2e0a 2020 2020 2020 2020 5468  sive..        Th
+0001d4d0: 6174 206d 6561 6e73 2c20 696e 206f 7264  at means, in ord
+0001d4e0: 6572 2074 6f20 7175 6572 7920 6120 7369  er to query a si
+0001d4f0: 6e67 6c65 2063 6f6d 6d69 742c 2079 6f75  ngle commit, you
+0001d500: 206e 6565 6420 746f 2071 7565 7279 2074   need to query t
+0001d510: 6861 7420 636f 6d6d 6974 2074 696d 650a  hat commit time.
+0001d520: 2020 2020 2020 2020 616e 6420 6578 636c          and excl
+0001d530: 7564 6520 6576 6572 7974 6869 6e67 206a  ude everything j
+0001d540: 7573 7420 6265 666f 7265 2074 6865 2063  ust before the c
+0001d550: 6f6d 6d69 742e 0a0a 2020 2020 2020 2020  ommit...        
+0001d560: 2121 2120 6578 616d 706c 6520 2252 6561  !!! example "Rea
+0001d570: 6469 6e67 206f 6e6c 7920 7468 6520 6368  ding only the ch
+0001d580: 616e 6765 7320 6672 6f6d 2061 2073 696e  anges from a sin
+0001d590: 676c 6520 636f 6d6d 6974 220a 2020 2020  gle commit".    
+0001d5a0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+0001d5b0: 6e0a 2020 2020 2020 2020 2020 2020 6667  n.            fg
+0001d5c0: 2e61 735f 6f66 2822 3230 3230 2d31 302d  .as_of("2020-10-
+0001d5d0: 3230 2030 373a 3331 3a33 3822 2c20 6578  20 07:31:38", ex
+0001d5e0: 636c 7564 655f 756e 7469 6c3d 2232 3032  clude_until="202
+0001d5f0: 302d 3130 2d32 3020 3037 3a33 313a 3337  0-10-20 07:31:37
+0001d600: 2229 2e72 6561 6428 292e 7368 6f77 2829  ").read().show()
+0001d610: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+0001d620: 0a0a 2020 2020 2020 2020 5768 656e 206e  ..        When n
+0001d630: 6f20 7761 6c6c 636c 6f63 6b5f 7469 6d65  o wallclock_time
+0001d640: 2069 7320 6769 7665 6e2c 2074 6865 206c   is given, the l
+0001d650: 6174 6573 7420 7374 6174 6520 6f66 2066  atest state of f
+0001d660: 6561 7475 7265 7320 6973 2072 6574 7572  eatures is retur
+0001d670: 6e65 642e 204f 7074 696f 6e61 6c6c 792c  ned. Optionally,
+0001d680: 2063 6f6d 6d69 7473 2062 6566 6f72 650a   commits before.
+0001d690: 2020 2020 2020 2020 6120 7370 6563 6966          a specif
+0001d6a0: 6965 6420 706f 696e 7420 696e 2074 696d  ied point in tim
+0001d6b0: 6520 6361 6e20 7374 696c 6c20 6265 2065  e can still be e
+0001d6c0: 7863 6c75 6465 642e 0a0a 2020 2020 2020  xcluded...      
+0001d6d0: 2020 2121 2120 6578 616d 706c 6520 2252    !!! example "R
+0001d6e0: 6561 6469 6e67 2074 6865 206c 6174 6573  eading the lates
+0001d6f0: 7420 7374 6174 6520 6f66 2066 6561 7475  t state of featu
+0001d700: 7265 732c 2065 7863 6c75 6469 6e67 2063  res, excluding c
+0001d710: 6f6d 6d69 7473 2062 6566 6f72 6520 6120  ommits before a 
+0001d720: 7370 6563 6966 6965 6420 706f 696e 7420  specified point 
+0001d730: 696e 2074 696d 653a 220a 2020 2020 2020  in time:".      
+0001d740: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+0001d750: 2020 2020 2020 2020 2020 2020 6667 2e61              fg.a
+0001d760: 735f 6f66 284e 6f6e 652c 2065 7863 6c75  s_of(None, exclu
+0001d770: 6465 5f75 6e74 696c 3d22 3230 3230 2d31  de_until="2020-1
+0001d780: 302d 3230 2030 373a 3331 3a33 3822 292e  0-20 07:31:38").
+0001d790: 7265 6164 2829 2e73 686f 7728 290a 2020  read().show().  
+0001d7a0: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+0001d7b0: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+0001d7c0: 2074 6865 2069 6e74 6572 7661 6c20 7769   the interval wi
+0001d7d0: 6c6c 2062 6520 6170 706c 6965 6420 746f  ll be applied to
+0001d7e0: 2061 6c6c 206a 6f69 6e73 2069 6e20 7468   all joins in th
+0001d7f0: 6520 7175 6572 792e 0a20 2020 2020 2020  e query..       
+0001d800: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+0001d810: 7175 6572 7920 6469 6666 6572 656e 7420  query different 
+0001d820: 696e 7465 7276 616c 7320 666f 7220 6469  intervals for di
+0001d830: 6666 6572 656e 7420 6665 6174 7572 6520  fferent feature 
+0001d840: 6772 6f75 7073 2069 6e0a 2020 2020 2020  groups in.      
+0001d850: 2020 7468 6520 7175 6572 792c 2079 6f75    the query, you
+0001d860: 2068 6176 6520 746f 2061 7070 6c79 2074   have to apply t
+0001d870: 6865 6d20 696e 2061 206e 6573 7465 6420  hem in a nested 
+0001d880: 6661 7368 696f 6e3a 0a20 2020 2020 2020  fashion:.       
+0001d890: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+0001d8a0: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+0001d8b0: 6f6e 0a20 2020 2020 2020 2020 2020 2023  on.            #
+0001d8c0: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
+0001d8d0: 4665 6174 7572 6520 5374 6f72 650a 2020  Feature Store.  
+0001d8e0: 2020 2020 2020 2020 2020 6673 203d 202e            fs = .
+0001d8f0: 2e2e 0a0a 2020 2020 2020 2020 2020 2020  ....            
+0001d900: 2320 6765 7420 7468 6520 4665 6174 7572  # get the Featur
+0001d910: 6520 4772 6f75 7020 696e 7374 616e 6365  e Group instance
+0001d920: 0a20 2020 2020 2020 2020 2020 2066 6731  .            fg1
+0001d930: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
+0001d940: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+0001d950: 7028 2e2e 2e29 0a20 2020 2020 2020 2020  p(...).         
+0001d960: 2020 2066 6732 203d 2066 732e 6765 745f     fg2 = fs.get_
+0001d970: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+0001d980: 655f 6772 6f75 7028 2e2e 2e29 0a0a 2020  e_group(...)..  
+0001d990: 2020 2020 2020 2020 2020 6667 312e 7365            fg1.se
+0001d9a0: 6c65 6374 5f61 6c6c 2829 2e61 735f 6f66  lect_all().as_of
+0001d9b0: 2822 3230 3230 2d31 302d 3230 222c 2065  ("2020-10-20", e
+0001d9c0: 7863 6c75 6465 5f75 6e74 696c 3d22 3230  xclude_until="20
+0001d9d0: 3230 2d31 302d 3139 2229 0a20 2020 2020  20-10-19").     
+0001d9e0: 2020 2020 2020 2020 2020 202e 6a6f 696e             .join
+0001d9f0: 2866 6732 2e73 656c 6563 745f 616c 6c28  (fg2.select_all(
+0001da00: 292e 6173 5f6f 6628 2232 3032 302d 3130  ).as_of("2020-10
+0001da10: 2d32 3022 2c20 6578 636c 7564 655f 756e  -20", exclude_un
+0001da20: 7469 6c3d 2232 3032 302d 3130 2d31 3922  til="2020-10-19"
+0001da30: 2929 0a20 2020 2020 2020 2020 2020 2060  )).            `
+0001da40: 6060 0a0a 2020 2020 2020 2020 4966 2069  ``..        If i
+0001da50: 6e73 7465 6164 2079 6f75 2061 7070 6c79  nstead you apply
+0001da60: 2061 6e6f 7468 6572 2060 6173 5f6f 6660   another `as_of`
+0001da70: 2073 656c 6563 7469 6f6e 2061 6674 6572   selection after
+0001da80: 2074 6865 206a 6f69 6e2c 2061 6c6c 0a20   the join, all. 
+0001da90: 2020 2020 2020 206a 6f69 6e65 6420 6665         joined fe
+0001daa0: 6174 7572 6520 6772 6f75 7073 2077 696c  ature groups wil
+0001dab0: 6c20 6265 2071 7565 7269 6564 2077 6974  l be queried wit
+0001dac0: 6820 7468 6973 2069 6e74 6572 7661 6c3a  h this interval:
+0001dad0: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+0001dae0: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
+0001daf0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+0001db00: 2020 2020 2020 2066 6731 2e73 656c 6563         fg1.selec
+0001db10: 745f 616c 6c28 292e 6173 5f6f 6628 2232  t_all().as_of("2
+0001db20: 3032 302d 3130 2d32 3022 2c20 6578 636c  020-10-20", excl
+0001db30: 7564 655f 756e 7469 6c3d 2232 3032 302d  ude_until="2020-
+0001db40: 3130 2d31 3922 2920 2023 2061 735f 6f66  10-19")  # as_of
+0001db50: 2069 7320 6e6f 7420 6170 706c 6965 640a   is not applied.
+0001db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db70: 2e6a 6f69 6e28 6667 322e 7365 6c65 6374  .join(fg2.select
+0001db80: 5f61 6c6c 2829 2e61 735f 6f66 2822 3230  _all().as_of("20
+0001db90: 3230 2d31 302d 3230 222c 2065 7863 6c75  20-10-20", exclu
+0001dba0: 6465 5f75 6e74 696c 3d22 3230 3230 2d31  de_until="2020-1
+0001dbb0: 302d 3135 2229 2920 2023 2061 735f 6f66  0-15"))  # as_of
+0001dbc0: 2069 7320 6e6f 7420 6170 706c 6965 640a   is not applied.
+0001dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbe0: 2e61 735f 6f66 2822 3230 3230 2d31 302d  .as_of("2020-10-
+0001dbf0: 3230 222c 2065 7863 6c75 6465 5f75 6e74  20", exclude_unt
+0001dc00: 696c 3d22 3230 3230 2d31 302d 3139 2229  il="2020-10-19")
+0001dc10: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+0001dc20: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
+0001dc30: 726e 696e 670a 2020 2020 2020 2020 2020  rning.          
+0001dc40: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
+0001dc50: 6f6e 6c79 2077 6f72 6b73 2066 6f72 2066  only works for f
+0001dc60: 6561 7475 7265 2067 726f 7570 7320 7769  eature groups wi
+0001dc70: 7468 2074 696d 655f 7472 6176 656c 5f66  th time_travel_f
+0001dc80: 6f72 6d61 743d 2748 5544 4927 2e0a 0a20  ormat='HUDI'... 
+0001dc90: 2020 2020 2020 2021 2121 2077 6172 6e69         !!! warni
+0001dca0: 6e67 0a20 2020 2020 2020 2020 2020 2045  ng.            E
+0001dcb0: 7863 6c75 6469 6e67 2063 6f6d 6d69 7473  xcluding commits
+0001dcc0: 2076 6961 2065 7863 6c75 6465 5f75 6e74   via exclude_unt
+0001dcd0: 696c 2069 7320 6f6e 6c79 2070 6f73 7369  il is only possi
+0001dce0: 626c 6520 7769 7468 696e 2074 6865 2072  ble within the r
+0001dcf0: 616e 6765 206f 6620 7468 6520 4875 6469  ange of the Hudi
+0001dd00: 2061 6374 6976 6520 7469 6d65 6c69 6e65   active timeline
+0001dd10: 2e0a 2020 2020 2020 2020 2020 2020 4279  ..            By
+0001dd20: 2064 6566 6175 6c74 2c20 4875 6469 206b   default, Hudi k
+0001dd30: 6565 7073 2074 6865 206c 6173 7420 3230  eeps the last 20
+0001dd40: 2074 6f20 3330 2063 6f6d 6d69 7473 2069   to 30 commits i
+0001dd50: 6e20 7468 6520 6163 7469 7665 2074 696d  n the active tim
+0001dd60: 656c 696e 652e 0a20 2020 2020 2020 2020  eline..         
+0001dd70: 2020 2049 6620 796f 7520 6e65 6564 2074     If you need t
+0001dd80: 6f20 6b65 6570 2061 206c 6f6e 6765 7220  o keep a longer 
+0001dd90: 6163 7469 7665 2074 696d 656c 696e 652c  active timeline,
+0001dda0: 2079 6f75 2063 616e 206f 7665 7277 7269   you can overwri
+0001ddb0: 7465 2074 6865 206f 7074 696f 6e73 3a0a  te the options:.
+0001ddc0: 2020 2020 2020 2020 2020 2020 6068 6f6f              `hoo
+0001ddd0: 6469 652e 6b65 6570 2e6d 696e 2e63 6f6d  die.keep.min.com
+0001dde0: 6d69 7473 6020 616e 6420 6068 6f6f 6469  mits` and `hoodi
+0001ddf0: 652e 6b65 6570 2e6d 6178 2e63 6f6d 6d69  e.keep.max.commi
+0001de00: 7473 600a 2020 2020 2020 2020 2020 2020  ts`.            
+0001de10: 7768 656e 2063 616c 6c69 6e67 2074 6865  when calling the
+0001de20: 2060 696e 7365 7274 2829 6020 6d65 7468   `insert()` meth
+0001de30: 6f64 2e0a 0a20 2020 2020 2020 2023 2041  od...        # A
+0001de40: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+0001de50: 2020 2020 2077 616c 6c63 6c6f 636b 5f74       wallclock_t
+0001de60: 696d 653a 2052 6561 6420 6461 7461 2061  ime: Read data a
+0001de70: 7320 6f66 2074 6869 7320 706f 696e 7420  s of this point 
+0001de80: 696e 2074 696d 652e 2053 7472 696e 6773  in time. Strings
+0001de90: 2073 686f 756c 6420 6265 2066 6f72 6d61   should be forma
+0001dea0: 7474 6564 2069 6e20 6f6e 6520 6f66 2074  tted in one of t
+0001deb0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+0001dec0: 2020 2066 6f6c 6c6f 7769 6e67 2066 6f72     following for
+0001ded0: 6d61 7473 2060 2559 2d25 6d2d 2564 602c  mats `%Y-%m-%d`,
+0001dee0: 2060 2559 2d25 6d2d 2564 2025 4860 2c20   `%Y-%m-%d %H`, 
+0001def0: 6025 592d 256d 2d25 6420 2548 3a25 4d60  `%Y-%m-%d %H:%M`
+0001df00: 2c20 6f72 2060 2559 2d25 6d2d 2564 2025  , or `%Y-%m-%d %
+0001df10: 483a 254d 3a25 5360 2e0a 2020 2020 2020  H:%M:%S`..      
+0001df20: 2020 2020 2020 6578 636c 7564 655f 756e        exclude_un
+0001df30: 7469 6c3a 2045 7863 6c75 6465 2063 6f6d  til: Exclude com
+0001df40: 6d69 7473 2075 6e74 696c 2074 6869 7320  mits until this 
+0001df50: 706f 696e 7420 696e 2074 696d 652e 2053  point in time. S
+0001df60: 7472 696e 6720 7368 6f75 6c64 2062 6520  tring should be 
+0001df70: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
+0001df80: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+0001df90: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
+0001dfa0: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
+0001dfb0: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
+0001dfc0: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
+0001dfd0: 483a 254d 602c 206f 7220 6025 592d 256d  H:%M`, or `%Y-%m
+0001dfe0: 2d25 6420 2548 3a25 4d3a 2553 602e 0a0a  -%d %H:%M:%S`...
+0001dff0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+0001e000: 730a 2020 2020 2020 2020 2020 2020 6051  s.            `Q
+0001e010: 7565 7279 602e 2054 6865 2071 7565 7279  uery`. The query
+0001e020: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+0001e030: 2061 7070 6c69 6564 2074 696d 6520 7472   applied time tr
+0001e040: 6176 656c 2063 6f6e 6469 7469 6f6e 2e0a  avel condition..
+0001e050: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001e060: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0001e070: 7365 6c65 6374 5f61 6c6c 2829 2e61 735f  select_all().as_
+0001e080: 6f66 280a 2020 2020 2020 2020 2020 2020  of(.            
+0001e090: 7761 6c6c 636c 6f63 6b5f 7469 6d65 3d77  wallclock_time=w
+0001e0a0: 616c 6c63 6c6f 636b 5f74 696d 652c 2065  allclock_time, e
+0001e0b0: 7863 6c75 6465 5f75 6e74 696c 3d65 7863  xclude_until=exc
+0001e0c0: 6c75 6465 5f75 6e74 696c 0a20 2020 2020  lude_until.     
+0001e0d0: 2020 2029 0a0a 2020 2020 6465 6620 6765     )..    def ge
+0001e0e0: 745f 7374 6174 6973 7469 6373 5f62 795f  t_statistics_by_
+0001e0f0: 636f 6d6d 6974 5f77 696e 646f 7728 0a20  commit_window(. 
+0001e100: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0001e110: 2020 2020 2066 726f 6d5f 636f 6d6d 6974       from_commit
+0001e120: 5f74 696d 653a 204f 7074 696f 6e61 6c5b  _time: Optional[
+0001e130: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
+0001e140: 6461 7465 7469 6d65 2c20 6461 7465 5d5d  datetime, date]]
+0001e150: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001e160: 2074 6f5f 636f 6d6d 6974 5f74 696d 653a   to_commit_time:
+0001e170: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+0001e180: 7374 722c 2069 6e74 2c20 6461 7465 7469  str, int, dateti
+0001e190: 6d65 2c20 6461 7465 5d5d 203d 204e 6f6e  me, date]] = Non
+0001e1a0: 652c 0a20 2020 2020 2020 2066 6561 7475  e,.        featu
+0001e1b0: 7265 5f6e 616d 6573 3a20 4f70 7469 6f6e  re_names: Option
+0001e1c0: 616c 5b4c 6973 745b 7374 725d 5d20 3d20  al[List[str]] = 
+0001e1d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0001e1e0: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
+0001e1f0: 7468 6520 7374 6174 6973 7469 6373 2063  the statistics c
+0001e200: 6f6d 7075 7465 6420 6f6e 2061 2073 7065  omputed on a spe
+0001e210: 6369 6669 6320 636f 6d6d 6974 2077 696e  cific commit win
+0001e220: 646f 7720 666f 7220 7468 6973 2066 6561  dow for this fea
+0001e230: 7475 7265 2067 726f 7570 2e20 4966 2074  ture group. If t
+0001e240: 696d 6520 7472 6176 656c 2069 7320 6e6f  ime travel is no
+0001e250: 7420 656e 6162 6c65 642c 2069 7420 7261  t enabled, it ra
+0001e260: 6973 6573 2061 6e20 6578 6365 7074 696f  ises an exceptio
+0001e270: 6e2e 0a0a 2020 2020 2020 2020 4966 2060  n...        If `
+0001e280: 6672 6f6d 5f63 6f6d 6d69 745f 7469 6d65  from_commit_time
+0001e290: 6020 6973 2060 4e6f 6e65 602c 2074 6865  ` is `None`, the
+0001e2a0: 2063 6f6d 6d69 7420 7769 6e64 6f77 2073   commit window s
+0001e2b0: 7461 7274 7320 6672 6f6d 2074 6865 2066  tarts from the f
+0001e2c0: 6972 7374 2063 6f6d 6d69 742e 0a20 2020  irst commit..   
+0001e2d0: 2020 2020 2049 6620 6074 6f5f 636f 6d6d       If `to_comm
+0001e2e0: 6974 5f74 696d 6560 2069 7320 604e 6f6e  it_time` is `Non
+0001e2f0: 6560 2c20 7468 6520 636f 6d6d 6974 2077  e`, the commit w
+0001e300: 696e 646f 7720 656e 6473 2061 7420 7468  indow ends at th
+0001e310: 6520 6c61 7374 2063 6f6d 6d69 742e 0a0a  e last commit...
+0001e320: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
+0001e330: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+0001e340: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+0001e350: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
+0001e360: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
+0001e370: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
+0001e380: 2066 7320 3d20 2e2e 2e0a 2020 2020 2020   fs = ....      
+0001e390: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
+0001e3a0: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
+0001e3b0: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
+0001e3c0: 2020 2066 6720 3d20 6673 2e67 6574 5f6f     fg = fs.get_o
+0001e3d0: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
+0001e3e0: 5f67 726f 7570 282e 2e2e 290a 2020 2020  _group(...).    
+0001e3f0: 2020 2020 2020 2020 6667 5f73 7461 7469          fg_stati
+0001e400: 7374 6963 7320 3d20 6667 2e67 6574 5f73  stics = fg.get_s
+0001e410: 7461 7469 7374 6963 735f 6279 5f63 6f6d  tatistics_by_com
+0001e420: 6d69 745f 7769 6e64 6f77 2866 726f 6d5f  mit_window(from_
+0001e430: 636f 6d6d 6974 5f74 696d 653d 4e6f 6e65  commit_time=None
+0001e440: 2c20 746f 5f63 6f6d 6d69 745f 7469 6d65  , to_commit_time
+0001e450: 3d4e 6f6e 6529 0a20 2020 2020 2020 2020  =None).         
+0001e460: 2020 2060 6060 0a20 2020 2020 2020 2023     ```.        #
+0001e470: 2041 7267 756d 656e 7473 0a20 2020 2020   Arguments.     
+0001e480: 2020 2020 2020 2074 6f5f 636f 6d6d 6974         to_commit
+0001e490: 5f74 696d 653a 2044 6174 6520 616e 6420  _time: Date and 
+0001e4a0: 7469 6d65 206f 6620 7468 6520 6c61 7374  time of the last
+0001e4b0: 2063 6f6d 6d69 7420 6f66 2074 6865 2077   commit of the w
+0001e4c0: 696e 646f 772e 2044 6566 6175 6c74 7320  indow. Defaults 
+0001e4d0: 746f 2060 4e6f 6e65 602e 2053 7472 696e  to `None`. Strin
+0001e4e0: 6773 2073 686f 756c 640a 2020 2020 2020  gs should.      
+0001e4f0: 2020 2020 2020 2020 2020 6265 2066 6f72            be for
+0001e500: 6d61 7474 6564 2069 6e20 6f6e 6520 6f66  matted in one of
+0001e510: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
+0001e520: 6f72 6d61 7473 2060 2559 2d25 6d2d 2564  ormats `%Y-%m-%d
+0001e530: 602c 2060 2559 2d25 6d2d 2564 2025 4860  `, `%Y-%m-%d %H`
+0001e540: 2c20 6025 592d 256d 2d25 6420 2548 3a25  , `%Y-%m-%d %H:%
+0001e550: 4d60 2c20 6025 592d 256d 2d25 6420 2548  M`, `%Y-%m-%d %H
+0001e560: 3a25 4d3a 2553 602c 0a20 2020 2020 2020  :%M:%S`,.       
+0001e570: 2020 2020 2020 2020 206f 7220 6025 592d           or `%Y-
+0001e580: 256d 2d25 6420 2548 3a25 4d3a 2553 2e25  %m-%d %H:%M:%S.%
+0001e590: 6660 2e0a 2020 2020 2020 2020 2020 2020  f`..            
+0001e5a0: 6672 6f6d 5f63 6f6d 6d69 745f 7469 6d65  from_commit_time
+0001e5b0: 3a20 4461 7465 2061 6e64 2074 696d 6520  : Date and time 
+0001e5c0: 6f66 2074 6865 2066 6972 7374 2063 6f6d  of the first com
+0001e5d0: 6d69 7420 6f66 2074 6865 2077 696e 646f  mit of the windo
+0001e5e0: 772e 2044 6566 6175 6c74 7320 746f 2060  w. Defaults to `
+0001e5f0: 4e6f 6e65 602e 2053 7472 696e 6773 2073  None`. Strings s
+0001e600: 686f 756c 640a 2020 2020 2020 2020 2020  hould.          
+0001e610: 2020 2020 2020 6265 2066 6f72 6d61 7474        be formatt
+0001e620: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
+0001e630: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
+0001e640: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
+0001e650: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
+0001e660: 592d 256d 2d25 6420 2548 3a25 4d60 2c20  Y-%m-%d %H:%M`, 
+0001e670: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
+0001e680: 2553 602c 0a20 2020 2020 2020 2020 2020  %S`,.           
+0001e690: 2020 2020 206f 7220 6025 592d 256d 2d25       or `%Y-%m-%
+0001e6a0: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
+0001e6b0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+0001e6c0: 7572 655f 6e61 6d65 733a 204c 6973 7420  ure_names: List 
+0001e6d0: 6f66 2066 6561 7475 7265 206e 616d 6573  of feature names
+0001e6e0: 206f 6620 7768 6963 6820 7374 6174 6973   of which statis
+0001e6f0: 7469 6373 2061 7265 2072 6574 7269 6576  tics are retriev
+0001e700: 6564 2e0a 2020 2020 2020 2020 2320 5265  ed..        # Re
+0001e710: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
+0001e720: 2020 6053 7461 7469 7374 6963 7360 2e20    `Statistics`. 
+0001e730: 5374 6174 6973 7469 6373 206f 626a 6563  Statistics objec
+0001e740: 742e 0a20 2020 2020 2020 2023 2052 6169  t..        # Rai
+0001e750: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
+0001e760: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
+0001e770: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
+0001e780: 7272 6f72 602e 0a20 2020 2020 2020 2022  rror`..        "
+0001e790: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+0001e7a0: 7420 7365 6c66 2e5f 6973 5f74 696d 655f  t self._is_time_
+0001e7b0: 7472 6176 656c 5f65 6e61 626c 6564 2829  travel_enabled()
+0001e7c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001e7d0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0001e7e0: 5469 6d65 2074 7261 7665 6c20 6973 206e  Time travel is n
+0001e7f0: 6f74 2065 6e61 626c 6564 2066 6f72 2074  ot enabled for t
+0001e800: 6869 7320 6665 6174 7572 6520 6772 6f75  his feature grou
+0001e810: 7022 290a 2020 2020 2020 2020 7265 7475  p").        retu
+0001e820: 726e 2073 656c 662e 5f73 7461 7469 7374  rn self._statist
+0001e830: 6963 735f 656e 6769 6e65 2e67 6574 5f62  ics_engine.get_b
+0001e840: 795f 7469 6d65 5f77 696e 646f 7728 0a20  y_time_window(. 
+0001e850: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+0001e860: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+0001e870: 7274 5f63 6f6d 6d69 745f 7469 6d65 3d66  rt_commit_time=f
+0001e880: 726f 6d5f 636f 6d6d 6974 5f74 696d 652c  rom_commit_time,
+0001e890: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+0001e8a0: 5f63 6f6d 6d69 745f 7469 6d65 3d74 6f5f  _commit_time=to_
+0001e8b0: 636f 6d6d 6974 5f74 696d 652c 0a20 2020  commit_time,.   
+0001e8c0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+0001e8d0: 5f6e 616d 6573 3d66 6561 7475 7265 5f6e  _names=feature_n
+0001e8e0: 616d 6573 2c0a 2020 2020 2020 2020 290a  ames,.        ).
+0001e8f0: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+0001e900: 5f73 7461 7469 7374 6963 7328 0a20 2020  _statistics(.   
+0001e910: 2020 2020 2073 656c 662c 2077 616c 6c63       self, wallc
+0001e920: 6c6f 636b 5f74 696d 653a 204f 7074 696f  lock_time: Optio
+0001e930: 6e61 6c5b 556e 696f 6e5b 7374 722c 2069  nal[Union[str, i
+0001e940: 6e74 2c20 6461 7465 7469 6d65 2c20 6461  nt, datetime, da
+0001e950: 7465 5d5d 203d 204e 6f6e 650a 2020 2020  te]] = None.    
+0001e960: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+0001e970: 636f 6d70 7574 6520 7468 6520 7374 6174  compute the stat
+0001e980: 6973 7469 6373 2066 6f72 2074 6865 2066  istics for the f
+0001e990: 6561 7475 7265 2067 726f 7570 2061 6e64  eature group and
+0001e9a0: 2073 6176 6520 7468 656d 2074 6f20 7468   save them to th
+0001e9b0: 650a 2020 2020 2020 2020 6665 6174 7572  e.        featur
+0001e9c0: 6520 7374 6f72 652e 0a0a 2020 2020 2020  e store...      
+0001e9d0: 2020 5374 6174 6973 7469 6373 2061 7265    Statistics are
+0001e9e0: 206f 6e6c 7920 636f 6d70 7574 6564 2066   only computed f
+0001e9f0: 6f72 2064 6174 6120 696e 2074 6865 206f  or data in the o
+0001ea00: 6666 6c69 6e65 2073 746f 7261 6765 206f  ffline storage o
+0001ea10: 6620 7468 6520 6665 6174 7572 650a 2020  f the feature.  
+0001ea20: 2020 2020 2020 6772 6f75 702e 0a0a 2020        group...  
+0001ea30: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
+0001ea40: 730a 2020 2020 2020 2020 2020 2020 7761  s.            wa
+0001ea50: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4966  llclock_time: If
+0001ea60: 2073 7065 6369 6669 6564 2077 696c 6c20   specified will 
+0001ea70: 7265 636f 6d70 7574 6520 7374 6174 6973  recompute statis
+0001ea80: 7469 6373 206f 6e0a 2020 2020 2020 2020  tics on.        
+0001ea90: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
+0001eaa0: 6772 6f75 7020 6173 206f 6620 7370 6563  group as of spec
+0001eab0: 6966 6963 2070 6f69 6e74 2069 6e20 7469  ific point in ti
+0001eac0: 6d65 2e20 4966 206e 6f74 2073 7065 6369  me. If not speci
+0001ead0: 6669 6564 2074 6865 6e20 7769 6c6c 2063  fied then will c
+0001eae0: 6f6d 7075 7465 2073 7461 7469 7374 6963  ompute statistic
+0001eaf0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001eb00: 2020 6173 206f 6620 6d6f 7374 2072 6563    as of most rec
+0001eb10: 656e 7420 7469 6d65 206f 6620 7468 6973  ent time of this
+0001eb20: 2066 6561 7475 7265 2067 726f 7570 2e20   feature group. 
+0001eb30: 4465 6661 756c 7473 2074 6f20 604e 6f6e  Defaults to `Non
+0001eb40: 6560 2e20 5374 7269 6e67 7320 7368 6f75  e`. Strings shou
+0001eb50: 6c64 0a20 2020 2020 2020 2020 2020 2020  ld.             
+0001eb60: 2020 2062 6520 666f 726d 6174 7465 6420     be formatted 
+0001eb70: 696e 206f 6e65 206f 6620 7468 6520 666f  in one of the fo
+0001eb80: 6c6c 6f77 696e 6720 666f 726d 6174 7320  llowing formats 
+0001eb90: 6025 592d 256d 2d25 6460 2c20 6025 592d  `%Y-%m-%d`, `%Y-
+0001eba0: 256d 2d25 6420 2548 602c 2060 2559 2d25  %m-%d %H`, `%Y-%
+0001ebb0: 6d2d 2564 2025 483a 254d 602c 2060 2559  m-%d %H:%M`, `%Y
+0001ebc0: 2d25 6d2d 2564 2025 483a 254d 3a25 5360  -%m-%d %H:%M:%S`
+0001ebd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ebe0: 2020 6f72 2060 2559 2d25 6d2d 2564 2025    or `%Y-%m-%d %
+0001ebf0: 483a 254d 3a25 532e 2566 602e 0a0a 2020  H:%M:%S.%f`...  
+0001ec00: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+0001ec10: 2020 2020 2020 2020 2020 2020 6053 7461              `Sta
+0001ec20: 7469 7374 6963 7360 2e20 5468 6520 7374  tistics`. The st
+0001ec30: 6174 6973 7469 6373 206d 6574 6164 6174  atistics metadat
+0001ec40: 6120 6f62 6a65 6374 2e0a 0a20 2020 2020  a object...     
+0001ec50: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
+0001ec60: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
+0001ec70: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
+0001ec80: 5265 7374 4150 4945 7272 6f72 602e 2055  RestAPIError`. U
+0001ec90: 6e61 626c 6520 746f 2070 6572 7369 7374  nable to persist
+0001eca0: 2074 6865 2073 7461 7469 7374 6963 732e   the statistics.
+0001ecb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001ecc0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+0001ecd0: 7469 7374 6963 735f 636f 6e66 6967 2e65  tistics_config.e
+0001ece0: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
+0001ecf0: 2020 2020 6966 2073 656c 662e 5f69 735f      if self._is_
+0001ed00: 7469 6d65 5f74 7261 7665 6c5f 656e 6162  time_travel_enab
+0001ed10: 6c65 6428 2920 6f72 2077 616c 6c63 6c6f  led() or wallclo
+0001ed20: 636b 5f74 696d 6520 6973 206e 6f74 204e  ck_time is not N
+0001ed30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001ed40: 2020 2020 2077 616c 6c63 6c6f 636b 5f74       wallclock_t
+0001ed50: 696d 6520 3d20 7761 6c6c 636c 6f63 6b5f  ime = wallclock_
+0001ed60: 7469 6d65 206f 7220 6461 7465 7469 6d65  time or datetime
+0001ed70: 2e6e 6f77 2829 0a20 2020 2020 2020 2020  .now().         
+0001ed80: 2020 2020 2020 2023 2052 6574 7269 6576         # Retriev
+0001ed90: 6520 6667 2063 6f6d 6d69 7420 6964 2072  e fg commit id r
+0001eda0: 656c 6174 6564 2074 6f20 7468 6973 2077  elated to this w
+0001edb0: 616c 6c20 636c 6f63 6b20 7469 6d65 2061  all clock time a
+0001edc0: 6e64 2072 6563 6f6d 7075 7465 2073 7461  nd recompute sta
+0001edd0: 7469 7374 6963 732e 2049 7420 7769 6c6c  tistics. It will
+0001ede0: 2074 6872 6f77 0a20 2020 2020 2020 2020   throw.         
+0001edf0: 2020 2020 2020 2023 2065 7863 6570 7469         # excepti
+0001ee00: 6f6e 2069 6620 6974 7320 6e6f 7420 7469  on if its not ti
+0001ee10: 6d65 2074 7261 7665 6c20 656e 6162 6c65  me travel enable
+0001ee20: 6420 6665 6174 7572 6520 6772 6f75 702e  d feature group.
+0001ee30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ee40: 2066 675f 636f 6d6d 6974 5f69 6420 3d20   fg_commit_id = 
+0001ee50: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+0001ee60: 2020 2020 2020 636f 6d6d 6974 5f69 640a        commit_id.
+0001ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ee80: 2020 2020 666f 7220 636f 6d6d 6974 5f69      for commit_i
+0001ee90: 6420 696e 2073 656c 662e 5f66 6561 7475  d in self._featu
+0001eea0: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
+0001eeb0: 636f 6d6d 6974 5f64 6574 6169 6c73 280a  commit_details(.
+0001eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eed0: 2020 2020 2020 2020 7365 6c66 2c20 7761          self, wa
+0001eee0: 6c6c 636c 6f63 6b5f 7469 6d65 2c20 310a  llclock_time, 1.
+0001eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef00: 2020 2020 292e 6b65 7973 2829 0a20 2020      ).keys().   
+0001ef10: 2020 2020 2020 2020 2020 2020 205d 5b30               ][0
+0001ef20: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001ef30: 2020 7265 6769 7374 6572 6564 5f73 7461    registered_sta
+0001ef40: 7473 203d 2073 656c 662e 6765 745f 7374  ts = self.get_st
+0001ef50: 6174 6973 7469 6373 5f62 795f 636f 6d6d  atistics_by_comm
+0001ef60: 6974 5f77 696e 646f 7728 0a20 2020 2020  it_window(.     
+0001ef70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001ef80: 6f5f 636f 6d6d 6974 5f74 696d 653d 6667  o_commit_time=fg
+0001ef90: 5f63 6f6d 6d69 745f 6964 0a20 2020 2020  _commit_id.     
+0001efa0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001efb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001efc0: 7265 6769 7374 6572 6564 5f73 7461 7473  registered_stats
+0001efd0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0001efe0: 2073 656c 662e 5f61 7265 5f73 7461 7469   self._are_stati
+0001eff0: 7374 6963 735f 6d69 7373 696e 6728 0a20  stics_missing(. 
+0001f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f010: 2020 2072 6567 6973 7465 7265 645f 7374     registered_st
+0001f020: 6174 730a 2020 2020 2020 2020 2020 2020  ats.            
+0001f030: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0001f040: 2020 2020 2020 2020 2020 2072 6567 6973             regis
+0001f050: 7465 7265 645f 7374 6174 7320 3d20 4e6f  tered_stats = No
+0001f060: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0001f070: 2020 2023 2044 6f6e 2774 2072 6561 6420     # Don't read 
+0001f080: 7468 6520 6461 7461 6672 616d 6520 6865  the dataframe he
+0001f090: 7265 2c20 746f 2061 766f 6964 2074 7269  re, to avoid tri
+0001f0a0: 6767 6572 696e 6720 6120 7265 6164 206f  ggering a read o
+0001f0b0: 7065 7261 7469 6f6e 0a20 2020 2020 2020  peration.       
+0001f0c0: 2020 2020 2020 2020 2023 2066 6f72 2074           # for t
+0001f0d0: 6865 2050 7974 686f 6e20 656e 6769 6e65  he Python engine
+0001f0e0: 2e20 5468 6520 5079 7468 6f6e 2065 6e67  . The Python eng
+0001f0f0: 696e 6520 6973 2067 6f69 6e67 2074 6f20  ine is going to 
+0001f100: 7365 7475 7020 6120 5370 6172 6b20 4a6f  setup a Spark Jo
+0001f110: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
+0001f120: 2020 2320 746f 2075 7064 6174 6520 7468    # to update th
+0001f130: 6520 7374 6174 6973 7469 6373 2e0a 2020  e statistics..  
+0001f140: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001f150: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
+0001f160: 2020 2020 2020 2020 2020 2072 6567 6973             regis
+0001f170: 7465 7265 645f 7374 6174 730a 2020 2020  tered_stats.    
+0001f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f190: 6f72 2073 656c 662e 5f73 7461 7469 7374  or self._statist
+0001f1a0: 6963 735f 656e 6769 6e65 2e63 6f6d 7075  ics_engine.compu
+0001f1b0: 7465 5f61 6e64 5f73 6176 655f 7374 6174  te_and_save_stat
+0001f1c0: 6973 7469 6373 280a 2020 2020 2020 2020  istics(.        
+0001f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f1e0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+0001f1f0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+0001f200: 6174 7572 655f 6772 6f75 705f 636f 6d6d  ature_group_comm
+0001f210: 6974 5f69 643d 6667 5f63 6f6d 6d69 745f  it_id=fg_commit_
+0001f220: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0001f230: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001f240: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001f250: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+0001f260: 2829 2e63 6f6d 7075 7465 5f73 7461 7469  ().compute_stati
+0001f270: 7374 6963 7328 290a 0a20 2020 2040 636c  stics()..    @cl
+0001f280: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+0001f290: 6620 6672 6f6d 5f72 6573 706f 6e73 655f  f from_response_
+0001f2a0: 6a73 6f6e 2863 6c73 2c20 6a73 6f6e 5f64  json(cls, json_d
+0001f2b0: 6963 7429 3a0a 2020 2020 2020 2020 6a73  ict):.        js
+0001f2c0: 6f6e 5f64 6563 616d 656c 697a 6564 203d  on_decamelized =
+0001f2d0: 2068 756d 7073 2e64 6563 616d 656c 697a   humps.decameliz
+0001f2e0: 6528 6a73 6f6e 5f64 6963 7429 0a20 2020  e(json_dict).   
+0001f2f0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0001f300: 6365 286a 736f 6e5f 6465 6361 6d65 6c69  ce(json_decameli
+0001f310: 7a65 642c 2064 6963 7429 3a0a 2020 2020  zed, dict):.    
+0001f320: 2020 2020 2020 2020 6966 2022 7479 7065          if "type
+0001f330: 2220 696e 206a 736f 6e5f 6465 6361 6d65  " in json_decame
+0001f340: 6c69 7a65 643a 0a20 2020 2020 2020 2020  lized:.         
+0001f350: 2020 2020 2020 206a 736f 6e5f 6465 6361         json_deca
+0001f360: 6d65 6c69 7a65 645b 2273 7472 6561 6d22  melized["stream"
+0001f370: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+0001f380: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
+0001f390: 6563 616d 656c 697a 6564 5b22 7479 7065  ecamelized["type
+0001f3a0: 225d 203d 3d20 2273 7472 6561 6d46 6561  "] == "streamFea
+0001f3b0: 7475 7265 4772 6f75 7044 544f 220a 2020  tureGroupDTO".  
+0001f3c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0001f3d0: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
+0001f3e0: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+0001f3f0: 2e70 6f70 2822 7479 7065 222c 204e 6f6e  .pop("type", Non
+0001f400: 6529 0a20 2020 2020 2020 2020 2020 206a  e).            j
+0001f410: 736f 6e5f 6465 6361 6d65 6c69 7a65 642e  son_decamelized.
+0001f420: 706f 7028 2276 616c 6964 6174 696f 6e5f  pop("validation_
+0001f430: 7479 7065 222c 204e 6f6e 6529 0a20 2020  type", None).   
+0001f440: 2020 2020 2020 2020 2069 6620 2265 6d62           if "emb
+0001f450: 6564 6469 6e67 5f69 6e64 6578 2220 696e  edding_index" in
+0001f460: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+0001f470: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+0001f480: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
+0001f490: 7a65 645b 2265 6d62 6564 6469 6e67 5f69  zed["embedding_i
+0001f4a0: 6e64 6578 225d 203d 2045 6d62 6564 6469  ndex"] = Embeddi
+0001f4b0: 6e67 496e 6465 782e 6672 6f6d 5f6a 736f  ngIndex.from_jso
+0001f4c0: 6e5f 7265 7370 6f6e 7365 280a 2020 2020  n_response(.    
+0001f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f4e0: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+0001f4f0: 5b22 656d 6265 6464 696e 675f 696e 6465  ["embedding_inde
+0001f500: 7822 5d0a 2020 2020 2020 2020 2020 2020  x"].            
+0001f510: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001f520: 2020 7265 7475 726e 2063 6c73 282a 2a6a    return cls(**j
+0001f530: 736f 6e5f 6465 6361 6d65 6c69 7a65 6429  son_decamelized)
+0001f540: 0a20 2020 2020 2020 2066 6f72 2066 6720  .        for fg 
+0001f550: 696e 206a 736f 6e5f 6465 6361 6d65 6c69  in json_decameli
+0001f560: 7a65 643a 0a20 2020 2020 2020 2020 2020  zed:.           
+0001f570: 2069 6620 2274 7970 6522 2069 6e20 6667   if "type" in fg
+0001f580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f590: 2020 6667 5b22 7374 7265 616d 225d 203d    fg["stream"] =
+0001f5a0: 2066 675b 2274 7970 6522 5d20 3d3d 2022   fg["type"] == "
+0001f5b0: 7374 7265 616d 4665 6174 7572 6547 726f  streamFeatureGro
+0001f5c0: 7570 4454 4f22 0a20 2020 2020 2020 2020  upDTO".         
+0001f5d0: 2020 205f 203d 2066 672e 706f 7028 2274     _ = fg.pop("t
+0001f5e0: 7970 6522 2c20 4e6f 6e65 290a 2020 2020  ype", None).    
+0001f5f0: 2020 2020 2020 2020 6667 2e70 6f70 2822          fg.pop("
+0001f600: 7661 6c69 6461 7469 6f6e 5f74 7970 6522  validation_type"
+0001f610: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+0001f620: 2020 2020 6966 2022 656d 6265 6464 696e      if "embeddin
+0001f630: 675f 696e 6465 7822 2069 6e20 6667 3a0a  g_index" in fg:.
+0001f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f650: 6667 5b22 656d 6265 6464 696e 675f 696e  fg["embedding_in
+0001f660: 6465 7822 5d20 3d20 456d 6265 6464 696e  dex"] = Embeddin
+0001f670: 6749 6e64 6578 2e66 726f 6d5f 6a73 6f6e  gIndex.from_json
+0001f680: 5f72 6573 706f 6e73 6528 0a20 2020 2020  _response(.     
+0001f690: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001f6a0: 675b 2265 6d62 6564 6469 6e67 5f69 6e64  g["embedding_ind
+0001f6b0: 6578 225d 0a20 2020 2020 2020 2020 2020  ex"].           
+0001f6c0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0001f6d0: 6574 7572 6e20 5b63 6c73 282a 2a66 6729  eturn [cls(**fg)
+0001f6e0: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
+0001f6f0: 6465 6361 6d65 6c69 7a65 645d 0a0a 2020  decamelized]..  
+0001f700: 2020 6465 6620 7570 6461 7465 5f66 726f    def update_fro
+0001f710: 6d5f 7265 7370 6f6e 7365 5f6a 736f 6e28  m_response_json(
+0001f720: 7365 6c66 2c20 6a73 6f6e 5f64 6963 7429  self, json_dict)
+0001f730: 3a0a 2020 2020 2020 2020 6a73 6f6e 5f64  :.        json_d
+0001f740: 6563 616d 656c 697a 6564 203d 2068 756d  ecamelized = hum
+0001f750: 7073 2e64 6563 616d 656c 697a 6528 6a73  ps.decamelize(js
+0001f760: 6f6e 5f64 6963 7429 0a20 2020 2020 2020  on_dict).       
+0001f770: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+0001f780: 645b 2273 7472 6561 6d22 5d20 3d20 6a73  d["stream"] = js
+0001f790: 6f6e 5f64 6563 616d 656c 697a 6564 5b22  on_decamelized["
+0001f7a0: 7479 7065 225d 203d 3d20 2273 7472 6561  type"] == "strea
+0001f7b0: 6d46 6561 7475 7265 4772 6f75 7044 544f  mFeatureGroupDTO
+0001f7c0: 220a 2020 2020 2020 2020 5f20 3d20 6a73  ".        _ = js
+0001f7d0: 6f6e 5f64 6563 616d 656c 697a 6564 2e70  on_decamelized.p
+0001f7e0: 6f70 2822 7479 7065 2229 0a20 2020 2020  op("type").     
+0001f7f0: 2020 2069 6620 2265 6d62 6564 6469 6e67     if "embedding
+0001f800: 5f69 6e64 6578 2220 696e 206a 736f 6e5f  _index" in json_
+0001f810: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
+0001f820: 2020 2020 2020 2020 206a 736f 6e5f 6465           json_de
+0001f830: 6361 6d65 6c69 7a65 645b 2265 6d62 6564  camelized["embed
+0001f840: 6469 6e67 5f69 6e64 6578 225d 203d 2045  ding_index"] = E
+0001f850: 6d62 6564 6469 6e67 496e 6465 782e 6672  mbeddingIndex.fr
+0001f860: 6f6d 5f6a 736f 6e5f 7265 7370 6f6e 7365  om_json_response
+0001f870: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001f880: 2020 6a73 6f6e 5f64 6563 616d 656c 697a    json_decameliz
+0001f890: 6564 5b22 656d 6265 6464 696e 675f 696e  ed["embedding_in
+0001f8a0: 6465 7822 5d0a 2020 2020 2020 2020 2020  dex"].          
+0001f8b0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0001f8c0: 2e5f 5f69 6e69 745f 5f28 2a2a 6a73 6f6e  .__init__(**json
+0001f8d0: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
+0001f8e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001f8f0: 660a 0a20 2020 2064 6566 206a 736f 6e28  f..    def json(
+0001f900: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0001f910: 2222 4765 7420 7370 6563 6966 6963 2046  ""Get specific F
+0001f920: 6561 7475 7265 2047 726f 7570 206d 6574  eature Group met
+0001f930: 6164 6174 6120 696e 206a 736f 6e20 666f  adata in json fo
+0001f940: 726d 6174 2e0a 0a20 2020 2020 2020 2021  rmat...        !
+0001f950: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+0001f960: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+0001f970: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+0001f980: 6a73 6f6e 2829 0a20 2020 2020 2020 2020  json().         
+0001f990: 2020 2060 6060 0a20 2020 2020 2020 2022     ```.        "
+0001f9a0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0001f9b0: 6e20 6a73 6f6e 2e64 756d 7073 2873 656c  n json.dumps(sel
+0001f9c0: 662c 2063 6c73 3d75 7469 6c2e 4665 6174  f, cls=util.Feat
+0001f9d0: 7572 6553 746f 7265 456e 636f 6465 7229  ureStoreEncoder)
+0001f9e0: 0a0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
+0001f9f0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0001fa00: 2022 2222 4765 7420 7374 7275 6374 7572   """Get structur
+0001fa10: 6564 2069 6e66 6f20 6162 6f75 7420 7370  ed info about sp
+0001fa20: 6563 6966 6963 2046 6561 7475 7265 2047  ecific Feature G
+0001fa30: 726f 7570 2069 6e20 7079 7468 6f6e 2064  roup in python d
+0001fa40: 6963 7469 6f6e 6172 7920 666f 726d 6174  ictionary format
+0001fa50: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
+0001fa60: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
+0001fa70: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+0001fa80: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
+0001fa90: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
+0001faa0: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
+0001fab0: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
+0001fac0: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
+0001fad0: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
+0001fae0: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
+0001faf0: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
+0001fb00: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
+0001fb10: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
+0001fb20: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+0001fb30: 746f 5f64 6963 7428 290a 2020 2020 2020  to_dict().      
+0001fb40: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+0001fb50: 2020 2222 220a 2020 2020 2020 2020 6667    """.        fg
+0001fb60: 5f6d 6574 615f 6469 6374 203d 207b 0a20  _meta_dict = {. 
+0001fb70: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+0001fb80: 2073 656c 662e 5f69 642c 0a20 2020 2020   self._id,.     
+0001fb90: 2020 2020 2020 2022 6e61 6d65 223a 2073         "name": s
+0001fba0: 656c 662e 5f6e 616d 652c 0a20 2020 2020  elf._name,.     
+0001fbb0: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+0001fbc0: 3a20 7365 6c66 2e5f 7665 7273 696f 6e2c  : self._version,
+0001fbd0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+0001fbe0: 7363 7269 7074 696f 6e22 3a20 7365 6c66  scription": self
+0001fbf0: 2e5f 6465 7363 7269 7074 696f 6e2c 0a20  ._description,. 
+0001fc00: 2020 2020 2020 2020 2020 2022 6f6e 6c69             "onli
+0001fc10: 6e65 456e 6162 6c65 6422 3a20 7365 6c66  neEnabled": self
+0001fc20: 2e5f 6f6e 6c69 6e65 5f65 6e61 626c 6564  ._online_enabled
+0001fc30: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+0001fc40: 696d 6554 7261 7665 6c46 6f72 6d61 7422  imeTravelFormat"
+0001fc50: 3a20 7365 6c66 2e5f 7469 6d65 5f74 7261  : self._time_tra
+0001fc60: 7665 6c5f 666f 726d 6174 2c0a 2020 2020  vel_format,.    
+0001fc70: 2020 2020 2020 2020 2266 6561 7475 7265          "feature
+0001fc80: 7322 3a20 7365 6c66 2e5f 6665 6174 7572  s": self._featur
+0001fc90: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0001fca0: 2266 6561 7475 7265 7374 6f72 6549 6422  "featurestoreId"
+0001fcb0: 3a20 7365 6c66 2e5f 6665 6174 7572 655f  : self._feature_
+0001fcc0: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
+0001fcd0: 2020 2020 2020 2274 7970 6522 3a20 2263        "type": "c
+0001fce0: 6163 6865 6446 6561 7475 7265 6772 6f75  achedFeaturegrou
+0001fcf0: 7044 544f 220a 2020 2020 2020 2020 2020  pDTO".          
+0001fd00: 2020 6966 206e 6f74 2073 656c 662e 5f73    if not self._s
+0001fd10: 7472 6561 6d0a 2020 2020 2020 2020 2020  tream.          
+0001fd20: 2020 656c 7365 2022 7374 7265 616d 4665    else "streamFe
+0001fd30: 6174 7572 6547 726f 7570 4454 4f22 2c0a  atureGroupDTO",.
+0001fd40: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+0001fd50: 7469 7374 6963 7343 6f6e 6669 6722 3a20  tisticsConfig": 
+0001fd60: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
+0001fd70: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
+0001fd80: 2020 2020 2022 6576 656e 7454 696d 6522       "eventTime"
+0001fd90: 3a20 7365 6c66 2e65 7665 6e74 5f74 696d  : self.event_tim
+0001fda0: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+0001fdb0: 6578 7065 6374 6174 696f 6e53 7569 7465  expectationSuite
+0001fdc0: 223a 2073 656c 662e 5f65 7870 6563 7461  ": self._expecta
+0001fdd0: 7469 6f6e 5f73 7569 7465 2c0a 2020 2020  tion_suite,.    
+0001fde0: 2020 2020 2020 2020 2270 6172 656e 7473          "parents
+0001fdf0: 223a 2073 656c 662e 5f70 6172 656e 7473  ": self._parents
+0001fe00: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+0001fe10: 6f70 6963 4e61 6d65 223a 2073 656c 662e  opicName": self.
+0001fe20: 746f 7069 635f 6e61 6d65 2c0a 2020 2020  topic_name,.    
+0001fe30: 2020 2020 2020 2020 226e 6f74 6966 6963          "notific
+0001fe40: 6174 696f 6e54 6f70 6963 4e61 6d65 223a  ationTopicName":
+0001fe50: 2073 656c 662e 6e6f 7469 6669 6361 7469   self.notificati
+0001fe60: 6f6e 5f74 6f70 6963 5f6e 616d 652c 0a20  on_topic_name,. 
+0001fe70: 2020 2020 2020 2020 2020 2022 6465 7072             "depr
+0001fe80: 6563 6174 6564 223a 2073 656c 662e 6465  ecated": self.de
+0001fe90: 7072 6563 6174 6564 2c0a 2020 2020 2020  precated,.      
+0001fea0: 2020 7d0a 2020 2020 2020 2020 6966 2073    }.        if s
+0001feb0: 656c 662e 656d 6265 6464 696e 675f 696e  elf.embedding_in
+0001fec0: 6465 783a 0a20 2020 2020 2020 2020 2020  dex:.           
+0001fed0: 2066 675f 6d65 7461 5f64 6963 745b 2265   fg_meta_dict["e
+0001fee0: 6d62 6564 6469 6e67 496e 6465 7822 5d20  mbeddingIndex"] 
+0001fef0: 3d20 7365 6c66 2e65 6d62 6564 6469 6e67  = self.embedding
+0001ff00: 5f69 6e64 6578 0a20 2020 2020 2020 2069  _index.        i
+0001ff10: 6620 7365 6c66 2e5f 7374 7265 616d 3a0a  f self._stream:.
+0001ff20: 2020 2020 2020 2020 2020 2020 6667 5f6d              fg_m
+0001ff30: 6574 615f 6469 6374 5b22 6465 6c74 6153  eta_dict["deltaS
+0001ff40: 7472 6561 6d65 724a 6f62 436f 6e66 225d  treamerJobConf"]
+0001ff50: 203d 2073 656c 662e 5f64 656c 7461 7374   = self._deltast
+0001ff60: 7265 616d 6572 5f6a 6f62 636f 6e66 0a20  reamer_jobconf. 
+0001ff70: 2020 2020 2020 2072 6574 7572 6e20 6667         return fg
+0001ff80: 5f6d 6574 615f 6469 6374 0a0a 2020 2020  _meta_dict..    
+0001ff90: 6465 6620 5f67 6574 5f74 6162 6c65 5f6e  def _get_table_n
+0001ffa0: 616d 6528 7365 6c66 293a 0a20 2020 2020  ame(self):.     
+0001ffb0: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+0001ffc0: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
+0001ffd0: 6520 2b20 222e 2220 2b20 7365 6c66 2e67  e + "." + self.g
+0001ffe0: 6574 5f66 675f 6e61 6d65 2829 0a0a 2020  et_fg_name()..  
+0001fff0: 2020 6465 6620 5f69 735f 7469 6d65 5f74    def _is_time_t
+00020000: 7261 7665 6c5f 656e 6162 6c65 6428 7365  ravel_enabled(se
+00020010: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00020020: 5768 6574 6865 7220 7469 6d65 2d74 7261  Whether time-tra
+00020030: 7665 6c20 6973 2065 6e61 626c 6564 206f  vel is enabled o
+00020040: 7220 6e6f 7422 2222 0a20 2020 2020 2020  r not""".       
+00020050: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
+00020060: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
+00020070: 5f74 7261 7665 6c5f 666f 726d 6174 2069  _travel_format i
+00020080: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+00020090: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
+000200a0: 5f74 696d 655f 7472 6176 656c 5f66 6f72  _time_travel_for
+000200b0: 6d61 742e 7570 7065 7228 2920 3d3d 2022  mat.upper() == "
+000200c0: 4855 4449 220a 2020 2020 2020 2020 290a  HUDI".        ).
+000200d0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000200e0: 2020 2064 6566 2069 6428 7365 6c66 293a     def id(self):
+000200f0: 0a20 2020 2020 2020 2022 2222 4665 6174  .        """Feat
+00020100: 7572 6520 6772 6f75 7020 6964 2e22 2222  ure group id."""
+00020110: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00020120: 7365 6c66 2e5f 6964 0a0a 2020 2020 4070  self._id..    @p
+00020130: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00020140: 6465 7363 7269 7074 696f 6e28 7365 6c66  description(self
+00020150: 293a 0a20 2020 2020 2020 2022 2222 4465  ):.        """De
+00020160: 7363 7269 7074 696f 6e20 6f66 2074 6865  scription of the
+00020170: 2066 6561 7475 7265 2067 726f 7570 2063   feature group c
+00020180: 6f6e 7465 6e74 732e 2222 220a 2020 2020  ontents.""".    
+00020190: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000201a0: 5f64 6573 6372 6970 7469 6f6e 0a0a 2020  _description..  
+000201b0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000201c0: 6465 6620 7469 6d65 5f74 7261 7665 6c5f  def time_travel_
+000201d0: 666f 726d 6174 2873 656c 6629 3a0a 2020  format(self):.  
+000201e0: 2020 2020 2020 2222 2253 6574 7469 6e67        """Setting
+000201f0: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00020200: 6772 6f75 7020 7469 6d65 2074 7261 7665  group time trave
+00020210: 6c20 666f 726d 6174 2e22 2222 0a20 2020  l format.""".   
+00020220: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00020230: 2e5f 7469 6d65 5f74 7261 7665 6c5f 666f  ._time_travel_fo
+00020240: 726d 6174 0a0a 2020 2020 4070 726f 7065  rmat..    @prope
+00020250: 7274 790a 2020 2020 6465 6620 7061 7274  rty.    def part
+00020260: 6974 696f 6e5f 6b65 7928 7365 6c66 293a  ition_key(self):
+00020270: 0a20 2020 2020 2020 2022 2222 4c69 7374  .        """List
+00020280: 206f 6620 6665 6174 7572 6573 2062 7569   of features bui
+00020290: 6c64 696e 6720 7468 6520 7061 7274 6974  lding the partit
+000202a0: 696f 6e20 6b65 792e 2222 220a 2020 2020  ion key.""".    
+000202b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000202c0: 5f70 6172 7469 7469 6f6e 5f6b 6579 0a0a  _partition_key..
+000202d0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000202e0: 2020 6465 6620 6875 6469 5f70 7265 636f    def hudi_preco
+000202f0: 6d62 696e 655f 6b65 7928 7365 6c66 293a  mbine_key(self):
+00020300: 0a20 2020 2020 2020 2022 2222 4665 6174  .        """Feat
+00020310: 7572 6520 6e61 6d65 2074 6861 7420 6973  ure name that is
+00020320: 2074 6865 2068 7564 6920 7072 6563 6f6d   the hudi precom
+00020330: 6269 6e65 206b 6579 2e22 2222 0a20 2020  bine key.""".   
+00020340: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00020350: 2e5f 6875 6469 5f70 7265 636f 6d62 696e  ._hudi_precombin
+00020360: 655f 6b65 790a 0a20 2020 2040 7072 6f70  e_key..    @prop
+00020370: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
+00020380: 7475 7265 5f73 746f 7265 5f6e 616d 6528  ture_store_name(
+00020390: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000203a0: 2222 4e61 6d65 206f 6620 7468 6520 6665  ""Name of the fe
+000203b0: 6174 7572 6520 7374 6f72 6520 696e 2077  ature store in w
+000203c0: 6869 6368 2074 6865 2066 6561 7475 7265  hich the feature
+000203d0: 2067 726f 7570 2069 7320 6c6f 6361 7465   group is locate
+000203e0: 642e 2222 220a 2020 2020 2020 2020 7265  d.""".        re
+000203f0: 7475 726e 2073 656c 662e 5f66 6561 7475  turn self._featu
+00020400: 7265 5f73 746f 7265 5f6e 616d 650a 0a20  re_store_name.. 
+00020410: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00020420: 2064 6566 2063 7265 6174 6f72 2873 656c   def creator(sel
+00020430: 6629 3a0a 2020 2020 2020 2020 2222 2255  f):.        """U
+00020440: 7365 726e 616d 6520 6f66 2074 6865 2063  sername of the c
+00020450: 7265 6174 6f72 2e22 2222 0a20 2020 2020  reator.""".     
+00020460: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00020470: 6372 6561 746f 720a 0a20 2020 2040 7072  creator..    @pr
+00020480: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00020490: 7265 6174 6564 2873 656c 6629 3a0a 2020  reated(self):.  
+000204a0: 2020 2020 2020 2222 2254 696d 6573 7461        """Timesta
+000204b0: 6d70 2077 6865 6e20 7468 6520 6665 6174  mp when the feat
+000204c0: 7572 6520 6772 6f75 7020 7761 7320 6372  ure group was cr
+000204d0: 6561 7465 642e 2222 220a 2020 2020 2020  eated.""".      
+000204e0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
+000204f0: 7265 6174 6564 0a0a 2020 2020 4070 726f  reated..    @pro
+00020500: 7065 7274 790a 2020 2020 6465 6620 7374  perty.    def st
+00020510: 7265 616d 2873 656c 6629 3a0a 2020 2020  ream(self):.    
+00020520: 2020 2020 2222 2257 6865 7468 6572 2074      """Whether t
+00020530: 6f20 656e 6162 6c65 2072 6561 6c20 7469  o enable real ti
+00020540: 6d65 2073 7472 6561 6d20 7772 6974 696e  me stream writin
+00020550: 6720 6361 7061 6269 6c69 7469 6573 2e22  g capabilities."
+00020560: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00020570: 6e20 7365 6c66 2e5f 7374 7265 616d 0a0a  n self._stream..
+00020580: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00020590: 2020 6465 6620 7061 7265 6e74 7328 7365    def parents(se
+000205a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000205b0: 5061 7265 6e74 2066 6561 7475 7265 2067  Parent feature g
+000205c0: 726f 7570 7320 6173 206f 7269 6769 6e20  roups as origin 
+000205d0: 6f66 2074 6865 2064 6174 6120 696e 2074  of the data in t
+000205e0: 6865 2063 7572 7265 6e74 2066 6561 7475  he current featu
+000205f0: 7265 2067 726f 7570 2e0a 2020 2020 2020  re group..      
+00020600: 2020 5468 6973 2069 7320 7061 7274 206f    This is part o
+00020610: 6620 6578 706c 6963 6974 2070 726f 7665  f explicit prove
+00020620: 6e61 6e63 6522 2222 0a20 2020 2020 2020  nance""".       
+00020630: 2072 6574 7572 6e20 7365 6c66 2e5f 7061   return self._pa
+00020640: 7265 6e74 730a 0a20 2020 2040 7072 6f70  rents..    @prop
+00020650: 6572 7479 0a20 2020 2064 6566 206d 6174  erty.    def mat
+00020660: 6572 6961 6c69 7a61 7469 6f6e 5f6a 6f62  erialization_job
+00020670: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00020680: 2222 2247 6574 2074 6865 204a 6f62 206f  """Get the Job o
+00020690: 626a 6563 7420 7265 6665 7265 6e63 6520  bject reference 
+000206a0: 666f 7220 7468 6520 6d61 7465 7269 616c  for the material
+000206b0: 697a 6174 696f 6e20 6a6f 6220 666f 7220  ization job for 
+000206c0: 7468 6973 0a20 2020 2020 2020 2046 6561  this.        Fea
+000206d0: 7475 7265 2047 726f 7570 2e22 2222 0a20  ture Group.""". 
+000206e0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+000206f0: 6d61 7465 7269 616c 697a 6174 696f 6e5f  materialization_
+00020700: 6a6f 6220 6973 206e 6f74 204e 6f6e 653a  job is not None:
+00020710: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00020720: 7572 6e20 7365 6c66 2e5f 6d61 7465 7269  urn self._materi
+00020730: 616c 697a 6174 696f 6e5f 6a6f 620a 2020  alization_job.  
+00020740: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00020750: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
+00020760: 6772 6f75 705f 6e61 6d65 203d 2075 7469  group_name = uti
+00020770: 6c2e 6665 6174 7572 655f 6772 6f75 705f  l.feature_group_
+00020780: 6e61 6d65 2873 656c 6629 0a20 2020 2020  name(self).     
+00020790: 2020 2020 2020 206a 6f62 5f73 7566 6669         job_suffi
+000207a0: 785f 6c69 7374 203d 205b 226d 6174 6572  x_list = ["mater
+000207b0: 6961 6c69 7a61 7469 6f6e 222c 2022 6261  ialization", "ba
+000207c0: 636b 6669 6c6c 225d 0a20 2020 2020 2020  ckfill"].       
+000207d0: 2020 2020 2066 6f72 206a 6f62 5f73 7566       for job_suf
+000207e0: 6669 7820 696e 206a 6f62 5f73 7566 6669  fix in job_suffi
+000207f0: 785f 6c69 7374 3a0a 2020 2020 2020 2020  x_list:.        
+00020800: 2020 2020 2020 2020 6a6f 625f 6e61 6d65          job_name
+00020810: 203d 2022 7b7d 5f6f 6666 6c69 6e65 5f66   = "{}_offline_f
+00020820: 675f 7b7d 222e 666f 726d 6174 2866 6561  g_{}".format(fea
+00020830: 7475 7265 5f67 726f 7570 5f6e 616d 652c  ture_group_name,
+00020840: 206a 6f62 5f73 7566 6669 7829 0a20 2020   job_suffix).   
+00020850: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00020860: 205f 2069 6e20 7261 6e67 6528 3329 3a20   _ in range(3): 
+00020870: 2023 2072 6574 7279 2073 7461 7274 696e   # retry startin
+00020880: 6720 6a6f 620a 2020 2020 2020 2020 2020  g job.          
+00020890: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+000208a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208b0: 2020 2020 2020 2073 656c 662e 5f6d 6174         self._mat
+000208c0: 6572 6961 6c69 7a61 7469 6f6e 5f6a 6f62  erialization_job
+000208d0: 203d 206a 6f62 5f61 7069 2e4a 6f62 4170   = job_api.JobAp
+000208e0: 6928 292e 6765 7428 6a6f 625f 6e61 6d65  i().get(job_name
+000208f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00020900: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00020910: 2073 656c 662e 5f6d 6174 6572 6961 6c69   self._materiali
+00020920: 7a61 7469 6f6e 5f6a 6f62 0a20 2020 2020  zation_job.     
+00020930: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00020940: 7863 6570 7420 5265 7374 4150 4945 7272  xcept RestAPIErr
+00020950: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
+00020960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020970: 2069 6620 652e 7265 7370 6f6e 7365 2e73   if e.response.s
+00020980: 7461 7475 735f 636f 6465 203d 3d20 3430  tatus_code == 40
+00020990: 343a 0a20 2020 2020 2020 2020 2020 2020  4:.             
+000209a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000209b0: 6620 652e 7265 7370 6f6e 7365 2e6a 736f  f e.response.jso
+000209c0: 6e28 292e 6765 7428 2265 7272 6f72 436f  n().get("errorCo
+000209d0: 6465 222c 2022 2229 203d 3d20 3133 3030  de", "") == 1300
+000209e0: 3039 3a0a 2020 2020 2020 2020 2020 2020  09:.            
+000209f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a00: 2020 2020 6272 6561 6b20 2023 206e 6f20      break  # no 
+00020a10: 6e65 6564 2074 6f20 7265 7472 792c 2073  need to retry, s
+00020a20: 696e 6365 206e 6f20 7375 6368 206a 6f62  ince no such job
+00020a30: 2065 7869 7374 730a 2020 2020 2020 2020   exists.        
+00020a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00020a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a70: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00020a80: 6c65 6570 2831 2920 2023 2062 6163 6b6f  leep(1)  # backo
+00020a90: 6666 2061 6e64 2074 6865 6e20 7265 7472  ff and then retr
+00020aa0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+00020ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ac0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00020ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ae0: 2020 2072 6169 7365 2065 0a20 2020 2020     raise e.     
+00020af0: 2020 2020 2020 2072 6169 7365 2046 6561         raise Fea
+00020b00: 7475 7265 5374 6f72 6545 7863 6570 7469  tureStoreExcepti
+00020b10: 6f6e 2822 4e6f 206d 6174 6572 6961 6c69  on("No materiali
+00020b20: 7a61 7469 6f6e 206a 6f62 2077 6173 2066  zation job was f
+00020b30: 6f75 6e64 2229 0a0a 2020 2020 4070 726f  ound")..    @pro
+00020b40: 7065 7274 790a 2020 2020 6465 6620 7374  perty.    def st
+00020b50: 6174 6973 7469 6373 2873 656c 6629 3a0a  atistics(self):.
+00020b60: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+00020b70: 6865 206c 6174 6573 7420 636f 6d70 7574  he latest comput
+00020b80: 6564 2073 7461 7469 7374 6963 7320 666f  ed statistics fo
+00020b90: 7220 7468 6520 7768 6f6c 6520 6665 6174  r the whole feat
+00020ba0: 7572 6520 6772 6f75 702e 2222 220a 2020  ure group.""".  
+00020bb0: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
+00020bc0: 735f 7469 6d65 5f74 7261 7665 6c5f 656e  s_time_travel_en
+00020bd0: 6162 6c65 6428 293a 0a20 2020 2020 2020  abled():.       
+00020be0: 2020 2020 2023 2072 6574 7269 6576 6520       # retrieve 
+00020bf0: 7468 6520 6c61 7465 7374 7320 7374 6174  the latests stat
+00020c00: 6973 7469 6373 2063 6f6d 7075 7465 6420  istics computed 
+00020c10: 6f6e 2074 6865 2077 686f 6c65 2046 6561  on the whole Fea
+00020c20: 7475 7265 2047 726f 7570 2c20 696e 636c  ture Group, incl
+00020c30: 7564 696e 6720 616c 6c20 7468 6520 636f  uding all the co
+00020c40: 6d6d 6974 732e 0a20 2020 2020 2020 2020  mmits..         
+00020c50: 2020 206e 6f77 203d 2075 7469 6c2e 636f     now = util.co
+00020c60: 6e76 6572 745f 6576 656e 745f 7469 6d65  nvert_event_time
+00020c70: 5f74 6f5f 7469 6d65 7374 616d 7028 6461  _to_timestamp(da
+00020c80: 7465 7469 6d65 2e6e 6f77 2829 290a 2020  tetime.now()).  
+00020c90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00020ca0: 2073 656c 662e 5f73 7461 7469 7374 6963   self._statistic
+00020cb0: 735f 656e 6769 6e65 2e67 6574 5f62 795f  s_engine.get_by_
+00020cc0: 7469 6d65 5f77 696e 646f 7728 0a20 2020  time_window(.   
+00020cd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00020ce0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00020cf0: 2020 2073 7461 7274 5f63 6f6d 6d69 745f     start_commit_
+00020d00: 7469 6d65 3d4e 6f6e 652c 0a20 2020 2020  time=None,.     
+00020d10: 2020 2020 2020 2020 2020 2065 6e64 5f63             end_c
+00020d20: 6f6d 6d69 745f 7469 6d65 3d6e 6f77 2c0a  ommit_time=now,.
+00020d30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00020d40: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+00020d50: 6572 2829 2e73 7461 7469 7374 6963 730a  er().statistics.
+00020d60: 0a20 2020 2040 6465 7363 7269 7074 696f  .    @descriptio
+00020d70: 6e2e 7365 7474 6572 0a20 2020 2064 6566  n.setter.    def
+00020d80: 2064 6573 6372 6970 7469 6f6e 2873 656c   description(sel
+00020d90: 662c 206e 6577 5f64 6573 6372 6970 7469  f, new_descripti
+00020da0: 6f6e 293a 0a20 2020 2020 2020 2073 656c  on):.        sel
+00020db0: 662e 5f64 6573 6372 6970 7469 6f6e 203d  f._description =
+00020dc0: 206e 6577 5f64 6573 6372 6970 7469 6f6e   new_description
+00020dd0: 0a0a 2020 2020 4074 696d 655f 7472 6176  ..    @time_trav
+00020de0: 656c 5f66 6f72 6d61 742e 7365 7474 6572  el_format.setter
+00020df0: 0a20 2020 2064 6566 2074 696d 655f 7472  .    def time_tr
+00020e00: 6176 656c 5f66 6f72 6d61 7428 7365 6c66  avel_format(self
+00020e10: 2c20 6e65 775f 7469 6d65 5f74 7261 7665  , new_time_trave
+00020e20: 6c5f 666f 726d 6174 293a 0a20 2020 2020  l_format):.     
+00020e30: 2020 2073 656c 662e 5f74 696d 655f 7472     self._time_tr
+00020e40: 6176 656c 5f66 6f72 6d61 7420 3d20 6e65  avel_format = ne
+00020e50: 775f 7469 6d65 5f74 7261 7665 6c5f 666f  w_time_travel_fo
+00020e60: 726d 6174 0a0a 2020 2020 4070 6172 7469  rmat..    @parti
+00020e70: 7469 6f6e 5f6b 6579 2e73 6574 7465 720a  tion_key.setter.
+00020e80: 2020 2020 6465 6620 7061 7274 6974 696f      def partitio
+00020e90: 6e5f 6b65 7928 7365 6c66 2c20 6e65 775f  n_key(self, new_
+00020ea0: 7061 7274 6974 696f 6e5f 6b65 7929 3a0a  partition_key):.
+00020eb0: 2020 2020 2020 2020 7365 6c66 2e5f 7061          self._pa
+00020ec0: 7274 6974 696f 6e5f 6b65 7920 3d20 5b70  rtition_key = [p
+00020ed0: 6b2e 6c6f 7765 7228 2920 666f 7220 706b  k.lower() for pk
+00020ee0: 2069 6e20 6e65 775f 7061 7274 6974 696f   in new_partitio
+00020ef0: 6e5f 6b65 795d 0a0a 2020 2020 4068 7564  n_key]..    @hud
+00020f00: 695f 7072 6563 6f6d 6269 6e65 5f6b 6579  i_precombine_key
+00020f10: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00020f20: 6875 6469 5f70 7265 636f 6d62 696e 655f  hudi_precombine_
+00020f30: 6b65 7928 7365 6c66 2c20 6875 6469 5f70  key(self, hudi_p
+00020f40: 7265 636f 6d62 696e 655f 6b65 7929 3a0a  recombine_key):.
+00020f50: 2020 2020 2020 2020 7365 6c66 2e5f 6875          self._hu
+00020f60: 6469 5f70 7265 636f 6d62 696e 655f 6b65  di_precombine_ke
+00020f70: 7920 3d20 6875 6469 5f70 7265 636f 6d62  y = hudi_precomb
+00020f80: 696e 655f 6b65 792e 6c6f 7765 7228 290a  ine_key.lower().
+00020f90: 0a20 2020 2040 7374 7265 616d 2e73 6574  .    @stream.set
+00020fa0: 7465 720a 2020 2020 6465 6620 7374 7265  ter.    def stre
+00020fb0: 616d 2873 656c 662c 2073 7472 6561 6d29  am(self, stream)
+00020fc0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00020fd0: 7374 7265 616d 203d 2073 7472 6561 6d0a  stream = stream.
+00020fe0: 0a20 2020 2040 7061 7265 6e74 732e 7365  .    @parents.se
+00020ff0: 7474 6572 0a20 2020 2064 6566 2070 6172  tter.    def par
+00021000: 656e 7473 2873 656c 662c 206e 6577 5f70  ents(self, new_p
+00021010: 6172 656e 7473 293a 0a20 2020 2020 2020  arents):.       
+00021020: 2073 656c 662e 5f70 6172 656e 7473 203d   self._parents =
+00021030: 206e 6577 5f70 6172 656e 7473 0a0a 0a63   new_parents...c
+00021040: 6c61 7373 2045 7874 6572 6e61 6c46 6561  lass ExternalFea
+00021050: 7475 7265 4772 6f75 7028 4665 6174 7572  tureGroup(Featur
+00021060: 6547 726f 7570 4261 7365 293a 0a20 2020  eGroupBase):.   
+00021070: 2045 5854 4552 4e41 4c5f 4645 4154 5552   EXTERNAL_FEATUR
+00021080: 455f 4752 4f55 5020 3d20 224f 4e5f 4445  E_GROUP = "ON_DE
+00021090: 4d41 4e44 5f46 4541 5455 5245 5f47 524f  MAND_FEATURE_GRO
+000210a0: 5550 220a 2020 2020 454e 5449 5459 5f54  UP".    ENTITY_T
+000210b0: 5950 4520 3d20 2266 6561 7475 7265 6772  YPE = "featuregr
+000210c0: 6f75 7073 220a 0a20 2020 2064 6566 205f  oups"..    def _
+000210d0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000210e0: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
+000210f0: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
+00021100: 2c0a 2020 2020 2020 2020 7175 6572 793d  ,.        query=
+00021110: 4e6f 6e65 2c0a 2020 2020 2020 2020 6461  None,.        da
+00021120: 7461 5f66 6f72 6d61 743d 4e6f 6e65 2c0a  ta_format=None,.
+00021130: 2020 2020 2020 2020 7061 7468 3d4e 6f6e          path=Non
+00021140: 652c 0a20 2020 2020 2020 206f 7074 696f  e,.        optio
+00021150: 6e73 3d7b 7d2c 0a20 2020 2020 2020 206e  ns={},.        n
+00021160: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
+00021170: 2020 7665 7273 696f 6e3d 4e6f 6e65 2c0a    version=None,.
+00021180: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00021190: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
+000211a0: 2020 7072 696d 6172 795f 6b65 793d 4e6f    primary_key=No
+000211b0: 6e65 2c0a 2020 2020 2020 2020 6665 6174  ne,.        feat
+000211c0: 7572 6573 746f 7265 5f69 643d 4e6f 6e65  urestore_id=None
+000211d0: 2c0a 2020 2020 2020 2020 6665 6174 7572  ,.        featur
+000211e0: 6573 746f 7265 5f6e 616d 653d 4e6f 6e65  estore_name=None
+000211f0: 2c0a 2020 2020 2020 2020 6372 6561 7465  ,.        create
+00021200: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
+00021210: 6372 6561 746f 723d 4e6f 6e65 2c0a 2020  creator=None,.  
+00021220: 2020 2020 2020 6964 3d4e 6f6e 652c 0a20        id=None,. 
+00021230: 2020 2020 2020 2066 6561 7475 7265 733d         features=
+00021240: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c6f  None,.        lo
+00021250: 6361 7469 6f6e 3d4e 6f6e 652c 0a20 2020  cation=None,.   
+00021260: 2020 2020 2073 7461 7469 7374 6963 735f       statistics_
+00021270: 636f 6e66 6967 3d4e 6f6e 652c 0a20 2020  config=None,.   
+00021280: 2020 2020 2065 7665 6e74 5f74 696d 653d       event_time=
+00021290: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
+000212a0: 7065 6374 6174 696f 6e5f 7375 6974 653d  pectation_suite=
+000212b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f6e  None,.        on
+000212c0: 6c69 6e65 5f65 6e61 626c 6564 3d46 616c  line_enabled=Fal
+000212d0: 7365 2c0a 2020 2020 2020 2020 6872 6566  se,.        href
+000212e0: 3d4e 6f6e 652c 0a20 2020 2020 2020 206f  =None,.        o
+000212f0: 6e6c 696e 655f 746f 7069 635f 6e61 6d65  nline_topic_name
+00021300: 3d4e 6f6e 652c 0a20 2020 2020 2020 2074  =None,.        t
+00021310: 6f70 6963 5f6e 616d 653d 4e6f 6e65 2c0a  opic_name=None,.
+00021320: 2020 2020 2020 2020 6e6f 7469 6669 6361          notifica
+00021330: 7469 6f6e 5f74 6f70 6963 5f6e 616d 653d  tion_topic_name=
+00021340: 4e6f 6e65 2c0a 2020 2020 2020 2020 7370  None,.        sp
+00021350: 696e 653d 4661 6c73 652c 0a20 2020 2020  ine=False,.     
+00021360: 2020 2064 6570 7265 6361 7465 643d 4661     deprecated=Fa
+00021370: 6c73 652c 0a20 2020 2020 2020 202a 2a6b  lse,.        **k
+00021380: 7761 7267 732c 0a20 2020 2029 3a0a 2020  wargs,.    ):.  
+00021390: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000213a0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000213b0: 2020 2020 6e61 6d65 2c0a 2020 2020 2020      name,.      
+000213c0: 2020 2020 2020 7665 7273 696f 6e2c 0a20        version,. 
+000213d0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+000213e0: 7265 7374 6f72 655f 6964 2c0a 2020 2020  restore_id,.    
+000213f0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
+00021400: 2c0a 2020 2020 2020 2020 2020 2020 6576  ,.            ev
+00021410: 656e 745f 7469 6d65 3d65 7665 6e74 5f74  ent_time=event_t
+00021420: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
+00021430: 206f 6e6c 696e 655f 656e 6162 6c65 643d   online_enabled=
+00021440: 6f6e 6c69 6e65 5f65 6e61 626c 6564 2c0a  online_enabled,.
+00021450: 2020 2020 2020 2020 2020 2020 6964 3d69              id=i
+00021460: 642c 0a20 2020 2020 2020 2020 2020 2065  d,.            e
+00021470: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+00021480: 3d65 7870 6563 7461 7469 6f6e 5f73 7569  =expectation_sui
+00021490: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
+000214a0: 6f6e 6c69 6e65 5f74 6f70 6963 5f6e 616d  online_topic_nam
+000214b0: 653d 6f6e 6c69 6e65 5f74 6f70 6963 5f6e  e=online_topic_n
+000214c0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+000214d0: 2074 6f70 6963 5f6e 616d 653d 746f 7069   topic_name=topi
+000214e0: 635f 6e61 6d65 2c0a 2020 2020 2020 2020  c_name,.        
+000214f0: 2020 2020 6e6f 7469 6669 6361 7469 6f6e      notification
+00021500: 5f74 6f70 6963 5f6e 616d 653d 6e6f 7469  _topic_name=noti
+00021510: 6669 6361 7469 6f6e 5f74 6f70 6963 5f6e  fication_topic_n
+00021520: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00021530: 2064 6570 7265 6361 7465 643d 6465 7072   deprecated=depr
+00021540: 6563 6174 6564 2c0a 2020 2020 2020 2020  ecated,.        
+00021550: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00021560: 5f66 6561 7475 7265 5f73 746f 7265 5f6e  _feature_store_n
+00021570: 616d 6520 3d20 6665 6174 7572 6573 746f  ame = featuresto
+00021580: 7265 5f6e 616d 650a 2020 2020 2020 2020  re_name.        
+00021590: 7365 6c66 2e5f 6465 7363 7269 7074 696f  self._descriptio
+000215a0: 6e20 3d20 6465 7363 7269 7074 696f 6e0a  n = description.
+000215b0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+000215c0: 6561 7465 6420 3d20 6372 6561 7465 640a  eated = created.
+000215d0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+000215e0: 6561 746f 7220 3d20 7573 6572 2e55 7365  eator = user.Use
+000215f0: 722e 6672 6f6d 5f72 6573 706f 6e73 655f  r.from_response_
+00021600: 6a73 6f6e 2863 7265 6174 6f72 290a 2020  json(creator).  
+00021610: 2020 2020 2020 7365 6c66 2e5f 7175 6572        self._quer
+00021620: 7920 3d20 7175 6572 790a 2020 2020 2020  y = query.      
+00021630: 2020 7365 6c66 2e5f 6461 7461 5f66 6f72    self._data_for
+00021640: 6d61 7420 3d20 6461 7461 5f66 6f72 6d61  mat = data_forma
+00021650: 742e 7570 7065 7228 2920 6966 2064 6174  t.upper() if dat
+00021660: 615f 666f 726d 6174 2065 6c73 6520 4e6f  a_format else No
+00021670: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00021680: 5f70 6174 6820 3d20 7061 7468 0a0a 2020  _path = path..  
+00021690: 2020 2020 2020 7365 6c66 2e5f 6665 6174        self._feat
+000216a0: 7572 6573 203d 205b 0a20 2020 2020 2020  ures = [.       
+000216b0: 2020 2020 2066 6561 7475 7265 2e46 6561       feature.Fea
+000216c0: 7475 7265 2e66 726f 6d5f 7265 7370 6f6e  ture.from_respon
+000216d0: 7365 5f6a 736f 6e28 6665 6174 2920 6966  se_json(feat) if
+000216e0: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
+000216f0: 2c20 6469 6374 2920 656c 7365 2066 6561  , dict) else fea
+00021700: 740a 2020 2020 2020 2020 2020 2020 666f  t.            fo
+00021710: 7220 6665 6174 2069 6e20 2866 6561 7475  r feat in (featu
+00021720: 7265 7320 6f72 205b 5d29 0a20 2020 2020  res or []).     
+00021730: 2020 205d 0a0a 2020 2020 2020 2020 7365     ]..        se
+00021740: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+00021750: 705f 656e 6769 6e65 203d 2028 0a20 2020  p_engine = (.   
+00021760: 2020 2020 2020 2020 2065 7874 6572 6e61           externa
+00021770: 6c5f 6665 6174 7572 655f 6772 6f75 705f  l_feature_group_
+00021780: 656e 6769 6e65 2e45 7874 6572 6e61 6c46  engine.ExternalF
+00021790: 6561 7475 7265 4772 6f75 7045 6e67 696e  eatureGroupEngin
+000217a0: 6528 6665 6174 7572 6573 746f 7265 5f69  e(featurestore_i
+000217b0: 6429 0a20 2020 2020 2020 2029 0a0a 2020  d).        )..  
+000217c0: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
+000217d0: 643a 0a20 2020 2020 2020 2020 2020 2023  d:.            #
+000217e0: 2047 6f74 2066 726f 6d20 486f 7073 776f   Got from Hopswo
+000217f0: 726b 732c 2064 6573 6572 6961 6c69 7a65  rks, deserialize
+00021800: 2066 6561 7475 7265 7320 616e 6420 7374   features and st
+00021810: 6f72 6167 6520 636f 6e6e 6563 746f 720a  orage connector.
+00021820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00021830: 2e5f 6665 6174 7572 6573 203d 2028 0a20  ._features = (. 
+00021840: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00021850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021860: 2020 2020 2066 6561 7475 7265 2e46 6561       feature.Fea
+00021870: 7475 7265 2e66 726f 6d5f 7265 7370 6f6e  ture.from_respon
+00021880: 7365 5f6a 736f 6e28 6665 6174 290a 2020  se_json(feat).  
+00021890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218a0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000218b0: 6665 6174 2c20 6469 6374 290a 2020 2020  feat, dict).    
+000218c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218d0: 656c 7365 2066 6561 740a 2020 2020 2020  else feat.      
+000218e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000218f0: 7220 6665 6174 2069 6e20 6665 6174 7572  r feat in featur
+00021900: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00021910: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00021920: 2020 2020 2069 6620 6665 6174 7572 6573       if features
+00021930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021940: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00021950: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00021960: 2020 2020 2073 656c 662e 7072 696d 6172       self.primar
+00021970: 795f 6b65 7920 3d20 280a 2020 2020 2020  y_key = (.      
+00021980: 2020 2020 2020 2020 2020 5b66 6561 742e            [feat.
+00021990: 6e61 6d65 2066 6f72 2066 6561 7420 696e  name for feat in
+000219a0: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
+000219b0: 6966 2066 6561 742e 7072 696d 6172 7920  if feat.primary 
+000219c0: 6973 2054 7275 655d 0a20 2020 2020 2020  is True].       
+000219d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000219e0: 2e5f 6665 6174 7572 6573 0a20 2020 2020  ._features.     
+000219f0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00021a00: 5b5d 0a20 2020 2020 2020 2020 2020 2029  [].            )
+00021a10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00021a20: 662e 7374 6174 6973 7469 6373 5f63 6f6e  f.statistics_con
+00021a30: 6669 6720 3d20 7374 6174 6973 7469 6373  fig = statistics
+00021a40: 5f63 6f6e 6669 670a 0a20 2020 2020 2020  _config..       
+00021a50: 2020 2020 2073 656c 662e 5f6f 7074 696f       self._optio
+00021a60: 6e73 203d 2028 0a20 2020 2020 2020 2020  ns = (.         
+00021a70: 2020 2020 2020 207b 6f70 7469 6f6e 5b22         {option["
+00021a80: 6e61 6d65 225d 3a20 6f70 7469 6f6e 5b22  name"]: option["
+00021a90: 7661 6c75 6522 5d20 666f 7220 6f70 7469  value"] for opti
+00021aa0: 6f6e 2069 6e20 6f70 7469 6f6e 737d 0a20  on in options}. 
+00021ab0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00021ac0: 6620 6f70 7469 6f6e 730a 2020 2020 2020  f options.      
+00021ad0: 2020 2020 2020 2020 2020 656c 7365 204e            else N
+00021ae0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00021af0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00021b00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00021b10: 2e70 7269 6d61 7279 5f6b 6579 203d 2070  .primary_key = p
+00021b20: 7269 6d61 7279 5f6b 6579 0a20 2020 2020  rimary_key.     
+00021b30: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00021b40: 6973 7469 6373 5f63 6f6e 6669 6720 3d20  istics_config = 
+00021b50: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
+00021b60: 670a 2020 2020 2020 2020 2020 2020 7365  g.            se
+00021b70: 6c66 2e5f 6665 6174 7572 6573 203d 2066  lf._features = f
+00021b80: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
+00021b90: 2020 2020 7365 6c66 2e5f 6f70 7469 6f6e      self._option
+00021ba0: 7320 3d20 6f70 7469 6f6e 730a 0a20 2020  s = options..   
+00021bb0: 2020 2020 2069 6620 7374 6f72 6167 655f       if storage_
+00021bc0: 636f 6e6e 6563 746f 7220 6973 206e 6f74  connector is not
+00021bd0: 204e 6f6e 6520 616e 6420 6973 696e 7374   None and isinst
+00021be0: 616e 6365 2873 746f 7261 6765 5f63 6f6e  ance(storage_con
+00021bf0: 6e65 6374 6f72 2c20 6469 6374 293a 0a20  nector, dict):. 
+00021c00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00021c10: 5f73 746f 7261 6765 5f63 6f6e 6e65 6374  _storage_connect
+00021c20: 6f72 203d 2073 632e 5374 6f72 6167 6543  or = sc.StorageC
+00021c30: 6f6e 6e65 6374 6f72 2e66 726f 6d5f 7265  onnector.from_re
+00021c40: 7370 6f6e 7365 5f6a 736f 6e28 0a20 2020  sponse_json(.   
+00021c50: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00021c60: 7261 6765 5f63 6f6e 6e65 6374 6f72 0a20  rage_connector. 
+00021c70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00021c80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00021c90: 2020 2020 2020 2073 656c 662e 5f73 746f         self._sto
+00021ca0: 7261 6765 5f63 6f6e 6e65 6374 6f72 203d  rage_connector =
+00021cb0: 2073 746f 7261 6765 5f63 6f6e 6e65 6374   storage_connect
+00021cc0: 6f72 0a0a 2020 2020 2020 2020 7365 6c66  or..        self
+00021cd0: 2e5f 6872 6566 203d 2068 7265 660a 0a20  ._href = href.. 
+00021ce0: 2020 2064 6566 2073 6176 6528 7365 6c66     def save(self
+00021cf0: 293a 0a20 2020 2020 2020 2022 2222 5065  ):.        """Pe
+00021d00: 7273 6973 7420 7468 6520 6d65 7461 6461  rsist the metada
+00021d10: 7461 2066 6f72 2074 6869 7320 6578 7465  ta for this exte
+00021d20: 726e 616c 2066 6561 7475 7265 2067 726f  rnal feature gro
+00021d30: 7570 2e0a 0a20 2020 2020 2020 2057 6974  up...        Wit
+00021d40: 686f 7574 2063 616c 6c69 6e67 2074 6869  hout calling thi
+00021d50: 7320 6d65 7468 6f64 2c20 796f 7572 2066  s method, your f
+00021d60: 6561 7475 7265 2067 726f 7570 2077 696c  eature group wil
+00021d70: 6c20 6f6e 6c79 2065 7869 7374 0a20 2020  l only exist.   
+00021d80: 2020 2020 2069 6e20 796f 7572 2050 7974       in your Pyt
+00021d90: 686f 6e20 4b65 726e 656c 2c20 6275 7420  hon Kernel, but 
+00021da0: 6e6f 7420 696e 2048 6f70 7377 6f72 6b73  not in Hopsworks
+00021db0: 2e0a 0a20 2020 2020 2020 2060 6060 7079  ...        ```py
+00021dc0: 7468 6f6e 0a20 2020 2020 2020 2071 7565  thon.        que
+00021dd0: 7279 203d 2022 5345 4c45 4354 202a 2046  ry = "SELECT * F
+00021de0: 524f 4d20 7361 6c65 7322 0a0a 2020 2020  ROM sales"..    
+00021df0: 2020 2020 6667 203d 2066 6561 7475 7265      fg = feature
+00021e00: 5f73 746f 7265 2e63 7265 6174 655f 6578  _store.create_ex
+00021e10: 7465 726e 616c 5f66 6561 7475 7265 5f67  ternal_feature_g
+00021e20: 726f 7570 286e 616d 653d 2273 616c 6573  roup(name="sales
+00021e30: 222c 0a20 2020 2020 2020 2020 2020 2076  ",.            v
+00021e40: 6572 7369 6f6e 3d31 2c0a 2020 2020 2020  ersion=1,.      
+00021e50: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00021e60: 6e3d 2250 6879 7369 6361 6c20 7368 6f70  n="Physical shop
+00021e70: 2073 616c 6573 2066 6561 7475 7265 7322   sales features"
+00021e80: 2c0a 2020 2020 2020 2020 2020 2020 7175  ,.            qu
+00021e90: 6572 793d 7175 6572 792c 0a20 2020 2020  ery=query,.     
+00021ea0: 2020 2020 2020 2073 746f 7261 6765 5f63         storage_c
+00021eb0: 6f6e 6e65 6374 6f72 3d63 6f6e 6e65 6374  onnector=connect
+00021ec0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00021ed0: 7072 696d 6172 795f 6b65 793d 5b27 7373  primary_key=['ss
+00021ee0: 5f73 746f 7265 5f73 6b27 5d2c 0a20 2020  _store_sk'],.   
+00021ef0: 2020 2020 2020 2020 2065 7665 6e74 5f74           event_t
+00021f00: 696d 653d 2773 616c 655f 6461 7465 270a  ime='sale_date'.
+00021f10: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00021f20: 2020 2066 672e 7361 7665 2829 0a20 2020     fg.save().   
+00021f30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00021f40: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
+00021f50: 726f 7570 5f65 6e67 696e 652e 7361 7665  roup_engine.save
+00021f60: 2873 656c 6629 0a20 2020 2020 2020 2073  (self).        s
+00021f70: 656c 662e 5f63 6f64 655f 656e 6769 6e65  elf._code_engine
+00021f80: 2e73 6176 655f 636f 6465 2873 656c 6629  .save_code(self)
+00021f90: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00021fa0: 662e 7374 6174 6973 7469 6373 5f63 6f6e  f.statistics_con
+00021fb0: 6669 672e 656e 6162 6c65 643a 0a20 2020  fig.enabled:.   
+00021fc0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+00021fd0: 7461 7469 7374 6963 735f 656e 6769 6e65  tatistics_engine
+00021fe0: 2e63 6f6d 7075 7465 5f61 6e64 5f73 6176  .compute_and_sav
+00021ff0: 655f 7374 6174 6973 7469 6373 2873 656c  e_statistics(sel
+00022000: 6629 0a0a 2020 2020 6465 6620 696e 7365  f)..    def inse
+00022010: 7274 280a 2020 2020 2020 2020 7365 6c66  rt(.        self
+00022020: 2c0a 2020 2020 2020 2020 6665 6174 7572  ,.        featur
+00022030: 6573 3a20 556e 696f 6e5b 0a20 2020 2020  es: Union[.     
+00022040: 2020 2020 2020 2070 642e 4461 7461 4672         pd.DataFr
+00022050: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00022060: 2054 7970 6556 6172 2822 7079 7370 6172   TypeVar("pyspar
+00022070: 6b2e 7371 6c2e 4461 7461 4672 616d 6522  k.sql.DataFrame"
+00022080: 292c 2020 2320 6e6f 7161 3a20 4638 3231  ),  # noqa: F821
+00022090: 0a20 2020 2020 2020 2020 2020 2054 7970  .            Typ
+000220a0: 6556 6172 2822 7079 7370 6172 6b2e 5244  eVar("pyspark.RD
+000220b0: 4422 292c 2020 2320 6e6f 7161 3a20 4638  D"),  # noqa: F8
+000220c0: 3231 0a20 2020 2020 2020 2020 2020 206e  21.            n
+000220d0: 702e 6e64 6172 7261 792c 0a20 2020 2020  p.ndarray,.     
+000220e0: 2020 2020 2020 204c 6973 745b 6c69 7374         List[list
+000220f0: 5d2c 0a20 2020 2020 2020 205d 2c0a 2020  ],.        ],.  
+00022100: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
+00022110: 6f6e 733a 204f 7074 696f 6e61 6c5b 4469  ons: Optional[Di
+00022120: 6374 5b73 7472 2c20 416e 795d 5d20 3d20  ct[str, Any]] = 
+00022130: 7b7d 2c0a 2020 2020 2020 2020 7661 6c69  {},.        vali
+00022140: 6461 7469 6f6e 5f6f 7074 696f 6e73 3a20  dation_options: 
+00022150: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+00022160: 722c 2041 6e79 5d5d 203d 207b 7d2c 0a20  r, Any]] = {},. 
+00022170: 2020 2020 2020 2073 6176 655f 636f 6465         save_code
+00022180: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00022190: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+000221a0: 2077 6169 743a 2062 6f6f 6c20 3d20 4661   wait: bool = Fa
+000221b0: 6c73 652c 0a20 2020 2029 202d 3e20 5475  lse,.    ) -> Tu
+000221c0: 706c 655b 4f70 7469 6f6e 616c 5b4a 6f62  ple[Optional[Job
+000221d0: 5d2c 204f 7074 696f 6e61 6c5b 5661 6c69  ], Optional[Vali
+000221e0: 6461 7469 6f6e 5265 706f 7274 5d5d 3a0a  dationReport]]:.
+000221f0: 2020 2020 2020 2020 2222 2249 6e73 6572          """Inser
+00022200: 7420 7468 6520 6461 7461 6672 616d 6520  t the dataframe 
+00022210: 6665 6174 7572 6520 7661 6c75 6573 204f  feature values O
+00022220: 4e4c 5920 696e 2074 6865 206f 6e6c 696e  NLY in the onlin
+00022230: 6520 6665 6174 7572 6520 7374 6f72 652e  e feature store.
+00022240: 0a0a 2020 2020 2020 2020 4578 7465 726e  ..        Extern
+00022250: 616c 2046 6561 7475 7265 2047 726f 7570  al Feature Group
+00022260: 7320 636f 6e74 6169 6e73 206d 6574 6164  s contains metad
+00022270: 6174 6120 6162 6f75 7420 6665 6174 7572  ata about featur
+00022280: 6520 6461 7461 2069 6e20 616e 2065 7874  e data in an ext
+00022290: 6572 6e61 6c20 7374 6f72 6167 6520 7379  ernal storage sy
+000222a0: 7374 656d 2e0a 2020 2020 2020 2020 4578  stem..        Ex
+000222b0: 7465 726e 616c 2073 746f 7261 6765 2073  ternal storage s
+000222c0: 7973 7465 6d20 6172 6520 7573 7561 6c6c  ystem are usuall
+000222d0: 7920 6f66 666c 696e 652c 206d 6561 6e69  y offline, meani
+000222e0: 6e67 2066 6561 7475 7265 2076 616c 7565  ng feature value
+000222f0: 7320 6361 6e6e 6f74 2062 6520 7265 7472  s cannot be retr
+00022300: 6965 7665 6420 696e 2072 6561 6c2d 7469  ieved in real-ti
+00022310: 6d65 2e0a 2020 2020 2020 2020 496e 206f  me..        In o
+00022320: 7264 6572 2074 6f20 7573 6520 7468 6520  rder to use the 
+00022330: 6665 6174 7572 6520 7661 6c75 6573 2066  feature values f
+00022340: 6f72 2072 6561 6c2d 7469 6d65 2075 7365  or real-time use
+00022350: 2d63 6173 6573 2c20 796f 7520 6361 6e20  -cases, you can 
+00022360: 696e 7365 7274 2074 6865 6d0a 2020 2020  insert them.    
+00022370: 2020 2020 696e 2048 6f70 736f 776f 726b      in Hopsowork
+00022380: 7320 4f6e 6c69 6e65 2046 6561 7475 7265  s Online Feature
+00022390: 2053 746f 7265 2076 6961 2074 6869 7320   Store via this 
+000223a0: 6d65 7468 6f64 2e0a 0a20 2020 2020 2020  method...       
+000223b0: 2054 6865 204f 6e6c 696e 6520 4665 6174   The Online Feat
+000223c0: 7572 6520 5374 6f72 6520 6861 7320 6120  ure Store has a 
+000223d0: 7369 6e67 6c65 2d65 6e74 7279 2070 6572  single-entry per
+000223e0: 2070 7269 6d61 7279 206b 6579 2076 616c   primary key val
+000223f0: 7565 2c20 6d65 6169 6e69 6e67 2074 6861  ue, meaining tha
+00022400: 7420 7072 6f76 6964 696e 6720 6120 6e65  t providing a ne
+00022410: 7720 7661 6c75 6520 7769 7468 0a20 2020  w value with.   
+00022420: 2020 2020 2066 6f72 2061 2067 6976 656e       for a given
+00022430: 2070 7269 6d61 7279 206b 6579 2077 696c   primary key wil
+00022440: 6c20 6f76 6572 7772 6974 6520 7468 6520  l overwrite the 
+00022450: 6578 6973 7469 6e67 2076 616c 7565 2e20  existing value. 
+00022460: 4e6f 2072 6563 6f72 6420 6f66 2074 6865  No record of the
+00022470: 2070 7265 7669 6f75 7320 7661 6c75 6520   previous value 
+00022480: 6973 206b 6570 742e 0a0a 2020 2020 2020  is kept...      
+00022490: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
+000224a0: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
+000224b0: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
+000224c0: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
+000224d0: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
+000224e0: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
+000224f0: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
+00022500: 2023 2067 6574 2074 6865 2045 7874 6572   # get the Exter
+00022510: 6e61 6c20 4665 6174 7572 6520 4772 6f75  nal Feature Grou
+00022520: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
+00022530: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
+00022540: 6574 5f66 6561 7475 7265 5f67 726f 7570  et_feature_group
+00022550: 286e 616d 653d 2265 7874 6572 6e61 6c5f  (name="external_
+00022560: 7361 6c65 735f 7265 636f 7264 7322 2c20  sales_records", 
+00022570: 7665 7273 696f 6e3d 3129 0a0a 2020 2020  version=1)..    
+00022580: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+00022590: 6520 6665 6174 7572 6520 7661 6c75 6573  e feature values
+000225a0: 2c20 652e 6720 7265 6164 696e 6720 6672  , e.g reading fr
+000225b0: 6f6d 2063 7376 2066 696c 6573 2069 6e20  om csv files in 
+000225c0: 6120 5333 2062 7563 6b65 740a 2020 2020  a S3 bucket.    
+000225d0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
+000225e0: 7661 6c75 6573 203d 202e 2e2e 0a0a 2020  values = .....  
+000225f0: 2020 2020 2020 2020 2020 2320 696e 7365            # inse
+00022600: 7274 2074 6865 2066 6561 7475 7265 2076  rt the feature v
+00022610: 616c 7565 7320 696e 2074 6865 206f 6e6c  alues in the onl
+00022620: 696e 6520 6665 6174 7572 6520 7374 6f72  ine feature stor
+00022630: 650a 2020 2020 2020 2020 2020 2020 6667  e.            fg
+00022640: 2e69 6e73 6572 7428 6665 6174 7572 655f  .insert(feature_
+00022650: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
+00022660: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+00022670: 2021 2121 204e 6f74 650a 2020 2020 2020   !!! Note.      
+00022680: 2020 2020 2020 4461 7461 2056 616c 6964        Data Valid
+00022690: 6174 696f 6e20 7669 6120 4772 6561 7420  ation via Great 
+000226a0: 4578 7065 6374 6174 696f 6e20 6973 2073  Expectation is s
+000226b0: 7570 706f 7274 6564 2069 6620 796f 7520  upported if you 
+000226c0: 6861 7665 2061 7474 6163 6865 6420 616e  have attached an
+000226d0: 2065 7870 6563 7461 7469 6f6e 2073 7569   expectation sui
+000226e0: 7465 2074 6f0a 2020 2020 2020 2020 2020  te to.          
+000226f0: 2020 796f 7572 2045 7874 6572 6e61 6c20    your External 
+00022700: 4665 6174 7572 6520 4772 6f75 702e 2048  Feature Group. H
+00022710: 6f77 6576 6572 2c20 6173 206f 7070 6f73  owever, as oppos
+00022720: 6564 2074 6f20 7265 6775 6c61 7220 4665  ed to regular Fe
+00022730: 6174 7572 6520 4772 6f75 7073 2c20 7468  ature Groups, th
+00022740: 6973 2063 616e 206c 6561 6420 746f 0a20  is can lead to. 
+00022750: 2020 2020 2020 2020 2020 2064 6973 6372             discr
+00022760: 6570 616e 6369 6573 2062 6574 7765 656e  epancies between
+00022770: 2074 6865 2064 6174 6120 696e 2074 6865   the data in the
+00022780: 2065 7874 6572 6e61 6c20 7374 6f72 6167   external storag
+00022790: 6520 7379 7374 656d 2061 6e64 2074 6865  e system and the
+000227a0: 206f 6e6c 696e 6520 6665 6174 7572 6520   online feature 
+000227b0: 7374 6f72 652e 0a0a 2020 2020 2020 2020  store...        
+000227c0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+000227d0: 2020 2020 2020 2020 6665 6174 7572 6573          features
+000227e0: 3a20 4461 7461 4672 616d 652c 2052 4444  : DataFrame, RDD
+000227f0: 2c20 4e64 6172 7261 792c 206c 6973 742e  , Ndarray, list.
+00022800: 2046 6561 7475 7265 7320 746f 2062 6520   Features to be 
+00022810: 7361 7665 642e 0a20 2020 2020 2020 2020  saved..         
+00022820: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
+00022830: 3a20 4164 6469 7469 6f6e 616c 2077 7269  : Additional wri
+00022840: 7465 206f 7074 696f 6e73 2061 7320 6b65  te options as ke
+00022850: 792d 7661 6c75 6520 7061 6972 732c 2064  y-value pairs, d
+00022860: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
+00022870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022880: 2057 6865 6e20 7573 696e 6720 7468 6520   When using the 
+00022890: 6070 7974 686f 6e60 2065 6e67 696e 652c  `python` engine,
+000228a0: 2077 7269 7465 5f6f 7074 696f 6e73 2063   write_options c
+000228b0: 616e 2063 6f6e 7461 696e 2074 6865 0a20  an contain the. 
+000228c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000228d0: 6f6c 6c6f 7769 6e67 2065 6e74 7269 6573  ollowing entries
+000228e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000228f0: 2020 2a20 6b65 7920 606b 6166 6b61 5f70    * key `kafka_p
+00022900: 726f 6475 6365 725f 636f 6e66 6967 6020  roducer_config` 
+00022910: 616e 6420 7661 6c75 6520 616e 206f 626a  and value an obj
+00022920: 6563 7420 6f66 2074 7970 6520 5b70 726f  ect of type [pro
+00022930: 7065 7274 6965 735d 2868 7474 7073 3a2f  perties](https:/
+00022940: 2f64 6f63 732e 636f 6e66 6c75 656e 742e  /docs.confluent.
+00022950: 696f 2f70 6c61 7466 6f72 6d2f 6375 7272  io/platform/curr
+00022960: 656e 742f 636c 6965 6e74 732f 6c69 6272  ent/clients/libr
+00022970: 646b 6166 6b61 2f68 746d 6c2f 6d64 5f43  dkafka/html/md_C
+00022980: 4f4e 4649 4755 5241 5449 4f4e 2e68 746d  ONFIGURATION.htm
+00022990: 6c6e 290a 2020 2020 2020 2020 2020 2020  ln).            
+000229a0: 2020 2020 2020 7573 6564 2074 6f20 636f        used to co
+000229b0: 6e66 6967 7572 6520 7468 6520 4b61 666b  nfigure the Kafk
+000229c0: 6120 636c 6965 6e74 2e20 546f 206f 7074  a client. To opt
+000229d0: 696d 697a 6520 666f 7220 7468 726f 7567  imize for throug
+000229e0: 6870 7574 2069 6e20 6869 6768 206c 6174  hput in high lat
+000229f0: 656e 6379 2063 6f6e 6e65 6374 696f 6e20  ency connection 
+00022a00: 636f 6e73 6964 6572 0a20 2020 2020 2020  consider.       
+00022a10: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
+00022a20: 696e 6720 5b70 726f 6475 6365 7220 7072  ing [producer pr
+00022a30: 6f70 6572 7469 6573 5d28 6874 7470 733a  operties](https:
+00022a40: 2f2f 646f 6373 2e63 6f6e 666c 7565 6e74  //docs.confluent
+00022a50: 2e69 6f2f 636c 6f75 642f 6375 7272 656e  .io/cloud/curren
+00022a60: 742f 636c 6965 6e74 2d61 7070 732f 6f70  t/client-apps/op
+00022a70: 7469 6d69 7a69 6e67 2f74 6872 6f75 6768  timizing/through
+00022a80: 7075 742e 6874 6d6c 2370 726f 6475 6365  put.html#produce
+00022a90: 7229 2e0a 2020 2020 2020 2020 2020 2020  r)..            
+00022aa0: 2020 2020 2a20 6b65 7920 6069 6e74 6572      * key `inter
+00022ab0: 6e61 6c5f 6b61 666b 6160 2061 6e64 2076  nal_kafka` and v
+00022ac0: 616c 7565 2060 5472 7565 6020 6f72 2060  alue `True` or `
+00022ad0: 4661 6c73 6560 2069 6e20 6361 7365 2079  False` in case y
+00022ae0: 6f75 2065 7374 6162 6c69 7368 6564 0a20  ou established. 
+00022af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b00: 2063 6f6e 6e65 6374 6976 6974 7920 6672   connectivity fr
+00022b10: 6f6d 2079 6f75 2050 7974 686f 6e20 656e  om you Python en
+00022b20: 7669 726f 6e6d 656e 7420 746f 2074 6865  vironment to the
+00022b30: 2069 6e74 6572 6e61 6c20 6164 7665 7274   internal advert
+00022b40: 6973 6564 0a20 2020 2020 2020 2020 2020  ised.           
+00022b50: 2020 2020 2020 206c 6973 7465 6e65 7273         listeners
+00022b60: 206f 6620 7468 6520 486f 7073 776f 726b   of the Hopswork
+00022b70: 7320 4b61 666b 6120 436c 7573 7465 722e  s Kafka Cluster.
+00022b80: 2044 6566 6175 6c74 7320 746f 2060 4661   Defaults to `Fa
+00022b90: 6c73 6560 2061 6e64 0a20 2020 2020 2020  lse` and.       
+00022ba0: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
+00022bb0: 7573 6520 6578 7465 726e 616c 206c 6973  use external lis
+00022bc0: 7465 6e65 7273 2077 6865 6e20 636f 6e6e  teners when conn
+00022bd0: 6563 7469 6e67 2066 726f 6d20 6f75 7473  ecting from outs
+00022be0: 6964 6520 6f66 2048 6f70 7377 6f72 6b73  ide of Hopsworks
+00022bf0: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00022c00: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
+00022c10: 3a20 4164 6469 7469 6f6e 616c 2076 616c  : Additional val
+00022c20: 6964 6174 696f 6e20 6f70 7469 6f6e 7320  idation options 
+00022c30: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
+00022c40: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
+00022c50: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
+00022c60: 2020 2020 2020 2a20 6b65 7920 6072 756e        * key `run
+00022c70: 5f76 616c 6964 6174 696f 6e60 2062 6f6f  _validation` boo
+00022c80: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
+00022c90: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
+00022ca0: 6970 2076 616c 6964 6174 696f 6e20 7465  ip validation te
+00022cb0: 6d70 6f72 6172 696c 7920 6f6e 2069 6e67  mporarily on ing
+00022cc0: 6573 7469 6f6e 2e0a 2020 2020 2020 2020  estion..        
+00022cd0: 2020 2020 2020 2020 2a20 6b65 7920 6073          * key `s
+00022ce0: 6176 655f 7265 706f 7274 6020 626f 6f6c  ave_report` bool
+00022cf0: 6561 6e20 7661 6c75 652c 2073 6574 2074  ean value, set t
+00022d00: 6f20 6046 616c 7365 6020 746f 2073 6b69  o `False` to ski
+00022d10: 7020 7570 6c6f 6164 206f 6620 7468 6520  p upload of the 
+00022d20: 7661 6c69 6461 7469 6f6e 2072 6570 6f72  validation repor
+00022d30: 7420 746f 2048 6f70 7377 6f72 6b73 2e0a  t to Hopsworks..
+00022d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022d50: 2a20 6b65 7920 6067 655f 7661 6c69 6461  * key `ge_valida
+00022d60: 7465 5f6b 7761 7267 7360 2061 2064 6963  te_kwargs` a dic
+00022d70: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+00022d80: 6e67 206b 7761 7267 7320 666f 7220 7468  ng kwargs for th
+00022d90: 6520 7661 6c69 6461 7465 206d 6574 686f  e validate metho
+00022da0: 6420 6f66 2047 7265 6174 2045 7870 6563  d of Great Expec
+00022db0: 7461 7469 6f6e 732e 0a20 2020 2020 2020  tations..       
+00022dc0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
+00022dd0: 6665 7463 685f 6578 7065 6374 6174 696f  fetch_expectatio
+00022de0: 6e5f 7375 6974 6560 2061 2062 6f6f 6c65  n_suite` a boole
+00022df0: 616e 2076 616c 7565 2c20 6279 2064 6566  an value, by def
+00022e00: 6175 6c74 2060 5472 7565 602c 2074 6f20  ault `True`, to 
+00022e10: 636f 6e74 726f 6c20 7768 6574 6865 7220  control whether 
+00022e20: 7468 6520 6578 7065 6374 6174 696f 6e0a  the expectation.
+00022e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022e40: 2020 2073 7569 7465 206f 6620 7468 6520     suite of the 
+00022e50: 6665 6174 7572 6520 6772 6f75 7020 7368  feature group sh
+00022e60: 6f75 6c64 2062 6520 6665 7463 6865 6420  ould be fetched 
+00022e70: 6265 666f 7265 2065 7665 7279 2069 6e73  before every ins
+00022e80: 6572 742e 0a20 2020 2020 2020 2020 2020  ert..           
+00022e90: 2073 6176 655f 636f 6465 3a20 5768 656e   save_code: When
+00022ea0: 2072 756e 6e69 6e67 2048 5346 5320 6f6e   running HSFS on
+00022eb0: 2048 6f70 7377 6f72 6b73 206f 7220 4461   Hopsworks or Da
+00022ec0: 7461 6272 6963 6b73 2c20 4853 4653 2063  tabricks, HSFS c
+00022ed0: 616e 2073 6176 6520 7468 6520 636f 6465  an save the code
+00022ee0: 2f6e 6f74 6562 6f6f 6b20 7573 6564 2074  /notebook used t
+00022ef0: 6f20 6372 6561 7465 0a20 2020 2020 2020  o create.       
+00022f00: 2020 2020 2020 2020 2074 6865 2066 6561           the fea
+00022f10: 7475 7265 2067 726f 7570 206f 7220 7573  ture group or us
+00022f20: 6564 2074 6f20 696e 7365 7274 2064 6174  ed to insert dat
+00022f30: 6120 746f 2069 742e 2057 6865 6e20 6361  a to it. When ca
+00022f40: 6c6c 696e 6720 7468 6520 6069 6e73 6572  lling the `inser
+00022f50: 7460 206d 6574 686f 6420 7265 7065 6174  t` method repeat
+00022f60: 6564 6c79 0a20 2020 2020 2020 2020 2020  edly.           
+00022f70: 2020 2020 2077 6974 6820 736d 616c 6c20       with small 
+00022f80: 6261 7463 6865 7320 6f66 2064 6174 612c  batches of data,
+00022f90: 2074 6869 7320 6361 6e20 736c 6f77 2064   this can slow d
+00022fa0: 6f77 6e20 7468 6520 7772 6974 6573 2e20  own the writes. 
+00022fb0: 5573 6520 7468 6973 206f 7074 696f 6e20  Use this option 
+00022fc0: 746f 2074 7572 6e20 6f66 6620 7361 7669  to turn off savi
+00022fd0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00022fe0: 2020 2063 6f64 652e 2044 6566 6175 6c74     code. Default
+00022ff0: 7320 746f 2060 5472 7565 602e 0a0a 2020  s to `True`...  
+00023000: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+00023010: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+00023020: 6528 604a 6f62 602c 2060 5661 6c69 6461  e(`Job`, `Valida
+00023030: 7469 6f6e 5265 706f 7274 6029 2054 6865  tionReport`) The
+00023040: 2076 616c 6964 6174 696f 6e20 7265 706f   validation repo
+00023050: 7274 2069 6620 7661 6c69 6461 7469 6f6e  rt if validation
+00023060: 2069 7320 656e 6162 6c65 642e 0a0a 2020   is enabled...  
+00023070: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
+00023080: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
+00023090: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
+000230a0: 6e73 2e52 6573 7441 5049 4572 726f 7260  ns.RestAPIError`
+000230b0: 2e20 652e 6720 6661 696c 2074 6f20 6372  . e.g fail to cr
+000230c0: 6561 7465 2066 6561 7475 7265 2067 726f  eate feature gro
+000230d0: 7570 2c20 6461 7461 6672 616d 6520 7363  up, dataframe sc
+000230e0: 6865 6d61 2064 6f65 7320 6e6f 7420 6d61  hema does not ma
+000230f0: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
+00023100: 2020 2020 6578 6973 7469 6e67 2066 6561      existing fea
+00023110: 7475 7265 2067 726f 7570 2073 6368 656d  ture group schem
+00023120: 612c 2065 7463 2e0a 2020 2020 2020 2020  a, etc..        
+00023130: 2020 2020 6068 7366 732e 636c 6965 6e74      `hsfs.client
+00023140: 2e65 7863 6570 7469 6f6e 732e 4461 7461  .exceptions.Data
+00023150: 5661 6c69 6461 7469 6f6e 4578 6365 7074  ValidationExcept
+00023160: 696f 6e60 2e20 4966 2064 6174 6120 7661  ion`. If data va
+00023170: 6c69 6461 7469 6f6e 2066 6169 6c73 2061  lidation fails a
+00023180: 6e64 2074 6865 2065 7870 6563 7461 7469  nd the expectati
+00023190: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+000231a0: 2020 2073 7569 7465 2060 7661 6c69 6461     suite `valida
+000231b0: 7469 6f6e 5f69 6e67 6573 7469 6f6e 5f70  tion_ingestion_p
+000231c0: 6f6c 6963 7960 2069 7320 7365 7420 746f  olicy` is set to
+000231d0: 2060 5354 5249 4354 602e 2044 6174 6120   `STRICT`. Data 
+000231e0: 6973 204e 4f54 2069 6e67 6573 7465 642e  is NOT ingested.
+000231f0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00023200: 2020 2020 2020 6665 6174 7572 655f 6461        feature_da
+00023210: 7461 6672 616d 6520 3d20 656e 6769 6e65  taframe = engine
+00023220: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
+00023230: 636f 6e76 6572 745f 746f 5f64 6566 6175  convert_to_defau
+00023240: 6c74 5f64 6174 6166 7261 6d65 2866 6561  lt_dataframe(fea
+00023250: 7475 7265 7329 0a0a 2020 2020 2020 2020  tures)..        
+00023260: 6966 2077 7269 7465 5f6f 7074 696f 6e73  if write_options
+00023270: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00023280: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
+00023290: 6f6e 7320 3d20 7b7d 0a20 2020 2020 2020  ons = {}.       
+000232a0: 2069 6620 2277 6169 745f 666f 725f 6a6f   if "wait_for_jo
+000232b0: 6222 206e 6f74 2069 6e20 7772 6974 655f  b" not in write_
+000232c0: 6f70 7469 6f6e 733a 0a20 2020 2020 2020  options:.       
+000232d0: 2020 2020 2077 7269 7465 5f6f 7074 696f       write_optio
+000232e0: 6e73 5b22 7761 6974 5f66 6f72 5f6a 6f62  ns["wait_for_job
+000232f0: 225d 203d 2077 6169 740a 0a20 2020 2020  "] = wait..     
+00023300: 2020 206a 6f62 2c20 6765 5f72 6570 6f72     job, ge_repor
+00023310: 7420 3d20 7365 6c66 2e5f 6665 6174 7572  t = self._featur
+00023320: 655f 6772 6f75 705f 656e 6769 6e65 2e69  e_group_engine.i
+00023330: 6e73 6572 7428 0a20 2020 2020 2020 2020  nsert(.         
+00023340: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00023350: 2020 2020 2066 6561 7475 7265 5f64 6174       feature_dat
+00023360: 6166 7261 6d65 3d66 6561 7475 7265 5f64  aframe=feature_d
+00023370: 6174 6166 7261 6d65 2c0a 2020 2020 2020  ataframe,.      
+00023380: 2020 2020 2020 7772 6974 655f 6f70 7469        write_opti
+00023390: 6f6e 733d 7772 6974 655f 6f70 7469 6f6e  ons=write_option
+000233a0: 732c 0a20 2020 2020 2020 2020 2020 2076  s,.            v
+000233b0: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
+000233c0: 733d 7b22 7361 7665 5f72 6570 6f72 7422  s={"save_report"
+000233d0: 3a20 5472 7565 2c20 2a2a 7661 6c69 6461  : True, **valida
+000233e0: 7469 6f6e 5f6f 7074 696f 6e73 7d2c 0a20  tion_options},. 
+000233f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00023400: 2020 6966 2073 6176 655f 636f 6465 2061    if save_code a
+00023410: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
+00023420: 2067 655f 7265 706f 7274 2069 7320 4e6f   ge_report is No
+00023430: 6e65 206f 7220 6765 5f72 6570 6f72 742e  ne or ge_report.
+00023440: 696e 6765 7374 696f 6e5f 7265 7375 6c74  ingestion_result
+00023450: 203d 3d20 2249 4e47 4553 5445 4422 0a20   == "INGESTED". 
+00023460: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00023470: 2020 2020 2020 7365 6c66 2e5f 636f 6465        self._code
+00023480: 5f65 6e67 696e 652e 7361 7665 5f63 6f64  _engine.save_cod
+00023490: 6528 7365 6c66 290a 0a20 2020 2020 2020  e(self)..       
+000234a0: 2069 6620 7365 6c66 2e73 7461 7469 7374   if self.statist
+000234b0: 6963 735f 636f 6e66 6967 2e65 6e61 626c  ics_config.enabl
+000234c0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+000234d0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+000234e0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000234f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023500: 2020 2020 2022 5374 6174 6973 7469 6373       "Statistics
+00023510: 2061 7265 206e 6f74 2063 6f6d 7075 7465   are not compute
+00023520: 6420 666f 7220 696e 7365 7274 696f 6e20  d for insertion 
+00023530: 746f 206f 6e6c 696e 6520 656e 6162 6c65  to online enable
+00023540: 6420 6578 7465 726e 616c 2066 6561 7475  d external featu
+00023550: 7265 2067 726f 7570 2060 7b7d 602c 2077  re group `{}`, w
+00023560: 6974 6820 7665 7273 696f 6e22 0a20 2020  ith version".   
+00023570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023580: 2022 2060 7b7d 602e 2043 616c 6c20 6063   " `{}`. Call `c
+00023590: 6f6d 7075 7465 5f73 7461 7469 7374 6963  ompute_statistic
+000235a0: 7360 2065 7870 6c69 6369 746c 7920 746f  s` explicitly to
+000235b0: 2063 6f6d 7075 7465 2073 7461 7469 7374   compute statist
+000235c0: 6963 7320 6f76 6572 2074 6865 2064 6174  ics over the dat
+000235d0: 6120 696e 2074 6865 2065 7874 6572 6e61  a in the externa
+000235e0: 6c20 7374 6f72 6167 6520 7379 7374 656d  l storage system
+000235f0: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+00023600: 2020 2029 2e66 6f72 6d61 7428 7365 6c66     ).format(self
+00023610: 2e5f 6e61 6d65 2c20 7365 6c66 2e5f 7665  ._name, self._ve
+00023620: 7273 696f 6e29 2c0a 2020 2020 2020 2020  rsion),.        
+00023630: 2020 2020 2020 2020 7574 696c 2e53 746f          util.Sto
+00023640: 7261 6765 5761 726e 696e 672c 0a20 2020  rageWarning,.   
+00023650: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00023660: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+00023670: 2020 2020 2020 2020 206a 6f62 2c0a 2020           job,.  
+00023680: 2020 2020 2020 2020 2020 6765 5f72 6570            ge_rep
+00023690: 6f72 742e 746f 5f67 655f 7479 7065 2829  ort.to_ge_type()
+000236a0: 2069 6620 6765 5f72 6570 6f72 7420 6973   if ge_report is
+000236b0: 206e 6f74 204e 6f6e 6520 656c 7365 204e   not None else N
+000236c0: 6f6e 652c 0a20 2020 2020 2020 2029 0a0a  one,.        )..
+000236d0: 2020 2020 6465 6620 7265 6164 280a 2020      def read(.  
+000236e0: 2020 2020 2020 7365 6c66 2c20 6461 7461        self, data
+000236f0: 6672 616d 655f 7479 7065 3a20 4f70 7469  frame_type: Opti
+00023700: 6f6e 616c 5b73 7472 5d20 3d20 2264 6566  onal[str] = "def
+00023710: 6175 6c74 222c 206f 6e6c 696e 653a 204f  ault", online: O
+00023720: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00023730: 4661 6c73 650a 2020 2020 293a 0a20 2020  False.    ):.   
+00023740: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
+00023750: 6665 6174 7572 6520 6772 6f75 7020 6173  feature group as
+00023760: 2061 2044 6174 6146 7261 6d65 2e0a 0a20   a DataFrame... 
+00023770: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
+00023780: 6c65 0a20 2020 2020 2020 2020 2020 2060  le.            `
+00023790: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
+000237a0: 2020 2020 2023 2063 6f6e 6e65 6374 2074       # connect t
+000237b0: 6f20 7468 6520 4665 6174 7572 6520 5374  o the Feature St
+000237c0: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
+000237d0: 6673 203d 202e 2e2e 0a0a 2020 2020 2020  fs = .....      
+000237e0: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
+000237f0: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
+00023800: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
+00023810: 2020 2066 6720 3d20 6673 2e67 6574 5f6f     fg = fs.get_o
+00023820: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
+00023830: 5f67 726f 7570 282e 2e2e 290a 0a20 2020  _group(...)..   
+00023840: 2020 2020 2020 2020 2064 6620 3d20 6667           df = fg
+00023850: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
+00023860: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+00023870: 2021 2121 2077 6172 6e69 6e67 2022 456e   !!! warning "En
+00023880: 6769 6e65 2053 7570 706f 7274 220a 2020  gine Support".  
+00023890: 2020 2020 2020 2020 2020 2a2a 5370 6172            **Spar
+000238a0: 6b20 6f6e 6c79 2a2a 0a0a 2020 2020 2020  k only**..      
+000238b0: 2020 2020 2020 5265 6164 696e 6720 616e        Reading an
+000238c0: 2045 7874 6572 6e61 6c20 4665 6174 7572   External Featur
+000238d0: 6520 4772 6f75 7020 6469 7265 6374 6c79  e Group directly
+000238e0: 2069 6e74 6f20 6120 5061 6e64 6173 2044   into a Pandas D
+000238f0: 6174 6166 7261 6d65 2075 7369 6e67 0a20  ataframe using. 
+00023900: 2020 2020 2020 2020 2020 2050 7974 686f             Pytho
+00023910: 6e2f 5061 6e64 6173 2061 7320 456e 6769  n/Pandas as Engi
+00023920: 6e65 2069 7320 6e6f 7420 7375 7070 6f72  ne is not suppor
+00023930: 7465 642c 2068 6f77 6576 6572 2c20 796f  ted, however, yo
+00023940: 7520 6361 6e20 7573 6520 7468 650a 2020  u can use the.  
+00023950: 2020 2020 2020 2020 2020 5175 6572 7920            Query 
+00023960: 4150 4920 746f 2063 7265 6174 6520 4665  API to create Fe
+00023970: 6174 7572 6520 5669 6577 732f 5472 6169  ature Views/Trai
+00023980: 6e69 6e67 2044 6174 6120 636f 6e74 6169  ning Data contai
+00023990: 6e69 6e67 2045 7874 6572 6e61 6c0a 2020  ning External.  
+000239a0: 2020 2020 2020 2020 2020 4665 6174 7572            Featur
+000239b0: 6520 4772 6f75 7073 2e0a 0a20 2020 2020  e Groups...     
+000239c0: 2020 2023 2041 7267 756d 656e 7473 0a20     # Arguments. 
+000239d0: 2020 2020 2020 2020 2020 2064 6174 6166             dataf
+000239e0: 7261 6d65 5f74 7970 653a 2073 7472 2c20  rame_type: str, 
+000239f0: 6f70 7469 6f6e 616c 2e20 506f 7373 6962  optional. Possib
+00023a00: 6c65 2076 616c 7565 7320 6172 6520 6022  le values are `"
+00023a10: 6465 6661 756c 7422 602c 2060 2273 7061  default"`, `"spa
+00023a20: 726b 2260 2c0a 2020 2020 2020 2020 2020  rk"`,.          
+00023a30: 2020 2020 2020 6022 7061 6e64 6173 2260        `"pandas"`
+00023a40: 2c20 6022 6e75 6d70 7922 6020 6f72 2060  , `"numpy"` or `
+00023a50: 2270 7974 686f 6e22 602c 2064 6566 6175  "python"`, defau
+00023a60: 6c74 7320 746f 2060 2264 6566 6175 6c74  lts to `"default
+00023a70: 2260 2e0a 2020 2020 2020 2020 2020 2020  "`..            
+00023a80: 6f6e 6c69 6e65 3a20 626f 6f6c 2c20 6f70  online: bool, op
+00023a90: 7469 6f6e 616c 2e20 4966 2060 5472 7565  tional. If `True
+00023aa0: 6020 7265 6164 2066 726f 6d20 6f6e 6c69  ` read from onli
+00023ab0: 6e65 2066 6561 7475 7265 2073 746f 7265  ne feature store
+00023ac0: 2c20 6465 6661 756c 7473 0a20 2020 2020  , defaults.     
+00023ad0: 2020 2020 2020 2020 2020 2074 6f20 6046             to `F
+00023ae0: 616c 7365 602e 0a0a 2020 2020 2020 2020  alse`...        
+00023af0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
+00023b00: 2020 2020 2020 6044 6174 6146 7261 6d65        `DataFrame
+00023b10: 603a 2054 6865 2073 7061 726b 2064 6174  `: The spark dat
+00023b20: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
+00023b30: 6720 7468 6520 6665 6174 7572 6520 6461  g the feature da
+00023b40: 7461 2e0a 2020 2020 2020 2020 2020 2020  ta..            
+00023b50: 6070 7973 7061 726b 2e44 6174 6146 7261  `pyspark.DataFra
+00023b60: 6d65 602e 2041 2053 7061 726b 2044 6174  me`. A Spark Dat
+00023b70: 6146 7261 6d65 2e0a 2020 2020 2020 2020  aFrame..        
+00023b80: 2020 2020 6070 616e 6461 732e 4461 7461      `pandas.Data
+00023b90: 4672 616d 6560 2e20 4120 5061 6e64 6173  Frame`. A Pandas
+00023ba0: 2044 6174 6146 7261 6d65 2e0a 2020 2020   DataFrame..    
+00023bb0: 2020 2020 2020 2020 606e 756d 7079 2e6e          `numpy.n
+00023bc0: 6461 7272 6179 602e 2041 2074 776f 2d64  darray`. A two-d
+00023bd0: 696d 656e 7369 6f6e 616c 204e 756d 7079  imensional Numpy
+00023be0: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+00023bf0: 2020 2020 606c 6973 7460 2e20 4120 7477      `list`. A tw
+00023c00: 6f2d 6469 6d65 6e73 696f 6e61 6c20 5079  o-dimensional Py
+00023c10: 7468 6f6e 206c 6973 742e 0a0a 2020 2020  thon list...    
+00023c20: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
+00023c30: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
+00023c40: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
+00023c50: 2e52 6573 7441 5049 4572 726f 7260 2e0a  .RestAPIError`..
+00023c60: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00023c70: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00023c80: 2020 2020 2020 656e 6769 6e65 2e67 6574        engine.get
+00023c90: 5f74 7970 6528 2920 3d3d 2022 7079 7468  _type() == "pyth
+00023ca0: 6f6e 220a 2020 2020 2020 2020 2020 2020  on".            
+00023cb0: 616e 6420 6e6f 7420 6f6e 6c69 6e65 0a20  and not online. 
+00023cc0: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
+00023cd0: 6f74 2065 6e67 696e 652e 6765 745f 696e  ot engine.get_in
+00023ce0: 7374 616e 6365 2829 2e69 735f 666c 7969  stance().is_flyi
+00023cf0: 6e67 6475 636b 5f71 7565 7279 5f73 7570  ngduck_query_sup
+00023d00: 706f 7274 6564 280a 2020 2020 2020 2020  ported(.        
+00023d10: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
+00023d20: 6563 745f 616c 6c28 290a 2020 2020 2020  ect_all().      
+00023d30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00023d40: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00023d50: 6169 7365 2046 6561 7475 7265 5374 6f72  aise FeatureStor
+00023d60: 6545 7863 6570 7469 6f6e 280a 2020 2020  eException(.    
+00023d70: 2020 2020 2020 2020 2020 2020 2252 6561              "Rea
+00023d80: 6469 6e67 2061 6e20 4578 7465 726e 616c  ding an External
+00023d90: 2046 6561 7475 7265 2047 726f 7570 2064   Feature Group d
+00023da0: 6972 6563 746c 7920 696e 746f 2061 2050  irectly into a P
+00023db0: 616e 6461 7320 4461 7461 6672 616d 6520  andas Dataframe 
+00023dc0: 7573 696e 6720 220a 2020 2020 2020 2020  using ".        
+00023dd0: 2020 2020 2020 2020 2b20 2250 7974 686f          + "Pytho
+00023de0: 6e2f 5061 6e64 6173 2061 7320 456e 6769  n/Pandas as Engi
+00023df0: 6e65 2066 726f 6d20 7468 6520 6578 7465  ne from the exte
+00023e00: 726e 616c 2073 746f 7261 6765 2073 7973  rnal storage sys
+00023e10: 7465 6d20 220a 2020 2020 2020 2020 2020  tem ".          
+00023e20: 2020 2020 2020 2b20 2269 7320 6e6f 7420        + "is not 
+00023e30: 7375 7070 6f72 7465 642c 2068 6f77 6576  supported, howev
+00023e40: 6572 2c20 6966 2074 6865 2066 6561 7475  er, if the featu
+00023e50: 7265 2067 726f 7570 2069 7320 6f6e 6c69  re group is onli
+00023e60: 6e65 2065 6e61 626c 6564 2c20 796f 7520  ne enabled, you 
+00023e70: 6361 6e20 7265 6164 2022 0a20 2020 2020  can read ".     
+00023e80: 2020 2020 2020 2020 2020 202b 2022 6672             + "fr
+00023e90: 6f6d 206f 6e6c 696e 6520 7374 6f72 6167  om online storag
+00023ea0: 6520 6f72 2079 6f75 2063 616e 2075 7365  e or you can use
+00023eb0: 2074 6865 2022 0a20 2020 2020 2020 2020   the ".         
+00023ec0: 2020 2020 2020 202b 2022 5175 6572 7920         + "Query 
+00023ed0: 4150 4920 746f 2063 7265 6174 6520 4665  API to create Fe
+00023ee0: 6174 7572 6520 5669 6577 732f 5472 6169  ature Views/Trai
+00023ef0: 6e69 6e67 2044 6174 6120 636f 6e74 6169  ning Data contai
+00023f00: 6e69 6e67 2045 7874 6572 6e61 6c20 220a  ning External ".
+00023f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023f20: 2b20 2246 6561 7475 7265 2047 726f 7570  + "Feature Group
+00023f30: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
+00023f40: 290a 2020 2020 2020 2020 656e 6769 6e65  ).        engine
+00023f50: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
+00023f60: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
+00023f70: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
+00023f80: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
+00023f90: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
+00023fa0: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
+00023fb0: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
+00023fc0: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
+00023fd0: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
+00023fe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00023ff0: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
+00024000: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
+00024010: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
+00024020: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00024030: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00024040: 7365 6c65 6374 5f61 6c6c 2829 2e72 6561  select_all().rea
+00024050: 6428 6461 7461 6672 616d 655f 7479 7065  d(dataframe_type
+00024060: 3d64 6174 6166 7261 6d65 5f74 7970 652c  =dataframe_type,
+00024070: 206f 6e6c 696e 653d 6f6e 6c69 6e65 290a   online=online).
+00024080: 0a20 2020 2064 6566 2073 686f 7728 7365  .    def show(se
+00024090: 6c66 2c20 6e29 3a0a 2020 2020 2020 2020  lf, n):.        
+000240a0: 2222 2253 686f 7720 7468 6520 6669 7273  """Show the firs
+000240b0: 7420 6e20 726f 7773 206f 6620 7468 6520  t n rows of the 
+000240c0: 6665 6174 7572 6520 6772 6f75 702e 0a0a  feature group...
+000240d0: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
+000240e0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+000240f0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00024100: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
+00024110: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
+00024120: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
+00024130: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
+00024140: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+00024150: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
+00024160: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
+00024170: 2020 2020 6667 203d 2066 732e 6765 745f      fg = fs.get_
+00024180: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+00024190: 655f 6772 6f75 7028 2e2e 2e29 0a0a 2020  e_group(...)..  
+000241a0: 2020 2020 2020 2020 2020 6667 2e73 686f            fg.sho
+000241b0: 7728 3529 0a20 2020 2020 2020 2020 2020  w(5).           
+000241c0: 2060 6060 0a20 2020 2020 2020 2022 2222   ```.        """
+000241d0: 0a20 2020 2020 2020 2065 6e67 696e 652e  .        engine.
+000241e0: 6765 745f 696e 7374 616e 6365 2829 2e73  get_instance().s
+000241f0: 6574 5f6a 6f62 5f67 726f 7570 280a 2020  et_job_group(.  
+00024200: 2020 2020 2020 2020 2020 2246 6574 6368            "Fetch
+00024210: 696e 6720 4665 6174 7572 6520 6772 6f75  ing Feature grou
+00024220: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
+00024230: 2247 6574 7469 6e67 2066 6561 7475 7265  "Getting feature
+00024240: 2067 726f 7570 3a20 7b7d 2066 726f 6d20   group: {} from 
+00024250: 7468 6520 6665 6174 7572 6573 746f 7265  the featurestore
+00024260: 207b 7d22 2e66 6f72 6d61 7428 0a20 2020   {}".format(.   
+00024270: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00024280: 662e 5f6e 616d 652c 2073 656c 662e 5f66  f._name, self._f
+00024290: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
+000242a0: 650a 2020 2020 2020 2020 2020 2020 292c  e.            ),
+000242b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000242c0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+000242d0: 656c 6563 745f 616c 6c28 292e 7368 6f77  elect_all().show
+000242e0: 286e 290a 0a20 2020 2040 636c 6173 736d  (n)..    @classm
+000242f0: 6574 686f 640a 2020 2020 6465 6620 6672  ethod.    def fr
+00024300: 6f6d 5f72 6573 706f 6e73 655f 6a73 6f6e  om_response_json
+00024310: 2863 6c73 2c20 6a73 6f6e 5f64 6963 7429  (cls, json_dict)
+00024320: 3a0a 2020 2020 2020 2020 6a73 6f6e 5f64  :.        json_d
+00024330: 6563 616d 656c 697a 6564 203d 2068 756d  ecamelized = hum
+00024340: 7073 2e64 6563 616d 656c 697a 6528 6a73  ps.decamelize(js
+00024350: 6f6e 5f64 6963 7429 0a20 2020 2020 2020  on_dict).       
+00024360: 2069 6620 6973 696e 7374 616e 6365 286a   if isinstance(j
+00024370: 736f 6e5f 6465 6361 6d65 6c69 7a65 642c  son_decamelized,
+00024380: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00024390: 2020 2020 5f20 3d20 6a73 6f6e 5f64 6563      _ = json_dec
+000243a0: 616d 656c 697a 6564 2e70 6f70 2822 7479  amelized.pop("ty
+000243b0: 7065 222c 204e 6f6e 6529 0a20 2020 2020  pe", None).     
+000243c0: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
+000243d0: 7328 2a2a 6a73 6f6e 5f64 6563 616d 656c  s(**json_decamel
+000243e0: 697a 6564 290a 2020 2020 2020 2020 666f  ized).        fo
+000243f0: 7220 6667 2069 6e20 6a73 6f6e 5f64 6563  r fg in json_dec
+00024400: 616d 656c 697a 6564 3a0a 2020 2020 2020  amelized:.      
+00024410: 2020 2020 2020 5f20 3d20 6667 2e70 6f70        _ = fg.pop
+00024420: 2822 7479 7065 222c 204e 6f6e 6529 0a20  ("type", None). 
+00024430: 2020 2020 2020 2072 6574 7572 6e20 5b63         return [c
+00024440: 6c73 282a 2a66 6729 2066 6f72 2066 6720  ls(**fg) for fg 
+00024450: 696e 206a 736f 6e5f 6465 6361 6d65 6c69  in json_decameli
+00024460: 7a65 645d 0a0a 2020 2020 6465 6620 7570  zed]..    def up
+00024470: 6461 7465 5f66 726f 6d5f 7265 7370 6f6e  date_from_respon
+00024480: 7365 5f6a 736f 6e28 7365 6c66 2c20 6a73  se_json(self, js
+00024490: 6f6e 5f64 6963 7429 3a0a 2020 2020 2020  on_dict):.      
+000244a0: 2020 6a73 6f6e 5f64 6563 616d 656c 697a    json_decameliz
+000244b0: 6564 203d 2068 756d 7073 2e64 6563 616d  ed = humps.decam
+000244c0: 656c 697a 6528 6a73 6f6e 5f64 6963 7429  elize(json_dict)
+000244d0: 0a20 2020 2020 2020 2069 6620 2274 7970  .        if "typ
+000244e0: 6522 2069 6e20 6a73 6f6e 5f64 6563 616d  e" in json_decam
+000244f0: 656c 697a 6564 3a0a 2020 2020 2020 2020  elized:.        
+00024500: 2020 2020 5f20 3d20 6a73 6f6e 5f64 6563      _ = json_dec
+00024510: 616d 656c 697a 6564 2e70 6f70 2822 7479  amelized.pop("ty
+00024520: 7065 2229 0a20 2020 2020 2020 2073 656c  pe").        sel
+00024530: 662e 5f5f 696e 6974 5f5f 282a 2a6a 736f  f.__init__(**jso
+00024540: 6e5f 6465 6361 6d65 6c69 7a65 6429 0a20  n_decamelized). 
+00024550: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00024560: 6c66 0a0a 2020 2020 6465 6620 6a73 6f6e  lf..    def json
+00024570: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00024580: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
+00024590: 7328 7365 6c66 2c20 636c 733d 7574 696c  s(self, cls=util
+000245a0: 2e46 6561 7475 7265 5374 6f72 6545 6e63  .FeatureStoreEnc
+000245b0: 6f64 6572 290a 0a20 2020 2064 6566 2074  oder)..    def t
+000245c0: 6f5f 6469 6374 2873 656c 6629 3a0a 2020  o_dict(self):.  
+000245d0: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+000245e0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+000245f0: 2073 656c 662e 5f69 642c 0a20 2020 2020   self._id,.     
+00024600: 2020 2020 2020 2022 6e61 6d65 223a 2073         "name": s
+00024610: 656c 662e 5f6e 616d 652c 0a20 2020 2020  elf._name,.     
+00024620: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00024630: 696f 6e22 3a20 7365 6c66 2e5f 6465 7363  ion": self._desc
+00024640: 7269 7074 696f 6e2c 0a20 2020 2020 2020  ription,.       
+00024650: 2020 2020 2022 7665 7273 696f 6e22 3a20       "version": 
+00024660: 7365 6c66 2e5f 7665 7273 696f 6e2c 0a20  self._version,. 
+00024670: 2020 2020 2020 2020 2020 2022 6665 6174             "feat
+00024680: 7572 6573 223a 2073 656c 662e 5f66 6561  ures": self._fea
+00024690: 7475 7265 732c 0a20 2020 2020 2020 2020  tures,.         
+000246a0: 2020 2022 6665 6174 7572 6573 746f 7265     "featurestore
+000246b0: 4964 223a 2073 656c 662e 5f66 6561 7475  Id": self._featu
+000246c0: 7265 5f73 746f 7265 5f69 642c 0a20 2020  re_store_id,.   
+000246d0: 2020 2020 2020 2020 2022 7175 6572 7922           "query"
+000246e0: 3a20 7365 6c66 2e5f 7175 6572 792c 0a20  : self._query,. 
+000246f0: 2020 2020 2020 2020 2020 2022 6461 7461             "data
+00024700: 466f 726d 6174 223a 2073 656c 662e 5f64  Format": self._d
+00024710: 6174 615f 666f 726d 6174 2c0a 2020 2020  ata_format,.    
+00024720: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
+00024730: 7365 6c66 2e5f 7061 7468 2c0a 2020 2020  self._path,.    
+00024740: 2020 2020 2020 2020 226f 7074 696f 6e73          "options
+00024750: 223a 205b 7b22 6e61 6d65 223a 206b 2c20  ": [{"name": k, 
+00024760: 2276 616c 7565 223a 2076 7d20 666f 7220  "value": v} for 
+00024770: 6b2c 2076 2069 6e20 7365 6c66 2e5f 6f70  k, v in self._op
+00024780: 7469 6f6e 732e 6974 656d 7328 295d 0a20  tions.items()]. 
+00024790: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000247a0: 6c66 2e5f 6f70 7469 6f6e 730a 2020 2020  lf._options.    
+000247b0: 2020 2020 2020 2020 656c 7365 204e 6f6e          else Non
+000247c0: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+000247d0: 7374 6f72 6167 6543 6f6e 6e65 6374 6f72  storageConnector
+000247e0: 223a 2073 656c 662e 5f73 746f 7261 6765  ": self._storage
+000247f0: 5f63 6f6e 6e65 6374 6f72 2e74 6f5f 6469  _connector.to_di
+00024800: 6374 2829 2c0a 2020 2020 2020 2020 2020  ct(),.          
+00024810: 2020 2274 7970 6522 3a20 226f 6e44 656d    "type": "onDem
+00024820: 616e 6446 6561 7475 7265 6772 6f75 7044  andFeaturegroupD
+00024830: 544f 222c 0a20 2020 2020 2020 2020 2020  TO",.           
+00024840: 2022 7374 6174 6973 7469 6373 436f 6e66   "statisticsConf
+00024850: 6967 223a 2073 656c 662e 5f73 7461 7469  ig": self._stati
+00024860: 7374 6963 735f 636f 6e66 6967 2c0a 2020  stics_config,.  
+00024870: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00024880: 5469 6d65 223a 2073 656c 662e 5f65 7665  Time": self._eve
+00024890: 6e74 5f74 696d 652c 0a20 2020 2020 2020  nt_time,.       
+000248a0: 2020 2020 2022 6578 7065 6374 6174 696f       "expectatio
+000248b0: 6e53 7569 7465 223a 2073 656c 662e 5f65  nSuite": self._e
+000248c0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+000248d0: 2c0a 2020 2020 2020 2020 2020 2020 226f  ,.            "o
+000248e0: 6e6c 696e 6545 6e61 626c 6564 223a 2073  nlineEnabled": s
+000248f0: 656c 662e 5f6f 6e6c 696e 655f 656e 6162  elf._online_enab
+00024900: 6c65 642c 0a20 2020 2020 2020 2020 2020  led,.           
+00024910: 2022 7370 696e 6522 3a20 4661 6c73 652c   "spine": False,
+00024920: 0a20 2020 2020 2020 2020 2020 2022 746f  .            "to
+00024930: 7069 634e 616d 6522 3a20 7365 6c66 2e74  picName": self.t
+00024940: 6f70 6963 5f6e 616d 652c 0a20 2020 2020  opic_name,.     
+00024950: 2020 2020 2020 2022 6e6f 7469 6669 6361         "notifica
+00024960: 7469 6f6e 546f 7069 634e 616d 6522 3a20  tionTopicName": 
+00024970: 7365 6c66 2e6e 6f74 6966 6963 6174 696f  self.notificatio
+00024980: 6e5f 746f 7069 635f 6e61 6d65 2c0a 2020  n_topic_name,.  
+00024990: 2020 2020 2020 2020 2020 2264 6570 7265            "depre
+000249a0: 6361 7465 6422 3a20 7365 6c66 2e64 6570  cated": self.dep
+000249b0: 7265 6361 7465 642c 0a20 2020 2020 2020  recated,.       
+000249c0: 207d 0a0a 2020 2020 4070 726f 7065 7274   }..    @propert
+000249d0: 790a 2020 2020 6465 6620 6964 2873 656c  y.    def id(sel
+000249e0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+000249f0: 726e 2073 656c 662e 5f69 640a 0a20 2020  rn self._id..   
+00024a00: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00024a10: 6566 2064 6573 6372 6970 7469 6f6e 2873  ef description(s
+00024a20: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00024a30: 7475 726e 2073 656c 662e 5f64 6573 6372  turn self._descr
+00024a40: 6970 7469 6f6e 0a0a 2020 2020 4070 726f  iption..    @pro
+00024a50: 7065 7274 790a 2020 2020 6465 6620 7175  perty.    def qu
+00024a60: 6572 7928 7365 6c66 293a 0a20 2020 2020  ery(self):.     
+00024a70: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00024a80: 7175 6572 790a 0a20 2020 2040 7072 6f70  query..    @prop
+00024a90: 6572 7479 0a20 2020 2064 6566 2064 6174  erty.    def dat
+00024aa0: 615f 666f 726d 6174 2873 656c 6629 3a0a  a_format(self):.
+00024ab0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00024ac0: 656c 662e 5f64 6174 615f 666f 726d 6174  elf._data_format
+00024ad0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00024ae0: 2020 2020 6465 6620 7061 7468 2873 656c      def path(sel
+00024af0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00024b00: 726e 2073 656c 662e 5f70 6174 680a 0a20  rn self._path.. 
+00024b10: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00024b20: 2064 6566 206f 7074 696f 6e73 2873 656c   def options(sel
+00024b30: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00024b40: 726e 2073 656c 662e 5f6f 7074 696f 6e73  rn self._options
+00024b50: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00024b60: 2020 2020 6465 6620 7374 6f72 6167 655f      def storage_
+00024b70: 636f 6e6e 6563 746f 7228 7365 6c66 293a  connector(self):
+00024b80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00024b90: 7365 6c66 2e5f 7374 6f72 6167 655f 636f  self._storage_co
+00024ba0: 6e6e 6563 746f 720a 0a20 2020 2040 7072  nnector..    @pr
+00024bb0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00024bc0: 7265 6174 6f72 2873 656c 6629 3a0a 2020  reator(self):.  
+00024bd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00024be0: 662e 5f63 7265 6174 6f72 0a0a 2020 2020  f._creator..    
+00024bf0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00024c00: 6620 6372 6561 7465 6428 7365 6c66 293a  f created(self):
+00024c10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00024c20: 7365 6c66 2e5f 6372 6561 7465 640a 0a20  self._created.. 
+00024c30: 2020 2040 6465 7363 7269 7074 696f 6e2e     @description.
+00024c40: 7365 7474 6572 0a20 2020 2064 6566 2064  setter.    def d
+00024c50: 6573 6372 6970 7469 6f6e 2873 656c 662c  escription(self,
+00024c60: 206e 6577 5f64 6573 6372 6970 7469 6f6e   new_description
+00024c70: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00024c80: 5f64 6573 6372 6970 7469 6f6e 203d 206e  _description = n
+00024c90: 6577 5f64 6573 6372 6970 7469 6f6e 0a0a  ew_description..
+00024ca0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00024cb0: 2020 6465 6620 6665 6174 7572 655f 7374    def feature_st
+00024cc0: 6f72 655f 6e61 6d65 2873 656c 6629 3a0a  ore_name(self):.
+00024cd0: 2020 2020 2020 2020 2222 224e 616d 6520          """Name 
+00024ce0: 6f66 2074 6865 2066 6561 7475 7265 2073  of the feature s
+00024cf0: 746f 7265 2069 6e20 7768 6963 6820 7468  tore in which th
+00024d00: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
+00024d10: 6973 206c 6f63 6174 6564 2e22 2222 0a20  is located.""". 
+00024d20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00024d30: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
+00024d40: 655f 6e61 6d65 0a0a 0a63 6c61 7373 2053  e_name...class S
+00024d50: 7069 6e65 4772 6f75 7028 4665 6174 7572  pineGroup(Featur
+00024d60: 6547 726f 7570 4261 7365 293a 0a20 2020  eGroupBase):.   
+00024d70: 2053 5049 4e45 5f47 524f 5550 203d 2022   SPINE_GROUP = "
+00024d80: 4f4e 5f44 454d 414e 445f 4645 4154 5552  ON_DEMAND_FEATUR
+00024d90: 455f 4752 4f55 5022 0a20 2020 2045 4e54  E_GROUP".    ENT
+00024da0: 4954 595f 5459 5045 203d 2022 6665 6174  ITY_TYPE = "feat
+00024db0: 7572 6567 726f 7570 7322 0a0a 2020 2020  uregroups"..    
+00024dc0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00024dd0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00024de0: 2020 2020 7374 6f72 6167 655f 636f 6e6e      storage_conn
+00024df0: 6563 746f 723d 4e6f 6e65 2c0a 2020 2020  ector=None,.    
+00024e00: 2020 2020 7175 6572 793d 4e6f 6e65 2c0a      query=None,.
+00024e10: 2020 2020 2020 2020 6461 7461 5f66 6f72          data_for
+00024e20: 6d61 743d 4e6f 6e65 2c0a 2020 2020 2020  mat=None,.      
+00024e30: 2020 7061 7468 3d4e 6f6e 652c 0a20 2020    path=None,.   
+00024e40: 2020 2020 206f 7074 696f 6e73 3d7b 7d2c       options={},
+00024e50: 0a20 2020 2020 2020 206e 616d 653d 4e6f  .        name=No
+00024e60: 6e65 2c0a 2020 2020 2020 2020 7665 7273  ne,.        vers
+00024e70: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
+00024e80: 2020 6465 7363 7269 7074 696f 6e3d 4e6f    description=No
+00024e90: 6e65 2c0a 2020 2020 2020 2020 7072 696d  ne,.        prim
+00024ea0: 6172 795f 6b65 793d 4e6f 6e65 2c0a 2020  ary_key=None,.  
+00024eb0: 2020 2020 2020 6665 6174 7572 6573 746f        featuresto
+00024ec0: 7265 5f69 643d 4e6f 6e65 2c0a 2020 2020  re_id=None,.    
+00024ed0: 2020 2020 6665 6174 7572 6573 746f 7265      featurestore
+00024ee0: 5f6e 616d 653d 4e6f 6e65 2c0a 2020 2020  _name=None,.    
+00024ef0: 2020 2020 6372 6561 7465 643d 4e6f 6e65      created=None
+00024f00: 2c0a 2020 2020 2020 2020 6372 6561 746f  ,.        creato
+00024f10: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
+00024f20: 6964 3d4e 6f6e 652c 0a20 2020 2020 2020  id=None,.       
+00024f30: 2066 6561 7475 7265 733d 4e6f 6e65 2c0a   features=None,.
+00024f40: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
+00024f50: 3d4e 6f6e 652c 0a20 2020 2020 2020 2073  =None,.        s
+00024f60: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
+00024f70: 3d4e 6f6e 652c 0a20 2020 2020 2020 2065  =None,.        e
+00024f80: 7665 6e74 5f74 696d 653d 4e6f 6e65 2c0a  vent_time=None,.
+00024f90: 2020 2020 2020 2020 6578 7065 6374 6174          expectat
+00024fa0: 696f 6e5f 7375 6974 653d 4e6f 6e65 2c0a  ion_suite=None,.
+00024fb0: 2020 2020 2020 2020 6f6e 6c69 6e65 5f65          online_e
+00024fc0: 6e61 626c 6564 3d46 616c 7365 2c0a 2020  nabled=False,.  
+00024fd0: 2020 2020 2020 6872 6566 3d4e 6f6e 652c        href=None,
+00024fe0: 0a20 2020 2020 2020 206f 6e6c 696e 655f  .        online_
+00024ff0: 746f 7069 635f 6e61 6d65 3d4e 6f6e 652c  topic_name=None,
+00025000: 0a20 2020 2020 2020 2074 6f70 6963 5f6e  .        topic_n
+00025010: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
+00025020: 2020 7370 696e 653d 5472 7565 2c0a 2020    spine=True,.  
+00025030: 2020 2020 2020 6461 7461 6672 616d 653d        dataframe=
+00025040: 2273 7069 6e65 222c 0a20 2020 2020 2020  "spine",.       
+00025050: 2064 6570 7265 6361 7465 643d 4661 6c73   deprecated=Fals
+00025060: 652c 0a20 2020 2020 2020 202a 2a6b 7761  e,.        **kwa
+00025070: 7267 732c 0a20 2020 2029 3a0a 2020 2020  rgs,.    ):.    
+00025080: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00025090: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
+000250a0: 2020 6e61 6d65 2c0a 2020 2020 2020 2020    name,.        
+000250b0: 2020 2020 7665 7273 696f 6e2c 0a20 2020      version,.   
+000250c0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+000250d0: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
+000250e0: 2020 2020 2020 6c6f 6361 7469 6f6e 2c0a        location,.
+000250f0: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00025100: 745f 7469 6d65 3d65 7665 6e74 5f74 696d  t_time=event_tim
+00025110: 652c 0a20 2020 2020 2020 2020 2020 206f  e,.            o
+00025120: 6e6c 696e 655f 656e 6162 6c65 643d 6f6e  nline_enabled=on
+00025130: 6c69 6e65 5f65 6e61 626c 6564 2c0a 2020  line_enabled,.  
+00025140: 2020 2020 2020 2020 2020 6964 3d69 642c            id=id,
+00025150: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+00025160: 6563 7461 7469 6f6e 5f73 7569 7465 3d65  ectation_suite=e
+00025170: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+00025180: 2c0a 2020 2020 2020 2020 2020 2020 6f6e  ,.            on
+00025190: 6c69 6e65 5f74 6f70 6963 5f6e 616d 653d  line_topic_name=
+000251a0: 6f6e 6c69 6e65 5f74 6f70 6963 5f6e 616d  online_topic_nam
+000251b0: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
+000251c0: 6f70 6963 5f6e 616d 653d 746f 7069 635f  opic_name=topic_
+000251d0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+000251e0: 2020 6465 7072 6563 6174 6564 3d64 6570    deprecated=dep
+000251f0: 7265 6361 7465 642c 0a20 2020 2020 2020  recated,.       
+00025200: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00025210: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
+00025220: 6e61 6d65 203d 2066 6561 7475 7265 7374  name = featurest
+00025230: 6f72 655f 6e61 6d65 0a20 2020 2020 2020  ore_name.       
+00025240: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
+00025250: 6f6e 203d 2064 6573 6372 6970 7469 6f6e  on = description
+00025260: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00025270: 7265 6174 6564 203d 2063 7265 6174 6564  reated = created
+00025280: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00025290: 7265 6174 6f72 203d 2075 7365 722e 5573  reator = user.Us
+000252a0: 6572 2e66 726f 6d5f 7265 7370 6f6e 7365  er.from_response
+000252b0: 5f6a 736f 6e28 6372 6561 746f 7229 0a0a  _json(creator)..
+000252c0: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+000252d0: 6174 7572 6573 203d 205b 0a20 2020 2020  atures = [.     
+000252e0: 2020 2020 2020 2066 6561 7475 7265 2e46         feature.F
+000252f0: 6561 7475 7265 2e66 726f 6d5f 7265 7370  eature.from_resp
+00025300: 6f6e 7365 5f6a 736f 6e28 6665 6174 2920  onse_json(feat) 
+00025310: 6966 2069 7369 6e73 7461 6e63 6528 6665  if isinstance(fe
+00025320: 6174 2c20 6469 6374 2920 656c 7365 2066  at, dict) else f
+00025330: 6561 740a 2020 2020 2020 2020 2020 2020  eat.            
+00025340: 666f 7220 6665 6174 2069 6e20 2866 6561  for feat in (fea
+00025350: 7475 7265 7320 6f72 205b 5d29 0a20 2020  tures or []).   
+00025360: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00025370: 7365 6c66 2e5f 6665 6174 7572 655f 6772  self._feature_gr
+00025380: 6f75 705f 656e 6769 6e65 203d 2073 7069  oup_engine = spi
+00025390: 6e65 5f67 726f 7570 5f65 6e67 696e 652e  ne_group_engine.
+000253a0: 5370 696e 6547 726f 7570 456e 6769 6e65  SpineGroupEngine
+000253b0: 280a 2020 2020 2020 2020 2020 2020 6665  (.            fe
+000253c0: 6174 7572 6573 746f 7265 5f69 640a 2020  aturestore_id.  
+000253d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000253e0: 2069 6620 7365 6c66 2e5f 6964 3a0a 2020   if self._id:.  
+000253f0: 2020 2020 2020 2020 2020 2320 476f 7420            # Got 
+00025400: 6672 6f6d 2048 6f70 7377 6f72 6b73 2c20  from Hopsworks, 
+00025410: 6465 7365 7269 616c 697a 6520 6665 6174  deserialize feat
+00025420: 7572 6573 2061 6e64 2073 746f 7261 6765  ures and storage
+00025430: 2063 6f6e 6e65 6374 6f72 0a20 2020 2020   connector.     
+00025440: 2020 2020 2020 2073 656c 662e 5f66 6561         self._fea
+00025450: 7475 7265 7320 3d20 280a 2020 2020 2020  tures = (.      
+00025460: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00025470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025480: 6665 6174 7572 652e 4665 6174 7572 652e  feature.Feature.
+00025490: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
+000254a0: 6f6e 2866 6561 7429 0a20 2020 2020 2020  on(feat).       
+000254b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000254c0: 6973 696e 7374 616e 6365 2866 6561 742c  isinstance(feat,
+000254d0: 2064 6963 7429 0a20 2020 2020 2020 2020   dict).         
+000254e0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+000254f0: 6665 6174 0a20 2020 2020 2020 2020 2020  feat.           
+00025500: 2020 2020 2020 2020 2066 6f72 2066 6561           for fea
+00025510: 7420 696e 2066 6561 7475 7265 730a 2020  t in features.  
+00025520: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+00025530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025540: 6966 2066 6561 7475 7265 730a 2020 2020  if features.    
+00025550: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00025560: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00025570: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00025580: 7365 6c66 2e70 7269 6d61 7279 5f6b 6579  self.primary_key
+00025590: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000255a0: 2020 2020 205b 6665 6174 2e6e 616d 6520       [feat.name 
+000255b0: 666f 7220 6665 6174 2069 6e20 7365 6c66  for feat in self
+000255c0: 2e5f 6665 6174 7572 6573 2069 6620 6665  ._features if fe
+000255d0: 6174 2e70 7269 6d61 7279 2069 7320 5472  at.primary is Tr
+000255e0: 7565 5d0a 2020 2020 2020 2020 2020 2020  ue].            
+000255f0: 2020 2020 6966 2073 656c 662e 5f66 6561      if self._fea
+00025600: 7475 7265 730a 2020 2020 2020 2020 2020  tures.          
+00025610: 2020 2020 2020 656c 7365 205b 5d0a 2020        else [].  
+00025620: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00025630: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00025640: 7469 7374 6963 735f 636f 6e66 6967 203d  tistics_config =
+00025650: 2073 7461 7469 7374 6963 735f 636f 6e66   statistics_conf
+00025660: 6967 0a20 2020 2020 2020 2065 6c73 653a  ig.        else:
+00025670: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00025680: 662e 7072 696d 6172 795f 6b65 7920 3d20  f.primary_key = 
+00025690: 7072 696d 6172 795f 6b65 790a 2020 2020  primary_key.    
+000256a0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000256b0: 7469 7374 6963 735f 636f 6e66 6967 203d  tistics_config =
+000256c0: 2073 7461 7469 7374 6963 735f 636f 6e66   statistics_conf
+000256d0: 6967 0a20 2020 2020 2020 2020 2020 2073  ig.            s
+000256e0: 656c 662e 5f66 6561 7475 7265 7320 3d20  elf._features = 
+000256f0: 6665 6174 7572 6573 0a0a 2020 2020 2020  features..      
+00025700: 2020 7365 6c66 2e5f 6872 6566 203d 2068    self._href = h
+00025710: 7265 660a 0a20 2020 2020 2020 2023 2068  ref..        # h
+00025720: 6173 2074 6f20 6861 7070 656e 206c 6173  as to happen las
+00025730: 7420 2d3e 2066 6561 7475 7265 7320 616e  t -> features an
+00025740: 6420 6964 2061 7265 206e 6565 6465 6420  d id are needed 
+00025750: 666f 7220 7363 6865 6d61 2076 6572 6966  for schema verif
+00025760: 6963 6174 696f 6e0a 2020 2020 2020 2020  ication.        
+00025770: 2320 7573 6520 7365 7474 6572 2074 6f20  # use setter to 
+00025780: 636f 6e76 6572 7420 746f 2064 6566 6175  convert to defau
+00025790: 6c74 2064 6174 6166 7261 6d65 2074 7970  lt dataframe typ
+000257a0: 6520 666f 7220 656e 6769 6e65 0a20 2020  e for engine.   
+000257b0: 2020 2020 2073 656c 662e 6461 7461 6672       self.datafr
+000257c0: 616d 6520 3d20 6461 7461 6672 616d 650a  ame = dataframe.
+000257d0: 0a20 2020 2064 6566 205f 7361 7665 2873  .    def _save(s
+000257e0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000257f0: 2250 6572 7369 7374 2074 6865 206d 6574  "Persist the met
+00025800: 6164 6174 6120 666f 7220 7468 6973 2073  adata for this s
+00025810: 7069 6e65 2067 726f 7570 2e0a 0a20 2020  pine group...   
+00025820: 2020 2020 2057 6974 686f 7574 2063 616c       Without cal
+00025830: 6c69 6e67 2074 6869 7320 6d65 7468 6f64  ling this method
+00025840: 2c20 796f 7572 2066 6561 7475 7265 2067  , your feature g
+00025850: 726f 7570 2077 696c 6c20 6f6e 6c79 2065  roup will only e
+00025860: 7869 7374 0a20 2020 2020 2020 2069 6e20  xist.        in 
+00025870: 796f 7572 2050 7974 686f 6e20 4b65 726e  your Python Kern
+00025880: 656c 2c20 6275 7420 6e6f 7420 696e 2048  el, but not in H
+00025890: 6f70 7377 6f72 6b73 2e0a 0a20 2020 2020  opsworks...     
+000258a0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+000258b0: 2020 2020 2071 7565 7279 203d 2022 5345       query = "SE
+000258c0: 4c45 4354 202a 2046 524f 4d20 7361 6c65  LECT * FROM sale
+000258d0: 7322 0a0a 2020 2020 2020 2020 6667 203d  s"..        fg =
+000258e0: 2066 6561 7475 7265 5f73 746f 7265 2e63   feature_store.c
+000258f0: 7265 6174 655f 7370 696e 655f 6772 6f75  reate_spine_grou
+00025900: 7028 6e61 6d65 3d22 7361 6c65 7322 2c0a  p(name="sales",.
+00025910: 2020 2020 2020 2020 2020 2020 7665 7273              vers
+00025920: 696f 6e3d 312c 0a20 2020 2020 2020 2020  ion=1,.         
+00025930: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00025940: 5068 7973 6963 616c 2073 686f 7020 7361  Physical shop sa
+00025950: 6c65 7320 6665 6174 7572 6573 222c 0a20  les features",. 
+00025960: 2020 2020 2020 2020 2020 2070 7269 6d61             prima
+00025970: 7279 5f6b 6579 3d5b 2773 735f 7374 6f72  ry_key=['ss_stor
+00025980: 655f 736b 275d 2c0a 2020 2020 2020 2020  e_sk'],.        
+00025990: 2020 2020 6576 656e 745f 7469 6d65 3d27      event_time='
+000259a0: 7361 6c65 5f64 6174 6527 2c0a 2020 2020  sale_date',.    
+000259b0: 2020 2020 2020 2020 6461 7461 6672 616d          datafram
+000259c0: 653d 6466 2c0a 2020 2020 2020 2020 290a  e=df,.        ).
+000259d0: 0a20 2020 2020 2020 2066 672e 5f73 6176  .        fg._sav
+000259e0: 6528 290a 2020 2020 2020 2020 2222 220a  e().        """.
+000259f0: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+00025a00: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
+00025a10: 6e65 2e73 6176 6528 7365 6c66 290a 2020  ne.save(self).  
+00025a20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00025a30: 660a 0a20 2020 2040 7072 6f70 6572 7479  f..    @property
+00025a40: 0a20 2020 2064 6566 2064 6174 6166 7261  .    def datafra
+00025a50: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
+00025a60: 2020 2222 2253 7069 6e65 2064 6174 6166    """Spine dataf
+00025a70: 7261 6d65 2077 6974 6820 7072 696d 6172  rame with primar
+00025a80: 7920 6b65 792c 2065 7665 6e74 2074 696d  y key, event tim
+00025a90: 6520 616e 640a 2020 2020 2020 2020 6c61  e and.        la
+00025aa0: 6265 6c20 636f 6c75 6d6e 2074 6f20 7573  bel column to us
+00025ab0: 6520 666f 7220 706f 696e 7420 696e 2074  e for point in t
+00025ac0: 696d 6520 6a6f 696e 2077 6865 6e20 6665  ime join when fe
+00025ad0: 7463 6869 6e67 2066 6561 7475 7265 732e  tching features.
+00025ae0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00025af0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00025b00: 2e5f 6461 7461 6672 616d 650a 0a20 2020  ._dataframe..   
+00025b10: 2040 6461 7461 6672 616d 652e 7365 7474   @dataframe.sett
+00025b20: 6572 0a20 2020 2064 6566 2064 6174 6166  er.    def dataf
+00025b30: 7261 6d65 2873 656c 662c 2064 6174 6166  rame(self, dataf
+00025b40: 7261 6d65 293a 0a20 2020 2020 2020 2022  rame):.        "
+00025b50: 2222 5570 6461 7465 2074 6865 2073 7069  ""Update the spi
+00025b60: 6e65 2064 6174 6166 7261 6d65 2063 6f6e  ne dataframe con
+00025b70: 7461 696e 6564 2069 6e20 7468 6520 7370  tained in the sp
+00025b80: 696e 6520 6772 6f75 702e 2222 220a 2020  ine group.""".  
+00025b90: 2020 2020 2020 7365 6c66 2e5f 6461 7461        self._data
+00025ba0: 6672 616d 6520 3d20 656e 6769 6e65 2e67  frame = engine.g
+00025bb0: 6574 5f69 6e73 7461 6e63 6528 292e 636f  et_instance().co
+00025bc0: 6e76 6572 745f 746f 5f64 6566 6175 6c74  nvert_to_default
+00025bd0: 5f64 6174 6166 7261 6d65 2864 6174 6166  _dataframe(dataf
+00025be0: 7261 6d65 290a 0a20 2020 2020 2020 2023  rame)..        #
+00025bf0: 2069 6e20 6673 2071 7565 7279 2074 6865   in fs query the
+00025c00: 2066 6561 7475 7265 7320 6172 6520 6e6f   features are no
+00025c10: 7420 7365 6e74 2c20 736f 2074 6865 6e20  t sent, so then 
+00025c20: 646f 6e27 7420 646f 2076 616c 6964 6174  don't do validat
+00025c30: 696f 6e0a 2020 2020 2020 2020 6966 2028  ion.        if (
+00025c40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00025c50: 662e 5f69 6420 6973 206e 6f74 204e 6f6e  f._id is not Non
+00025c60: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
+00025c70: 6420 7365 6c66 2e5f 6461 7461 6672 616d  d self._datafram
+00025c80: 6520 6973 206e 6f74 204e 6f6e 650a 2020  e is not None.  
+00025c90: 2020 2020 2020 2020 2020 616e 6420 7365            and se
+00025ca0: 6c66 2e5f 6665 6174 7572 6573 2069 7320  lf._features is 
+00025cb0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00025cc0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00025cd0: 6461 7461 6672 616d 655f 6665 6174 7572  dataframe_featur
+00025ce0: 6573 203d 2065 6e67 696e 652e 6765 745f  es = engine.get_
+00025cf0: 696e 7374 616e 6365 2829 2e70 6172 7365  instance().parse
+00025d00: 5f73 6368 656d 615f 6665 6174 7572 655f  _schema_feature_
+00025d10: 6772 6f75 7028 0a20 2020 2020 2020 2020  group(.         
+00025d20: 2020 2020 2020 2073 656c 662e 5f64 6174         self._dat
+00025d30: 6166 7261 6d65 0a20 2020 2020 2020 2020  aframe.         
+00025d40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00025d50: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
+00025d60: 726f 7570 5f65 6e67 696e 652e 5f76 6572  roup_engine._ver
+00025d70: 6966 795f 7363 6865 6d61 5f63 6f6d 7061  ify_schema_compa
+00025d80: 7469 6269 6c69 7479 280a 2020 2020 2020  tibility(.      
+00025d90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00025da0: 6665 6174 7572 6573 2c20 6461 7461 6672  features, datafr
+00025db0: 616d 655f 6665 6174 7572 6573 0a20 2020  ame_features.   
+00025dc0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00025dd0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00025de0: 2064 6566 2066 726f 6d5f 7265 7370 6f6e   def from_respon
+00025df0: 7365 5f6a 736f 6e28 636c 732c 206a 736f  se_json(cls, jso
+00025e00: 6e5f 6469 6374 293a 0a20 2020 2020 2020  n_dict):.       
+00025e10: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+00025e20: 6420 3d20 6875 6d70 732e 6465 6361 6d65  d = humps.decame
+00025e30: 6c69 7a65 286a 736f 6e5f 6469 6374 290a  lize(json_dict).
+00025e40: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00025e50: 7461 6e63 6528 6a73 6f6e 5f64 6563 616d  tance(json_decam
+00025e60: 656c 697a 6564 2c20 6469 6374 293a 0a20  elized, dict):. 
+00025e70: 2020 2020 2020 2020 2020 205f 203d 206a             _ = j
+00025e80: 736f 6e5f 6465 6361 6d65 6c69 7a65 642e  son_decamelized.
+00025e90: 706f 7028 2274 7970 6522 2c20 4e6f 6e65  pop("type", None
+00025ea0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00025eb0: 7475 726e 2063 6c73 282a 2a6a 736f 6e5f  turn cls(**json_
+00025ec0: 6465 6361 6d65 6c69 7a65 6429 0a20 2020  decamelized).   
+00025ed0: 2020 2020 2066 6f72 2066 6720 696e 206a       for fg in j
+00025ee0: 736f 6e5f 6465 6361 6d65 6c69 7a65 643a  son_decamelized:
+00025ef0: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+00025f00: 2066 672e 706f 7028 2274 7970 6522 2c20   fg.pop("type", 
+00025f10: 4e6f 6e65 290a 2020 2020 2020 2020 7265  None).        re
+00025f20: 7475 726e 205b 636c 7328 2a2a 6667 2920  turn [cls(**fg) 
+00025f30: 666f 7220 6667 2069 6e20 6a73 6f6e 5f64  for fg in json_d
+00025f40: 6563 616d 656c 697a 6564 5d0a 0a20 2020  ecamelized]..   
+00025f50: 2064 6566 2075 7064 6174 655f 6672 6f6d   def update_from
+00025f60: 5f72 6573 706f 6e73 655f 6a73 6f6e 2873  _response_json(s
+00025f70: 656c 662c 206a 736f 6e5f 6469 6374 293a  elf, json_dict):
+00025f80: 0a20 2020 2020 2020 206a 736f 6e5f 6465  .        json_de
+00025f90: 6361 6d65 6c69 7a65 6420 3d20 6875 6d70  camelized = hump
+00025fa0: 732e 6465 6361 6d65 6c69 7a65 286a 736f  s.decamelize(jso
+00025fb0: 6e5f 6469 6374 290a 2020 2020 2020 2020  n_dict).        
+00025fc0: 6966 2022 7479 7065 2220 696e 206a 736f  if "type" in jso
+00025fd0: 6e5f 6465 6361 6d65 6c69 7a65 643a 0a20  n_decamelized:. 
+00025fe0: 2020 2020 2020 2020 2020 205f 203d 206a             _ = j
+00025ff0: 736f 6e5f 6465 6361 6d65 6c69 7a65 642e  son_decamelized.
+00026000: 706f 7028 2274 7970 6522 290a 2020 2020  pop("type").    
+00026010: 2020 2020 7365 6c66 2e5f 5f69 6e69 745f      self.__init_
+00026020: 5f28 2a2a 6a73 6f6e 5f64 6563 616d 656c  _(**json_decamel
+00026030: 697a 6564 290a 2020 2020 2020 2020 7265  ized).        re
+00026040: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
+00026050: 6566 206a 736f 6e28 7365 6c66 293a 0a20  ef json(self):. 
+00026060: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
+00026070: 6f6e 2e64 756d 7073 2873 656c 662c 2063  on.dumps(self, c
+00026080: 6c73 3d75 7469 6c2e 4665 6174 7572 6553  ls=util.FeatureS
+00026090: 746f 7265 456e 636f 6465 7229 0a0a 2020  toreEncoder)..  
+000260a0: 2020 6465 6620 746f 5f64 6963 7428 7365    def to_dict(se
+000260b0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+000260c0: 7572 6e20 7b0a 2020 2020 2020 2020 2020  urn {.          
+000260d0: 2020 2269 6422 3a20 7365 6c66 2e5f 6964    "id": self._id
+000260e0: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+000260f0: 616d 6522 3a20 7365 6c66 2e5f 6e61 6d65  ame": self._name
+00026100: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
+00026110: 6573 6372 6970 7469 6f6e 223a 2073 656c  escription": sel
+00026120: 662e 5f64 6573 6372 6970 7469 6f6e 2c0a  f._description,.
+00026130: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00026140: 7369 6f6e 223a 2073 656c 662e 5f76 6572  sion": self._ver
+00026150: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00026160: 2020 2266 6561 7475 7265 7322 3a20 7365    "features": se
+00026170: 6c66 2e5f 6665 6174 7572 6573 2c0a 2020  lf._features,.  
+00026180: 2020 2020 2020 2020 2020 2266 6561 7475            "featu
+00026190: 7265 7374 6f72 6549 6422 3a20 7365 6c66  restoreId": self
+000261a0: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
+000261b0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000261c0: 2274 7970 6522 3a20 226f 6e44 656d 616e  "type": "onDeman
+000261d0: 6446 6561 7475 7265 6772 6f75 7044 544f  dFeaturegroupDTO
+000261e0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000261f0: 7374 6174 6973 7469 6373 436f 6e66 6967  statisticsConfig
+00026200: 223a 2073 656c 662e 5f73 7461 7469 7374  ": self._statist
+00026210: 6963 735f 636f 6e66 6967 2c0a 2020 2020  ics_config,.    
+00026220: 2020 2020 2020 2020 2265 7665 6e74 5469          "eventTi
+00026230: 6d65 223a 2073 656c 662e 5f65 7665 6e74  me": self._event
+00026240: 5f74 696d 652c 0a20 2020 2020 2020 2020  _time,.         
+00026250: 2020 2022 7370 696e 6522 3a20 5472 7565     "spine": True
+00026260: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00026270: 6f70 6963 4e61 6d65 223a 2073 656c 662e  opicName": self.
+00026280: 746f 7069 635f 6e61 6d65 2c0a 2020 2020  topic_name,.    
+00026290: 2020 2020 2020 2020 2264 6570 7265 6361          "depreca
+000262a0: 7465 6422 3a20 7365 6c66 2e64 6570 7265  ted": self.depre
+000262b0: 6361 7465 642c 0a20 2020 2020 2020 207d  cated,.        }
+000262c0: 0a                                       .
```

### Comparing `hsfs-3.7.1/hsfs/feature_group_commit.py` & `hsfs-3.7.1rc0/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/feature_group_writer.py` & `hsfs-3.7.1rc0/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/feature_store.py` & `hsfs-3.7.1rc0/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/feature_view.py` & `hsfs-3.7.1rc0/hsfs/feature_view.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/ge_expectation.py` & `hsfs-3.7.1rc0/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/ge_validation_result.py` & `hsfs-3.7.1rc0/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/serving_key.py` & `hsfs-3.7.1rc0/hsfs/serving_key.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/split_statistics.py` & `hsfs-3.7.1rc0/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/statistics.py` & `hsfs-3.7.1rc0/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/statistics_config.py` & `hsfs-3.7.1rc0/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/storage_connector.py` & `hsfs-3.7.1rc0/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/tag.py` & `hsfs-3.7.1rc0/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/training_dataset.py` & `hsfs-3.7.1rc0/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/training_dataset_feature.py` & `hsfs-3.7.1rc0/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/training_dataset_split.py` & `hsfs-3.7.1rc0/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/transformation_function.py` & `hsfs-3.7.1rc0/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/transformation_function_attached.py` & `hsfs-3.7.1rc0/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/usage.py` & `hsfs-3.7.1rc0/hsfs/usage.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/user.py` & `hsfs-3.7.1rc0/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/util.py` & `hsfs-3.7.1rc0/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/validation_report.py` & `hsfs-3.7.1rc0/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/hsfs/version.py` & `hsfs-3.7.1rc0/hsfs/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.7.1"
+__version__ = "3.7.1rc0"
```

### Comparing `hsfs-3.7.1/hsfs.egg-info/PKG-INFO` & `hsfs-3.7.1rc0/hsfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.7.1
+Version: 3.7.1rc0
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1rc0
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.7.1 Summary: HSFS: An environment
-independent client to interact with the Hopsworks Featurestore Home-page:
-https://github.com/logicalclocks/feature-store-api Author: Hopsworks AB Author-
-email: moritz@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1
+Metadata-Version: 2.1 Name: hsfs Version: 3.7.1rc0 Summary: HSFS: An
+environment independent client to interact with the Hopsworks Featurestore
+Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
+AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.1rc0
 Description: # Hopsworks Feature Store
 _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _F_e_a_t_u_r_e_ _S_t_o_r_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_S_c_a_l_a_/
                 _J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.7.1/hsfs.egg-info/SOURCES.txt` & `hsfs-3.7.1rc0/hsfs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -118,10 +118,8 @@
 hsfs/core/validation_result_engine.py
 hsfs/core/variable_api.py
 hsfs/core/vector_db_client.py
 hsfs/core/vector_server.py
 hsfs/engine/__init__.py
 hsfs/engine/python.py
 hsfs/engine/spark.py
-hsfs/engine/spark_no_metastore.py
-tests/__init__.py
-tests/test_storage_connector.py
+hsfs/engine/spark_no_metastore.py
```

### Comparing `hsfs-3.7.1/hsfs.egg-info/requires.txt` & `hsfs-3.7.1rc0/hsfs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.1/setup.py` & `hsfs-3.7.1rc0/setup.py`

 * *Files identical despite different names*

