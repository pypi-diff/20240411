# Comparing `tmp/hopsworks-3.7.0rc0.tar.gz` & `tmp/hopsworks-3.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopsworks-3.7.0rc0.tar", last modified: Tue Feb  6 12:17:53 2024, max compression
+gzip compressed data, was "hopsworks-3.7.0rc1.tar", last modified: Tue Feb  6 22:01:45 2024, max compression
```

## Comparing `hopsworks-3.7.0rc0.tar` & `hopsworks-3.7.0rc1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/
--rw-r--r--   0     1006     1006       40 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/MANIFEST.in
--rw-r--r--   0     1006     1006     3473 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/PKG-INFO
--rw-r--r--   0     1006     1006     2061 2024-02-06 12:17:52.000000 hopsworks-3.7.0rc0/README.md
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.611810 hopsworks-3.7.0rc0/hopsworks/
--rw-r--r--   0     1006     1006    10722 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.611810 hopsworks-3.7.0rc0/hopsworks/client/
--rw-r--r--   0     1006     1006     1763 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/client/__init__.py
--rw-r--r--   0     1006     1006     1148 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/client/auth.py
--rw-r--r--   0     1006     1006     6661 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/client/base.py
--rw-r--r--   0     1006     1006     2393 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/client/exceptions.py
--rw-r--r--   0     1006     1006     5552 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/client/external.py
--rw-r--r--   0     1006     1006     8091 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/client/hopsworks.py
--rw-r--r--   0     1006     1006     1673 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/command.py
--rw-r--r--   0     1006     1006    12868 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/connection.py
--rw-r--r--   0     1006     1006     4462 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/constants.py
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/hopsworks/core/
--rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/__init__.py
--rw-r--r--   0     1006     1006    15479 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/core/dataset_api.py
--rw-r--r--   0     1006     1006     3795 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/environment_api.py
--rw-r--r--   0     1006     1006     2384 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/core/execution_api.py
--rw-r--r--   0     1006     1006    14755 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/flink_cluster_api.py
--rw-r--r--   0     1006     1006    16138 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/git_api.py
--rw-r--r--   0     1006     1006     1419 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/git_op_execution_api.py
--rw-r--r--   0     1006     1006     3289 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/git_provider_api.py
--rw-r--r--   0     1006     1006     3669 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/git_remote_api.py
--rw-r--r--   0     1006     1006     6421 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/job_api.py
--rw-r--r--   0     1006     1006    11478 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/core/kafka_api.py
--rw-r--r--   0     1006     1006     1588 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/library_api.py
--rw-r--r--   0     1006     1006     3935 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/core/opensearch_api.py
--rw-r--r--   0     1006     1006     3601 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/project_api.py
--rw-r--r--   0     1006     1006     3890 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/secret_api.py
--rw-r--r--   0     1006     1006     1336 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/core/variable_api.py
--rw-r--r--   0     1006     1006     1651 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/decorators.py
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/hopsworks/engine/
--rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/engine/__init__.py
--rw-r--r--   0     1006     1006     3471 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/engine/environment_engine.py
--rw-r--r--   0     1006     1006     5930 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/engine/execution_engine.py
--rw-r--r--   0     1006     1006     2025 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/engine/git_engine.py
--rw-r--r--   0     1006     1006     5688 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/environment.py
--rw-r--r--   0     1006     1006     6907 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/execution.py
--rw-r--r--   0     1006     1006    12664 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/flink_cluster.py
--rw-r--r--   0     1006     1006     2368 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/git_commit.py
--rw-r--r--   0     1006     1006     2181 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/git_file_status.py
--rw-r--r--   0     1006     1006     3487 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/git_op_execution.py
--rw-r--r--   0     1006     1006     2382 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/git_provider.py
--rw-r--r--   0     1006     1006     2285 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/git_remote.py
--rw-r--r--   0     1006     1006     8767 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/git_repo.py
--rw-r--r--   0     1006     1006     7946 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/job.py
--rw-r--r--   0     1006     1006     3072 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/job_schedule.py
--rw-r--r--   0     1006     1006     2766 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/kafka_schema.py
--rw-r--r--   0     1006     1006     3328 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/kafka_topic.py
--rw-r--r--   0     1006     1006     1667 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/library.py
--rw-r--r--   0     1006     1006     7379 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/project.py
--rw-r--r--   0     1006     1006     2937 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/secret.py
--rw-r--r--   0     1006     1006     2563 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/user.py
--rw-r--r--   0     1006     1006     2830 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/hopsworks/util.py
--rw-r--r--   0     1006     1006      631 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/hopsworks/version.py
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.611810 hopsworks-3.7.0rc0/hopsworks.egg-info/
--rw-r--r--   0     1006     1006     3473 2024-02-06 12:17:53.000000 hopsworks-3.7.0rc0/hopsworks.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     1655 2024-02-06 12:17:53.000000 hopsworks-3.7.0rc0/hopsworks.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2024-02-06 12:17:53.000000 hopsworks-3.7.0rc0/hopsworks.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      339 2024-02-06 12:17:53.000000 hopsworks-3.7.0rc0/hopsworks.egg-info/requires.txt
--rw-r--r--   0     1006     1006       16 2024-02-06 12:17:53.000000 hopsworks-3.7.0rc0/hopsworks.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/setup.cfg
--rw-r--r--   0     1006     1006     1878 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/setup.py
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/tests/
--rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-02-06 12:17:53.619810 hopsworks-3.7.0rc0/tests/hopsworks/
--rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc0/tests/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     7825 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc0/tests/hopsworks/test_login.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/
+-rw-r--r--   0     1006     1006       40 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/MANIFEST.in
+-rw-r--r--   0     1006     1006     3473 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/PKG-INFO
+-rw-r--r--   0     1006     1006     2061 2024-02-06 22:01:44.000000 hopsworks-3.7.0rc1/README.md
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.546180 hopsworks-3.7.0rc1/hopsworks/
+-rw-r--r--   0     1006     1006    10722 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.550180 hopsworks-3.7.0rc1/hopsworks/client/
+-rw-r--r--   0     1006     1006     1763 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/client/__init__.py
+-rw-r--r--   0     1006     1006     1148 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/client/auth.py
+-rw-r--r--   0     1006     1006     6661 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/client/base.py
+-rw-r--r--   0     1006     1006     2393 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/client/exceptions.py
+-rw-r--r--   0     1006     1006     5552 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/client/external.py
+-rw-r--r--   0     1006     1006     8091 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1673 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/command.py
+-rw-r--r--   0     1006     1006    12868 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/connection.py
+-rw-r--r--   0     1006     1006     4462 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/constants.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/hopsworks/core/
+-rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/__init__.py
+-rw-r--r--   0     1006     1006    15479 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/core/dataset_api.py
+-rw-r--r--   0     1006     1006     3795 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/environment_api.py
+-rw-r--r--   0     1006     1006     2384 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/core/execution_api.py
+-rw-r--r--   0     1006     1006    14755 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/flink_cluster_api.py
+-rw-r--r--   0     1006     1006    16138 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/git_api.py
+-rw-r--r--   0     1006     1006     1419 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/git_op_execution_api.py
+-rw-r--r--   0     1006     1006     3289 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/git_provider_api.py
+-rw-r--r--   0     1006     1006     3669 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/git_remote_api.py
+-rw-r--r--   0     1006     1006     6421 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/job_api.py
+-rw-r--r--   0     1006     1006    11478 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/core/kafka_api.py
+-rw-r--r--   0     1006     1006     1588 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/library_api.py
+-rw-r--r--   0     1006     1006     3935 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/core/opensearch_api.py
+-rw-r--r--   0     1006     1006     3601 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/project_api.py
+-rw-r--r--   0     1006     1006     3890 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/secret_api.py
+-rw-r--r--   0     1006     1006     1336 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/core/variable_api.py
+-rw-r--r--   0     1006     1006     1651 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/decorators.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/hopsworks/engine/
+-rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/engine/__init__.py
+-rw-r--r--   0     1006     1006     3471 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/engine/environment_engine.py
+-rw-r--r--   0     1006     1006     5930 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/engine/execution_engine.py
+-rw-r--r--   0     1006     1006     2025 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/engine/git_engine.py
+-rw-r--r--   0     1006     1006     5688 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/environment.py
+-rw-r--r--   0     1006     1006     6907 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/execution.py
+-rw-r--r--   0     1006     1006    12664 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/flink_cluster.py
+-rw-r--r--   0     1006     1006     2368 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/git_commit.py
+-rw-r--r--   0     1006     1006     2181 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/git_file_status.py
+-rw-r--r--   0     1006     1006     3487 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/git_op_execution.py
+-rw-r--r--   0     1006     1006     2382 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/git_provider.py
+-rw-r--r--   0     1006     1006     2285 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/git_remote.py
+-rw-r--r--   0     1006     1006     8767 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/git_repo.py
+-rw-r--r--   0     1006     1006     7946 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/job.py
+-rw-r--r--   0     1006     1006     3072 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/job_schedule.py
+-rw-r--r--   0     1006     1006     2766 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/kafka_schema.py
+-rw-r--r--   0     1006     1006     3328 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/kafka_topic.py
+-rw-r--r--   0     1006     1006     1667 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/library.py
+-rw-r--r--   0     1006     1006     7379 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/project.py
+-rw-r--r--   0     1006     1006     2937 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/secret.py
+-rw-r--r--   0     1006     1006     2563 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/hopsworks/user.py
+-rw-r--r--   0     1006     1006     2830 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/hopsworks/util.py
+-rw-r--r--   0     1006     1006      631 2024-02-06 22:01:40.000000 hopsworks-3.7.0rc1/hopsworks/version.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.546180 hopsworks-3.7.0rc1/hopsworks.egg-info/
+-rw-r--r--   0     1006     1006     3473 2024-02-06 22:01:45.000000 hopsworks-3.7.0rc1/hopsworks.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     1655 2024-02-06 22:01:45.000000 hopsworks-3.7.0rc1/hopsworks.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2024-02-06 22:01:45.000000 hopsworks-3.7.0rc1/hopsworks.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      331 2024-02-06 22:01:45.000000 hopsworks-3.7.0rc1/hopsworks.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       16 2024-02-06 22:01:45.000000 hopsworks-3.7.0rc1/hopsworks.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/setup.cfg
+-rw-r--r--   0     1006     1006     1870 2024-02-06 22:01:40.000000 hopsworks-3.7.0rc1/setup.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/tests/
+-rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 22:01:45.554180 hopsworks-3.7.0rc1/tests/hopsworks/
+-rw-r--r--   0     1006     1006      605 2024-01-10 11:19:35.000000 hopsworks-3.7.0rc1/tests/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     7825 2024-02-06 12:17:48.000000 hopsworks-3.7.0rc1/tests/hopsworks/test_login.py
```

### Comparing `hopsworks-3.7.0rc0/PKG-INFO` & `hopsworks-3.7.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hopsworks
-Version: 3.7.0rc0
+Version: 3.7.0rc1
 Summary: HOPSWORKS: An environment independent client to interact with the Hopsworks API
 Home-page: https://github.com/logicalclocks/hopsworks-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc0
+Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc1
 Description: # Hopsworks Client
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hopsworks Version: 3.7.0rc0 Summary: HOPSWORKS: An
+Metadata-Version: 2.1 Name: hopsworks Version: 3.7.0rc1 Summary: HOPSWORKS: An
 environment independent client to interact with the Hopsworks API Home-page:
 https://github.com/logicalclocks/hopsworks-api Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc0
+https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc1
 Description: # Hopsworks Client
      _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_D_o_w_n_l_o_a_d_s_]
                              _[_C_o_d_e_S_t_y_l_e_][License]
 *hopsworks* is the python API for interacting with a Hopsworks cluster. ##
 Getting Started On Hopsworks Instantiate a connection and get the project
 object ```python import hopsworks connection = hopsworks.connection() project =
 connection.get_project("my_project") ``` Create a new project ```python project
```

### Comparing `hopsworks-3.7.0rc0/README.md` & `hopsworks-3.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/__init__.py` & `hopsworks-3.7.0rc1/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/client/__init__.py` & `hopsworks-3.7.0rc1/hopsworks/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/client/auth.py` & `hopsworks-3.7.0rc1/hopsworks/client/auth.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/client/base.py` & `hopsworks-3.7.0rc1/hopsworks/client/base.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/client/exceptions.py` & `hopsworks-3.7.0rc1/hopsworks/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/client/external.py` & `hopsworks-3.7.0rc1/hopsworks/client/external.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/client/hopsworks.py` & `hopsworks-3.7.0rc1/hopsworks/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/command.py` & `hopsworks-3.7.0rc1/hopsworks/command.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/connection.py` & `hopsworks-3.7.0rc1/hopsworks/connection.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/constants.py` & `hopsworks-3.7.0rc1/hopsworks/constants.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/__init__.py` & `hopsworks-3.7.0rc1/hopsworks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/dataset_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/environment_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/environment_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/execution_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/execution_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/flink_cluster_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/flink_cluster_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/git_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/git_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/git_op_execution_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/git_op_execution_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/git_provider_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/git_provider_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/git_remote_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/git_remote_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/job_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/kafka_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/library_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/library_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/opensearch_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/opensearch_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/project_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/secret_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/secret_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/core/variable_api.py` & `hopsworks-3.7.0rc1/hopsworks/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/decorators.py` & `hopsworks-3.7.0rc1/hopsworks/decorators.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/engine/__init__.py` & `hopsworks-3.7.0rc1/hopsworks/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/engine/environment_engine.py` & `hopsworks-3.7.0rc1/hopsworks/engine/environment_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/engine/execution_engine.py` & `hopsworks-3.7.0rc1/hopsworks/engine/execution_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/engine/git_engine.py` & `hopsworks-3.7.0rc1/hopsworks/engine/git_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/environment.py` & `hopsworks-3.7.0rc1/hopsworks/environment.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/execution.py` & `hopsworks-3.7.0rc1/hopsworks/execution.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/flink_cluster.py` & `hopsworks-3.7.0rc1/hopsworks/flink_cluster.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/git_commit.py` & `hopsworks-3.7.0rc1/hopsworks/git_commit.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/git_file_status.py` & `hopsworks-3.7.0rc1/hopsworks/git_file_status.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/git_op_execution.py` & `hopsworks-3.7.0rc1/hopsworks/git_op_execution.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/git_provider.py` & `hopsworks-3.7.0rc1/hopsworks/git_provider.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/git_remote.py` & `hopsworks-3.7.0rc1/hopsworks/git_remote.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/git_repo.py` & `hopsworks-3.7.0rc1/hopsworks/git_repo.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/job.py` & `hopsworks-3.7.0rc1/hopsworks/job.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/job_schedule.py` & `hopsworks-3.7.0rc1/hopsworks/job_schedule.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/kafka_schema.py` & `hopsworks-3.7.0rc1/hopsworks/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/kafka_topic.py` & `hopsworks-3.7.0rc1/hopsworks/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/library.py` & `hopsworks-3.7.0rc1/hopsworks/library.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/project.py` & `hopsworks-3.7.0rc1/hopsworks/project.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/secret.py` & `hopsworks-3.7.0rc1/hopsworks/secret.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/user.py` & `hopsworks-3.7.0rc1/hopsworks/user.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/util.py` & `hopsworks-3.7.0rc1/hopsworks/util.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/hopsworks/version.py` & `hopsworks-3.7.0rc1/hopsworks/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.7.0rc0"
+__version__ = "3.7.0rc1"
```

### Comparing `hopsworks-3.7.0rc0/hopsworks.egg-info/PKG-INFO` & `hopsworks-3.7.0rc1/hopsworks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hopsworks
-Version: 3.7.0rc0
+Version: 3.7.0rc1
 Summary: HOPSWORKS: An environment independent client to interact with the Hopsworks API
 Home-page: https://github.com/logicalclocks/hopsworks-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc0
+Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc1
 Description: # Hopsworks Client
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hopsworks Version: 3.7.0rc0 Summary: HOPSWORKS: An
+Metadata-Version: 2.1 Name: hopsworks Version: 3.7.0rc1 Summary: HOPSWORKS: An
 environment independent client to interact with the Hopsworks API Home-page:
 https://github.com/logicalclocks/hopsworks-api Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc0
+https://github.com/logicalclocks/hopsworks-api/releases/tag/3.7.0rc1
 Description: # Hopsworks Client
      _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_D_o_w_n_l_o_a_d_s_]
                              _[_C_o_d_e_S_t_y_l_e_][License]
 *hopsworks* is the python API for interacting with a Hopsworks cluster. ##
 Getting Started On Hopsworks Instantiate a connection and get the project
 object ```python import hopsworks connection = hopsworks.connection() project =
 connection.get_project("my_project") ``` Create a new project ```python project
```

### Comparing `hopsworks-3.7.0rc0/hopsworks.egg-info/SOURCES.txt` & `hopsworks-3.7.0rc1/hopsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/setup.py` & `hopsworks-3.7.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="hopsworks",
     version=__version__,
     install_requires=[
-        "hsfs[python]>=3.7.0,<3.8.0",
-        "hsml>=3.7.0,<3.8.0",
+        "hsfs[python]~=3.7.0rc1",
+        "hsml~=3.7.0rc0",
         "pyhumps==1.6.1",
         "requests",
         "furl",
         "boto3",
         "pyjks",
         "mock",
         "tqdm",
```

### Comparing `hopsworks-3.7.0rc0/tests/__init__.py` & `hopsworks-3.7.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/tests/hopsworks/__init__.py` & `hopsworks-3.7.0rc1/tests/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.7.0rc0/tests/hopsworks/test_login.py` & `hopsworks-3.7.0rc1/tests/hopsworks/test_login.py`

 * *Files identical despite different names*

