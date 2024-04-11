# Comparing `tmp/dbgpt-0.5.3rc0.tar.gz` & `tmp/dbgpt-0.5.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbgpt-0.5.3rc0.tar", last modified: Wed Mar 27 11:52:07 2024, max compression
+gzip compressed data, was "dbgpt-0.5.4rc0.tar", last modified: Thu Apr 11 05:05:19 2024, max compression
```

## Comparing `dbgpt-0.5.3rc0.tar` & `dbgpt-0.5.4rc0.tar`

### file list

```diff
@@ -1,361 +1,461 @@
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.800004 dbgpt-0.5.3rc0/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.3rc0/LICENSE
--rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.3rc0/MANIFEST.in
--rw-r--r--   0 staneyffer   (501) staff       (20)    28866 2024-03-27 11:52:07.799475 dbgpt-0.5.3rc0/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    11764 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/README.md
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.552104 dbgpt-0.5.3rc0/dbgpt/
--rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.557319 dbgpt-0.5.3rc0/dbgpt/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13218 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/_private/config.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1625 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/_private/llm_metadata.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      943 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/_private/pydantic.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/_version.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.558092 dbgpt-0.5.3rc0/dbgpt/cli/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/cli/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5482 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/cli/cli_scripts.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.562932 dbgpt-0.5.3rc0/dbgpt/client/
--rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.3rc0/dbgpt/client/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/client/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.3rc0/dbgpt/client/app.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14121 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/client/client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3562 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/client/flow.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6906 2024-03-22 07:58:46.000000 dbgpt-0.5.3rc0/dbgpt/client/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8724 2024-03-22 07:58:46.000000 dbgpt-0.5.3rc0/dbgpt/client/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10212 2024-03-22 07:58:46.000000 dbgpt-0.5.3rc0/dbgpt/component.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.564044 dbgpt-0.5.3rc0/dbgpt/configs/
--rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/configs/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9570 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/configs/model_config.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.565051 dbgpt-0.5.3rc0/dbgpt/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.567119 dbgpt-0.5.3rc0/dbgpt/core/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/_private/example_base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/_private/prompt_registry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.567754 dbgpt-0.5.3rc0/dbgpt/core/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)     6044 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.571663 dbgpt-0.5.3rc0/dbgpt/core/awel/dag/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/dag/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/dag/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2792 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/dag/dag_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/dag/loader.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.575495 dbgpt-0.5.3rc0/dbgpt/core/awel/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    32108 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/flow/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/flow/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    27785 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/flow/flow_factory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.579857 dbgpt-0.5.3rc0/dbgpt/core/awel/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/operators/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/operators/common_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/operators/stream_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.581431 dbgpt-0.5.3rc0/dbgpt/core/awel/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/resource/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.583876 dbgpt-0.5.3rc0/dbgpt/core/awel/runner/
--rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/runner/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/runner/job_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/runner/local_runner.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.586631 dbgpt-0.5.3rc0/dbgpt/core/awel/task/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/task/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/task/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/task/task_impl.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.591196 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/
--rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2540 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    37789 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/iterator_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/trigger_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.594375 dbgpt-0.5.3rc0/dbgpt/core/awel/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/util/_typing_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/util/http_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/awel/util/parameter_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.606720 dbgpt-0.5.3rc0/dbgpt/core/interface/
--rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/embeddings.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3793 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    30001 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/llm.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    42772 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/message.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.610696 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/message_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    16374 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/prompt_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/operators/retriever.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10802 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/output_parser.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    26524 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/prompt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1725 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15124 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/interface/storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.611307 dbgpt-0.5.3rc0/dbgpt/core/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/core/operators/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.613225 dbgpt-0.5.3rc0/dbgpt/core/operators/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/operators/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/operators/flow/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/core/operators/flow/dict_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.614247 dbgpt-0.5.3rc0/dbgpt/core/schema/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/core/schema/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3868 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/core/schema/api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.618445 dbgpt-0.5.3rc0/dbgpt/datasource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/conn_spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/db_conn_info.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.621245 dbgpt-0.5.3rc0/dbgpt/datasource/manages/
--rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/manages/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7345 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/manages/connect_config_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/manages/connector_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.622610 dbgpt-0.5.3rc0/dbgpt/datasource/nosql/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/nosql/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.624307 dbgpt-0.5.3rc0/dbgpt/datasource/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-27 08:37:36.000000 dbgpt-0.5.3rc0/dbgpt/datasource/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/operators/datasource_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.633974 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_doris.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_duckdb.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_hive.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_mssql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_mysql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_postgresql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_sqlite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_starrocks.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.634870 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.635620 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/
--rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.637934 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
--rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.3rc0/dbgpt/datasource/redis.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.642024 dbgpt-0.5.3rc0/dbgpt/model/
--rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.653768 dbgpt-0.5.3rc0/dbgpt/model/adapter/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/embeddings_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/fschat_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6619 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/hf_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/model_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    17036 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/old_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8945 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/proxy_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/adapter/vllm_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/cli.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.655475 dbgpt-0.5.3rc0/dbgpt/model/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/model/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/parameter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.656656 dbgpt-0.5.3rc0/dbgpt/model/proxy/
--rw-r--r--   0 staneyffer   (501) staff       (20)      924 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.665497 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/
--rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/baichuan.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/bard.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    10395 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/chatgpt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/claude.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/gemini.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/proxy_model.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/tongyi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/wenxin.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/yi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/zhipu.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.668269 dbgpt-0.5.3rc0/dbgpt/model/utils/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/utils/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/model/utils/chatgpt_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/utils/llm_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/model/utils/token_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.670039 dbgpt-0.5.3rc0/dbgpt/rag/
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.674034 dbgpt-0.5.3rc0/dbgpt/rag/assembler/
--rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/assembler/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/assembler/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/assembler/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/assembler/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/assembler/summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/chunk_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.677451 dbgpt-0.5.3rc0/dbgpt/rag/embedding/
--rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/embedding/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/embedding/_wrapped.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/embedding/embedding_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    24178 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/embedding/embeddings.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.679073 dbgpt-0.5.3rc0/dbgpt/rag/evaluation/
--rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/evaluation/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/evaluation/retriever.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.681934 dbgpt-0.5.3rc0/dbgpt/rag/extractor/
--rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/extractor/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/extractor/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/extractor/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.682725 dbgpt-0.5.3rc0/dbgpt/rag/graph/
--rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/graph/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.690684 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5481 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3253 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/csv.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1840 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2306 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/docx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6043 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2752 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/html.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/json.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2320 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/markdown.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3098 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/pdf.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2612 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/pptx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1540 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/string.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2232 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/txt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2129 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/knowledge/url.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.696260 dbgpt-0.5.3rc0/dbgpt/rag/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/assembler.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-27 11:34:54.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/rewrite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/schema_linking.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/operators/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.699248 dbgpt-0.5.3rc0/dbgpt/rag/retriever/
--rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/retriever/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2929 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/retriever/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6720 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/retriever/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7863 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/retriever/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/retriever/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/retriever/rewrite.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.701168 dbgpt-0.5.3rc0/dbgpt/rag/schemalinker/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/schemalinker/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/schemalinker/base_linker.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/schemalinker/schema_linking.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.702977 dbgpt-0.5.3rc0/dbgpt/rag/summary/
--rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/summary/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/summary/db_summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/summary/db_summary_client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3964 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/summary/rdbms_db_summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.704728 dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/
--rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31793 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/token_splitter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.706541 dbgpt-0.5.3rc0/dbgpt/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.709933 dbgpt-0.5.3rc0/dbgpt/storage/cache/
--rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/embedding_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/llm_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/operators.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.710465 dbgpt-0.5.3rc0/dbgpt/storage/cache/protocol/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/protocol/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.711207 dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.712209 dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/disk/
--rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/disk/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.713555 dbgpt-0.5.3rc0/dbgpt/storage/chat_history/
--rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/chat_history/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/chat_history/chat_history_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/chat_history/storage_adapter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.717307 dbgpt-0.5.3rc0/dbgpt/storage/metadata/
--rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/metadata/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9255 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/metadata/_base_dao.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/metadata/db_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/metadata/db_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/metadata/db_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/schema.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.721955 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/
--rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7188 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5846 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/chroma_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6317 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/connector.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18680 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/milvus_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3343 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/pgvector_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6645 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/storage/vector_store/weaviate_store.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.744219 dbgpt-0.5.3rc0/dbgpt/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/_db_migration_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/annotations.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/api_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.744816 dbgpt-0.5.3rc0/dbgpt/util/benchmarks/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/benchmarks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.746050 dbgpt-0.5.3rc0/dbgpt/util/benchmarks/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/benchmarks/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9300 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/chat_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/code_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/command_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/config_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.747191 dbgpt-0.5.3rc0/dbgpt/util/console/
--rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/util/console/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/util/console/console.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/custom_data_structure.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.750710 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9344 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11619 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/repo.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5905 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/dbgpts/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/error_types.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/executor_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1313 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/fastapi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/formatting.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/function_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/global_helper.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/util/i18n_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3739 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/json_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/memory_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/model_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/module_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/net_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/openai_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      545 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/pagination_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/parameter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/path_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/pd_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8661 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/prompt_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.751619 dbgpt-0.5.3rc0/dbgpt/util/serialization/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/serialization/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-03-25 14:27:11.000000 dbgpt-0.5.3rc0/dbgpt/util/serialization/json_serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/similarity_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/singleton.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.754939 dbgpt-0.5.3rc0/dbgpt/util/speech/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/brian.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/eleven_labs.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/gtts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/macos_tts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/speech/say.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/splitter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2964 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/string_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/system_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.758714 dbgpt-0.5.3rc0/dbgpt/util/tracer/
--rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/tracer/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6793 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/tracer/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5310 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/tracer/span_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/tracer/tracer_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7283 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/tracer/tracer_impl.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/tracer/tracer_middleware.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.3rc0/dbgpt/util/utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-03-27 11:52:07.554623 dbgpt-0.5.3rc0/dbgpt.egg-info/
--rw-r--r--   0 staneyffer   (501) staff       (20)    28866 2024-03-27 11:52:07.000000 dbgpt-0.5.3rc0/dbgpt.egg-info/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)     9662 2024-03-27 11:52:07.000000 dbgpt-0.5.3rc0/dbgpt.egg-info/SOURCES.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-03-27 11:52:07.000000 dbgpt-0.5.3rc0/dbgpt.egg-info/dependency_links.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-03-27 11:52:07.000000 dbgpt-0.5.3rc0/dbgpt.egg-info/entry_points.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)     4566 2024-03-27 11:52:07.000000 dbgpt-0.5.3rc0/dbgpt.egg-info/requires.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-03-27 11:52:07.000000 dbgpt-0.5.3rc0/dbgpt.egg-info/top_level.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-03-27 11:52:07.800109 dbgpt-0.5.3rc0/setup.cfg
--rw-r--r--   0 staneyffer   (501) staff       (20)    23063 2024-03-27 07:42:00.000000 dbgpt-0.5.3rc0/setup.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.368039 dbgpt-0.5.4rc0/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.4rc0/LICENSE
+-rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.4rc0/MANIFEST.in
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30382 2024-04-11 05:05:19.367289 dbgpt-0.5.4rc0/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/README.md
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.973762 dbgpt-0.5.4rc0/dbgpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.981845 dbgpt-0.5.4rc0/dbgpt/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13796 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/_private/config.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1625 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/_private/llm_metadata.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      983 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/_private/pydantic.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.4rc0/dbgpt/_version.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.982750 dbgpt-0.5.4rc0/dbgpt/agent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      944 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.989166 dbgpt-0.5.4rc0/dbgpt/agent/actions/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5106 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/blank_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/chart_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/code_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4312 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/dashboard_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/indicator_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/plugin_action.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.996611 dbgpt-0.5.4rc0/dbgpt/agent/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3463 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/agent_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    35778 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/base_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5616 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/base_team.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.998902 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3496 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm_client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.000032 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/priority.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3632 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/role.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      455 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/user_proxy_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.005797 dbgpt-0.5.4rc0/dbgpt/agent/expand/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-11 02:57:34.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/code_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5410 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/data_scientist_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2710 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/plugin_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22133 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1680 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/summary_assistant_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.008669 dbgpt-0.5.4rc0/dbgpt/agent/memory/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/default_gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/gpts_memory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.012326 dbgpt-0.5.4rc0/dbgpt/agent/plan/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.016378 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10858 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6004 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator_resource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8312 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/team_awel_layout.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/plan_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7577 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/planner_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/team_auto_plan.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.019545 dbgpt-0.5.4rc0/dbgpt/agent/plugin/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.022966 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.023575 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.026320 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22478 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/plugins_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.030330 dbgpt-0.5.4rc0/dbgpt/agent/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3698 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 01:48:23.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_db_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_knowledge_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_plugin_api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.032017 dbgpt-0.5.4rc0/dbgpt/agent/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 04:29:39.000000 dbgpt-0.5.4rc0/dbgpt/agent/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/util/cmp.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.033422 dbgpt-0.5.4rc0/dbgpt/cli/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/cli/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/cli/cli_scripts.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.041821 dbgpt-0.5.4rc0/dbgpt/client/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/app.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14121 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3718 2024-03-28 01:32:30.000000 dbgpt-0.5.4rc0/dbgpt/client/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3562 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/flow.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6906 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9418 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/client/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10595 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/component.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.043705 dbgpt-0.5.4rc0/dbgpt/configs/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/configs/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/configs/model_config.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.044635 dbgpt-0.5.4rc0/dbgpt/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.047812 dbgpt-0.5.4rc0/dbgpt/core/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/example_base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/prompt_registry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.048644 dbgpt-0.5.4rc0/dbgpt/core/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6044 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.053927 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3515 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/dag_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/loader.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.059666 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    33486 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/compat.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    28676 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/flow_factory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.064144 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/common_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/stream_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.065894 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.068366 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/job_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/local_runner.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.071359 dbgpt-0.5.4rc0/dbgpt/core/awel/task/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/task_impl.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.077642 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37793 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/iterator_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/trigger_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.081292 dbgpt-0.5.4rc0/dbgpt/core/awel/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/_typing_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/http_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/parameter_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.093577 dbgpt-0.5.4rc0/dbgpt/core/interface/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3793 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31087 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/llm.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    42772 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/message.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.101651 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/message_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16374 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/prompt_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/retriever.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/output_parser.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    26524 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/prompt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1725 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15124 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.102606 dbgpt-0.5.4rc0/dbgpt/core/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.105315 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/dict_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.107003 dbgpt-0.5.4rc0/dbgpt/core/schema/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/schema/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3868 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/schema/api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.111492 dbgpt-0.5.4rc0/dbgpt/datasource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/conn_spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/db_conn_info.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.114151 dbgpt-0.5.4rc0/dbgpt/datasource/manages/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/connect_config_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/connector_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.114912 dbgpt-0.5.4rc0/dbgpt/datasource/nosql/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/nosql/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.116360 dbgpt-0.5.4rc0/dbgpt/datasource/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.4rc0/dbgpt/datasource/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/operators/datasource_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.126686 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_doris.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_duckdb.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_hive.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mssql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mysql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_postgresql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_sqlite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_starrocks.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.127572 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.128426 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.130689 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/redis.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.135298 dbgpt-0.5.4rc0/dbgpt/model/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.150106 dbgpt-0.5.4rc0/dbgpt/model/adapter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/embeddings_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/fschat_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/hf_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/model_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/old_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/proxy_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/vllm_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/cli.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.152289 dbgpt-0.5.4rc0/dbgpt/model/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/model/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/parameter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.154070 dbgpt-0.5.4rc0/dbgpt/model/proxy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.165126 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/baichuan.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/bard.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/chatgpt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/claude.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/gemini.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/moonshot.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/proxy_model.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/tongyi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/wenxin.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/yi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/zhipu.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.167691 dbgpt-0.5.4rc0/dbgpt/model/utils/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/chatgpt_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/llm_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/token_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.169670 dbgpt-0.5.4rc0/dbgpt/rag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.174299 dbgpt-0.5.4rc0/dbgpt/rag/assembler/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/chunk_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.178536 dbgpt-0.5.4rc0/dbgpt/rag/embedding/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/_wrapped.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/embedding_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24178 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/embeddings.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.180597 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/retriever.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.184058 dbgpt-0.5.4rc0/dbgpt/rag/extractor/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.187268 dbgpt-0.5.4rc0/dbgpt/rag/graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/graph/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.203704 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/csv.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/docx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/html.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/json.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/markdown.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pdf.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pptx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/string.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/txt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/url.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.217047 dbgpt-0.5.4rc0/dbgpt/rag/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/assembler.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/schema_linking.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.222651 dbgpt-0.5.4rc0/dbgpt/rag/retriever/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/rewrite.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.224784 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/base_linker.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/schema_linking.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.227962 dbgpt-0.5.4rc0/dbgpt/rag/summary/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary_client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3964 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/rdbms_db_summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.231422 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/token_splitter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.233812 dbgpt-0.5.4rc0/dbgpt/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.238853 dbgpt-0.5.4rc0/dbgpt/storage/cache/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/embedding_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/llm_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.240028 dbgpt-0.5.4rc0/dbgpt/storage/cache/protocol/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/protocol/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.241804 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.243560 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.245833 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/chat_history_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/storage_adapter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.250741 dbgpt-0.5.4rc0/dbgpt/storage/metadata/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9255 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/_base_dao.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/schema.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.257290 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7796 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8232 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/chroma_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/connector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/filters.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    21307 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/milvus_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3462 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/pgvector_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6749 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/weaviate_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.298070 dbgpt-0.5.4rc0/dbgpt/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/_db_migration_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/annotations.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/api_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.298880 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.300181 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9300 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/chat_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/code_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/command_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/config_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.301400 dbgpt-0.5.4rc0/dbgpt/util/console/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/console/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/console/console.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/custom_data_structure.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.4rc0/dbgpt/util/date_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.304988 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9344 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11619 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/repo.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5905 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/error_types.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/executor_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1313 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/fastapi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/formatting.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/function_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/global_helper.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/util/i18n_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/util/json_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/memory_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/model_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/module_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/net_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.305930 dbgpt-0.5.4rc0/dbgpt/util/network/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/network/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9777 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/network/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/openai_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      545 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/pagination_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/parameter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/path_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/pd_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8661 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/prompt_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.306804 dbgpt-0.5.4rc0/dbgpt/util/serialization/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/serialization/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/util/serialization/json_serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/similarity_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/singleton.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.310685 dbgpt-0.5.4rc0/dbgpt/util/speech/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/brian.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/eleven_labs.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/gtts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/macos_tts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/say.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/splitter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/util/string_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/system_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.315968 dbgpt-0.5.4rc0/dbgpt/util/tracer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/span_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_impl.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_middleware.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.317582 dbgpt-0.5.4rc0/dbgpt/vis/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 04:24:29.000000 dbgpt-0.5.4rc0/dbgpt/vis/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.323394 dbgpt-0.5.4rc0/dbgpt/vis/tags/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_agent_message.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_agent_plans.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_chart.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_code.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_dashboard.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_gpts_execution.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_gpts_result.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_plugin.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.977858 dbgpt-0.5.4rc0/dbgpt.egg-info/
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30382 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12638 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/entry_points.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4943 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/requires.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/top_level.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-11 05:05:19.368143 dbgpt-0.5.4rc0/setup.cfg
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23342 2024-04-11 01:47:19.000000 dbgpt-0.5.4rc0/setup.py
```

### Comparing `dbgpt-0.5.3rc0/LICENSE` & `dbgpt-0.5.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/PKG-INFO` & `dbgpt-0.5.4rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.3rc0
+Version: 0.5.4rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -46,14 +46,32 @@
 Requires-Dist: fastapi==0.98.0; extra == "cli"
 Requires-Dist: prettytable; extra == "cli"
 Requires-Dist: click; extra == "cli"
 Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
 Requires-Dist: rich; extra == "cli"
+Provides-Extra: agent
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: importlib-resources==5.12.0; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: pydantic<2,>=1; extra == "agent"
+Requires-Dist: typeguard; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
+Requires-Dist: fastapi==0.98.0; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
+Requires-Dist: click; extra == "agent"
+Requires-Dist: psutil==5.9.4; extra == "agent"
+Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: rich; extra == "agent"
+Requires-Dist: termcolor; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
 Provides-Extra: simple-framework
 Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
 Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
 Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
 Requires-Dist: cachetools; extra == "simple-framework"
 Requires-Dist: pydantic<2,>=1; extra == "simple-framework"
@@ -62,14 +80,16 @@
 Requires-Dist: fastapi==0.98.0; extra == "simple-framework"
 Requires-Dist: prettytable; extra == "simple-framework"
 Requires-Dist: click; extra == "simple-framework"
 Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: colorama==0.4.6; extra == "simple-framework"
 Requires-Dist: tomlkit; extra == "simple-framework"
 Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: termcolor; extra == "simple-framework"
+Requires-Dist: pandas==2.0.3; extra == "simple-framework"
 Requires-Dist: jinja2; extra == "simple-framework"
 Requires-Dist: uvicorn; extra == "simple-framework"
 Requires-Dist: shortuuid; extra == "simple-framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
 Requires-Dist: msgpack; extra == "simple-framework"
 Requires-Dist: pympler; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
@@ -89,53 +109,58 @@
 Requires-Dist: fastapi==0.98.0; extra == "framework"
 Requires-Dist: prettytable; extra == "framework"
 Requires-Dist: click; extra == "framework"
 Requires-Dist: psutil==5.9.4; extra == "framework"
 Requires-Dist: colorama==0.4.6; extra == "framework"
 Requires-Dist: tomlkit; extra == "framework"
 Requires-Dist: rich; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: jinja2; extra == "framework"
 Requires-Dist: uvicorn; extra == "framework"
 Requires-Dist: shortuuid; extra == "framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
 Requires-Dist: msgpack; extra == "framework"
 Requires-Dist: pympler; extra == "framework"
 Requires-Dist: duckdb; extra == "framework"
 Requires-Dist: duckdb-engine; extra == "framework"
 Requires-Dist: schedule; extra == "framework"
 Requires-Dist: sqlparse==0.4.4; extra == "framework"
 Requires-Dist: fschat; extra == "framework"
 Requires-Dist: coloredlogs; extra == "framework"
 Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: auto-gpt-plugin-template; extra == "framework"
 Requires-Dist: gTTS==2.3.1; extra == "framework"
 Requires-Dist: pymysql; extra == "framework"
 Requires-Dist: jsonschema; extra == "framework"
 Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: alembic==1.12.0; extra == "framework"
 Requires-Dist: openpyxl==3.1.2; extra == "framework"
 Requires-Dist: chardet==5.1.0; extra == "framework"
 Requires-Dist: xlrd==2.0.1; extra == "framework"
 Requires-Dist: aiofiles; extra == "framework"
 Requires-Dist: GitPython; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torch==2.0.1; extra == "torch"
-Requires-Dist: torchvision==0.15.2; extra == "torch"
-Requires-Dist: torchaudio==2.0.2; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
+Requires-Dist: torchvision==0.17.1; extra == "torch"
+Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torch==2.0.1; extra == "torch-cpu"
-Requires-Dist: torchvision==0.15.2; extra == "torch-cpu"
-Requires-Dist: torchaudio==2.0.2; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
+Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
+Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
+Provides-Extra: bitsandbytes
+Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
-Requires-Dist: bitsandbytes; extra == "quantization"
 Requires-Dist: cpm_kernels; extra == "quantization"
 Provides-Extra: vstore
 Requires-Dist: pymilvus; extra == "vstore"
 Requires-Dist: weaviate-client; extra == "vstore"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
@@ -176,28 +201,29 @@
 Requires-Dist: fastapi==0.98.0; extra == "openai"
 Requires-Dist: prettytable; extra == "openai"
 Requires-Dist: click; extra == "openai"
 Requires-Dist: psutil==5.9.4; extra == "openai"
 Requires-Dist: colorama==0.4.6; extra == "openai"
 Requires-Dist: tomlkit; extra == "openai"
 Requires-Dist: rich; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
 Requires-Dist: jinja2; extra == "openai"
 Requires-Dist: uvicorn; extra == "openai"
 Requires-Dist: shortuuid; extra == "openai"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
 Requires-Dist: msgpack; extra == "openai"
 Requires-Dist: pympler; extra == "openai"
 Requires-Dist: duckdb; extra == "openai"
 Requires-Dist: duckdb-engine; extra == "openai"
 Requires-Dist: schedule; extra == "openai"
 Requires-Dist: sqlparse==0.4.4; extra == "openai"
 Requires-Dist: fschat; extra == "openai"
 Requires-Dist: coloredlogs; extra == "openai"
 Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
 Requires-Dist: auto-gpt-plugin-template; extra == "openai"
 Requires-Dist: gTTS==2.3.1; extra == "openai"
 Requires-Dist: pymysql; extra == "openai"
 Requires-Dist: jsonschema; extra == "openai"
 Requires-Dist: transformers>=4.34.0; extra == "openai"
 Requires-Dist: alembic==1.12.0; extra == "openai"
 Requires-Dist: openpyxl==3.1.2; extra == "openai"
@@ -227,14 +253,15 @@
 Provides-Extra: default
 Requires-Dist: tokenizers>=0.14; extra == "default"
 Requires-Dist: accelerate>=0.20.3; extra == "default"
 Requires-Dist: protobuf==3.20.3; extra == "default"
 Requires-Dist: zhipuai; extra == "default"
 Requires-Dist: dashscope; extra == "default"
 Requires-Dist: chardet; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
 Requires-Dist: aiohttp==3.8.4; extra == "default"
 Requires-Dist: chardet==5.1.0; extra == "default"
 Requires-Dist: importlib-resources==5.12.0; extra == "default"
 Requires-Dist: python-dotenv==1.0.0; extra == "default"
 Requires-Dist: cachetools; extra == "default"
 Requires-Dist: pydantic<2,>=1; extra == "default"
 Requires-Dist: typeguard; extra == "default"
@@ -242,28 +269,29 @@
 Requires-Dist: fastapi==0.98.0; extra == "default"
 Requires-Dist: prettytable; extra == "default"
 Requires-Dist: click; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
 Requires-Dist: colorama==0.4.6; extra == "default"
 Requires-Dist: tomlkit; extra == "default"
 Requires-Dist: rich; extra == "default"
+Requires-Dist: termcolor; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
 Requires-Dist: jinja2; extra == "default"
 Requires-Dist: uvicorn; extra == "default"
 Requires-Dist: shortuuid; extra == "default"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
 Requires-Dist: msgpack; extra == "default"
 Requires-Dist: pympler; extra == "default"
 Requires-Dist: duckdb; extra == "default"
 Requires-Dist: duckdb-engine; extra == "default"
 Requires-Dist: schedule; extra == "default"
 Requires-Dist: sqlparse==0.4.4; extra == "default"
 Requires-Dist: fschat; extra == "default"
 Requires-Dist: coloredlogs; extra == "default"
 Requires-Dist: seaborn; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
 Requires-Dist: auto-gpt-plugin-template; extra == "default"
 Requires-Dist: gTTS==2.3.1; extra == "default"
 Requires-Dist: pymysql; extra == "default"
 Requires-Dist: jsonschema; extra == "default"
 Requires-Dist: transformers>=4.34.0; extra == "default"
 Requires-Dist: alembic==1.12.0; extra == "default"
 Requires-Dist: openpyxl==3.1.2; extra == "default"
@@ -281,99 +309,100 @@
 Requires-Dist: bs4; extra == "default"
 Requires-Dist: python-pptx; extra == "default"
 Requires-Dist: python-docx; extra == "default"
 Requires-Dist: pypdf; extra == "default"
 Requires-Dist: python-multipart; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
 Requires-Dist: pymysql; extra == "default"
-Requires-Dist: torch==2.0.1; extra == "default"
-Requires-Dist: torchvision==0.15.2; extra == "default"
-Requires-Dist: torchaudio==2.0.2; extra == "default"
-Requires-Dist: bitsandbytes; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
 Requires-Dist: cpm_kernels; extra == "default"
 Requires-Dist: rocksdict; extra == "default"
 Provides-Extra: all
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: python-docx; extra == "all"
-Requires-Dist: spacy==3.5.3; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: pymssql; extra == "all"
 Requires-Dist: chromadb==0.4.10; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: jinja2; extra == "all"
 Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
+Requires-Dist: protobuf==3.20.3; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: fschat; extra == "all"
 Requires-Dist: pypdf; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
 Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
 Requires-Dist: pympler; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: pyspark; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
 Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: langchain>=0.0.286; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: spacy==3.5.3; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
 Requires-Dist: graphviz; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
 Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: httpx; extra == "all"
+Requires-Dist: fastapi==0.98.0; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: vllm; extra == "all"
 Requires-Dist: msgpack; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: duckdb; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: torchvision==0.15.2; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: protobuf==3.20.3; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
 Requires-Dist: pydantic<2,>=1; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: torch==2.0.1; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: fschat; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
 Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: openai; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: termcolor; extra == "all"
 Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: fastapi==0.98.0; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: torchaudio==2.0.2; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: markdown; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -449,15 +478,15 @@
 
 - **RAG (Retrieval Augmented Generation)**: RAG is currently the most practically implemented and urgently needed domain. DB-GPT has already implemented a framework based on RAG, allowing users to build knowledge-based applications using the RAG capabilities of DB-GPT.
 
 - **GBI (Generative Business Intelligence)**: Generative BI is one of the core capabilities of the DB-GPT project, providing the foundational data intelligence technology to build enterprise report analysis and business insights.
 
 - **Fine-tuning Framework**: Model fine-tuning is an indispensable capability for any enterprise to implement in vertical and niche domains. DB-GPT provides a complete fine-tuning framework that integrates seamlessly with the DB-GPT project. In recent fine-tuning efforts, an accuracy rate based on the Spider dataset has been achieved at 82.5%.
 
-- **Data-Driven Multi-Agents Framework**: DB-GPT offers a data-driven self-evolving fine-tuning framework, aiming to continuously make decisions and execute based on data.
+- **Data-Driven Multi-Agents Framework**: DB-GPT offers a data-driven self-evolving multi-agents framework, aiming to continuously make decisions and execute based on data.
 
 - **Data Factory**: The Data Factory is mainly about cleaning and processing trustworthy knowledge and data in the era of large models.
 
 - **Data Sources**: Integrating various data sources to seamlessly connect production business data to the core capabilities of DB-GPT.
 
 ### SubModule
 - [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) Text-to-SQL workflow with high performance by applying Supervised Fine-Tuning (SFT) on Large Language Models (LLMs).
@@ -527,14 +556,16 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
+    - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
     - 🔥🔥🔥  [Yi-34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat)
   - [More Supported LLMs](http://docs.dbgpt.site/docs/modules/smmf)
```

### Comparing `dbgpt-0.5.3rc0/README.md` & `dbgpt-0.5.4rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 - **RAG (Retrieval Augmented Generation)**: RAG is currently the most practically implemented and urgently needed domain. DB-GPT has already implemented a framework based on RAG, allowing users to build knowledge-based applications using the RAG capabilities of DB-GPT.
 
 - **GBI (Generative Business Intelligence)**: Generative BI is one of the core capabilities of the DB-GPT project, providing the foundational data intelligence technology to build enterprise report analysis and business insights.
 
 - **Fine-tuning Framework**: Model fine-tuning is an indispensable capability for any enterprise to implement in vertical and niche domains. DB-GPT provides a complete fine-tuning framework that integrates seamlessly with the DB-GPT project. In recent fine-tuning efforts, an accuracy rate based on the Spider dataset has been achieved at 82.5%.
 
-- **Data-Driven Multi-Agents Framework**: DB-GPT offers a data-driven self-evolving fine-tuning framework, aiming to continuously make decisions and execute based on data.
+- **Data-Driven Multi-Agents Framework**: DB-GPT offers a data-driven self-evolving multi-agents framework, aiming to continuously make decisions and execute based on data.
 
 - **Data Factory**: The Data Factory is mainly about cleaning and processing trustworthy knowledge and data in the era of large models.
 
 - **Data Sources**: Integrating various data sources to seamlessly connect production business data to the core capabilities of DB-GPT.
 
 ### SubModule
 - [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) Text-to-SQL workflow with high performance by applying Supervised Fine-Tuning (SFT) on Large Language Models (LLMs).
@@ -154,14 +154,16 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
+    - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
     - 🔥🔥🔥  [Yi-34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat)
   - [More Supported LLMs](http://docs.dbgpt.site/docs/modules/smmf)
```

#### html2text {}

```diff
@@ -36,15 +36,15 @@
 of the core capabilities of the DB-GPT project, providing the foundational data
 intelligence technology to build enterprise report analysis and business
 insights. - **Fine-tuning Framework**: Model fine-tuning is an indispensable
 capability for any enterprise to implement in vertical and niche domains. DB-
 GPT provides a complete fine-tuning framework that integrates seamlessly with
 the DB-GPT project. In recent fine-tuning efforts, an accuracy rate based on
 the Spider dataset has been achieved at 82.5%. - **Data-Driven Multi-Agents
-Framework**: DB-GPT offers a data-driven self-evolving fine-tuning framework,
+Framework**: DB-GPT offers a data-driven self-evolving multi-agents framework,
 aiming to continuously make decisions and execute based on data. - **Data
 Factory**: The Data Factory is mainly about cleaning and processing trustworthy
 knowledge and data in the era of large models. - **Data Sources**: Integrating
 various data sources to seamlessly connect production business data to the core
 capabilities of DB-GPT. ### SubModule - [DB-GPT-Hub](https://github.com/
 eosphoros-ai/DB-GPT-Hub) Text-to-SQL workflow with high performance by applying
 Supervised Fine-Tuning (SFT) on Large Language Models (LLMs). - [dbgpts](https:
@@ -99,23 +99,25 @@
 tuning lightweight framework centred on large language models (LLMs), Text2SQL
 datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework
 simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly
 line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) - **SMMF
 (Service-oriented Multi-model Management Framework)** We offer extensive model
 support, including dozens of large language models (LLMs) from both open-source
 and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu,
-and many more. - News - ð¥ð¥ð¥ [gemma-7b-it](https://huggingface.co/
-google/gemma-7b-it) - ð¥ð¥ð¥ [gemma-2b-it](https://huggingface.co/google/
-gemma-2b-it) - ð¥ð¥ð¥ [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-
-10.7B-Instruct-v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B](https://huggingface.co/
-mistralai/Mixtral-8x7B-Instruct-v0.1) - ð¥ð¥ð¥ [Qwen-72B-Chat](https://
-huggingface.co/Qwen/Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-34B-Chat](https://
-huggingface.co/01-ai/Yi-34B-Chat) - [More Supported LLMs](http://
-docs.dbgpt.site/docs/modules/smmf) - **Privacy and Security** We ensure the
-privacy and security of data through the implementation of various
+and many more. - News - ð¥ð¥ð¥ [Qwen1.5-32B-Chat](https://huggingface.co/
+Qwen/Qwen1.5-32B-Chat) - ð¥ð¥ð¥ [Starling-LM-7B-beta](https://
+huggingface.co/Nexusflow/Starling-LM-7B-beta) - ð¥ð¥ð¥ [gemma-7b-it]
+(https://huggingface.co/google/gemma-7b-it) - ð¥ð¥ð¥ [gemma-2b-it](https:
+//huggingface.co/google/gemma-2b-it) - ð¥ð¥ð¥ [SOLAR-10.7B](https://
+huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B]
+(https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) - ð¥ð¥ð¥
+[Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-
+34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat) - [More Supported LLMs]
+(http://docs.dbgpt.site/docs/modules/smmf) - **Privacy and Security** We ensure
+the privacy and security of data through the implementation of various
 technologies, including privatized large models and proxy desensitization. -
 Support Datasources - [Datasources](http://docs.dbgpt.site/docs/modules/
 connections) ## Image ð [AutoDL Image](https://www.codewithgpu.com/i/
 eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the .env configuration
 file, modify the LANGUAGE parameter to switch to different languages. The
 default is English (Chinese: zh, English: en, other languages to be added
 later). ## Contribution - To check detailed guidelines for new contributions,
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/_private/config.py` & `dbgpt-0.5.4rc0/dbgpt/_private/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING, List, Optional
 
 from dbgpt.util.singleton import Singleton
 
 if TYPE_CHECKING:
     from auto_gpt_plugin_template import AutoGPTPluginTemplate
 
+    from dbgpt.agent.plugin import CommandRegistry
     from dbgpt.component import SystemApp
     from dbgpt.datasource.manages import ConnectorManager
 
 
 class Config(metaclass=Singleton):
     """Configuration class to store the state of bools for different scripts access"""
 
@@ -21,15 +22,15 @@
         """Initialize the Config class"""
 
         self.NEW_SERVER_MODE = False
         self.SERVER_LIGHT_MODE = False
 
         # Gradio language version: en, zh
         self.LANGUAGE = os.getenv("LANGUAGE", "en")
-        self.WEB_SERVER_PORT = int(os.getenv("WEB_SERVER_PORT", 7860))
+        self.WEB_SERVER_PORT = int(os.getenv("WEB_SERVER_PORT", 5000))
 
         self.debug_mode = False
         self.skip_reprompt = False
         self.temperature = float(os.getenv("TEMPERATURE", 0.7))
 
         # self.NUM_GPUS = int(os.getenv("NUM_GPUS", 1))
 
@@ -113,14 +114,24 @@
             os.environ["yi_proxyllm_proxy_api_key"] = self.yi_proxy_api_key
             os.environ["yi_proxyllm_proxyllm_backend"] = os.getenv(
                 "YI_MODEL_VERSION", "yi-34b-chat-0205"
             )
             os.environ["yi_proxyllm_proxy_api_base"] = os.getenv(
                 "YI_API_BASE", "https://api.lingyiwanwu.com/v1"
             )
+        # Moonshot proxy
+        self.moonshot_proxy_api_key = os.getenv("MOONSHOT_API_KEY")
+        if self.moonshot_proxy_api_key:
+            os.environ["moonshot_proxyllm_proxy_api_key"] = self.moonshot_proxy_api_key
+            os.environ["moonshot_proxyllm_proxyllm_backend"] = os.getenv(
+                "MOONSHOT_MODEL_VERSION", "moonshot-v1-8k"
+            )
+            os.environ["moonshot_proxyllm_api_base"] = os.getenv(
+                "MOONSHOT_API_BASE", "https://api.moonshot.cn/v1"
+            )
 
         self.proxy_server_url = os.getenv("PROXY_SERVER_URL")
 
         self.elevenlabs_api_key = os.getenv("ELEVENLABS_API_KEY")
         self.elevenlabs_voice_1_id = os.getenv("ELEVENLABS_VOICE_1_ID")
         self.elevenlabs_voice_2_id = os.getenv("ELEVENLABS_VOICE_2_ID")
 
@@ -141,15 +152,15 @@
         )
         self.speak_mode = False
 
         from dbgpt.core._private.prompt_registry import PromptTemplateRegistry
 
         self.prompt_template_registry = PromptTemplateRegistry()
         ### Related configuration of built-in commands
-        self.command_registry = []  # type: ignore
+        self.command_registry: Optional[CommandRegistry] = None
 
         disabled_command_categories = os.getenv("DISABLED_COMMAND_CATEGORIES")
         if disabled_command_categories:
             self.disabled_command_categories = disabled_command_categories.split(",")
         else:
             self.disabled_command_categories = []
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/_private/llm_metadata.py` & `dbgpt-0.5.4rc0/dbgpt/_private/llm_metadata.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/_private/pydantic.py` & `dbgpt-0.5.4rc0/dbgpt/_private/pydantic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pydantic
 
 if pydantic.VERSION.startswith("1."):
     PYDANTIC_VERSION = 1
     from pydantic import (
         BaseModel,
+        ConfigDict,
         Extra,
         Field,
         NonNegativeFloat,
         NonNegativeInt,
         PositiveFloat,
         PositiveInt,
         PrivateAttr,
@@ -16,14 +17,15 @@
         validator,
     )
 else:
     PYDANTIC_VERSION = 2
     # pydantic 2.x
     from pydantic.v1 import (
         BaseModel,
+        ConfigDict,
         Extra,
         Field,
         NonNegativeFloat,
         NonNegativeInt,
         PositiveFloat,
         PositiveInt,
         PrivateAttr,
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/cli/cli_scripts.py` & `dbgpt-0.5.4rc0/dbgpt/cli/cli_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 
 @click.group()
 def run():
     """Run your dbgpts."""
     pass
 
 
+@click.group()
+def net():
+    """Net tools."""
+    pass
+
+
 stop_all_func_list = []
 
 
 @click.command(name="all")
 def stop_all():
     """Stop all servers"""
     for stop_func in stop_all_func_list:
@@ -96,14 +102,15 @@
 cli.add_command(stop)
 cli.add_command(install)
 cli.add_command(db)
 cli.add_command(new)
 cli.add_command(app)
 cli.add_command(repo)
 cli.add_command(run)
+cli.add_command(net)
 add_command_alias(stop_all, name="all", parent_group=stop)
 
 try:
     from dbgpt.model.cli import (
         _stop_all_model_server,
         model_cli_group,
         start_apiserver,
@@ -196,14 +203,21 @@
 try:
     from dbgpt.client._cli import run_flow
 
     add_command_alias(run_flow, name="flow", parent_group=run)
 except ImportError as e:
     logging.warning(f"Integrating dbgpt client command line tool failed: {e}")
 
+try:
+    from dbgpt.util.network._cli import start_forward
+
+    add_command_alias(start_forward, name="forward", parent_group=net)
+except ImportError as e:
+    logging.warning(f"Integrating dbgpt net command line tool failed: {e}")
+
 
 def main():
     return cli()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/client/_cli.py` & `dbgpt-0.5.4rc0/dbgpt/client/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/client/app.py` & `dbgpt-0.5.4rc0/dbgpt/client/app.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/client/client.py` & `dbgpt-0.5.4rc0/dbgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/client/flow.py` & `dbgpt-0.5.4rc0/dbgpt/client/flow.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/client/knowledge.py` & `dbgpt-0.5.4rc0/dbgpt/client/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/client/schema.py` & `dbgpt-0.5.4rc0/dbgpt/client/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,18 +68,19 @@
 class ChatMode(Enum):
     """Chat mode."""
 
     CHAT_NORMAL = "chat_normal"
     CHAT_APP = "chat_app"
     CHAT_AWEL_FLOW = "chat_flow"
     CHAT_KNOWLEDGE = "chat_knowledge"
+    CHAT_DATA = "chat_data"
 
 
-class AwelTeamModel(BaseModel):
-    """Awel team model."""
+class AWELTeamModel(BaseModel):
+    """AWEL team model."""
 
     dag_id: str = Field(
         ...,
         description="The unique id of dag",
         examples=["flow_dag_testflow_66d8e9d6-f32e-4540-a5bd-ea0648145d0e"],
     )
     uid: str = Field(
@@ -132,15 +133,15 @@
     DB = "database"
     Knowledge = "knowledge"
     Internet = "internet"
     Plugin = "plugin"
     TextFile = "text_file"
     ExcelFile = "excel_file"
     ImageFile = "image_file"
-    AwelFlow = "awel_flow"
+    AWELFlow = "awel_flow"
 
 
 class AgentResourceModel(BaseModel):
     """Agent resource model."""
 
     type: AgentResourceType
     name: str
@@ -201,15 +202,15 @@
     """App model."""
 
     app_code: Optional[str] = Field(None, title="app code")
     app_name: Optional[str] = Field(None, title="app name")
     app_describe: Optional[str] = Field(None, title="app describe")
     team_mode: Optional[str] = Field(None, title="team mode")
     language: Optional[str] = Field("en", title="language")
-    team_context: Optional[Union[str, AwelTeamModel]] = Field(
+    team_context: Optional[Union[str, AWELTeamModel]] = Field(
         None, title="team context"
     )
     user_code: Optional[str] = Field(None, title="user code")
     sys_code: Optional[str] = Field(None, title="sys code")
     is_collected: Optional[str] = Field(None, title="is collected")
     icon: Optional[str] = Field(None, title="icon")
     created_at: datetime = datetime.now()
@@ -274,7 +275,21 @@
 
     """model_name: model name"""
     model_name: Optional[str] = Field(None, description="model name")
 
     """chunk_parameters: chunk parameters
     """
     chunk_parameters: ChunkParameters = Field(None, description="chunk parameters")
+
+
+class DatasourceModel(BaseModel):
+    """Datasource model."""
+
+    id: Optional[int] = Field(None, description="The datasource id")
+    db_type: str = Field(..., description="Database type, e.g. sqlite, mysql, etc.")
+    db_name: str = Field(..., description="Database name.")
+    db_path: str = Field("", description="File path for file-based database.")
+    db_host: str = Field("", description="Database host.")
+    db_port: int = Field(0, description="Database port.")
+    db_user: str = Field("", description="Database user.")
+    db_pwd: str = Field("", description="Database password.")
+    comment: str = Field("", description="Comment for the database.")
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/component.py` & `dbgpt-0.5.4rc0/dbgpt/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Component module for dbgpt.
 
 Manages the lifecycle and registration of components.
 """
 from __future__ import annotations
 
 import asyncio
+import atexit
 import logging
 import sys
+import threading
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import TYPE_CHECKING, Dict, Optional, Type, TypeVar, Union
 
 from dbgpt.util import AppConfig
 from dbgpt.util.annotations import PublicAPI
 
@@ -158,14 +160,16 @@
         app_config: Optional[AppConfig] = None,
     ) -> None:
         self.components: Dict[
             str, BaseComponent
         ] = {}  # Dictionary to store registered components.
         self._asgi_app = asgi_app
         self._app_config = app_config or AppConfig()
+        self._stop_event = threading.Event()
+        self._stop_event.clear()
         self._build()
 
     @property
     def app(self) -> Optional["FastAPI"]:
         """Returns the internal ASGI app."""
         return self._asgi_app
 
@@ -269,28 +273,32 @@
     async def async_after_start(self):
         """Asynchronously invoke the after_start hooks for all registered components."""
         tasks = [v.async_after_start() for _, v in self.components.items()]
         await asyncio.gather(*tasks)
 
     def before_stop(self):
         """Invoke the before_stop hooks for all registered components."""
+        if self._stop_event.is_set():
+            return
         for _, v in self.components.items():
             try:
                 v.before_stop()
             except Exception as e:
                 pass
+        self._stop_event.set()
 
     async def async_before_stop(self):
         """Asynchronously invoke the before_stop hooks for all registered components."""
         tasks = [v.async_before_stop() for _, v in self.components.items()]
         await asyncio.gather(*tasks)
 
     def _build(self):
         """Integrate lifecycle events with the internal ASGI app if available."""
         if not self.app:
+            self._register_exit_handler()
             return
 
         @self.app.on_event("startup")
         async def startup_event():
             """ASGI app startup event handler."""
 
             async def _startup_func():
@@ -304,7 +312,11 @@
             self.after_start()
 
         @self.app.on_event("shutdown")
         async def shutdown_event():
             """ASGI app shutdown event handler."""
             await self.async_before_stop()
             self.before_stop()
+
+    def _register_exit_handler(self):
+        """Register an exit handler to stop the system app."""
+        atexit.register(self.before_stop)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/configs/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/configs/model_config.py` & `dbgpt-0.5.4rc0/dbgpt/configs/model_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     "tongyi_proxyllm": "tongyi_proxyllm",
     "zhipu_proxyllm": "zhipu_proxyllm",
     "gemini_proxyllm": "gemini_proxyllm",
     "bc_proxyllm": "bc_proxyllm",
     "spark_proxyllm": "spark_proxyllm",
     # https://platform.lingyiwanwu.com/docs/
     "yi_proxyllm": "yi_proxyllm",
+    # https://platform.moonshot.cn/docs/
+    "moonshot_proxyllm": "moonshot_proxyllm",
     "llama-2-7b": os.path.join(MODEL_PATH, "Llama-2-7b-chat-hf"),
     "llama-2-13b": os.path.join(MODEL_PATH, "Llama-2-13b-chat-hf"),
     "llama-2-70b": os.path.join(MODEL_PATH, "Llama-2-70b-chat-hf"),
     "baichuan-13b": os.path.join(MODEL_PATH, "Baichuan-13B-Chat"),
     # please rename "fireballoon/baichuan-vicuna-chinese-7b" to "baichuan-7b"
     "baichuan-7b": os.path.join(MODEL_PATH, "baichuan-7b"),
     "baichuan2-7b": os.path.join(MODEL_PATH, "Baichuan2-7B-Chat"),
@@ -95,14 +97,21 @@
     "qwen-72b-chat-int4": os.path.join(MODEL_PATH, "Qwen-72B-Chat-Int4"),
     # https://huggingface.co/Qwen/Qwen-1_8B-Chat
     "qwen-1.8b-chat": os.path.join(MODEL_PATH, "Qwen-1_8B-Chat"),
     # https://huggingface.co/Qwen/Qwen-1_8B-Chat-Int8
     "qwen-1.8b-chat-int8": os.path.join(MODEL_PATH, "wen-1_8B-Chat-Int8"),
     # https://huggingface.co/Qwen/Qwen-1_8B-Chat-Int4
     "qwen-1.8b-chat-int4": os.path.join(MODEL_PATH, "Qwen-1_8B-Chat-Int4"),
+    # https://huggingface.co/Qwen/Qwen1.5-1.8B-Chat
+    "qwen1.5-1.8b-chat": os.path.join(MODEL_PATH, "Qwen1.5-1.8B-Chat"),
+    "qwen1.5-7b-chat": os.path.join(MODEL_PATH, "Qwen1.5-7B-Chat"),
+    "qwen1.5-14b-chat": os.path.join(MODEL_PATH, "Qwen1.5-14B-Chat"),
+    # https://huggingface.co/Qwen/Qwen1.5-32B-Chat
+    "qwen1.5-32b-chat": os.path.join(MODEL_PATH, "Qwen1.5-32B-Chat"),
+    "qwen1.5-72b-chat": os.path.join(MODEL_PATH, "Qwen1.5-72B-Chat"),
     # (Llama2 based) We only support WizardLM-13B-V1.2 for now, which is trained from Llama-2 13b, see https://huggingface.co/WizardLM/WizardLM-13B-V1.2
     "wizardlm-13b": os.path.join(MODEL_PATH, "WizardLM-13B-V1.2"),
     # wget https://huggingface.co/TheBloke/vicuna-13B-v1.5-GGUF/resolve/main/vicuna-13b-v1.5.Q4_K_M.gguf -O models/ggml-model-q4_0.gguf
     "llama-cpp": os.path.join(MODEL_PATH, "ggml-model-q4_0.gguf"),
     # https://huggingface.co/internlm/internlm-chat-7b-v1_1, 7b vs 7b-v1.1: https://github.com/InternLM/InternLM/issues/288
     "internlm-7b": os.path.join(MODEL_PATH, "internlm-chat-7b"),
     "internlm-7b-8k": os.path.join(MODEL_PATH, "internlm-chat-7b-8k"),
@@ -152,14 +161,15 @@
     # https://huggingface.co/01-ai/Yi-34B-Chat-4bits
     "yi-34b-chat-4bits": os.path.join(MODEL_PATH, "Yi-34B-Chat-4bits"),
     "yi-6b-chat": os.path.join(MODEL_PATH, "Yi-6B-Chat"),
     # https://huggingface.co/google/gemma-7b-it
     "gemma-7b-it": os.path.join(MODEL_PATH, "gemma-7b-it"),
     # https://huggingface.co/google/gemma-2b-it
     "gemma-2b-it": os.path.join(MODEL_PATH, "gemma-2b-it"),
+    "starling-lm-7b-beta": os.path.join(MODEL_PATH, "Starling-LM-7B-beta"),
 }
 
 EMBEDDING_MODEL_CONFIG = {
     "text2vec": os.path.join(MODEL_PATH, "text2vec-large-chinese"),
     "text2vec-base": os.path.join(MODEL_PATH, "text2vec-base-chinese"),
     # https://huggingface.co/moka-ai/m3e-large
     "m3e-base": os.path.join(MODEL_PATH, "m3e-base"),
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/_private/example_base.py` & `dbgpt-0.5.4rc0/dbgpt/core/_private/example_base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/_private/prompt_registry.py` & `dbgpt-0.5.4rc0/dbgpt/core/_private/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/dag/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/dag/dag_manager.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/dag_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         """
         from ..trigger.trigger_manager import DefaultTriggerManager
 
         super().__init__(system_app)
         self.dag_loader = LocalFileDAGLoader(dag_dirs)
         self.system_app = system_app
         self.dag_map: Dict[str, DAG] = {}
+        self.dag_alias_map: Dict[str, str] = {}
         self._trigger_manager: Optional["DefaultTriggerManager"] = None
 
     def init_app(self, system_app: SystemApp):
         """Initialize the DAGManager."""
         self.system_app = system_app
 
     def load_dags(self):
@@ -54,30 +55,47 @@
             default_component=None,
         )
 
     def after_start(self):
         """Execute after the application starts."""
         self.load_dags()
 
-    def register_dag(self, dag: DAG):
+    def register_dag(self, dag: DAG, alias_name: Optional[str] = None):
         """Register a DAG."""
         dag_id = dag.dag_id
         if dag_id in self.dag_map:
             raise ValueError(f"Register DAG error, DAG ID {dag_id} has already exist")
         self.dag_map[dag_id] = dag
+        if alias_name:
+            self.dag_alias_map[alias_name] = dag_id
 
         if self._trigger_manager:
             for trigger in dag.trigger_nodes:
                 self._trigger_manager.register_trigger(trigger, self.system_app)
             self._trigger_manager.after_register()
         else:
             logger.warning("No trigger manager, not register dag trigger")
 
     def unregister_dag(self, dag_id: str):
         """Unregister a DAG."""
         if dag_id not in self.dag_map:
             raise ValueError(f"Unregister DAG error, DAG ID {dag_id} does not exist")
         dag = self.dag_map[dag_id]
+        # Clear the alias map
+        for alias_name, _dag_id in self.dag_alias_map.items():
+            if _dag_id == dag_id:
+                del self.dag_alias_map[alias_name]
+
         if self._trigger_manager:
             for trigger in dag.trigger_nodes:
                 self._trigger_manager.unregister_trigger(trigger, self.system_app)
         del self.dag_map[dag_id]
+
+    def get_dag(
+        self, dag_id: Optional[str] = None, alias_name: Optional[str] = None
+    ) -> Optional[DAG]:
+        """Get a DAG by dag_id or alias_name."""
+        if dag_id and dag_id in self.dag_map:
+            return self.dag_map[dag_id]
+        if alias_name in self.dag_alias_map:
+            return self.dag_map.get(self.dag_alias_map[alias_name])
+        return None
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/dag/loader.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/flow/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/flow/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,29 +42,42 @@
 
     if type_name not in _TYPE_REGISTRY:
         _TYPE_REGISTRY[type_name] = type_
 
     return type_name
 
 
+def _register_alias_types(type_: Type[Any], alias_ids: Optional[List[str]] = None):
+    if alias_ids:
+        for alias_id in alias_ids:
+            if alias_id not in _TYPE_REGISTRY:
+                _TYPE_REGISTRY[alias_id] = type_
+
+
 def _get_type_cls(type_name: str) -> Type[Any]:
     """Get the type class by the type name.
 
     Args:
         type_name (str): The type name.
 
     Returns:
         Type[Any]: The type class.
 
     Raises:
         ValueError: If the type is not registered.
     """
-    if type_name not in _TYPE_REGISTRY:
+    from .compat import get_new_class_name
+
+    new_cls = get_new_class_name(type_name)
+    if type_name in _TYPE_REGISTRY:
+        return _TYPE_REGISTRY[type_name]
+    elif new_cls and new_cls in _TYPE_REGISTRY:
+        return _TYPE_REGISTRY[new_cls]
+    else:
         raise ValueError(f"Type {type_name} not registered.")
-    return _TYPE_REGISTRY[type_name]
 
 
 # Register the basic types.
 for t in _BASIC_TYPES:
     _get_type_name(t)
 
 
@@ -104,27 +117,29 @@
         """Init the category detail."""
         self.label = label
         self.description = description
 
 
 _OPERATOR_CATEGORY_DETAIL = {
     "trigger": _CategoryDetail("Trigger", "Trigger your AWEL flow"),
+    "sender": _CategoryDetail("Sender", "Send the data to the target"),
     "llm": _CategoryDetail("LLM", "Invoke LLM model"),
     "conversion": _CategoryDetail("Conversion", "Handle the conversion"),
     "output_parser": _CategoryDetail("Output Parser", "Parse the output of LLM model"),
     "common": _CategoryDetail("Common", "The common operator"),
     "agent": _CategoryDetail("Agent", "The agent operator"),
     "rag": _CategoryDetail("RAG", "The RAG operator"),
 }
 
 
 class OperatorCategory(str, Enum):
     """The category of the operator."""
 
     TRIGGER = "trigger"
+    SENDER = "sender"
     LLM = "llm"
     CONVERSION = "conversion"
     OUTPUT_PARSER = "output_parser"
     COMMON = "common"
     AGENT = "agent"
     RAG = "rag"
 
@@ -728,35 +743,45 @@
         """Pre fill the metadata."""
         if "flow_type" not in values:
             values["flow_type"] = "resource"
         if "id" not in values:
             values["id"] = values["flow_type"] + "_" + values["type_cls"]
         return values
 
+    def new_alias(self, alias: Optional[List[str]] = None) -> List[str]:
+        """Get the new alias id."""
+        if not alias:
+            return []
+        return [f"{self.flow_type}_{a}" for a in alias]
+
 
 def register_resource(
     label: str,
     name: Optional[str] = None,
     category: ResourceCategory = ResourceCategory.COMMON,
     parameters: Optional[List[Parameter]] = None,
     description: Optional[str] = None,
     resource_type: ResourceType = ResourceType.INSTANCE,
+    alias: Optional[List[str]] = None,
     **kwargs,
 ):
     """Register the resource.
 
     Args:
         label (str): The label of the resource.
         name (Optional[str], optional): The name of the resource. Defaults to None.
         category (str, optional): The category of the resource. Defaults to "common".
         parameters (Optional[List[Parameter]], optional): The parameters of the
             resource. Defaults to None.
         description (Optional[str], optional): The description of the resource.
             Defaults to None.
         resource_type (ResourceType, optional): The type of the resource.
+        alias (Optional[List[str]], optional): The alias of the resource. Defaults to
+            None. For compatibility, we can use the alias to register the resource.
+
     """
     if resource_type == ResourceType.CLASS and parameters:
         raise ValueError("Class resource can't have parameters.")
 
     def decorator(cls):
         """Wrap the class."""
         resource_description = description or cls.__doc__
@@ -778,15 +803,17 @@
             type_name=type_name,
             type_cls=type_cls,
             parameters=parameters or [],
             parent_cls=parent_cls,
             resource_type=resource_type,
             **kwargs,
         )
-        _register_resource(cls, resource_metadata)
+        alias_ids = resource_metadata.new_alias(alias)
+        _register_alias_types(cls, alias_ids)
+        _register_resource(cls, resource_metadata, alias_ids)
         # Attach the metadata to the class
         cls._resource_metadata = resource_metadata
         return cls
 
     return decorator
 
 
@@ -943,19 +970,27 @@
     """The registry of the operator and resource."""
 
     def __init__(self):
         """Init the registry."""
         self._registry: Dict[str, _RegistryItem] = {}
 
     def register_flow(
-        self, view_cls: Type, metadata: Union[ViewMetadata, ResourceMetadata]
+        self,
+        view_cls: Type,
+        metadata: Union[ViewMetadata, ResourceMetadata],
+        alias_ids: Optional[List[str]] = None,
     ):
         """Register the operator."""
         key = metadata.id
         self._registry[key] = _RegistryItem(key=key, cls=view_cls, metadata=metadata)
+        if alias_ids:
+            for alias_id in alias_ids:
+                self._registry[alias_id] = _RegistryItem(
+                    key=alias_id, cls=view_cls, metadata=metadata
+                )
 
     def get_registry_item(self, key: str) -> Optional[_RegistryItem]:
         """Get the registry item by the key."""
         return self._registry.get(key)
 
     def metadata_list(self):
         """Get the metadata list."""
@@ -992,10 +1027,14 @@
     if not item:
         raise FlowMetadataException(f"Resource {type_key} not registered.")
     if not isinstance(item.metadata, ResourceMetadata):
         raise ValueError(f"Resource {type_key} is not a ResourceMetadata.")
     return item
 
 
-def _register_resource(cls: Type, resource_metadata: ResourceMetadata):
+def _register_resource(
+    cls: Type,
+    resource_metadata: ResourceMetadata,
+    alias_ids: Optional[List[str]] = None,
+):
     """Register the operator."""
-    _OPERATOR_REGISTRY.register_flow(cls, resource_metadata)
+    _OPERATOR_REGISTRY.register_flow(cls, resource_metadata, alias_ids)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/flow/exceptions.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/flow/flow_factory.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/flow_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,19 @@
     OperatorType,
     ResourceMetadata,
     ResourceType,
     ViewMetadata,
     _get_operator_class,
     _get_resource_class,
 )
+from .compat import get_new_class_name
 from .exceptions import (
     FlowClassMetadataException,
     FlowDAGMetadataException,
+    FlowException,
     FlowMetadataException,
 )
 
 logger = logging.getLogger(__name__)
 
 
 AWEL_FLOW_VERSION = "0.1.1"
@@ -602,17 +604,34 @@
             try:
                 metadata_cls = import_from_string(node_data.type_cls)
                 logger.debug(
                     f"Import {node_data.type_cls} successfully, metadata_cls is : "
                     f"{metadata_cls}"
                 )
             except ImportError as e:
-                raise FlowClassMetadataException(
-                    f"Import {node_data.type_cls} failed: {e}"
-                )
+                raise_error = True
+                new_type_cls: Optional[str] = None
+                try:
+                    new_type_cls = get_new_class_name(node_data.type_cls)
+                    if new_type_cls:
+                        metadata_cls = import_from_string(new_type_cls)
+                        logger.info(
+                            f"Import {new_type_cls} successfully, metadata_cls is : "
+                            f"{metadata_cls}"
+                        )
+                        raise_error = False
+                except ImportError as ex:
+                    raise FlowClassMetadataException(
+                        f"Import {node_data.type_cls} with new type {new_type_cls} "
+                        f"failed: {ex}"
+                    )
+                if raise_error:
+                    raise FlowClassMetadataException(
+                        f"Import {node_data.type_cls} failed: {e}"
+                    )
 
 
 def _topological_sort(
     key_to_upstream_node: Dict[str, List[FlowNodeData]]
 ) -> Dict[str, int]:
     """Topological sort.
 
@@ -716,9 +735,9 @@
                     new_param = parameters_map[param.name]
                     param.label = new_param.label
                     param.description = new_param.description
                     param.options = new_param.get_dict_options()  # type: ignore
                     param.default = new_param.default
                     param.placeholder = new_param.placeholder
 
-        except ValueError as e:
+        except (FlowException, ValueError) as e:
             logger.warning(f"Unable to fill the flow panel: {e}")
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/operators/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/operators/common_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/common_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/operators/stream_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/stream_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/runner/job_manager.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/runner/job_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/runner/local_runner.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/task/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/task/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/task/task_impl.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/task/task_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/http_trigger.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/http_trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1032,15 +1032,15 @@
         dict_value = request_body.dict()
         if not self._key:
             return dict_value
         else:
             keys = self._key.split(".")
             for k in keys:
                 dict_value = dict_value[k]
-            if isinstance(dict_value, dict):
+            if not isinstance(dict_value, dict):
                 raise ValueError(
                     f"Prefix key {self._key} is not a valid key of the request body"
                 )
             return dict_value
 
 
 class UserInputParsedOperator(MapOperator[CommonLLMHttpRequestBody, Dict[str, Any]]):
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/iterator_trigger.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/iterator_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/trigger/trigger_manager.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/awel/util/parameter_util.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/util/parameter_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/cache.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/embeddings.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/evaluation.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/knowledge.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/llm.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -853,7 +853,35 @@
         model_metadata_key = f"____$llm_client_models_metadata_{model}$____"
         if model_metadata_key not in self.cache:
             await self.cached_models()
         model_metadata = self.cache.get(model_metadata_key)
         if not model_metadata:
             raise ValueError(f"Model {model} not found")
         return model_metadata
+
+    def __call__(self, *args, **kwargs) -> ModelOutput:
+        """Return the model output.
+
+        Call the LLM client to generate the response for the given message.
+
+        Please do not use this method in the production environment, it is only used
+        for debugging.
+        """
+        from dbgpt.util import get_or_create_event_loop
+
+        messages = kwargs.get("messages")
+        model = kwargs.get("model")
+        if messages:
+            del kwargs["messages"]
+            model_messages = ModelMessage.from_openai_messages(messages)
+        else:
+            model_messages = [ModelMessage.build_human_message(args[0])]
+        if not model:
+            if hasattr(self, "default_model"):
+                model = getattr(self, "default_model")
+            else:
+                raise ValueError("The default model is not set")
+        if "model" in kwargs:
+            del kwargs["model"]
+        req = ModelRequest.build_request(model, model_messages, **kwargs)
+        loop = get_or_create_event_loop()
+        return loop.run_until_complete(self.generate(req))
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/message.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/message.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/operators/composer_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/operators/llm_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/operators/message_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/message_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/operators/prompt_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/prompt_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/operators/retriever.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/output_parser.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/output_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,16 @@
             for i in range(len(tmp_resp)):
                 if tmp_resp[i].find("assistant:") != -1:
                     last_index = i
             ai_response = tmp_resp[last_index]
             ai_response = ai_response.replace("assistant:", "")
             ai_response = ai_response.replace("Assistant:", "")
             ai_response = ai_response.replace("ASSISTANT:", "")
-            ai_response = ai_response.replace("\_", "_")
-            ai_response = ai_response.replace("\*", "*")
+            ai_response = ai_response.replace("\\_", "_")
+            ai_response = ai_response.replace("\\*", "*")
             ai_response = ai_response.replace("\t", "")
 
             # ai_response = ai_response.strip().replace("\\n", " ").replace("\n", " ")
             print("un_stream ai response:", ai_response)
             return ai_response
         else:
             raise ValueError(
@@ -230,15 +230,15 @@
             return model_out_text
 
         cleaned_output = (
             cleaned_output.strip()
             .replace("\\n", " ")
             .replace("\n", " ")
             .replace("\\", " ")
-            .replace("\_", "_")
+            .replace("\\_", "_")
         )
         cleaned_output = self._illegal_json_ends(cleaned_output)
         return cleaned_output
 
     def parse_view_response(
         self, ai_text, data, parse_prompt_response: Any = None
     ) -> str:
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/prompt.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/prompt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/serialization.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/interface/storage.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/operators/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/operators/flow/composer_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/operators/flow/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/operators/flow/dict_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/operators/flow/dict_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/core/schema/api.py` & `dbgpt-0.5.4rc0/dbgpt/core/schema/api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/base.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/conn_spark.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/conn_spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/db_conn_info.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/db_conn_info.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/manages/connector_manager.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/manages/connector_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/operators/datasource_operator.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/operators/datasource_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/base.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_clickhouse.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_clickhouse.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_doris.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_doris.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_duckdb.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_duckdb.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_hive.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_hive.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_mssql.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mssql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_postgresql.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_postgresql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_sqlite.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_sqlite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/conn_starrocks.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_starrocks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/base.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/embeddings_loader.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/embeddings_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/fschat_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/fschat_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/hf_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/hf_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -189,11 +189,90 @@
         return (
             lower_model_name_or_path
             and "gemma-" in lower_model_name_or_path
             and "it" in lower_model_name_or_path
         )
 
 
+class StarlingLMAdapter(NewHFChatModelAdapter):
+    """
+    https://huggingface.co/Nexusflow/Starling-LM-7B-beta
+    """
+
+    support_4bit: bool = True
+    support_8bit: bool = True
+    support_system_message: bool = False
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "starling-" in lower_model_name_or_path
+            and "lm" in lower_model_name_or_path
+        )
+
+    def get_str_prompt(
+        self,
+        params: Dict,
+        messages: List[ModelMessage],
+        tokenizer: Any,
+        prompt_template: str = None,
+        convert_to_compatible_format: bool = False,
+    ) -> Optional[str]:
+        str_prompt = super().get_str_prompt(
+            params,
+            messages,
+            tokenizer,
+            prompt_template,
+            convert_to_compatible_format,
+        )
+        chat_mode = None
+        if params and "context" in params and "chat_mode" in params["context"]:
+            chat_mode = params["context"].get("chat_mode")
+        if chat_mode in [
+            "chat_dashboard",
+            "chat_with_db_execute",
+            "excel_learning",
+            "chat_excel",
+        ]:
+            # Coding conversation, use code prompt
+            # This is a temporary solution, we should use a better way to distinguish the conversation type
+            # https://huggingface.co/Nexusflow/Starling-LM-7B-beta#code-examples
+            str_prompt = str_prompt.replace("GPT4 Correct User:", "Code User:").replace(
+                "GPT4 Correct Assistant:", "Code Assistant:"
+            )
+            logger.info(
+                f"Use code prompt for chat_mode: {chat_mode}, transform 'GPT4 Correct User:' to 'Code User:' "
+                "and 'GPT4 Correct Assistant:' to 'Code Assistant:'"
+            )
+        return str_prompt
+
+
+class QwenAdapter(NewHFChatModelAdapter):
+    """
+    https://huggingface.co/Qwen/Qwen1.5-32B-Chat
+
+    TODO: There are problems with quantization.
+    """
+
+    support_4bit: bool = True
+    support_8bit: bool = False  # TODO: Support 8bit quantization
+
+    def check_transformer_version(self, current_version: str) -> None:
+        if not current_version >= "4.37.0":
+            raise ValueError(
+                "Qwen 1.5 require transformers.__version__>=4.37.0, please upgrade your transformers package."
+            )
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "qwen" in lower_model_name_or_path
+            and "1.5" in lower_model_name_or_path
+        )
+
+
 register_model_adapter(YiAdapter)
 register_model_adapter(Mixtral8x7BAdapter)
 register_model_adapter(SOLARAdapter)
 register_model_adapter(GemmaAdapter)
+register_model_adapter(StarlingLMAdapter)
+register_model_adapter(QwenAdapter)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/loader.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/model_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/model_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/old_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/old_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,15 +359,15 @@
             model_paths = list(path.glob("*ggml*.gguf"))
             if not model_paths:
                 return False, None
             model_path = str(model_paths[0])
             logger.warn(
                 f"Model path {model_path} is not single file, use first *gglm*.gguf model file: {model_path}"
             )
-        if not re.fullmatch(".*ggml.*\.gguf", model_path):
+        if not re.fullmatch(r".*ggml.*\.gguf", model_path):
             return False, None
         return True, model_path
 
     def model_type(self) -> ModelType:
         return ModelType.LLAMA_CPP
 
     def match(self, model_path: str):
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/proxy_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/proxy_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,16 +248,42 @@
 
     def get_async_generate_stream_function(self, model, model_path: str):
         from dbgpt.model.proxy.llms.yi import yi_generate_stream
 
         return yi_generate_stream
 
 
+class MoonshotProxyLLMModelAdapter(ProxyLLMModelAdapter):
+    """Moonshot proxy LLM model adapter.
+
+    See Also: `Moonshot Documentation <https://platform.moonshot.cn/docs/>`_
+    """
+
+    def support_async(self) -> bool:
+        return True
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return lower_model_name_or_path in ["moonshot_proxyllm"]
+
+    def get_llm_client_class(
+        self, params: ProxyModelParameters
+    ) -> Type[ProxyLLMClient]:
+        from dbgpt.model.proxy.llms.moonshot import MoonshotLLMClient
+
+        return MoonshotLLMClient
+
+    def get_async_generate_stream_function(self, model, model_path: str):
+        from dbgpt.model.proxy.llms.moonshot import moonshot_generate_stream
+
+        return moonshot_generate_stream
+
+
 register_model_adapter(OpenAIProxyLLMModelAdapter)
 register_model_adapter(TongyiProxyLLMModelAdapter)
 register_model_adapter(ZhipuProxyLLMModelAdapter)
 register_model_adapter(WenxinProxyLLMModelAdapter)
 register_model_adapter(GeminiProxyLLMModelAdapter)
 register_model_adapter(SparkProxyLLMModelAdapter)
 register_model_adapter(BardProxyLLMModelAdapter)
 register_model_adapter(BaichuanProxyLLMModelAdapter)
 register_model_adapter(YiProxyLLMModelAdapter)
+register_model_adapter(MoonshotProxyLLMModelAdapter)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/template.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/adapter/vllm_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/vllm_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/base.py` & `dbgpt-0.5.4rc0/dbgpt/model/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/cli.py` & `dbgpt-0.5.4rc0/dbgpt/model/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/operators/llm_operator.py` & `dbgpt-0.5.4rc0/dbgpt/model/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/parameter.py` & `dbgpt-0.5.4rc0/dbgpt/model/parameter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         "OpenAILLMClient": "dbgpt.model.proxy.llms.chatgpt",
         "GeminiLLMClient": "dbgpt.model.proxy.llms.gemini",
         "SparkLLMClient": "dbgpt.model.proxy.llms.spark",
         "TongyiLLMClient": "dbgpt.model.proxy.llms.tongyi",
         "WenxinLLMClient": "dbgpt.model.proxy.llms.wenxin",
         "ZhipuLLMClient": "dbgpt.model.proxy.llms.zhipu",
         "YiLLMClient": "dbgpt.model.proxy.llms.yi",
+        "MoonshotLLMClient": "dbgpt.model.proxy.llms.moonshot",
     }
 
     if name in module_path:
         module = __import__(module_path[name], fromlist=[name])
         return getattr(module, name)
     else:
         raise AttributeError(f"module {__name__} has no attribute {name}")
@@ -27,8 +28,9 @@
     "OpenAILLMClient",
     "GeminiLLMClient",
     "TongyiLLMClient",
     "ZhipuLLMClient",
     "WenxinLLMClient",
     "SparkLLMClient",
     "YiLLMClient",
+    "MoonshotLLMClient",
 ]
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/base.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/baichuan.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/bard.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/bard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/chatgpt.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,16 @@
         except ImportError as exc:
             raise ValueError(
                 "Could not import python package: openai "
                 "Please install openai by command `pip install openai"
             ) from exc
         self._openai_version = metadata.version("openai")
         self._openai_less_then_v1 = not self._openai_version >= "1.0.0"
+        self.check_sdk_version(self._openai_version)
+
         self._init_params = OpenAIParameters(
             api_type=api_type,
             api_base=api_base,
             api_key=api_key,
             api_version=api_version,
             proxies=proxies,
             full_url=kwargs.get("full_url"),
@@ -137,14 +139,22 @@
             model=model_params.proxyllm_backend,
             proxies=model_params.http_proxy,
             model_alias=model_params.model_name,
             context_length=max(model_params.max_context_size, 8192),
             full_url=model_params.proxy_server_url,
         )
 
+    def check_sdk_version(self, version: str) -> None:
+        """Check the sdk version of the client.
+
+        Raises:
+            ValueError: If check failed.
+        """
+        pass
+
     @property
     def client(self) -> ClientType:
         if self._openai_less_then_v1:
             raise ValueError(
                 "Current model (Load by OpenAILLMClient) require openai.__version__>=1.0.0"
             )
         if self._client is None:
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/gemini.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/gemini.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/proxy_model.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/proxy_model.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/spark.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/tongyi.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/wenxin.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/wenxin.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/yi.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/yi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/proxy/llms/zhipu.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/utils/chatgpt_utils.py` & `dbgpt-0.5.4rc0/dbgpt/model/utils/chatgpt_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/utils/llm_utils.py` & `dbgpt-0.5.4rc0/dbgpt/model/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/model/utils/token_utils.py` & `dbgpt-0.5.4rc0/dbgpt/model/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/assembler/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/assembler/db_schema.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/assembler/embedding.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/assembler/summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/chunk_manager.py` & `dbgpt-0.5.4rc0/dbgpt/rag/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/embedding/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/embedding/_wrapped.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/_wrapped.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/embedding/embedding_factory.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/embedding/embeddings.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/evaluation/retriever.py` & `dbgpt-0.5.4rc0/dbgpt/rag/evaluation/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/extractor/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/extractor/summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/extractor/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for Knowledge Base."""
 
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Any, List, Optional, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from dbgpt.core import Document
 from dbgpt.rag.text_splitter.text_splitter import (
     MarkdownHeaderTextSplitter,
     PageTextSplitter,
     ParagraphTextSplitter,
     RecursiveCharacterTextSplitter,
@@ -143,44 +143,46 @@
 class Knowledge(ABC):
     """Knowledge Base Class."""
 
     def __init__(
         self,
         path: Optional[str] = None,
         knowledge_type: Optional[KnowledgeType] = None,
-        data_loader: Optional[Any] = None,
+        loader: Optional[Any] = None,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize with Knowledge arguments."""
         self._path = path
         self._type = knowledge_type
-        self._data_loader = data_loader
+        self._loader = loader
+        self._metadata = metadata
 
     def load(self) -> List[Document]:
-        """Load knowledge from data_loader."""
+        """Load knowledge from data loader."""
         documents = self._load()
         return self._postprocess(documents)
 
     @classmethod
     @abstractmethod
     def type(cls) -> KnowledgeType:
         """Get knowledge type."""
 
     @classmethod
     def document_type(cls) -> Any:
         """Get document type."""
         return None
 
     def _postprocess(self, docs: List[Document]) -> List[Document]:
-        """Post process knowledge from data_loader."""
+        """Post process knowledge from data loader."""
         return docs
 
     @abstractmethod
     def _load(self) -> List[Document]:
-        """Preprocess knowledge from data_loader."""
+        """Preprocess knowledge from data loader."""
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return supported chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
             ChunkStrategy.CHUNK_BY_PAGE,
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/csv.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """CSV Knowledge."""
 import csv
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
     Knowledge,
     KnowledgeType,
@@ -17,28 +17,33 @@
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
         source_column: Optional[str] = None,
         encoding: Optional[str] = "utf-8",
         loader: Optional[Any] = None,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Create CSV Knowledge with Knowledge arguments.
 
         Args:
             file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
             source_column(str, optional): source column
             encoding(str, optional): csv encoding
             loader(Any, optional): loader
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
         self._encoding = encoding
         self._source_column = source_column
 
     def _load(self) -> List[Document]:
         """Load csv document from loader."""
         if self._loader:
             documents = self._loader.load()
@@ -63,14 +68,16 @@
                         )
                     except KeyError:
                         raise ValueError(
                             f"Source column '{self._source_column}' not in CSV "
                             f"file."
                         )
                     metadata = {"source": source, "row": i}
+                    if self._metadata:
+                        metadata.update(self._metadata)  # type: ignore
                     doc = Document(content=content, metadata=metadata)
                     docs.append(doc)
 
             return docs
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/datasource.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/datasource.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Datasource Knowledge."""
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
 from dbgpt.datasource import BaseConnector
 
 from ..summary.rdbms_db_summary import _parse_db_summary
 from .base import ChunkStrategy, DocumentType, Knowledge, KnowledgeType
 
@@ -12,34 +12,37 @@
     """Datasource Knowledge."""
 
     def __init__(
         self,
         connector: BaseConnector,
         summary_template: str = "{table_name}({columns})",
         knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Create Datasource Knowledge with Knowledge arguments.
 
         Args:
-            path(str,  optional): file path
+            connector(BaseConnector): connector
+            summary_template(str, optional): summary template
             knowledge_type(KnowledgeType, optional): knowledge type
-            data_loader(Any, optional): loader
+            metadata(Dict[str, Union[str, List[str]], optional): metadata
         """
         self._connector = connector
         self._summary_template = summary_template
-        super().__init__(knowledge_type=knowledge_type, **kwargs)
+        super().__init__(knowledge_type=knowledge_type, metadata=metadata, **kwargs)
 
     def _load(self) -> List[Document]:
         """Load datasource document from data_loader."""
         docs = []
         for table_summary in _parse_db_summary(self._connector, self._summary_template):
-            docs.append(
-                Document(content=table_summary, metadata={"source": "database"})
-            )
+            metadata = {"source": "database"}
+            if self._metadata:
+                metadata.update(self._metadata)  # type: ignore
+            docs.append(Document(content=table_summary, metadata=metadata))
         return docs
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/docx.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/url.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,66 @@
-"""Docx Knowledge."""
+"""URL Knowledge."""
 from typing import Any, List, Optional
 
-import docx
-
 from dbgpt.core import Document
-from dbgpt.rag.knowledge.base import (
-    ChunkStrategy,
-    DocumentType,
-    Knowledge,
-    KnowledgeType,
-)
+from dbgpt.rag.knowledge.base import ChunkStrategy, Knowledge, KnowledgeType
 
 
-class DocxKnowledge(Knowledge):
-    """Docx Knowledge."""
+class URLKnowledge(Knowledge):
+    """URL Knowledge."""
 
     def __init__(
         self,
-        file_path: Optional[str] = None,
-        knowledge_type: Any = KnowledgeType.DOCUMENT,
+        url: str = "",
+        knowledge_type: KnowledgeType = KnowledgeType.URL,
+        source_column: Optional[str] = None,
         encoding: Optional[str] = "utf-8",
         loader: Optional[Any] = None,
         **kwargs: Any,
     ) -> None:
-        """Create Docx Knowledge with Knowledge arguments.
+        """Create URL Knowledge with Knowledge arguments.
 
         Args:
-            file_path(str,  optional): file path
+            url(str,  optional): url
             knowledge_type(KnowledgeType, optional): knowledge type
+            source_column(str, optional): source column
             encoding(str, optional): csv encoding
             loader(Any, optional): loader
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=url, knowledge_type=knowledge_type, loader=loader, **kwargs
+        )
         self._encoding = encoding
+        self._source_column = source_column
 
     def _load(self) -> List[Document]:
-        """Load docx document from loader."""
+        """Fetch URL document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
-            docs = []
-            doc = docx.Document(self._path)
-            content = []
-            for i in range(len(doc.paragraphs)):
-                para = doc.paragraphs[i]
-                text = para.text
-                content.append(text)
-            docs.append(
-                Document(content="\n".join(content), metadata={"source": self._path})
-            )
-            return docs
+            from langchain.document_loaders import WebBaseLoader
+
+            if self._path is not None:
+                web_reader = WebBaseLoader(web_path=self._path)
+                documents = web_reader.load()
+            else:
+                # Handle the case where self._path is None
+                raise ValueError("web_path cannot be None")
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
-            ChunkStrategy.CHUNK_BY_PARAGRAPH,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
         ]
 
     @classmethod
     def default_chunk_strategy(cls) -> ChunkStrategy:
         """Return default chunk strategy."""
         return ChunkStrategy.CHUNK_BY_SIZE
 
     @classmethod
-    def type(cls) -> KnowledgeType:
+    def type(cls):
         """Return knowledge type."""
-        return KnowledgeType.DOCUMENT
-
-    @classmethod
-    def document_type(cls) -> DocumentType:
-        """Return document type."""
-        return DocumentType.DOCX
+        return KnowledgeType.URL
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/factory.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 """Knowledge Factory to create knowledge from file path and url."""
-from typing import List, Optional, Type
+from typing import Dict, List, Optional, Type, Union
 
 from dbgpt.rag.knowledge.base import Knowledge, KnowledgeType
 from dbgpt.rag.knowledge.string import StringKnowledge
 from dbgpt.rag.knowledge.url import URLKnowledge
 
 
 class KnowledgeFactory:
     """Knowledge Factory to create knowledge from file path and url."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
     ):
         """Create Knowledge Factory with file path and knowledge type.
 
         Args:
             file_path(str, optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
         """
         self._file_path = file_path
         self._knowledge_type = knowledge_type
+        self._metadata = metadata
 
     @classmethod
     def create(
         cls,
         datasource: str = "",
         knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
     ):
         """Create knowledge from file path, url or text.
 
         Args:
              datasource: path of the file to convert
              knowledge_type: type of knowledge
+             metadata: Optional[Dict[str, Union[str, List[str]]]]
 
         Examples:
             .. code-block:: python
 
                 from dbgpt.rag.knowledge.factory import KnowledgeFactory
 
                 url_knowlege = KnowledgeFactory.create(
@@ -48,28 +52,33 @@
                     knowledge_type=KnowledgeType.DOCUMENT,
                 )
 
         """
         match knowledge_type:
             case KnowledgeType.DOCUMENT:
                 return cls.from_file_path(
-                    file_path=datasource, knowledge_type=knowledge_type
+                    file_path=datasource,
+                    knowledge_type=knowledge_type,
+                    metadata=metadata,
                 )
             case KnowledgeType.URL:
                 return cls.from_url(url=datasource, knowledge_type=knowledge_type)
             case KnowledgeType.TEXT:
-                return cls.from_text(text=datasource, knowledge_type=knowledge_type)
+                return cls.from_text(
+                    text=datasource, knowledge_type=knowledge_type, metadata=metadata
+                )
             case _:
                 raise Exception(f"Unsupported knowledge type '{knowledge_type}'")
 
     @classmethod
     def from_file_path(
         cls,
         file_path: str = "",
         knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
     ) -> Knowledge:
         """Create knowledge from path.
 
         Args:
             param file_path: path of the file to convert
             param knowledge_type: type of knowledge
 
@@ -78,18 +87,19 @@
 
                 from dbgpt.rag.knowledge.factory import KnowledgeFactory
 
                 doc_knowlege = KnowledgeFactory.create(
                     datasource="path/to/document.pdf",
                     knowledge_type=KnowledgeType.DOCUMENT,
                 )
+
         """
         factory = cls(file_path=file_path, knowledge_type=knowledge_type)
         return factory._select_document_knowledge(
-            file_path=file_path, knowledge_type=knowledge_type
+            file_path=file_path, knowledge_type=knowledge_type, metadata=metadata
         )
 
     @staticmethod
     def from_url(
         url: str = "",
         knowledge_type: KnowledgeType = KnowledgeType.URL,
     ) -> Knowledge:
@@ -113,24 +123,26 @@
             knowledge_type=knowledge_type,
         )
 
     @staticmethod
     def from_text(
         text: str = "",
         knowledge_type: KnowledgeType = KnowledgeType.TEXT,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
     ) -> Knowledge:
         """Create knowledge from text.
 
         Args:
             param text: text to convert
             param knowledge_type: type of knowledge
         """
         return StringKnowledge(
             text=text,
             knowledge_type=knowledge_type,
+            metadata=metadata,
         )
 
     def _select_document_knowledge(self, **kwargs):
         """Select document knowledge from file path."""
         extension = self._file_path.rsplit(".", 1)[-1]
         knowledge_classes = self._get_knowledge_subclasses()
         implementation = None
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/html.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """HTML Knowledge."""
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import chardet
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
@@ -16,26 +16,31 @@
     """HTML Knowledge."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
         loader: Optional[Any] = None,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Create HTML Knowledge with Knowledge arguments.
 
         Args:
             file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
             loader(Any, optional): loader
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
 
     def _load(self) -> List[Document]:
         """Load html document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
             if not self._path:
@@ -44,14 +49,16 @@
                 raw_text = f.read()
                 result = chardet.detect(raw_text)
                 if result["encoding"] is None:
                     text = raw_text.decode("utf-8")
                 else:
                     text = raw_text.decode(result["encoding"])
             metadata = {"source": self._path}
+            if self._metadata:
+                metadata.update(self._metadata)  # type: ignore
             return [Document(content=text, metadata=metadata)]
 
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     def _postprocess(self, documents: List[Document]):
         import markdown
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/markdown.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/docx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,85 @@
-"""Markdown Knowledge."""
-from typing import Any, List, Optional
+"""Docx Knowledge."""
+from typing import Any, Dict, List, Optional, Union
+
+import docx
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
     Knowledge,
     KnowledgeType,
 )
 
 
-class MarkdownKnowledge(Knowledge):
-    """Markdown Knowledge."""
+class DocxKnowledge(Knowledge):
+    """Docx Knowledge."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
-        knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
+        knowledge_type: Any = KnowledgeType.DOCUMENT,
         encoding: Optional[str] = "utf-8",
         loader: Optional[Any] = None,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create Markdown Knowledge with Knowledge arguments.
+        """Create Docx Knowledge with Knowledge arguments.
 
         Args:
             file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
             encoding(str, optional): csv encoding
             loader(Any, optional): loader
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
         self._encoding = encoding
 
     def _load(self) -> List[Document]:
-        """Load markdown document from loader."""
+        """Load docx document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
-            if not self._path:
-                raise ValueError("file path is required")
-            with open(self._path, encoding=self._encoding, errors="ignore") as f:
-                markdown_text = f.read()
-                metadata = {"source": self._path}
-                documents = [Document(content=markdown_text, metadata=metadata)]
-                return documents
+            docs = []
+            doc = docx.Document(self._path)
+            content = []
+            for i in range(len(doc.paragraphs)):
+                para = doc.paragraphs[i]
+                text = para.text
+                content.append(text)
+            metadata = {"source": self._path}
+            if self._metadata:
+                metadata.update(self._metadata)  # type: ignore
+            docs.append(Document(content="\n".join(content), metadata=metadata))
+            return docs
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
-            ChunkStrategy.CHUNK_BY_MARKDOWN_HEADER,
+            ChunkStrategy.CHUNK_BY_PARAGRAPH,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
         ]
 
     @classmethod
     def default_chunk_strategy(cls) -> ChunkStrategy:
         """Return default chunk strategy."""
-        return ChunkStrategy.CHUNK_BY_MARKDOWN_HEADER
+        return ChunkStrategy.CHUNK_BY_SIZE
 
     @classmethod
     def type(cls) -> KnowledgeType:
         """Return knowledge type."""
         return KnowledgeType.DOCUMENT
 
     @classmethod
     def document_type(cls) -> DocumentType:
         """Return document type."""
-        return DocumentType.MARKDOWN
+        return DocumentType.DOCX
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/pdf.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """PDF Knowledge."""
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
     Knowledge,
     KnowledgeType,
@@ -15,27 +15,32 @@
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
         loader: Optional[Any] = None,
         language: Optional[str] = "zh",
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Create PDF Knowledge with Knowledge arguments.
 
         Args:
             file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
             loader(Any, optional): loader
             language(str, optional): language
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
         self._language = language
 
     def _load(self) -> List[Document]:
         """Load pdf document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
@@ -61,14 +66,16 @@
                         words = list(line)  # noqa: F841
                     else:
                         words = line.split()  # noqa: F841
                     cleaned_lines.append(line)
                 page = "\n".join(cleaned_lines)
                 # cleaned_pages.append(page)
                 metadata = {"source": self._path, "page": page_num}
+                if self._metadata:
+                    metadata.update(self._metadata)  # type: ignore
                 # text = "\f".join(cleaned_pages)
                 document = Document(content=page, metadata=metadata)
                 documents.append(document)
             return documents
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/pptx.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pptx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """PPTX Knowledge."""
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
     Knowledge,
     KnowledgeType,
@@ -15,26 +15,31 @@
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
         loader: Optional[Any] = None,
         language: Optional[str] = "zh",
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Create PPTX knowledge with PDF Knowledge arguments.
 
         Args:
             file_path:(Optional[str]) file path
             knowledge_type:(KnowledgeType) knowledge type
             loader:(Optional[Any]) loader
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
         self._language = language
 
     def _load(self) -> List[Document]:
         """Load pdf document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
@@ -43,17 +48,18 @@
             pr = Presentation(self._path)
             docs = []
             for slide in pr.slides:
                 content = ""
                 for shape in slide.shapes:
                     if hasattr(shape, "text") and shape.text:
                         content += shape.text
-                docs.append(
-                    Document(content=content, metadata={"source": slide.slide_id})
-                )
+                metadata = {"source": self._path}
+                if self._metadata:
+                    metadata.update(self._metadata)  # type: ignore
+                docs.append(Document(content=content, metadata=metadata))
             return docs
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy.
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/txt.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/txt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """TXT Knowledge."""
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import chardet
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import (
     ChunkStrategy,
     DocumentType,
@@ -16,26 +16,31 @@
     """TXT Knowledge."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         knowledge_type: KnowledgeType = KnowledgeType.DOCUMENT,
         loader: Optional[Any] = None,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
         """Create TXT Knowledge with Knowledge arguments.
 
         Args:
             file_path(str,  optional): file path
             knowledge_type(KnowledgeType, optional): knowledge type
             loader(Any, optional): loader
         """
-        self._path = file_path
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            path=file_path,
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
 
     def _load(self) -> List[Document]:
         """Load txt document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
             if not self._path:
@@ -44,14 +49,16 @@
                 raw_text = f.read()
                 result = chardet.detect(raw_text)
                 if result["encoding"] is None:
                     text = raw_text.decode("utf-8")
                 else:
                     text = raw_text.decode(result["encoding"])
             metadata = {"source": self._path}
+            if self._metadata:
+                metadata.update(self._metadata)  # type: ignore
             return [Document(content=text, metadata=metadata)]
 
         return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
     def support_chunk_strategy(cls):
         """Return support chunk strategy."""
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/knowledge/url.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/string.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,50 @@
-"""URL Knowledge."""
-from typing import Any, List, Optional
+"""String Knowledge."""
+from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import ChunkStrategy, Knowledge, KnowledgeType
 
 
-class URLKnowledge(Knowledge):
-    """URL Knowledge."""
+class StringKnowledge(Knowledge):
+    """String Knowledge."""
 
     def __init__(
         self,
-        url: str = "",
-        knowledge_type: KnowledgeType = KnowledgeType.URL,
-        source_column: Optional[str] = None,
+        text: str = "",
+        knowledge_type: KnowledgeType = KnowledgeType.TEXT,
         encoding: Optional[str] = "utf-8",
         loader: Optional[Any] = None,
+        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create URL Knowledge with Knowledge arguments.
+        """Create String knowledge parameters.
 
         Args:
-            url(str,  optional): url
-            knowledge_type(KnowledgeType, optional): knowledge type
-            source_column(str, optional): source column
-            encoding(str, optional): csv encoding
-            loader(Any, optional): loader
+            text(str): text
+            knowledge_type(KnowledgeType): knowledge type
+            encoding(str): encoding
+            loader(Any): loader
         """
-        self._path = url or None
-        self._type = knowledge_type
-        self._loader = loader
+        super().__init__(
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
+        self._text = text
         self._encoding = encoding
-        self._source_column = source_column
 
     def _load(self) -> List[Document]:
-        """Fetch URL document from loader."""
-        if self._loader:
-            documents = self._loader.load()
-        else:
-            from langchain.document_loaders import WebBaseLoader
-
-            if self._path is not None:
-                web_reader = WebBaseLoader(web_path=self._path)
-                documents = web_reader.load()
-            else:
-                # Handle the case where self._path is None
-                raise ValueError("web_path cannot be None")
-        return [Document.langchain2doc(lc_document) for lc_document in documents]
+        """Load raw text from loader."""
+        metadata = {"source": "raw text"}
+        if self._metadata:
+            metadata.update(self._metadata)  # type: ignore
+        docs = [Document(content=self._text, metadata=metadata)]
+        return docs
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
@@ -59,8 +54,8 @@
     def default_chunk_strategy(cls) -> ChunkStrategy:
         """Return default chunk strategy."""
         return ChunkStrategy.CHUNK_BY_SIZE
 
     @classmethod
     def type(cls):
         """Return knowledge type."""
-        return KnowledgeType.URL
+        return KnowledgeType.TEXT
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/assembler.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/assembler.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/datasource.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/db_schema.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/embedding.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/evaluation.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/knowledge.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/rerank.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/rewrite.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/schema_linking.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/operators/summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/retriever/db_schema.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/db_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from dbgpt.core import Chunk
 from dbgpt.datasource.base import BaseConnector
 from dbgpt.rag.retriever.base import BaseRetriever
 from dbgpt.rag.retriever.rerank import DefaultRanker, Ranker
 from dbgpt.rag.summary.rdbms_db_summary import _parse_db_summary
 from dbgpt.storage.vector_store.connector import VectorStoreConnector
+from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.chat_util import run_async_tasks
 
 
 class DBSchemaRetriever(BaseRetriever):
     """DBSchema retriever."""
 
     def __init__(
@@ -89,60 +90,72 @@
         self._query_rewrite = query_rewrite
         self._vector_store_connector = vector_store_connector
         self._need_embeddings = False
         if self._vector_store_connector:
             self._need_embeddings = True
         self._rerank = rerank or DefaultRanker(self._top_k)
 
-    def _retrieve(self, query: str) -> List[Chunk]:
+    def _retrieve(
+        self, query: str, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
         Args:
             query (str): query text
+            filters: metadata filters.
 
         Returns:
             List[Chunk]: list of chunks
         """
         if self._need_embeddings:
             queries = [query]
             candidates = [
-                self._vector_store_connector.similar_search(query, self._top_k)
+                self._vector_store_connector.similar_search(query, self._top_k, filters)
                 for query in queries
             ]
             return cast(List[Chunk], reduce(lambda x, y: x + y, candidates))
         else:
             if not self._connector:
                 raise RuntimeError("RDBMSConnector connection is required.")
             table_summaries = _parse_db_summary(self._connector)
             return [Chunk(content=table_summary) for table_summary in table_summaries]
 
-    def _retrieve_with_score(self, query: str, score_threshold: float) -> List[Chunk]:
+    def _retrieve_with_score(
+        self,
+        query: str,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
+    ) -> List[Chunk]:
         """Retrieve knowledge chunks with score.
 
         Args:
             query (str): query text
             score_threshold (float): score threshold
+            filters: metadata filters.
 
         Returns:
             List[Chunk]: list of chunks
         """
-        return self._retrieve(query)
+        return self._retrieve(query, filters)
 
-    async def _aretrieve(self, query: str) -> List[Chunk]:
+    async def _aretrieve(
+        self, query: str, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
         Args:
             query (str): query text
+            filters: metadata filters.
 
         Returns:
             List[Chunk]: list of chunks
         """
         if self._need_embeddings:
             queries = [query]
-            candidates = [self._similarity_search(query) for query in queries]
+            candidates = [self._similarity_search(query, filters) for query in queries]
             result_candidates = await run_async_tasks(
                 tasks=candidates, concurrency_limit=1
             )
             return result_candidates
         else:
             from dbgpt.rag.summary.rdbms_db_summary import (  # noqa: F401
                 _parse_db_summary,
@@ -150,30 +163,33 @@
 
             table_summaries = await run_async_tasks(
                 tasks=[self._aparse_db_summary()], concurrency_limit=1
             )
             return [Chunk(content=table_summary) for table_summary in table_summaries]
 
     async def _aretrieve_with_score(
-        self, query: str, score_threshold: float
+        self,
+        query: str,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
     ) -> List[Chunk]:
         """Retrieve knowledge chunks with score.
 
         Args:
             query (str): query text
             score_threshold (float): score threshold
+            filters: metadata filters.
         """
-        return await self._aretrieve(query)
+        return await self._aretrieve(query, filters)
 
-    async def _similarity_search(self, query) -> List[Chunk]:
+    async def _similarity_search(
+        self, query, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Similar search."""
-        return self._vector_store_connector.similar_search(
-            query,
-            self._top_k,
-        )
+        return self._vector_store_connector.similar_search(query, self._top_k, filters)
 
     async def _aparse_db_summary(self) -> List[str]:
         """Similar search."""
         from dbgpt.rag.summary.rdbms_db_summary import _parse_db_summary
 
         if not self._connector:
             raise RuntimeError("RDBMSConnector connection is required.")
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/retriever/embedding.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/embedding.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List, Optional, cast
 
 from dbgpt.core import Chunk
 from dbgpt.rag.retriever.base import BaseRetriever
 from dbgpt.rag.retriever.rerank import DefaultRanker, Ranker
 from dbgpt.rag.retriever.rewrite import QueryRewrite
 from dbgpt.storage.vector_store.connector import VectorStoreConnector
+from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.chat_util import run_async_tasks
 from dbgpt.util.tracer import root_tracer
 
 
 class EmbeddingRetriever(BaseRetriever):
     """Embedding retriever."""
 
@@ -61,95 +62,111 @@
                 )
         """
         self._top_k = top_k
         self._query_rewrite = query_rewrite
         self._vector_store_connector = vector_store_connector
         self._rerank = rerank or DefaultRanker(self._top_k)
 
-    def _retrieve(self, query: str) -> List[Chunk]:
+    def _retrieve(
+        self, query: str, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
         Args:
             query (str): query text
-
+            filters: metadata filters.
         Return:
             List[Chunk]: list of chunks
         """
         queries = [query]
         candidates = [
-            self._vector_store_connector.similar_search(query, self._top_k)
+            self._vector_store_connector.similar_search(query, self._top_k, filters)
             for query in queries
         ]
         res_candidates = cast(List[Chunk], reduce(lambda x, y: x + y, candidates))
         return res_candidates
 
-    def _retrieve_with_score(self, query: str, score_threshold: float) -> List[Chunk]:
+    def _retrieve_with_score(
+        self,
+        query: str,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
+    ) -> List[Chunk]:
         """Retrieve knowledge chunks with score.
 
         Args:
             query (str): query text
             score_threshold (float): score threshold
-
+            filters: metadata filters.
         Return:
             List[Chunk]: list of chunks with score
         """
         queries = [query]
         candidates_with_score = [
             self._vector_store_connector.similar_search_with_scores(
-                query, self._top_k, score_threshold
+                query, self._top_k, score_threshold, filters
             )
             for query in queries
         ]
         new_candidates_with_score = cast(
             List[Chunk], reduce(lambda x, y: x + y, candidates_with_score)
         )
         new_candidates_with_score = self._rerank.rank(new_candidates_with_score)
         return new_candidates_with_score
 
-    async def _aretrieve(self, query: str) -> List[Chunk]:
+    async def _aretrieve(
+        self, query: str, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
         Args:
-            query (str): query text
-
+            query (str): query text.
+            filters: metadata filters.
         Return:
             List[Chunk]: list of chunks
         """
         queries = [query]
         if self._query_rewrite:
-            candidates_tasks = [self._similarity_search(query) for query in queries]
+            candidates_tasks = [
+                self._similarity_search(query, filters) for query in queries
+            ]
             chunks = await self._run_async_tasks(candidates_tasks)
             context = "\n".join([chunk.content for chunk in chunks])
             new_queries = await self._query_rewrite.rewrite(
                 origin_query=query, context=context, nums=1
             )
             queries.extend(new_queries)
-        candidates = [self._similarity_search(query) for query in queries]
+        candidates = [self._similarity_search(query, filters) for query in queries]
         new_candidates = await run_async_tasks(tasks=candidates, concurrency_limit=1)
         return new_candidates
 
     async def _aretrieve_with_score(
-        self, query: str, score_threshold: float
+        self,
+        query: str,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
     ) -> List[Chunk]:
         """Retrieve knowledge chunks with score.
 
         Args:
             query (str): query text
             score_threshold (float): score threshold
-
+            filters: metadata filters.
         Return:
             List[Chunk]: list of chunks with score
         """
         queries = [query]
         if self._query_rewrite:
             with root_tracer.start_span(
                 "EmbeddingRetriever.query_rewrite.similarity_search",
                 metadata={"query": query, "score_threshold": score_threshold},
             ):
-                candidates_tasks = [self._similarity_search(query) for query in queries]
+                candidates_tasks = [
+                    self._similarity_search(query, filters) for query in queries
+                ]
                 chunks = await self._run_async_tasks(candidates_tasks)
                 context = "\n".join([chunk.content for chunk in chunks])
             with root_tracer.start_span(
                 "EmbeddingRetriever.query_rewrite.rewrite",
                 metadata={"query": query, "context": context, "nums": 1},
             ):
                 new_queries = await self._query_rewrite.rewrite(
@@ -158,15 +175,15 @@
                 queries.extend(new_queries)
 
         with root_tracer.start_span(
             "EmbeddingRetriever.similarity_search_with_score",
             metadata={"query": query, "score_threshold": score_threshold},
         ):
             candidates_with_score = [
-                self._similarity_search_with_score(query, score_threshold)
+                self._similarity_search_with_score(query, score_threshold, filters)
                 for query in queries
             ]
             res_candidates_with_score = await run_async_tasks(
                 tasks=candidates_with_score, concurrency_limit=1
             )
             new_candidates_with_score = cast(
                 List[Chunk], reduce(lambda x, y: x + y, res_candidates_with_score)
@@ -179,27 +196,26 @@
                 "score_threshold": score_threshold,
                 "rerank_cls": self._rerank.__class__.__name__,
             },
         ):
             new_candidates_with_score = self._rerank.rank(new_candidates_with_score)
             return new_candidates_with_score
 
-    async def _similarity_search(self, query) -> List[Chunk]:
+    async def _similarity_search(
+        self, query, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Similar search."""
-        return self._vector_store_connector.similar_search(
-            query,
-            self._top_k,
-        )
+        return self._vector_store_connector.similar_search(query, self._top_k, filters)
 
     async def _run_async_tasks(self, tasks) -> List[Chunk]:
         """Run async tasks."""
         candidates = await run_async_tasks(tasks=tasks, concurrency_limit=1)
         candidates = reduce(lambda x, y: x + y, candidates)
         return cast(List[Chunk], candidates)
 
     async def _similarity_search_with_score(
-        self, query, score_threshold
+        self, query, score_threshold, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Similar search with score."""
         return self._vector_store_connector.similar_search_with_scores(
-            query, self._top_k, score_threshold
+            query, self._top_k, score_threshold, filters
         )
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/retriever/rerank.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/retriever/rewrite.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/schemalinker/base_linker.py` & `dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/base_linker.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/schemalinker/schema_linking.py` & `dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/summary/db_summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/summary/db_summary_client.py` & `dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/summary/rdbms_db_summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/summary/rdbms_db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/pre_text_splitter.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/pre_text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/text_splitter.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/text_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,20 +453,20 @@
         Args:
             headers_to_split_on: Headers we want to track
             return_each_line: Return each line w/ associated headers
         """
         # Output line-by-line or aggregated into chunks w/ common headers
         if headers_to_split_on is None:
             headers_to_split_on = [
-                ("#", "Header 1"),
-                ("##", "Header 2"),
-                ("###", "Header 3"),
-                ("####", "Header 4"),
-                ("#####", "Header 5"),
-                ("######", "Header 6"),
+                ("#", "Header1"),
+                ("##", "Header2"),
+                ("###", "Header3"),
+                ("####", "Header4"),
+                ("#####", "Header5"),
+                ("######", "Header6"),
             ]
         if filters is None:
             filters = []
         self.return_each_line = return_each_line
         self._chunk_size = chunk_size
         # Given the headers we want to split on,
         # (e.g., "#, ##, etc") order by length
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/rag/text_splitter/token_splitter.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/token_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/cache/llm_cache.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/llm_cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/cache/manager.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/cache/operators.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/operators.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/base.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/cache/storage/disk/disk_storage.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/disk_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/chat_history/chat_history_db.py` & `dbgpt-0.5.4rc0/dbgpt/storage/chat_history/chat_history_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/chat_history/storage_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/storage/chat_history/storage_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/metadata/_base_dao.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/_base_dao.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/metadata/db_factory.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/metadata/db_manager.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/metadata/db_storage.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/schema.py` & `dbgpt-0.5.4rc0/dbgpt/storage/schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/base.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Vector store base class."""
 import logging
 import math
 import time
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.core import Chunk, Embeddings
 from dbgpt.core.awel.flow import Parameter
+from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.i18n_utils import _
 
 logger = logging.getLogger(__name__)
 
 
 _COMMON_PARAMETERS = [
     Parameter.build_from(
@@ -172,37 +173,44 @@
                 logger.info(f"Loaded {loaded_cnt} chunks, total {len(chunks)} chunks.")
         logger.info(
             f"Loaded {len(chunks)} chunks in {time.time() - start_time} seconds"
         )
         return ids
 
     @abstractmethod
-    def similar_search(self, text: str, topk: int) -> List[Chunk]:
+    def similar_search(
+        self, text: str, topk: int, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Similar search in vector database.
 
         Args:
             text(str): The query text.
             topk(int): The number of similar documents to return.
-
+            filters(Optional[MetadataFilters]): metadata filters.
         Return:
             List[Chunk]: The similar documents.
         """
         pass
 
     @abstractmethod
     def similar_search_with_scores(
-        self, text, topk, score_threshold: float
+        self,
+        text,
+        topk,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
     ) -> List[Chunk]:
         """Similar search with scores in vector database.
 
         Args:
             text(str): The query text.
             topk(int): The number of similar documents to return.
             score_threshold(int): score_threshold: Optional, a floating point value
                 between 0 to 1
+            filters(Optional[MetadataFilters]): metadata filters.
         Return:
             List[Chunk]: The similar documents.
         """
 
     @abstractmethod
     def vector_name_exists(self) -> bool:
         """Whether vector name exists."""
@@ -219,14 +227,23 @@
     @abstractmethod
     def delete_vector_name(self, vector_name: str):
         """Delete vector by name.
 
         Args:
             vector_name(str): The name of vector to delete.
         """
+        pass
+
+    def convert_metadata_filters(self, filters: MetadataFilters) -> Any:
+        """Convert metadata filters to vector store filters.
+
+        Args:
+            filters: (Optional[MetadataFilters]) metadata filters.
+        """
+        raise NotImplementedError
 
     def _normalization_vectors(self, vectors):
         """Return L2-normalization vectors to scale[0,1].
 
         Normalization vectors to scale[0,1].
         """
         import numpy as np
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/chroma_store.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,161 +1,183 @@
-"""Chroma vector store."""
+"""AIWrapper for LLM."""
+import json
 import logging
-import os
-from typing import Any, List
+import traceback
+from typing import Callable, Dict, Optional, Union
 
-from chromadb import PersistentClient
-from chromadb.config import Settings
+from dbgpt.core import LLMClient
+from dbgpt.core.interface.output_parser import BaseOutputParser
+from dbgpt.util.error_types import LLMChatError
+from dbgpt.util.tracer import root_tracer
 
-from dbgpt._private.pydantic import Field
-from dbgpt.configs.model_config import PILOT_PATH
-from dbgpt.core import Chunk
-from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
-from dbgpt.util.i18n_utils import _
-
-from .base import _COMMON_PARAMETERS, VectorStoreBase, VectorStoreConfig
+from .llm import _build_model_request
 
 logger = logging.getLogger(__name__)
 
 
-@register_resource(
-    _("Chroma Vector Store"),
-    "chroma_vector_store",
-    category=ResourceCategory.VECTOR_STORE,
-    description=_("Chroma vector store."),
-    parameters=[
-        *_COMMON_PARAMETERS,
-        Parameter.build_from(
-            _("Persist Path"),
-            "persist_path",
-            str,
-            description=_("the persist path of vector store."),
-            optional=True,
-            default=None,
-        ),
-    ],
-)
-class ChromaVectorConfig(VectorStoreConfig):
-    """Chroma vector store config."""
-
-    class Config:
-        """Config for BaseModel."""
-
-        arbitrary_types_allowed = True
-
-    persist_path: str = Field(
-        default=os.getenv("CHROMA_PERSIST_PATH", None),
-        description="the persist path of vector store.",
-    )
-    collection_metadata: dict = Field(
-        default=None,
-        description="the index metadata of vector store, if not set, will use the "
-        "default metadata.",
-    )
-
-
-class ChromaStore(VectorStoreBase):
-    """Chroma vector store."""
-
-    def __init__(self, vector_store_config: ChromaVectorConfig) -> None:
-        """Create a ChromaStore instance."""
-        from langchain.vectorstores import Chroma
-
-        chroma_vector_config = vector_store_config.dict(exclude_none=True)
-        chroma_path = chroma_vector_config.get(
-            "persist_path", os.path.join(PILOT_PATH, "data")
-        )
-        self.persist_dir = os.path.join(
-            chroma_path, vector_store_config.name + ".vectordb"
-        )
-        self.embeddings = vector_store_config.embedding_fn
-        chroma_settings = Settings(
-            # chroma_db_impl="duckdb+parquet", => deprecated configuration of Chroma
-            persist_directory=self.persist_dir,
-            anonymized_telemetry=False,
-        )
-        client = PersistentClient(path=self.persist_dir, settings=chroma_settings)
+class AIWrapper:
+    """AIWrapper for LLM."""
 
-        collection_metadata = chroma_vector_config.get("collection_metadata") or {
-            "hnsw:space": "cosine"
-        }
-        self.vector_store_client = Chroma(
-            persist_directory=self.persist_dir,
-            embedding_function=self.embeddings,
-            # client_settings=chroma_settings,
-            client=client,
-            collection_metadata=collection_metadata,
-        )
+    cache_path_root: str = ".cache"
+    extra_kwargs = {
+        "cache_seed",
+        "filter_func",
+        "allow_format_str_template",
+        "context",
+        "llm_model",
+    }
+
+    def __init__(
+        self, llm_client: LLMClient, output_parser: Optional[BaseOutputParser] = None
+    ):
+        """Create an AIWrapper instance."""
+        self.llm_echo = False
+        self.model_cache_enable = False
+        self._llm_client = llm_client
+        self._output_parser = output_parser or BaseOutputParser(is_stream_out=False)
+
+    @classmethod
+    def instantiate(
+        cls,
+        template: Optional[Union[str, Callable]] = None,
+        context: Optional[Dict] = None,
+        allow_format_str_template: Optional[bool] = False,
+    ):
+        """Instantiate the template with the context."""
+        if not context or template is None:
+            return template
+        if isinstance(template, str):
+            return template.format(**context) if allow_format_str_template else template
+        return template(context)
+
+    def _construct_create_params(self, create_config: Dict, extra_kwargs: Dict) -> Dict:
+        """Prime the create_config with additional_kwargs."""
+        # Validate the config
+        prompt = create_config.get("prompt")
+        messages = create_config.get("messages")
+        if prompt is None and messages is None:
+            raise ValueError(
+                "Either prompt or messages should be in create config but not both."
+            )
 
-    def similar_search(self, text, topk, **kwargs: Any) -> List[Chunk]:
-        """Search similar documents."""
-        logger.info("ChromaStore similar search")
-        lc_documents = self.vector_store_client.similarity_search(text, topk, **kwargs)
-        return [
-            Chunk(content=doc.page_content, metadata=doc.metadata)
-            for doc in lc_documents
-        ]
+        context = extra_kwargs.get("context")
+        if context is None:
+            # No need to instantiate if no context is provided.
+            return create_config
+        # Instantiate the prompt or messages
+        allow_format_str_template = extra_kwargs.get("allow_format_str_template", False)
+        # Make a copy of the config
+        params = create_config.copy()
+        if prompt is not None:
+            # Instantiate the prompt
+            params["prompt"] = self.instantiate(
+                prompt, context, allow_format_str_template
+            )
+        elif context and messages and isinstance(messages, list):
+            # Instantiate the messages
+            params["messages"] = [
+                {
+                    **m,
+                    "content": self.instantiate(
+                        m["content"], context, allow_format_str_template
+                    ),
+                }
+                if m.get("content")
+                else m
+                for m in messages
+            ]
+        return params
+
+    def _separate_create_config(self, config):
+        """Separate the config into create_config and extra_kwargs."""
+        create_config = {k: v for k, v in config.items() if k not in self.extra_kwargs}
+        extra_kwargs = {k: v for k, v in config.items() if k in self.extra_kwargs}
+        return create_config, extra_kwargs
 
-    def similar_search_with_scores(self, text, topk, score_threshold) -> List[Chunk]:
-        """Search similar documents with scores.
+    def _get_key(self, config):
+        """Get a unique identifier of a configuration.
 
-        Chroma similar_search_with_score.
-        Return docs and relevance scores in the range [0, 1].
         Args:
-            text(str): query text
-            topk(int): return docs nums. Defaults to 4.
-            score_threshold(float): score_threshold: Optional, a floating point value
-                between 0 to 1 to filter the resulting set of retrieved docs,0 is
-                dissimilar, 1 is most similar.
+            config (dict or list): A configuration.
+
+        Returns:
+            tuple: A unique identifier which can be used as a key for a dict.
         """
-        logger.info("ChromaStore similar search with scores")
-        docs_and_scores = (
-            self.vector_store_client.similarity_search_with_relevance_scores(
-                query=text, k=topk, score_threshold=score_threshold
+        non_cache_key = ["api_key", "base_url", "api_type", "api_version"]
+        copied = False
+        for key in non_cache_key:
+            if key in config:
+                config, copied = config.copy() if not copied else config, True
+                config.pop(key)
+        return json.dumps(config, sort_keys=True, ensure_ascii=False)
+
+    async def create(self, **config) -> Optional[str]:
+        """Create a response from the input config."""
+        # merge the input config with the i-th config in the config list
+        full_config = {**config}
+        # separate the config into create_config and extra_kwargs
+        create_config, extra_kwargs = self._separate_create_config(full_config)
+
+        # construct the create params
+        params = self._construct_create_params(create_config, extra_kwargs)
+        filter_func = extra_kwargs.get("filter_func")
+        context = extra_kwargs.get("context")
+        llm_model = extra_kwargs.get("llm_model")
+        try:
+            response = await self._completions_create(llm_model, params)
+        except LLMChatError as e:
+            logger.debug(f"{llm_model} generate failed!{str(e)}")
+            raise e
+        else:
+            pass_filter = filter_func is None or filter_func(
+                context=context, response=response
             )
+            if pass_filter:
+                # Return the response if it passes the filter
+                return response
+            else:
+                return None
+
+    def _get_span_metadata(self, payload: Dict) -> Dict:
+        metadata = {k: v for k, v in payload.items()}
+
+        metadata["messages"] = list(
+            map(lambda m: m if isinstance(m, dict) else m.dict(), metadata["messages"])
+        )
+        return metadata
+
+    def _llm_messages_convert(self, params):
+        gpts_messages = params["messages"]
+        # TODO
+
+        return gpts_messages
+
+    async def _completions_create(self, llm_model, params) -> str:
+        payload = {
+            "model": llm_model,
+            "prompt": params.get("prompt"),
+            "messages": self._llm_messages_convert(params),
+            "temperature": float(params.get("temperature")),
+            "max_new_tokens": int(params.get("max_new_tokens")),
+            "echo": self.llm_echo,
+        }
+        logger.info(f"Request: \n{payload}")
+        span = root_tracer.start_span(
+            "Agent.llm_client.no_streaming_call",
+            metadata=self._get_span_metadata(payload),
         )
-        return [
-            Chunk(content=doc.page_content, metadata=doc.metadata, score=score)
-            for doc, score in docs_and_scores
-        ]
-
-    def vector_name_exists(self) -> bool:
-        """Whether vector name exists."""
-        logger.info(f"Check persist_dir: {self.persist_dir}")
-        if not os.path.exists(self.persist_dir):
-            return False
-        files = os.listdir(self.persist_dir)
-        # Skip default file: chroma.sqlite3
-        files = list(filter(lambda f: f != "chroma.sqlite3", files))
-        return len(files) > 0
-
-    def load_document(self, chunks: List[Chunk]) -> List[str]:
-        """Load document to vector store."""
-        logger.info("ChromaStore load document")
-        texts = [chunk.content for chunk in chunks]
-        metadatas = [chunk.metadata for chunk in chunks]
-        ids = [chunk.chunk_id for chunk in chunks]
-        self.vector_store_client.add_texts(texts=texts, metadatas=metadatas, ids=ids)
-        return ids
-
-    def delete_vector_name(self, vector_name: str):
-        """Delete vector name."""
-        logger.info(f"chroma vector_name:{vector_name} begin delete...")
-        self.vector_store_client.delete_collection()
-        self._clean_persist_folder()
-        return True
-
-    def delete_by_ids(self, ids):
-        """Delete vector by ids."""
-        logger.info(f"begin delete chroma ids: {ids}")
-        ids = ids.split(",")
-        if len(ids) > 0:
-            collection = self.vector_store_client._collection
-            collection.delete(ids=ids)
-
-    def _clean_persist_folder(self):
-        for root, dirs, files in os.walk(self.persist_dir, topdown=False):
-            for name in files:
-                os.remove(os.path.join(root, name))
-            for name in dirs:
-                os.rmdir(os.path.join(root, name))
-        os.rmdir(self.persist_dir)
+        payload["span_id"] = span.span_id
+        payload["model_cache_enable"] = self.model_cache_enable
+        try:
+            model_request = _build_model_request(payload)
+            model_output = await self._llm_client.generate(model_request.copy())
+            parsed_output = self._output_parser.parse_model_nostream_resp(
+                model_output, "#########################"
+            )
+            return parsed_output
+        except Exception as e:
+            logger.error(
+                f"Call LLMClient error, {str(e)}, detail: {traceback.format_exc()}"
+            )
+            raise LLMChatError(original_exception=e) from e
+        finally:
+            span.end()
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/connector.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     OptionValue,
     Parameter,
     ResourceCategory,
     register_resource,
 )
 from dbgpt.storage import vector_store
 from dbgpt.storage.vector_store.base import VectorStoreBase, VectorStoreConfig
+from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.i18n_utils import _
 
 connector: Dict[str, Type] = {}
 
 
 def _load_vector_options() -> List[OptionValue]:
     return [
@@ -124,43 +125,52 @@
         )
         return self.client.load_document_with_limit(
             chunks,
             max_chunks_once_load,
             max_threads,
         )
 
-    def similar_search(self, doc: str, topk: int) -> List[Chunk]:
+    def similar_search(
+        self, doc: str, topk: int, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Similar search in vector database.
 
         Args:
            - doc: query text
            - topk: topk
+           - filters: metadata filters.
         Return:
             - chunks: chunks.
         """
-        return self.client.similar_search(doc, topk)
+        return self.client.similar_search(doc, topk, filters)
 
     def similar_search_with_scores(
-        self, doc: str, topk: int, score_threshold: float
+        self,
+        doc: str,
+        topk: int,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
     ) -> List[Chunk]:
-        """Similar search with scores in vector database.
+        """Similar_search_with_score in vector database.
 
-        similar_search_with_score in vector database..
         Return docs and relevance scores in the range [0, 1].
 
         Args:
             doc(str): query text
             topk(int): return docs nums. Defaults to 4.
             score_threshold(float): score_threshold: Optional, a floating point value
                 between 0 to 1 to filter the resulting set of retrieved docs,0 is
                 dissimilar, 1 is most similar.
+            filters: metadata filters.
         Return:
-            - chunks: chunks.
+            - chunks: Return docs and relevance scores in the range [0, 1].
         """
-        return self.client.similar_search_with_scores(doc, topk, score_threshold)
+        return self.client.similar_search_with_scores(
+            doc, topk, score_threshold, filters
+        )
 
     @property
     def vector_store_config(self) -> VectorStoreConfig:
         """Return the vector store config."""
         if not self._vector_store_config:
             raise ValueError("vector store config not set.")
         return self._vector_store_config
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/milvus_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/milvus_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from dbgpt.core import Chunk, Embeddings
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.storage.vector_store.base import (
     _COMMON_PARAMETERS,
     VectorStoreBase,
     VectorStoreConfig,
 )
+from dbgpt.storage.vector_store.filters import FilterOperator, MetadataFilters
 from dbgpt.util import string_utils
 from dbgpt.util.i18n_utils import _
 
 logger = logging.getLogger(__name__)
 
 
 @register_resource(
@@ -170,18 +171,18 @@
         self.collection_name = (
             milvus_vector_config.get("name") or vector_store_config.name
         )
         if string_utils.is_all_chinese(self.collection_name):
             bytes_str = self.collection_name.encode("utf-8")
             hex_str = bytes_str.hex()
             self.collection_name = hex_str
-
-        if not vector_store_config.embedding_fn:
-            raise ValueError("embedding is required for MilvusStore")
-
+        if vector_store_config.embedding_fn is None:
+            # Perform runtime checks on self.embedding to
+            # ensure it has been correctly set and loaded
+            raise ValueError("embedding_fn is required for MilvusStore")
         self.embedding: Embeddings = vector_store_config.embedding_fn
         self.fields: List = []
         self.alias = milvus_vector_config.get("alias") or "default"
 
         # use HNSW by default.
         self.index_params = {
             "index_type": "HNSW",
@@ -202,14 +203,15 @@
             "ANNOY": {"params": {"search_k": 10}},
         }
         # default collection schema
         self.primary_field = milvus_vector_config.get("primary_field") or "pk_id"
         self.vector_field = milvus_vector_config.get("embedding_field") or "vector"
         self.text_field = milvus_vector_config.get("text_field") or "content"
         self.metadata_field = milvus_vector_config.get("metadata_field") or "metadata"
+        self.props_field = milvus_vector_config.get("props_field") or "props_field"
 
         if (self.username is None) != (self.password is None):
             raise ValueError(
                 "Both username and password must be set to use authentication for "
                 "Milvus"
             )
         if self.username:
@@ -280,14 +282,15 @@
 
         dim = len(embeddings)
         # Generate unique names
         primary_field = self.primary_field
         vector_field = self.vector_field
         text_field = self.text_field
         metadata_field = self.metadata_field
+        props_field = self.props_field
         # self.text_field = text_field
         collection_name = vector_name
         fields = []
         max_length = 0
         for y in texts:
             max_length = max(max_length, len(y))
         # Create the text field
@@ -296,14 +299,15 @@
         fields.append(
             FieldSchema(primary_field, DataType.INT64, is_primary=True, auto_id=True)
         )
         # vector field
         fields.append(FieldSchema(vector_field, DataType.FLOAT_VECTOR, dim=dim))
 
         fields.append(FieldSchema(metadata_field, DataType.VARCHAR, max_length=65535))
+        fields.append(FieldSchema(props_field, DataType.JSON))
         schema = CollectionSchema(fields)
         # Create the collection
         collection = Collection(collection_name, schema)
         self.col = collection
         # index parameters for the collection
         index = self.index_params
         # milvus index
@@ -342,14 +346,15 @@
             ]
         # Collect the metadata into the insert dict.
         # self.fields.extend(metadatas[0].keys())
         if len(self.fields) > 2 and metadatas is not None:
             for d in metadatas:
                 # for key, value in d.items():
                 insert_dict.setdefault("metadata", []).append(json.dumps(d))
+                insert_dict.setdefault("props_field", []).append(d)
         # Convert dict to list of lists for insertion
         insert_list = [insert_dict[x] for x in self.fields]
         # Insert into the collection.
         res = self.col.insert(
             insert_list, partition_name=partition_name, timeout=timeout
         )
         # make sure data is searchable.
@@ -364,56 +369,61 @@
         ]
         doc_ids = []
         for doc_batch in batched_list:
             doc_ids.extend(self.init_schema_and_load(self.collection_name, doc_batch))
         doc_ids = [str(doc_id) for doc_id in doc_ids]
         return doc_ids
 
-    def similar_search(self, text, topk) -> List[Chunk]:
+    def similar_search(
+        self, text, topk, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Perform a search on a query string and return results."""
         from pymilvus import Collection, DataType
 
         """similar_search in vector database."""
         self.col = Collection(self.collection_name)
         schema = self.col.schema
         for x in schema.fields:
             self.fields.append(x.name)
             if x.auto_id:
                 self.fields.remove(x.name)
             if x.is_primary:
                 self.primary_field = x.name
             if x.dtype == DataType.FLOAT_VECTOR or x.dtype == DataType.BINARY_VECTOR:
                 self.vector_field = x.name
-        _, docs_and_scores = self._search(text, topk)
+        # convert to milvus expr filter.
+        milvus_filter_expr = self.convert_metadata_filters(filters) if filters else None
+        _, docs_and_scores = self._search(text, topk, expr=milvus_filter_expr)
 
         return [
             Chunk(
                 metadata=json.loads(doc.metadata.get("metadata", "")),
                 content=doc.content,
             )
             for doc, _, _ in docs_and_scores
         ]
 
-    def similar_search_with_scores(self, text, topk, score_threshold) -> List[Chunk]:
+    def similar_search_with_scores(
+        self,
+        text: str,
+        topk: int,
+        score_threshold: float,
+        filters: Optional[MetadataFilters] = None,
+    ) -> List[Chunk]:
         """Perform a search on a query string and return results with score.
 
         For more information about the search parameters, take a look at the pymilvus
         documentation found here:
         https://milvus.io/api-reference/pymilvus/v2.2.6/Collection/search().md
 
         Args:
-            embedding (List[float]): The embedding vector being searched.
-            k (int, optional): The amount of results to return. Defaults to 4.
-            param (dict): The search params for the specified index.
-                Defaults to None.
-            expr (str, optional): Filtering expression. Defaults to None.
-            timeout (int, optional): How long to wait before timeout error.
-                Defaults to None.
-            kwargs: Collection.search() keyword arguments.
-
+            text (str): The query text.
+            topk (int): The number of similar documents to return.
+            score_threshold (float): Optional, a floating point value between 0 to 1.
+            filters (Optional[MetadataFilters]): Optional, metadata filters.
         Returns:
             List[Tuple[Document, float]]: Result doc and score.
         """
         from pymilvus import Collection
 
         self.col = Collection(self.collection_name)
         schema = self.col.schema
@@ -423,15 +433,19 @@
                 self.fields.remove(x.name)
             if x.is_primary:
                 self.primary_field = x.name
             from pymilvus import DataType
 
             if x.dtype == DataType.FLOAT_VECTOR or x.dtype == DataType.BINARY_VECTOR:
                 self.vector_field = x.name
-        _, docs_and_scores = self._search(text, topk)
+        # convert to milvus expr filter.
+        milvus_filter_expr = self.convert_metadata_filters(filters) if filters else None
+        _, docs_and_scores = self._search(
+            query=text, topk=topk, expr=milvus_filter_expr
+        )
         if any(score < 0.0 or score > 1.0 for _, score, id in docs_and_scores):
             logger.warning(
                 "similarity score need between" f" 0 and 1, got {docs_and_scores}"
             )
 
         if score_threshold is not None:
             docs_and_scores = [
@@ -458,14 +472,28 @@
         param: Optional[dict] = None,
         expr: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         round_decimal: int = -1,
         timeout: Optional[int] = None,
         **kwargs: Any,
     ):
+        """Search in vector database.
+
+        Args:
+            query: query text.
+            k: topk.
+            param: search params.
+            expr: search expr.
+            partition_names: partition names.
+            round_decimal: round decimal.
+            timeout: timeout.
+            **kwargs: kwargs.
+        Returns:
+            Tuple[Document, float, int]: Result doc and score.
+        """
         self.col.load()
         # use default index params.
         if param is None:
             index_type = self.col.indexes[0].params["index_type"]
             param = self.index_params_map[index_type].get("params")
         #  query text embedding.
         query_vector = self.embedding.embed_query(query)
@@ -491,15 +519,17 @@
             ret.append(
                 (
                     Chunk(content=meta.pop(self.text_field), metadata=meta),
                     result.distance,
                     result.id,
                 )
             )
-
+        if len(ret) == 0:
+            logger.warning("No relevant docs were retrieved.")
+            return None, []
         return ret[0], ret
 
     def vector_name_exists(self):
         """Whether vector name exists."""
         from pymilvus import utility
 
         """is vector store name exist."""
@@ -519,10 +549,44 @@
         from pymilvus import Collection
 
         self.col = Collection(self.collection_name)
         # milvus delete vectors by ids
         logger.info(f"begin delete milvus ids: {ids}")
         delete_ids = ids.split(",")
         doc_ids = [int(doc_id) for doc_id in delete_ids]
-        delet_expr = f"{self.primary_field} in {doc_ids}"
-        self.col.delete(delet_expr)
+        delete_expr = f"{self.primary_field} in {doc_ids}"
+        self.col.delete(delete_expr)
         return True
+
+    def convert_metadata_filters(self, filters: MetadataFilters) -> str:
+        """Convert filter to milvus filters.
+
+        Args:
+            - filters: metadata filters.
+        Returns:
+            - metadata_filters: metadata filters.
+        """
+        metadata_filters = []
+        for metadata_filter in filters.filters:
+            if isinstance(metadata_filter.value, str):
+                expr = (
+                    f"{self.props_field}['{metadata_filter.key}'] "
+                    f"{FilterOperator.EQ} '{metadata_filter.value}'"
+                )
+                metadata_filters.append(expr)
+            elif isinstance(metadata_filter.value, List):
+                expr = (
+                    f"{self.props_field}['{metadata_filter.key}'] "
+                    f"{FilterOperator.IN} {metadata_filter.value}"
+                )
+                metadata_filters.append(expr)
+            else:
+                expr = (
+                    f"{self.props_field}['{metadata_filter.key}'] "
+                    f"{FilterOperator.EQ} {str(metadata_filter.value)}"
+                )
+                metadata_filters.append(expr)
+        if len(metadata_filters) > 1:
+            metadata_filter_expr = f" {filters.condition} ".join(metadata_filters)
+        else:
+            metadata_filter_expr = metadata_filters[0]
+        return metadata_filter_expr
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/pgvector_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/pgvector_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Postgres vector store."""
 import logging
-from typing import Any, List
+from typing import List, Optional
 
 from dbgpt._private.pydantic import Field
 from dbgpt.core import Chunk
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.storage.vector_store.base import (
     _COMMON_PARAMETERS,
     VectorStoreBase,
     VectorStoreConfig,
 )
+from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.i18n_utils import _
 
 logger = logging.getLogger(__name__)
 
 
 @register_resource(
     _("PG Vector Store"),
@@ -66,17 +67,19 @@
 
         self.vector_store_client = PGVector(
             embedding_function=self.embeddings,
             collection_name=self.collection_name,
             connection_string=self.connection_string,
         )
 
-    def similar_search(self, text: str, topk: int, **kwargs: Any) -> List[Chunk]:
+    def similar_search(
+        self, text: str, topk: int, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Perform similar search in PGVector."""
-        return self.vector_store_client.similarity_search(text, topk)
+        return self.vector_store_client.similarity_search(text, topk, filters)
 
     def vector_name_exists(self) -> bool:
         """Check if vector name exists."""
         try:
             self.vector_store_client.create_collection()
             return True
         except Exception as e:
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/storage/vector_store/weaviate_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/weaviate_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Weaviate vector store."""
 import logging
 import os
-from typing import List
+from typing import List, Optional
 
 from dbgpt._private.pydantic import Field
 from dbgpt.core import Chunk
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.util.i18n_utils import _
 
 from .base import _COMMON_PARAMETERS, VectorStoreBase, VectorStoreConfig
+from .filters import MetadataFilters
 
 logger = logging.getLogger(__name__)
 
 
 @register_resource(
     _("Weaviate Vector Store"),
     "weaviate_vector_store",
@@ -76,15 +77,17 @@
         self.vector_name = vector_store_config.name
         self.persist_dir = os.path.join(
             vector_store_config.persist_path, vector_store_config.name + ".vectordb"
         )
 
         self.vector_store_client = weaviate.Client(self.weaviate_url)
 
-    def similar_search(self, text: str, topk: int) -> List[Chunk]:
+    def similar_search(
+        self, text: str, topk: int, filters: Optional[MetadataFilters] = None
+    ) -> List[Chunk]:
         """Perform similar search in Weaviate."""
         logger.info("Weaviate similar search")
         # nearText = {
         #     "concepts": [text],
         #     "distance": 0.75,  # prior to v1.14 use "certainty" instead of "distance"
         # }
         # vector = self.embedding.embed_query(text)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/_db_migration_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/_db_migration_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/annotations.py` & `dbgpt-0.5.4rc0/dbgpt/util/annotations.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/api_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/api_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py` & `dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py` & `dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/chat_util.py` & `dbgpt-0.5.4rc0/dbgpt/util/chat_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/code_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/code_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/command_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/command_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/config_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/console/console.py` & `dbgpt-0.5.4rc0/dbgpt/util/console/console.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/custom_data_structure.py` & `dbgpt-0.5.4rc0/dbgpt/util/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/dbgpts/base.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/dbgpts/cli.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/dbgpts/loader.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/dbgpts/repo.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/repo.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/dbgpts/template.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/error_types.py` & `dbgpt-0.5.4rc0/dbgpt/util/error_types.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/executor_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/executor_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/fastapi.py` & `dbgpt-0.5.4rc0/dbgpt/util/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/formatting.py` & `dbgpt-0.5.4rc0/dbgpt/util/formatting.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/function_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/function_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/global_helper.py` & `dbgpt-0.5.4rc0/dbgpt/util/global_helper.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/i18n_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/i18n_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/json_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Utilities for the json_fixes package."""
 import json
 import logging
-import os.path
 import re
-from dataclasses import asdict, dataclass, is_dataclass
+from dataclasses import asdict, is_dataclass
 from datetime import date, datetime
 
-from jsonschema import Draft7Validator
-
 logger = logging.getLogger(__name__)
 
 LLM_DEFAULT_RESPONSE_FORMAT = "llm_response_format_1"
 
 
 def serialize(obj):
     if isinstance(obj, date):
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/model_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/model_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/module_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/module_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/net_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/net_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/openai_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/openai_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/pagination_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/pagination_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/parameter_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/parameter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/pd_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/prompt_util.py` & `dbgpt-0.5.4rc0/dbgpt/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/serialization/json_serialization.py` & `dbgpt-0.5.4rc0/dbgpt/util/serialization/json_serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/similarity_util.py` & `dbgpt-0.5.4rc0/dbgpt/util/similarity_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/singleton.py` & `dbgpt-0.5.4rc0/dbgpt/util/singleton.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/speech/base.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/speech/brian.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/brian.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/speech/eleven_labs.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/speech/macos_tts.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/speech/say.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/say.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/splitter_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/splitter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/string_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/string_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Dict
 
 
 def is_all_chinese(text):
     ### Determine whether the string is pure Chinese
     pattern = re.compile(r"^[一-龥]+$")
     match = re.match(pattern, text)
     return match is not None
@@ -30,15 +31,15 @@
     # 判断是否匹配成功
     if match is not None:
         return True
     else:
         return False
 
 
-def extract_content(long_string, s1, s2, is_include: bool = False):
+def extract_content(long_string, s1, s2, is_include: bool = False) -> Dict[int, str]:
     # extract text
     match_map = {}
     start_index = long_string.find(s1)
     while start_index != -1:
         if is_include:
             end_index = long_string.find(s2, start_index + len(s1) + 1)
             extracted_content = long_string[start_index : end_index + len(s2)]
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/system_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/system_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     cpu_info = "Unknown CPU"
     if os_type == OSType.LINUX:
         try:
             output = subprocess.check_output(["lscpu"]).decode("utf-8")
             match = re.search(r".*Model name:\s*(.+)", output)
             if match:
                 cpu_info = match.group(1).strip()
-            match = re.search(f".*型号名称：\s*(.+)", output)
+            match = re.search(r".*型号名称：\s*(.+)", output)
             if match:
                 cpu_info = match.group(1).strip()
         except:
             pass
     elif os_type == OSType.DARWIN:
         try:
             output = subprocess.check_output(
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/tracer/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/tracer/base.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from dbgpt.component import BaseComponent, ComponentType, SystemApp
 
 
 class SpanType(str, Enum):
     BASE = "base"
     RUN = "run"
     CHAT = "chat"
+    AGENT = "agent"
 
 
 class SpanTypeRunName(str, Enum):
     WEBSERVER = "Webserver"
     WORKER_MANAGER = "WorkerManager"
     MODEL_WORKER = "ModelWorker"
     EMBEDDING_MODEL = "EmbeddingModel"
@@ -95,14 +96,29 @@
             else self.start_time.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3],
             "end_time": None
             if not self.end_time
             else self.end_time.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3],
             "metadata": _clean_for_json(self.metadata),
         }
 
+    def copy(self) -> Span:
+        """Create a copy of this span."""
+        metadata = self.metadata.copy() if self.metadata else None
+        span = Span(
+            self.trace_id,
+            self.span_id,
+            self.span_type,
+            self.parent_span_id,
+            self.operation_name,
+            metadata=metadata,
+        )
+        span.start_time = self.start_time
+        span.end_time = self.end_time
+        return span
+
 
 class SpanStorageType(str, Enum):
     ON_CREATE = "on_create"
     ON_END = "on_end"
     ON_CREATE_END = "on_create_end"
 
 
@@ -187,15 +203,15 @@
 
 @dataclass
 class TracerContext:
     span_id: Optional[str] = None
 
 
 def _clean_for_json(data: Optional[str, Any] = None):
-    if not data:
+    if data is None:
         return None
     if isinstance(data, dict):
         cleaned_dict = {}
         for key, value in data.items():
             # Try to clean the sub-items
             cleaned_value = _clean_for_json(value)
             if cleaned_value is not None:
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/tracer/span_storage.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/span_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         self.batch_size = batch_size
         self.flush_interval = flush_interval
         self.last_flush_time = time.time()
         self.flush_signal_queue = queue.Queue()
         self.flush_thread = threading.Thread(
             target=self._flush_to_storages, daemon=True
         )
+        self._stop_event = threading.Event()
         self.flush_thread.start()
+        self._stop_event.clear()
 
     def append_storage(self, storage: SpanStorage):
         """Append sotrage to container
 
         Args:
             storage ([`SpanStorage`]): The storage to be append to current container
         """
@@ -64,15 +66,15 @@
         if self.queue.qsize() >= self.batch_size:
             try:
                 self.flush_signal_queue.put_nowait(True)
             except queue.Full:
                 pass  # If the signal queue is full, it's okay. The flush thread will handle it.
 
     def _flush_to_storages(self):
-        while True:
+        while not self._stop_event.is_set():
             interval = time.time() - self.last_flush_time
             if interval < self.flush_interval:
                 try:
                     self.flush_signal_queue.get(
                         block=True, timeout=self.flush_interval - interval
                     )
                 except Exception:
@@ -86,21 +88,32 @@
 
                 def append_and_ignore_error(
                     storage: SpanStorage, spans_to_write: List[SpanStorage]
                 ):
                     try:
                         storage.append_span_batch(spans_to_write)
                     except Exception as e:
-                        logger.warn(
+                        logger.warning(
                             f"Append spans to storage {str(storage)} failed: {str(e)}, span_data: {spans_to_write}"
                         )
 
-                self.executor.submit(append_and_ignore_error, s, spans_to_write)
+                try:
+                    self.executor.submit(append_and_ignore_error, s, spans_to_write)
+                except RuntimeError:
+                    append_and_ignore_error(s, spans_to_write)
             self.last_flush_time = time.time()
 
+    def before_stop(self):
+        try:
+            self.flush_signal_queue.put(True)
+            self._stop_event.set()
+            self.flush_thread.join()
+        except Exception:
+            pass
+
 
 class FileSpanStorage(SpanStorage):
     def __init__(self, filename: str):
         super().__init__()
         self.filename = filename
         # Split filename into prefix and suffix
         self.filename_prefix, self.filename_suffix = os.path.splitext(filename)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/tracer/tracer_cli.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/tracer/tracer_impl.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         if not default_storage:
             default_storage = MemorySpanStorage(system_app)
         self._default_storage = default_storage
         self._span_storage_type = span_storage_type
 
     def append_span(self, span: Span):
-        self._get_current_storage().append_span(span)
+        self._get_current_storage().append_span(span.copy())
 
     def start_span(
         self,
         operation_name: str,
         parent_span_id: str = None,
         span_type: SpanType = None,
         metadata: Dict = None,
@@ -126,17 +126,21 @@
         metadata: Dict = None,
     ) -> Span:
         """Start a new span with operation_name
         This method must not throw an exception under any case and try not to block as much as possible
         """
         tracer = self._get_tracer()
         if not tracer:
-            return Span("empty_span", "empty_span")
+            return Span(
+                "empty_span", "empty_span", span_type=span_type, metadata=metadata
+            )
         if not parent_span_id:
             parent_span_id = self.get_current_span_id()
+        if not span_type and parent_span_id:
+            span_type = self._get_current_span_type()
         return tracer.start_span(
             operation_name, parent_span_id, span_type=span_type, metadata=metadata
         )
 
     def end_span(self, span: Span, **kwargs):
         tracer = self._get_tracer()
         if not tracer or not span:
@@ -152,14 +156,18 @@
     def get_current_span_id(self) -> Optional[str]:
         current_span = self.get_current_span()
         if current_span:
             return current_span.span_id
         ctx = self._trace_context_var.get()
         return ctx.span_id if ctx else None
 
+    def _get_current_span_type(self) -> Optional[SpanType]:
+        current_span = self.get_current_span()
+        return current_span.span_type if current_span else None
+
 
 root_tracer: TracerManager = TracerManager()
 
 
 def trace(operation_name: Optional[str] = None, **trace_kwargs):
     def decorator(func):
         @wraps(func)
@@ -193,22 +201,27 @@
     func_name = func.__name__
     if self_name:
         return f"{self_name}.{func_name}"
     return func_name
 
 
 def initialize_tracer(
-    system_app: SystemApp,
     tracer_filename: str,
     root_operation_name: str = "DB-GPT-Web-Entry",
-    tracer_storage_cls: str = None,
+    system_app: Optional[SystemApp] = None,
+    tracer_storage_cls: Optional[str] = None,
+    create_system_app: bool = False,
 ):
+    """Initialize the tracer with the given filename and system app."""
+    from dbgpt.util.tracer.span_storage import FileSpanStorage, SpanStorageContainer
+
+    if not system_app and create_system_app:
+        system_app = SystemApp()
     if not system_app:
         return
-    from dbgpt.util.tracer.span_storage import FileSpanStorage, SpanStorageContainer
 
     trace_context_var = ContextVar(
         "trace_context",
         default=TracerContext(),
     )
     tracer = DefaultTracer(system_app)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/tracer/tracer_middleware.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_middleware.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt/util/utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.3rc0/dbgpt.egg-info/PKG-INFO` & `dbgpt-0.5.4rc0/dbgpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.3rc0
+Version: 0.5.4rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -46,14 +46,32 @@
 Requires-Dist: fastapi==0.98.0; extra == "cli"
 Requires-Dist: prettytable; extra == "cli"
 Requires-Dist: click; extra == "cli"
 Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
 Requires-Dist: rich; extra == "cli"
+Provides-Extra: agent
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: importlib-resources==5.12.0; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: pydantic<2,>=1; extra == "agent"
+Requires-Dist: typeguard; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
+Requires-Dist: fastapi==0.98.0; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
+Requires-Dist: click; extra == "agent"
+Requires-Dist: psutil==5.9.4; extra == "agent"
+Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: rich; extra == "agent"
+Requires-Dist: termcolor; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
 Provides-Extra: simple-framework
 Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
 Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
 Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
 Requires-Dist: cachetools; extra == "simple-framework"
 Requires-Dist: pydantic<2,>=1; extra == "simple-framework"
@@ -62,14 +80,16 @@
 Requires-Dist: fastapi==0.98.0; extra == "simple-framework"
 Requires-Dist: prettytable; extra == "simple-framework"
 Requires-Dist: click; extra == "simple-framework"
 Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: colorama==0.4.6; extra == "simple-framework"
 Requires-Dist: tomlkit; extra == "simple-framework"
 Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: termcolor; extra == "simple-framework"
+Requires-Dist: pandas==2.0.3; extra == "simple-framework"
 Requires-Dist: jinja2; extra == "simple-framework"
 Requires-Dist: uvicorn; extra == "simple-framework"
 Requires-Dist: shortuuid; extra == "simple-framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
 Requires-Dist: msgpack; extra == "simple-framework"
 Requires-Dist: pympler; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
@@ -89,53 +109,58 @@
 Requires-Dist: fastapi==0.98.0; extra == "framework"
 Requires-Dist: prettytable; extra == "framework"
 Requires-Dist: click; extra == "framework"
 Requires-Dist: psutil==5.9.4; extra == "framework"
 Requires-Dist: colorama==0.4.6; extra == "framework"
 Requires-Dist: tomlkit; extra == "framework"
 Requires-Dist: rich; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: jinja2; extra == "framework"
 Requires-Dist: uvicorn; extra == "framework"
 Requires-Dist: shortuuid; extra == "framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
 Requires-Dist: msgpack; extra == "framework"
 Requires-Dist: pympler; extra == "framework"
 Requires-Dist: duckdb; extra == "framework"
 Requires-Dist: duckdb-engine; extra == "framework"
 Requires-Dist: schedule; extra == "framework"
 Requires-Dist: sqlparse==0.4.4; extra == "framework"
 Requires-Dist: fschat; extra == "framework"
 Requires-Dist: coloredlogs; extra == "framework"
 Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: auto-gpt-plugin-template; extra == "framework"
 Requires-Dist: gTTS==2.3.1; extra == "framework"
 Requires-Dist: pymysql; extra == "framework"
 Requires-Dist: jsonschema; extra == "framework"
 Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: alembic==1.12.0; extra == "framework"
 Requires-Dist: openpyxl==3.1.2; extra == "framework"
 Requires-Dist: chardet==5.1.0; extra == "framework"
 Requires-Dist: xlrd==2.0.1; extra == "framework"
 Requires-Dist: aiofiles; extra == "framework"
 Requires-Dist: GitPython; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torch==2.0.1; extra == "torch"
-Requires-Dist: torchvision==0.15.2; extra == "torch"
-Requires-Dist: torchaudio==2.0.2; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
+Requires-Dist: torchvision==0.17.1; extra == "torch"
+Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torch==2.0.1; extra == "torch-cpu"
-Requires-Dist: torchvision==0.15.2; extra == "torch-cpu"
-Requires-Dist: torchaudio==2.0.2; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
+Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
+Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
+Provides-Extra: bitsandbytes
+Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
-Requires-Dist: bitsandbytes; extra == "quantization"
 Requires-Dist: cpm_kernels; extra == "quantization"
 Provides-Extra: vstore
 Requires-Dist: pymilvus; extra == "vstore"
 Requires-Dist: weaviate-client; extra == "vstore"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
@@ -176,28 +201,29 @@
 Requires-Dist: fastapi==0.98.0; extra == "openai"
 Requires-Dist: prettytable; extra == "openai"
 Requires-Dist: click; extra == "openai"
 Requires-Dist: psutil==5.9.4; extra == "openai"
 Requires-Dist: colorama==0.4.6; extra == "openai"
 Requires-Dist: tomlkit; extra == "openai"
 Requires-Dist: rich; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
 Requires-Dist: jinja2; extra == "openai"
 Requires-Dist: uvicorn; extra == "openai"
 Requires-Dist: shortuuid; extra == "openai"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
 Requires-Dist: msgpack; extra == "openai"
 Requires-Dist: pympler; extra == "openai"
 Requires-Dist: duckdb; extra == "openai"
 Requires-Dist: duckdb-engine; extra == "openai"
 Requires-Dist: schedule; extra == "openai"
 Requires-Dist: sqlparse==0.4.4; extra == "openai"
 Requires-Dist: fschat; extra == "openai"
 Requires-Dist: coloredlogs; extra == "openai"
 Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
 Requires-Dist: auto-gpt-plugin-template; extra == "openai"
 Requires-Dist: gTTS==2.3.1; extra == "openai"
 Requires-Dist: pymysql; extra == "openai"
 Requires-Dist: jsonschema; extra == "openai"
 Requires-Dist: transformers>=4.34.0; extra == "openai"
 Requires-Dist: alembic==1.12.0; extra == "openai"
 Requires-Dist: openpyxl==3.1.2; extra == "openai"
@@ -227,14 +253,15 @@
 Provides-Extra: default
 Requires-Dist: tokenizers>=0.14; extra == "default"
 Requires-Dist: accelerate>=0.20.3; extra == "default"
 Requires-Dist: protobuf==3.20.3; extra == "default"
 Requires-Dist: zhipuai; extra == "default"
 Requires-Dist: dashscope; extra == "default"
 Requires-Dist: chardet; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
 Requires-Dist: aiohttp==3.8.4; extra == "default"
 Requires-Dist: chardet==5.1.0; extra == "default"
 Requires-Dist: importlib-resources==5.12.0; extra == "default"
 Requires-Dist: python-dotenv==1.0.0; extra == "default"
 Requires-Dist: cachetools; extra == "default"
 Requires-Dist: pydantic<2,>=1; extra == "default"
 Requires-Dist: typeguard; extra == "default"
@@ -242,28 +269,29 @@
 Requires-Dist: fastapi==0.98.0; extra == "default"
 Requires-Dist: prettytable; extra == "default"
 Requires-Dist: click; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
 Requires-Dist: colorama==0.4.6; extra == "default"
 Requires-Dist: tomlkit; extra == "default"
 Requires-Dist: rich; extra == "default"
+Requires-Dist: termcolor; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
 Requires-Dist: jinja2; extra == "default"
 Requires-Dist: uvicorn; extra == "default"
 Requires-Dist: shortuuid; extra == "default"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
 Requires-Dist: msgpack; extra == "default"
 Requires-Dist: pympler; extra == "default"
 Requires-Dist: duckdb; extra == "default"
 Requires-Dist: duckdb-engine; extra == "default"
 Requires-Dist: schedule; extra == "default"
 Requires-Dist: sqlparse==0.4.4; extra == "default"
 Requires-Dist: fschat; extra == "default"
 Requires-Dist: coloredlogs; extra == "default"
 Requires-Dist: seaborn; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
 Requires-Dist: auto-gpt-plugin-template; extra == "default"
 Requires-Dist: gTTS==2.3.1; extra == "default"
 Requires-Dist: pymysql; extra == "default"
 Requires-Dist: jsonschema; extra == "default"
 Requires-Dist: transformers>=4.34.0; extra == "default"
 Requires-Dist: alembic==1.12.0; extra == "default"
 Requires-Dist: openpyxl==3.1.2; extra == "default"
@@ -281,99 +309,100 @@
 Requires-Dist: bs4; extra == "default"
 Requires-Dist: python-pptx; extra == "default"
 Requires-Dist: python-docx; extra == "default"
 Requires-Dist: pypdf; extra == "default"
 Requires-Dist: python-multipart; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
 Requires-Dist: pymysql; extra == "default"
-Requires-Dist: torch==2.0.1; extra == "default"
-Requires-Dist: torchvision==0.15.2; extra == "default"
-Requires-Dist: torchaudio==2.0.2; extra == "default"
-Requires-Dist: bitsandbytes; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
 Requires-Dist: cpm_kernels; extra == "default"
 Requires-Dist: rocksdict; extra == "default"
 Provides-Extra: all
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: python-docx; extra == "all"
-Requires-Dist: spacy==3.5.3; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: pymssql; extra == "all"
 Requires-Dist: chromadb==0.4.10; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: jinja2; extra == "all"
 Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
+Requires-Dist: protobuf==3.20.3; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: fschat; extra == "all"
 Requires-Dist: pypdf; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
 Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
 Requires-Dist: pympler; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: pyspark; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
 Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: langchain>=0.0.286; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: spacy==3.5.3; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
 Requires-Dist: graphviz; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
 Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: httpx; extra == "all"
+Requires-Dist: fastapi==0.98.0; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: vllm; extra == "all"
 Requires-Dist: msgpack; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: duckdb; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: torchvision==0.15.2; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: protobuf==3.20.3; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
 Requires-Dist: pydantic<2,>=1; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: torch==2.0.1; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: fschat; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
 Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: openai; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: termcolor; extra == "all"
 Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: fastapi==0.98.0; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: torchaudio==2.0.2; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: markdown; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -449,15 +478,15 @@
 
 - **RAG (Retrieval Augmented Generation)**: RAG is currently the most practically implemented and urgently needed domain. DB-GPT has already implemented a framework based on RAG, allowing users to build knowledge-based applications using the RAG capabilities of DB-GPT.
 
 - **GBI (Generative Business Intelligence)**: Generative BI is one of the core capabilities of the DB-GPT project, providing the foundational data intelligence technology to build enterprise report analysis and business insights.
 
 - **Fine-tuning Framework**: Model fine-tuning is an indispensable capability for any enterprise to implement in vertical and niche domains. DB-GPT provides a complete fine-tuning framework that integrates seamlessly with the DB-GPT project. In recent fine-tuning efforts, an accuracy rate based on the Spider dataset has been achieved at 82.5%.
 
-- **Data-Driven Multi-Agents Framework**: DB-GPT offers a data-driven self-evolving fine-tuning framework, aiming to continuously make decisions and execute based on data.
+- **Data-Driven Multi-Agents Framework**: DB-GPT offers a data-driven self-evolving multi-agents framework, aiming to continuously make decisions and execute based on data.
 
 - **Data Factory**: The Data Factory is mainly about cleaning and processing trustworthy knowledge and data in the era of large models.
 
 - **Data Sources**: Integrating various data sources to seamlessly connect production business data to the core capabilities of DB-GPT.
 
 ### SubModule
 - [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) Text-to-SQL workflow with high performance by applying Supervised Fine-Tuning (SFT) on Large Language Models (LLMs).
@@ -527,14 +556,16 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
+    - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
     - 🔥🔥🔥  [Yi-34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat)
   - [More Supported LLMs](http://docs.dbgpt.site/docs/modules/smmf)
```

### Comparing `dbgpt-0.5.3rc0/dbgpt.egg-info/requires.txt` & `dbgpt-0.5.4rc0/dbgpt.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,93 +2,117 @@
 chardet==5.1.0
 importlib-resources==5.12.0
 python-dotenv==1.0.0
 cachetools
 pydantic<2,>=1
 typeguard
 
-[all]
-httpx
-gTTS==2.3.1
-xlrd==2.0.1
-accelerate>=0.20.3
-chardet
+[agent]
+aiohttp==3.8.4
+chardet==5.1.0
+importlib-resources==5.12.0
+python-dotenv==1.0.0
 cachetools
-python-docx
-spacy==3.5.3
+pydantic<2,>=1
+typeguard
+httpx
+fastapi==0.98.0
+prettytable
+click
+psutil==5.9.4
+colorama==0.4.6
+tomlkit
+rich
+termcolor
+pandas==2.0.3
+
+[all]
+python-multipart
+clickhouse-connect
+pymysql
+GitPython
+markdown
+psycopg2
+pymssql
 chromadb==0.4.10
+torchaudio==2.2.1
+alembic==1.12.0
+schedule
 importlib-resources==5.12.0
-pymssql
-psutil==5.9.4
+duckdb-engine
+prettytable
+dashscope
+jinja2
 uvicorn
+duckdb
+SQLAlchemy<2.0.29,>=2.0.25
+python-dotenv==1.0.0
+gpt4all
+chardet
+python-pptx
+llama-cpp-python
+sentencepiece
+protobuf==3.20.3
+colorama==0.4.6
+mysqlclient==2.1.0
+coloredlogs
+fschat
 pypdf
-alembic==1.12.0
+torchvision==0.17.1
+rocksdict
 sqlparse==0.4.4
-bitsandbytes
-pymysql
-colorama==0.4.6
+xlrd==2.0.1
+tomlkit
 pympler
+sentence-transformers
+click
+pandas==2.0.3
+pyspark
+tiktoken
+aiohttp==3.8.4
+zhipuai
+torch==2.2.1
 transformers>=4.34.0
-prettytable
-openpyxl==3.1.2
-gpt4all
-mysqlclient==2.1.0
+pymilvus
+langchain>=0.0.286
+thrift
+bs4
+openai
+thrift_sasl
+spacy==3.5.3
+python-docx
+aiofiles
+tokenizers>=0.14
 graphviz
-pyspark
-rocksdict
 weaviate-client
-coloredlogs
+accelerate>=0.20.3
+psutil==5.9.4
+httpx
+fastapi==0.98.0
+chardet==5.1.0
+pyhive
+seaborn
+bitsandbytes
+vllm
 msgpack
-dashscope
-python-pptx
-duckdb
-jinja2
-SQLAlchemy<2.0.29,>=2.0.25
 auto-gpt-plugin-template
-torchvision==0.15.2
-GitPython
-rich
-protobuf==3.20.3
-thrift_sasl
-seaborn
-cpm_kernels
 pydantic<2,>=1
-pyhive
-pandas==2.0.3
-torch==2.0.1
-pymilvus
-tokenizers>=0.14
-tomlkit
-vllm
-schedule
-bs4
-thrift
-langchain>=0.0.286
-duckdb-engine
-python-multipart
-fschat
+pydoris<2.0.0,>=1.0.2
+rich
+openpyxl==3.1.2
 jsonschema
-psycopg2
-typeguard
-click
-openai
+cachetools
+termcolor
 shortuuid
-chardet==5.1.0
-aiohttp==3.8.4
-sentence-transformers
-tiktoken
-fastapi==0.98.0
-llama-cpp-python
-zhipuai
-python-dotenv==1.0.0
-aiofiles
-clickhouse-connect
-torchaudio==2.0.2
-pydoris<2.0.0,>=1.0.2
-markdown
+typeguard
+gTTS==2.3.1
+cpm_kernels
+
+[bitsandbytes]
+bitsandbytes
 
 [cache]
 rocksdict
 
 [cli]
 aiohttp==3.8.4
 chardet==5.1.0
@@ -144,14 +168,15 @@
 [default]
 tokenizers>=0.14
 accelerate>=0.20.3
 protobuf==3.20.3
 zhipuai
 dashscope
 chardet
+sentencepiece
 aiohttp==3.8.4
 chardet==5.1.0
 importlib-resources==5.12.0
 python-dotenv==1.0.0
 cachetools
 pydantic<2,>=1
 typeguard
@@ -159,28 +184,29 @@
 fastapi==0.98.0
 prettytable
 click
 psutil==5.9.4
 colorama==0.4.6
 tomlkit
 rich
+termcolor
+pandas==2.0.3
 jinja2
 uvicorn
 shortuuid
 SQLAlchemy<2.0.29,>=2.0.25
 msgpack
 pympler
 duckdb
 duckdb-engine
 schedule
 sqlparse==0.4.4
 fschat
 coloredlogs
 seaborn
-pandas==2.0.3
 auto-gpt-plugin-template
 gTTS==2.3.1
 pymysql
 jsonschema
 transformers>=4.34.0
 alembic==1.12.0
 openpyxl==3.1.2
@@ -196,18 +222,17 @@
 markdown
 bs4
 python-pptx
 python-docx
 pypdf
 python-multipart
 sentence-transformers
-torch==2.0.1
-torchvision==0.15.2
-torchaudio==2.0.2
-bitsandbytes
+torch==2.2.1
+torchvision==0.17.1
+torchaudio==2.2.1
 cpm_kernels
 rocksdict
 
 [framework]
 aiohttp==3.8.4
 chardet==5.1.0
 importlib-resources==5.12.0
@@ -219,28 +244,29 @@
 fastapi==0.98.0
 prettytable
 click
 psutil==5.9.4
 colorama==0.4.6
 tomlkit
 rich
+termcolor
+pandas==2.0.3
 jinja2
 uvicorn
 shortuuid
 SQLAlchemy<2.0.29,>=2.0.25
 msgpack
 pympler
 duckdb
 duckdb-engine
 schedule
 sqlparse==0.4.4
 fschat
 coloredlogs
 seaborn
-pandas==2.0.3
 auto-gpt-plugin-template
 gTTS==2.3.1
 pymysql
 jsonschema
 transformers>=4.34.0
 alembic==1.12.0
 openpyxl==3.1.2
@@ -269,28 +295,29 @@
 fastapi==0.98.0
 prettytable
 click
 psutil==5.9.4
 colorama==0.4.6
 tomlkit
 rich
+termcolor
+pandas==2.0.3
 jinja2
 uvicorn
 shortuuid
 SQLAlchemy<2.0.29,>=2.0.25
 msgpack
 pympler
 duckdb
 duckdb-engine
 schedule
 sqlparse==0.4.4
 fschat
 coloredlogs
 seaborn
-pandas==2.0.3
 auto-gpt-plugin-template
 gTTS==2.3.1
 pymysql
 jsonschema
 transformers>=4.34.0
 alembic==1.12.0
 openpyxl==3.1.2
@@ -308,15 +335,14 @@
 python-pptx
 python-docx
 pypdf
 python-multipart
 sentence-transformers
 
 [quantization]
-bitsandbytes
 cpm_kernels
 
 [rag]
 pymilvus
 weaviate-client
 langchain>=0.0.286
 spacy==3.5.3
@@ -341,37 +367,42 @@
 fastapi==0.98.0
 prettytable
 click
 psutil==5.9.4
 colorama==0.4.6
 tomlkit
 rich
+termcolor
+pandas==2.0.3
 jinja2
 uvicorn
 shortuuid
 SQLAlchemy<2.0.29,>=2.0.25
 msgpack
 pympler
 duckdb
 duckdb-engine
 schedule
 sqlparse==0.4.4
 fschat
 
 [torch]
-torch==2.0.1
-torchvision==0.15.2
-torchaudio==2.0.2
+torch==2.2.1
+torchvision==0.17.1
+torchaudio==2.2.1
 
 [torch_cpu]
-torch==2.0.1
-torchvision==0.15.2
-torchaudio==2.0.2
+torch==2.2.1
+torchvision==0.17.1
+torchaudio==2.2.1
 
 [torch_cuda]
+torch==2.2.1
+torchvision==0.17.1
+torchaudio==2.2.1
 
 [vllm]
 vllm
 
 [vstore]
 pymilvus
 weaviate-client
```

### Comparing `dbgpt-0.5.3rc0/setup.py` & `dbgpt-0.5.4rc0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import functools
 import os
 import platform
 import re
 import shutil
 import subprocess
+import sys
 import urllib.request
 from enum import Enum
 from typing import Callable, List, Optional, Tuple
 from urllib.parse import quote, urlparse
 
 import setuptools
 from setuptools import find_packages
 
 with open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 IS_DEV_MODE = os.getenv("IS_DEV_MODE", "true").lower() == "true"
 # If you modify the version, please modify the version in the following files:
 # dbgpt/_version.py
-DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.2")
+DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.4")
 
 BUILD_NO_CACHE = os.getenv("BUILD_NO_CACHE", "true").lower() == "true"
 LLAMA_CPP_GPU_ACCELERATION = (
     os.getenv("LLAMA_CPP_GPU_ACCELERATION", "true").lower() == "true"
 )
 BUILD_FROM_SOURCE = os.getenv("BUILD_FROM_SOURCE", "false").lower() == "true"
 BUILD_FROM_SOURCE_URL_FAST_CHAT = os.getenv(
@@ -36,47 +37,74 @@
         return [
             require.strip()
             for require in f
             if require.strip() and not require.startswith("#")
         ]
 
 
+def find_python():
+    python_path = sys.executable
+    print(python_path)
+    if not python_path:
+        print("Python command not found.")
+        return None
+    return python_path
+
+
 def get_latest_version(package_name: str, index_url: str, default_version: str):
-    python_command = shutil.which("python")
+    python_command = find_python()
     if not python_command:
-        python_command = shutil.which("python3")
-        if not python_command:
-            print("Python command not found.")
-            return default_version
+        print("Python command not found.")
+        return default_version
 
-    command = [
+    command_index_versions = [
         python_command,
         "-m",
         "pip",
         "index",
         "versions",
         package_name,
         "--index-url",
         index_url,
     ]
 
-    result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    if result.returncode != 0:
-        print("Error executing command.")
-        print(result.stderr.decode())
-        return default_version
+    result_index_versions = subprocess.run(
+        command_index_versions, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    )
+    if result_index_versions.returncode == 0:
+        output = result_index_versions.stdout.decode()
+        lines = output.split("\n")
+        for line in lines:
+            if "Available versions:" in line:
+                available_versions = line.split(":")[1].strip()
+                latest_version = available_versions.split(",")[0].strip()
+                # Query for compatibility with the latest version of torch
+                if package_name == "torch" or "torchvision":
+                    latest_version = latest_version.split("+")[0]
+                return latest_version
+    else:
+        command_simulate_install = [
+            python_command,
+            "-m",
+            "pip",
+            "install",
+            f"{package_name}==",
+        ]
 
-    output = result.stdout.decode()
-    lines = output.split("\n")
-    for line in lines:
-        if "Available versions:" in line:
-            available_versions = line.split(":")[1].strip()
-            latest_version = available_versions.split(",")[0].strip()
+        result_simulate_install = subprocess.run(
+            command_simulate_install, stderr=subprocess.PIPE
+        )
+        print(result_simulate_install)
+        stderr_output = result_simulate_install.stderr.decode()
+        print(stderr_output)
+        match = re.search(r"from versions: (.+?)\)", stderr_output)
+        if match:
+            available_versions = match.group(1).split(", ")
+            latest_version = available_versions[-1].strip()
             return latest_version
-
     return default_version
 
 
 def encode_url(package_url: str) -> str:
     parsed_url = urlparse(package_url)
     encoded_path = quote(parsed_url.path)
     safe_url = parsed_url._replace(path=encoded_path).geturl()
@@ -223,15 +251,15 @@
 
 def _build_wheels(
     pkg_name: str,
     pkg_version: str,
     base_url: str = None,
     base_url_func: Callable[[str, str, str], str] = None,
     pkg_file_func: Callable[[str, str, str, str, OSType], str] = None,
-    supported_cuda_versions: List[str] = ["11.7", "11.8"],
+    supported_cuda_versions: List[str] = ["11.8", "12.1"],
 ) -> Optional[str]:
     """
     Build the URL for the package wheel file based on the package name, version, and CUDA version.
     Args:
         pkg_name (str): The name of the package.
         pkg_version (str): The version of the package.
         base_url (str): The base URL for downloading the package.
@@ -244,19 +272,25 @@
     """
     os_type, _ = get_cpu_avx_support()
     cuda_version = get_cuda_version()
     py_version = platform.python_version()
     py_version = "cp" + "".join(py_version.split(".")[0:2])
     if os_type == OSType.DARWIN or not cuda_version:
         return None
-    if cuda_version not in supported_cuda_versions:
+
+    if cuda_version in supported_cuda_versions:
+        cuda_version = cuda_version
+    else:
         print(
-            f"Warnning: {pkg_name} supported cuda version: {supported_cuda_versions}, replace to {supported_cuda_versions[-1]}"
+            f"Warning: Your CUDA version {cuda_version} is not in our set supported_cuda_versions , we will use our set version."
         )
-        cuda_version = supported_cuda_versions[-1]
+        if cuda_version < "12.1":
+            cuda_version = supported_cuda_versions[0]
+        else:
+            cuda_version = supported_cuda_versions[-1]
 
     cuda_version = "cu" + cuda_version.replace(".", "")
     os_pkg_name = "linux_x86_64" if os_type == OSType.LINUX else "win_amd64"
     if base_url_func:
         base_url = base_url_func(pkg_version, cuda_version, py_version)
         if base_url and base_url.endswith("/"):
             base_url = base_url[:-1]
@@ -269,72 +303,77 @@
     if not base_url:
         return full_pkg_file
     else:
         return f"{base_url}/{full_pkg_file}"
 
 
 def torch_requires(
-    torch_version: str = "2.0.1",
-    torchvision_version: str = "0.15.2",
-    torchaudio_version: str = "2.0.2",
+    torch_version: str = "2.2.1",
+    torchvision_version: str = "0.17.1",
+    torchaudio_version: str = "2.2.1",
 ):
+    os_type, _ = get_cpu_avx_support()
     torch_pkgs = [
         f"torch=={torch_version}",
         f"torchvision=={torchvision_version}",
         f"torchaudio=={torchaudio_version}",
     ]
-    torch_cuda_pkgs = []
-    os_type, _ = get_cpu_avx_support()
+    # Initialize torch_cuda_pkgs for non-Darwin OSes;
+    # it will be the same as torch_pkgs for Darwin or when no specific CUDA handling is needed
+    torch_cuda_pkgs = torch_pkgs[:]
+
     if os_type != OSType.DARWIN:
-        cuda_version = get_cuda_version()
-        if cuda_version:
-            supported_versions = ["11.7", "11.8"]
-            # torch_url = f"https://download.pytorch.org/whl/{cuda_version}/torch-{torch_version}+{cuda_version}-{py_version}-{py_version}-{os_pkg_name}.whl"
-            # torchvision_url = f"https://download.pytorch.org/whl/{cuda_version}/torchvision-{torchvision_version}+{cuda_version}-{py_version}-{py_version}-{os_pkg_name}.whl"
-            torch_url = _build_wheels(
-                "torch",
-                torch_version,
-                base_url_func=lambda v, x, y: f"https://download.pytorch.org/whl/{x}",
-                supported_cuda_versions=supported_versions,
-            )
-            torchvision_url = _build_wheels(
-                "torchvision",
-                torchvision_version,
-                base_url_func=lambda v, x, y: f"https://download.pytorch.org/whl/{x}",
-                supported_cuda_versions=supported_versions,
-            )
+        supported_versions = ["11.8", "12.1"]
+        base_url_func = lambda v, x, y: f"https://download.pytorch.org/whl/{x}"
+        torch_url = _build_wheels(
+            "torch",
+            torch_version,
+            base_url_func=base_url_func,
+            supported_cuda_versions=supported_versions,
+        )
+        torchvision_url = _build_wheels(
+            "torchvision",
+            torchvision_version,
+            base_url_func=base_url_func,
+            supported_cuda_versions=supported_versions,
+        )
+
+        # Cache and add CUDA-dependent packages if URLs are available
+        if torch_url:
             torch_url_cached = cache_package(
                 torch_url, "torch", os_type == OSType.WINDOWS
             )
+            torch_cuda_pkgs[0] = f"torch @ {torch_url_cached}"
+        if torchvision_url:
             torchvision_url_cached = cache_package(
                 torchvision_url, "torchvision", os_type == OSType.WINDOWS
             )
+            torch_cuda_pkgs[1] = f"torchvision @ {torchvision_url_cached}"
 
-            torch_cuda_pkgs = [
-                f"torch @ {torch_url_cached}",
-                f"torchvision @ {torchvision_url_cached}",
-                f"torchaudio=={torchaudio_version}",
-            ]
-
+    # Assuming 'setup_spec' is a dictionary where we're adding these dependencies
     setup_spec.extras["torch"] = torch_pkgs
     setup_spec.extras["torch_cpu"] = torch_pkgs
     setup_spec.extras["torch_cuda"] = torch_cuda_pkgs
 
 
 def llama_cpp_python_cuda_requires():
     cuda_version = get_cuda_version()
+    supported_cuda_versions = ["11.8", "12.1"]
     device = "cpu"
     if not cuda_version:
         print("CUDA not support, use cpu version")
         return
     if not LLAMA_CPP_GPU_ACCELERATION:
         print("Disable GPU acceleration")
         return
     # Supports GPU acceleration
-    device = "cu" + cuda_version.replace(".", "")
+    if cuda_version <= "11.8" and not None:
+        device = "cu" + supported_cuda_versions[0].replace(".", "")
+    else:
+        device = "cu" + supported_cuda_versions[-1].replace(".", "")
     os_type, cpu_avx = get_cpu_avx_support()
     print(f"OS: {os_type}, cpu avx: {cpu_avx}")
     supported_os = [OSType.WINDOWS, OSType.LINUX]
     if os_type not in supported_os:
         print(
             f"llama_cpp_python_cuda just support in os: {[r._value_ for r in supported_os]}"
         )
@@ -342,15 +381,15 @@
     cpu_device = ""
     if cpu_avx == AVXType.AVX2 or cpu_avx == AVXType.AVX512:
         cpu_device = "avx"
     else:
         cpu_device = "basic"
     device += cpu_device
     base_url = "https://github.com/jllllll/llama-cpp-python-cuBLAS-wheels/releases/download/textgen-webui"
-    llama_cpp_version = "0.2.10"
+    llama_cpp_version = "0.2.26"
     py_version = "cp310"
     os_pkg_name = "manylinux_2_31_x86_64" if os_type == OSType.LINUX else "win_amd64"
     extra_index_url = f"{base_url}/llama_cpp_python_cuda-{llama_cpp_version}+{device}-{py_version}-{py_version}-{os_pkg_name}.whl"
     extra_index_url, _ = encode_url(extra_index_url)
     print(f"Install llama_cpp_python_cuda from {extra_index_url}")
 
     setup_spec.extras["llama_cpp"].append(f"llama_cpp_python_cuda @ {extra_index_url}")
@@ -380,18 +419,26 @@
         "prettytable",
         "click",
         "psutil==5.9.4",
         "colorama==0.4.6",
         "tomlkit",
         "rich",
     ]
+    # Agent dependencies
+    setup_spec.extras["agent"] = setup_spec.extras["cli"] + [
+        "termcolor",
+        # https://github.com/eosphoros-ai/DB-GPT/issues/551
+        # TODO: remove pandas dependency
+        "pandas==2.0.3",
+    ]
+
     # Just use by DB-GPT internal, we should find the smallest dependency set for run
     # we core unit test.
     # The dependency "framework" is too large for now.
-    setup_spec.extras["simple_framework"] = setup_spec.extras["cli"] + [
+    setup_spec.extras["simple_framework"] = setup_spec.extras["agent"] + [
         "jinja2",
         "uvicorn",
         "shortuuid",
         # 2.0.29 not support duckdb now
         "SQLAlchemy>=2.0.25,<2.0.29",
         # for cache
         "msgpack",
@@ -413,16 +460,14 @@
         )
     else:
         setup_spec.extras["simple_framework"].append("fschat")
 
     setup_spec.extras["framework"] = setup_spec.extras["simple_framework"] + [
         "coloredlogs",
         "seaborn",
-        # https://github.com/eosphoros-ai/DB-GPT/issues/551
-        "pandas==2.0.3",
         "auto-gpt-plugin-template",
         "gTTS==2.3.1",
         "pymysql",
         "jsonschema",
         # TODO move transformers to default
         # "transformers>=4.31.0",
         "transformers>=4.34.0",
@@ -465,88 +510,47 @@
     llama_cpp_python_cuda_requires()
 
 
 def _build_autoawq_requires() -> Optional[str]:
     os_type, _ = get_cpu_avx_support()
     if os_type == OSType.DARWIN:
         return None
-    auto_gptq_version = get_latest_version(
-        "auto-gptq", "https://huggingface.github.io/autogptq-index/whl/cu118/", "0.5.1"
-    )
-    # eg. 0.5.1+cu118
-    auto_gptq_version = auto_gptq_version.split("+")[0]
-
-    def pkg_file_func(pkg_name, pkg_version, cuda_version, py_version, os_type):
-        pkg_name = pkg_name.replace("-", "_")
-        if os_type == OSType.DARWIN:
-            return None
-        os_pkg_name = (
-            "manylinux_2_17_x86_64.manylinux2014_x86_64.whl"
-            if os_type == OSType.LINUX
-            else "win_amd64.whl"
-        )
-        return f"{pkg_name}-{pkg_version}+{cuda_version}-{py_version}-{py_version}-{os_pkg_name}"
-
-    auto_gptq_url = _build_wheels(
-        "auto-gptq",
-        auto_gptq_version,
-        base_url_func=lambda v, x, y: f"https://huggingface.github.io/autogptq-index/whl/{x}/auto-gptq",
-        pkg_file_func=pkg_file_func,
-        supported_cuda_versions=["11.8"],
-    )
-    if auto_gptq_url:
-        print(f"Install auto-gptq from {auto_gptq_url}")
-        return f"auto-gptq @ {auto_gptq_url}"
-    else:
-        "auto-gptq"
+    return "auto-gptq"
 
 
 def quantization_requires():
-    pkgs = []
     os_type, _ = get_cpu_avx_support()
-    if os_type != OSType.WINDOWS:
-        pkgs = ["bitsandbytes"]
-    else:
+    quantization_pkgs = []
+    if os_type == OSType.WINDOWS:
+        # For Windows, fetch a specific bitsandbytes WHL package
         latest_version = get_latest_version(
             "bitsandbytes",
             "https://jllllll.github.io/bitsandbytes-windows-webui",
             "0.41.1",
         )
-        extra_index_url = f"https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-{latest_version}-py3-none-win_amd64.whl"
-        local_pkg = cache_package(
-            extra_index_url, "bitsandbytes", os_type == OSType.WINDOWS
-        )
-        pkgs = [f"bitsandbytes @ {local_pkg}"]
-        print(pkgs)
-    # For chatglm2-6b-int4
-    pkgs += ["cpm_kernels"]
+        whl_url = f"https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-{latest_version}-py3-none-win_amd64.whl"
+        local_pkg_path = cache_package(whl_url, "bitsandbytes", True)
+        setup_spec.extras["bitsandbytes"] = [f"bitsandbytes @ {local_pkg_path}"]
+    else:
+        setup_spec.extras["bitsandbytes"] = ["bitsandbytes"]
 
     if os_type != OSType.DARWIN:
         # Since transformers 4.35.0, the GPT-Q/AWQ model can be loaded using AutoModelForCausalLM.
         # autoawq requirements:
         # 1. Compute Capability 7.5 (sm75). Turing and later architectures are supported.
         # 2. CUDA Toolkit 11.8 and later.
-        autoawq_url = _build_wheels(
-            "autoawq",
-            "0.1.7",
-            base_url_func=lambda v, x, y: f"https://github.com/casper-hansen/AutoAWQ/releases/download/v{v}",
-            supported_cuda_versions=["11.8"],
-        )
-        if autoawq_url:
-            print(f"Install autoawq from {autoawq_url}")
-            pkgs.append(f"autoawq @ {autoawq_url}")
+        cuda_version = get_cuda_version()
+        autoawq_latest_version = get_latest_version("autoawq", "", "0.2.4")
+        if cuda_version is None or cuda_version == "12.1":
+            quantization_pkgs.extend(["autoawq", _build_autoawq_requires(), "optimum"])
         else:
-            pkgs.append("autoawq")
-
-        auto_gptq_pkg = _build_autoawq_requires()
-        if auto_gptq_pkg:
-            pkgs.append(auto_gptq_pkg)
-            pkgs.append("optimum")
+            # TODO(yyhhyy): Add autoawq install method for CUDA version 11.8
+            quantization_pkgs.extend(["autoawq", _build_autoawq_requires(), "optimum"])
 
-    setup_spec.extras["quantization"] = pkgs
+    setup_spec.extras["quantization"] = ["cpm_kernels"] + quantization_pkgs
 
 
 def all_vector_store_requires():
     """
     pip install "dbgpt[vstore]"
     """
     setup_spec.extras["vstore"] = [
@@ -626,14 +630,15 @@
         # "tokenizers==0.13.3",
         "tokenizers>=0.14",
         "accelerate>=0.20.3",
         "protobuf==3.20.3",
         "zhipuai",
         "dashscope",
         "chardet",
+        "sentencepiece",
     ]
     setup_spec.extras["default"] += setup_spec.extras["framework"]
     setup_spec.extras["default"] += setup_spec.extras["rag"]
     setup_spec.extras["default"] += setup_spec.extras["datasource"]
     setup_spec.extras["default"] += setup_spec.extras["torch"]
     setup_spec.extras["default"] += setup_spec.extras["quantization"]
     setup_spec.extras["default"] += setup_spec.extras["cache"]
@@ -678,14 +683,16 @@
 else:
     packages = find_packages(
         exclude=excluded_packages,
         include=[
             "dbgpt",
             "dbgpt._private",
             "dbgpt._private.*",
+            "dbgpt.agent",
+            "dbgpt.agent.*",
             "dbgpt.cli",
             "dbgpt.cli.*",
             "dbgpt.client",
             "dbgpt.client.*",
             "dbgpt.configs",
             "dbgpt.configs.*",
             "dbgpt.core",
@@ -702,14 +709,16 @@
             "dbgpt.model.adapter",
             "dbgpt.rag",
             "dbgpt.rag.*",
             "dbgpt.storage",
             "dbgpt.storage.*",
             "dbgpt.util",
             "dbgpt.util.*",
+            "dbgpt.vis",
+            "dbgpt.vis.*",
         ],
     )
 
 setuptools.setup(
     name="dbgpt",
     packages=packages,
     version=DB_GPT_VERSION,
```

