# Comparing `tmp/MindsDB-24.3.5.0.tar.gz` & `tmp/MindsDB-24.4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MindsDB-24.3.5.0.tar", last modified: Tue Mar 26 10:48:19 2024, max compression
+gzip compressed data, was "MindsDB-24.4.2.0.tar", last modified: Wed Apr 10 21:13:20 2024, max compression
```

## Comparing `MindsDB-24.3.5.0.tar` & `MindsDB-24.4.2.0.tar`

### file list

```diff
@@ -1,2061 +1,2066 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     5804 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.509503 MindsDB-24.3.5.0/MindsDB.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-03-26 10:48:19.000000 MindsDB-24.3.5.0/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)   100113 2024-03-26 10:48:19.000000 MindsDB-24.3.5.0/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:48:19.000000 MindsDB-24.3.5.0/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    11044 2024-03-26 10:48:19.000000 MindsDB-24.3.5.0/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:48:19.000000 MindsDB-24.3.5.0/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     9634 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      189 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/default_handlers.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/
--rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13786 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/common/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1345 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)       51 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    83978 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/command_executor.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/controllers/
--rw-r--r--   0 runner    (1000) runner    (1000)      267 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/controllers/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4371 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/data_types/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/data_types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      673 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/data_types/answer.py
--rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/data_types/response_type.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/classes/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1794 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1000) runner    (1000)      175 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datahub.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/
--rw-r--r--   0 runner    (1000) runner    (1000)      185 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34279 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8227 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7001 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/project_datanode.py
--rw-r--r--   0 runner    (1000) runner    (1000)      566 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6775 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/result_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11126 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/sql_query.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/
--rw-r--r--   0 runner    (1000) runner    (1000)      728 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15677 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1286 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/delete_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3809 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3333 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/insert_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3164 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/join_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4728 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/map_reduce_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)      653 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/multiple_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1504 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/prepare_steps.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2802 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/project_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1001 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/sql_steps.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4149 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/subselect_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1619 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/union_step.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4471 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/update_step.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/executor/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      995 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/utilities/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6049 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/executor/utilities/sql.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/http/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3087 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14068 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.513503 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10916 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/agents.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3810 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5483 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10832 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/chatbots.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9382 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      124 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/agents.py
--rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/chatbots.py
--rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)      147 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1000) runner    (1000)       86 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1000) runner    (1000)      107 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/skills.py
--rw-r--r--   0 runner    (1000) runner    (1000)       98 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)       93 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10920 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4729 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6287 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6739 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11226 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1203 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5923 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/skills.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5359 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4054 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3380 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4569 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5675 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2096 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1170 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1000) runner    (1000)      177 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      746 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1764 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1000) runner    (1000)      769 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3217 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1000) runner    (1000)      812 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1000) runner    (1000)      266 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1000) runner    (1000)     2655 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2364 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1000) runner    (1000)      317 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1767 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1000) runner    (1000)      689 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1000) runner    (1000)      825 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4221 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1000) runner    (1000)      230 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5835 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1000) runner    (1000)      314 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1000) runner    (1000)      272 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1000) runner    (1000)      244 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9421 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1000) runner    (1000)      446 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1536 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1000) runner    (1000)      223 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1000) runner    (1000)      235 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1000) runner    (1000)      890 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1004 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1000) runner    (1000)      180 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14062 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1000) runner    (1000)      420 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7666 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4256 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2147 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3358 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1000) runner    (1000)       75 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      939 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)      586 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4436 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.517503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6316 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5094 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1000) runner    (1000)     1550 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4620 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1097 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2982 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5765 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1428 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1520 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)      486 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2927 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3770 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3785 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)      421 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1523 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1426 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1494 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1452 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5422 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9576 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)      619 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5534 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4116 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35316 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33693 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2341 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/nlp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6499 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12729 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1121 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1093 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40804 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1000) runner    (1000)      626 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8422 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19392 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)      259 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/integrations/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      633 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6392 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2406 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       25 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1074 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      670 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9103 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.521503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1139 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6830 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      182 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1938 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7556 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/requirements.txt
--rwxr-xr-x   0 runner    (1000) runner    (1000)      649 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      588 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3398 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-03-26 10:47:49.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8306 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1743 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      319 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/apache_doris_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1933 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      909 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/aqicn.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3216 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12837 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3304 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/icon.png
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6352 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      690 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      131 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1188 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)      956 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      560 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5618 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      693 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.525503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      710 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15729 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      584 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2303 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      914 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      484 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5334 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7458 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1020 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      475 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23840 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4454 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1645 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14968 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1353 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14733 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4199 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       25 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1950 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15883 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      472 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3515 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8453 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6583 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      387 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1445 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      555 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3157 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1759 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      669 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7521 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    75313 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1592 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      366 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5153 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27975 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)      195 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.529503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1857 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1187 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      542 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3248 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1163 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6043 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1658 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1909 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2768 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7031 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2500 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2163 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8067 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1237 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7007 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      634 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1484 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2136 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       68 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1687 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6919 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2675 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1231 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      685 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1000) runner    (1000)    86110 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    58645 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    35986 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    21694 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)    62078 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1000) runner    (1000)     8455 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.533503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1302 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      544 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      327 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      445 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8885 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56094 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1439 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8768 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2278 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1513 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5600 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/discord_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5899 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/discord_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1330 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2172 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2277 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4222 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16832 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3562 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2899 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       66 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7312 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5946 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1109 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7665 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2823 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1084 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dummy_data_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dummy_data_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      491 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dummy_data_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2740 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dummy_data_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      638 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6618 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1929 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.537503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      617 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1869 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      742 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8374 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3383 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1120 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2734 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_ingestor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5209 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32416 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1632 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      399 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7739 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)   328372 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1843 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3267 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18318 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7954 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9086 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2404 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10364 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1144 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14717 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/file_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      185 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/data/
--rw-r--r--   0 runner    (1000) runner    (1000)      570 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/data/test.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    12750 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9639 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4207 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       41 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1243 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.541503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1617 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4374 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7988 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2648 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4645 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30742 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1198 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2587 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15320 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1995 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      528 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20489 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      862 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1332 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      532 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4718 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10179 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1815 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      379 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6268 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)      962 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11062 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8111 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1915 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      110 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2215 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      424 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16267 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14279 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2651 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2436 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      495 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6631 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1511 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.545503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      581 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2647 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8089 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7375 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3303 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2178 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3722 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5281 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11129 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2135 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5972 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17076 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1638 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7519 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41120 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2796 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19979 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1453 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      536 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8782 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      549 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8085 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/finetune.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13592 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       77 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/requirements_cpu.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      984 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      761 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7598 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1013 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3532 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5655 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1559 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.549503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      514 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2681 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3065 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3019 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3200 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9626 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       89 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1702 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      389 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2321 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7607 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       79 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1817 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      987 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4076 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15203 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3716 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3738 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4953 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      508 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1246 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3225 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5472 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      758 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1986 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3475 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    14420 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       37 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7473 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    25097 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2737 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1704 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1000) runner    (1000)      259 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    11328 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/tools.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    99151 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1387 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6271 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.553503 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      540 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18709 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11253 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     3186 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20193 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5263 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1678 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6788 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      143 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9139 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    23643 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       91 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10985 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2242 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6694 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37122 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     4899 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2488 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2269 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12609 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    11554 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2395 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      250 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6041 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     1939 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/luma.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2434 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/luma_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5495 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/luma_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.557502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2843 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      315 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      501 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2689 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1285 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      612 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1573 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6895 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1776 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2141 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7528 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1905 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18250 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2182 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3299 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2721 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8696 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4456 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4330 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8498 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2657 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8238 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1117 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    20322 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1154 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3802 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8134 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1622 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1134 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      573 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9693 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3890 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.561502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6960 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14734 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3934 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7981 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5389 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22215 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    10638 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11944 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4660 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3895 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4136 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    10843 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      587 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6374 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements_extra.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      662 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2790 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     7178 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3188 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      575 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2157 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7537 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/notion_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12946 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/notion_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2037 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      786 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)      674 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1651 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/npm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9036 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/npm_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9850 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1626 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2615 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1741 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.565502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1695 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3389 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6516 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   113588 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     6030 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/constants.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5534 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2625 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    36107 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       34 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      373 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      525 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11289 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      613 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1758 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1390 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1379 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2669 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7765 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1228 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7078 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1064 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      810 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1307 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1747 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1485 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    16725 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/palm_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1833 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3815 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9866 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13760 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    11463 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       76 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.569502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43812 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     8788 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2683 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    14972 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10555 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8603 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1132 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      695 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54926 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     8203 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1389 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     8103 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5151 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      149 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      621 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      391 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1327 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      562 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3114 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13757 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    10782 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5815 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      564 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10283 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)     4759 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       24 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/test/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/test/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10377 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4258 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18842 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     1907 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7043 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    19040 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2029 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.573502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1172 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1289 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3395 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13384 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5873 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/ingest.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4758 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/rag.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/rag_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      230 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    15361 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      595 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1990 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     2661 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3986 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     3265 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6558 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1000) runner    (1000)        4 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      765 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7618 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1212 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.577502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/
--rw-r--r--   0 runner    (1000) runner    (1000)   355320 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png
--rw-r--r--   0 runner    (1000) runner    (1000)  1314584 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/groot.png
--rw-r--r--   0 runner    (1000) runner    (1000)  1556534 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6893 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      499 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2492 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5293 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6298 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      539 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       72 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1424 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   194064 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1000) runner    (1000)   108141 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      591 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     7336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2168 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5407 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    59422 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9670 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8412 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1290 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2730 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2601 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10852 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      394 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2691 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       70 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2686 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      276 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/settings.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)    20746 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4175 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17973 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1896 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5229 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5628 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5785 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1059 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.581502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2452 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     4954 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31708 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2064 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1446 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    17306 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      882 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4088 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     4746 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1309 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5647 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/solace_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     6928 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3544 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5829 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     7023 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      623 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3379 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1033 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19052 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     6297 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1434 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1284 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7274 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1945 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1301 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1746 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.585502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/requirements_extra.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8220 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      529 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     5441 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4803 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1904 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3433 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8188 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      704 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2858 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16193 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1174 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      326 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1408 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1449 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     7492 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1891 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      632 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3586 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18160 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4903 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5370 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1564 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      465 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8286 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      593 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      470 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1338 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      390 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     9845 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      497 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6197 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.589502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1552 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1242 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      526 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   114250 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3335 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      457 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9363 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1630 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6813 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      527 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)     9888 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10822 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14054 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      559 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2110 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     9351 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16821 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10747 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1547 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    13129 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      471 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    16111 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/api_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/api_utilities/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/
--rw-r--r--   0 runner    (1000) runner    (1000)       56 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3086 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      148 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/exceptions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/
--rw-r--r--   0 runner    (1000) runner    (1000)       55 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4226 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_oauth_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/
--rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4114 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)      279 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1555 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)      432 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3110 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4239 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2557 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/validation_utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       72 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/validation_utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      678 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.593502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      498 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23708 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/icon.png
--rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/requirements.txt
--rwxr-xr-x   0 runner    (1000) runner    (1000)     3634 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/vertex_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3664 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1482 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1663 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6038 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2834 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1727 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   115913 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    25567 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1385 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1046 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/tests/example_data.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1516 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10860 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3161 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/web_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1042 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5777 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/webz_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6219 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/webz_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3521 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)    14477 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12498 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/evaluate.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1814 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/ingest.py
--rw-r--r--   0 runner    (1000) runner    (1000)      409 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/rag.py
--rw-r--r--   0 runner    (1000) runner    (1000)      166 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     2878 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6883 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      646 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2726 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16519 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/xata_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      954 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     5286 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16797 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3292 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1612 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1969 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.597502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/
--rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/__about__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1113 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/tests/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2043 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3953 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15080 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1375 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5252 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_client/db_grpc_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7869 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5549 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1098 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10701 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)      236 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/api_handler_exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12851 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)      407 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1931 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17269 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/llm_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16707 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_exec_base.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/
--rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      444 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/create_validation_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4225 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/describe_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      771 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6498 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/learn_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1346 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/predict_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      784 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/update_process.py
--rw-r--r--   0 runner    (1000) runner    (1000)      966 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14566 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/process_cache.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1171 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/realtime_chat_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3119 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/storage_handler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15599 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/libs/vectordatabase_handler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1665 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/dataset.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/question_answering/
--rw-r--r--   0 runner    (1000) runner    (1000)     6906 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv
--rw-r--r--   0 runner    (1000) runner    (1000)   104035 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv
--rw-r--r--   0 runner    (1000) runner    (1000)     2769 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2113 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/handler_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      977 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1000) runner    (1000)      384 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5928 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      684 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)      972 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/interfaces/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/interfaces/agents/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/agents/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11433 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/agents/agents_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11171 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/chatbot_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6514 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/chatbot_executor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3790 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/chatbot_task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5550 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/memory.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3473 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/model_executor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4292 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/polling.py
--rw-r--r--   0 runner    (1000) runner    (1000)      929 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/types.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4063 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28097 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11064 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/database/log.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11134 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3737 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.601502 MindsDB-24.3.5.0/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4629 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14357 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3602 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/knowledge_base/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/knowledge_base/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13849 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/knowledge_base/controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20365 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/query_context/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/query_context/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8971 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/query_context/context_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7156 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/query_context/last_query.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/skills/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/skills/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4240 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/skills/skill_tool.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5414 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/skills/skills_controller.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7268 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/skills/sql_agent.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17504 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19996 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2925 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8267 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/tabs/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/tabs/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8761 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/tabs/tabs_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/tasks/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/tasks/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      401 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/tasks/task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3863 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/tasks/task_monitor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1666 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/tasks/task_thread.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/interfaces/triggers/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/triggers/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2911 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/triggers/trigger_task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5376 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/interfaces/triggers/triggers_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/metrics/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/metrics/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1819 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/metrics/metrics.py
--rw-r--r--   0 runner    (1000) runner    (1000)      985 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/metrics/server.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2327 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12845 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14810 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2170 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5430 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.605502 MindsDB-24.3.5.0/mindsdb/migrations/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2193 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1000) runner    (1000)     2218 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1000) runner    (1000)     5871 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10817 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6163 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2788 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1000) runner    (1000)      849 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1000) runner    (1000)      998 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1045 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2330 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1957 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1789 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2384 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3486 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1802 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3487 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)      799 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2035 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1008 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1115 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1000) runner    (1000)      836 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1000) runner    (1000)      930 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1567 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
--rw-r--r--   0 runner    (1000) runner    (1000)      730 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      856 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1138 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1940 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py
--rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py
--rw-r--r--   0 runner    (1000) runner    (1000)      732 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      983 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      605 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2519 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)      701 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1023 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py
--rw-r--r--   0 runner    (1000) runner    (1000)      824 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1323 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py
--rw-r--r--   0 runner    (1000) runner    (1000)      837 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1419 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/mindsdb/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7245 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6450 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1450 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/context_executor.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1034 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/exception.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4662 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6345 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2262 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1039 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/
--rw-r--r--   0 runner    (1000) runner    (1000)     2810 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/base.py
--rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/const.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9413 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/consumer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2702 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/producer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3166 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/task.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3177 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1000) runner    (1000)      251 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3936 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2339 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1000) runner    (1000)      751 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/security.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1377 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1708 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1000) runner    (1000)      122 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/requirements/
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/requirements/requirements-grpc.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      790 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-26 10:48:19.609501 MindsDB-24.3.5.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     5998 2024-03-26 10:47:50.000000 MindsDB-24.3.5.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5804 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-04-10 21:13:20.000000 MindsDB-24.4.2.0/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)   100365 2024-04-10 21:13:20.000000 MindsDB-24.4.2.0/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:20.000000 MindsDB-24.4.2.0/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    10883 2024-04-10 21:13:20.000000 MindsDB-24.4.2.0/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:20.000000 MindsDB-24.4.2.0/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    14576 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     9634 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      189 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/default_handlers.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/
+-rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13732 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/common/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)       51 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    83269 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/command_executor.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/controllers/
+-rw-r--r--   0 runner    (1000) runner    (1000)      267 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/controllers/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4371 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/data_types/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/data_types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      673 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/data_types/answer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/data_types/response_type.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/classes/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1794 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      175 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datahub.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/
+-rw-r--r--   0 runner    (1000) runner    (1000)      185 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34279 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8233 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7001 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/project_datanode.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      566 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.225937 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6775 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/result_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11126 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/sql_query.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/
+-rw-r--r--   0 runner    (1000) runner    (1000)      728 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15677 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1286 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/delete_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3809 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3333 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/insert_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3164 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/join_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4728 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/map_reduce_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      653 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/multiple_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/prepare_steps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2802 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/project_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1001 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/sql_steps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4149 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/subselect_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1619 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/union_step.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4471 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/update_step.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/executor/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      995 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/utilities/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6049 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/executor/utilities/sql.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/http/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3087 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14068 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10916 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/agents.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3810 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5483 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10832 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/chatbots.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9382 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      124 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/agents.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/chatbots.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      147 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      103 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       86 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      107 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      130 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/skills.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       98 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       93 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10920 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4729 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6319 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6739 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11226 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1203 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5923 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/skills.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4054 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3380 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4569 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5675 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2096 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      589 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1000) runner    (1000)      177 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      746 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1764 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3217 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      812 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.229937 MindsDB-24.4.2.0/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1000) runner    (1000)      266 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2655 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2364 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      317 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1767 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      689 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      825 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4221 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      230 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5835 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      314 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      272 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      244 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9421 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      446 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1536 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      223 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      235 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      890 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1004 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      180 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14062 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      420 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7666 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4256 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2147 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3358 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1000) runner    (1000)       75 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      939 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      586 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4436 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6316 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5094 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1550 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4620 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1097 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2982 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5765 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1428 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1520 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      486 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2927 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3770 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3785 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      421 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1523 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1426 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1494 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1452 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5422 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9576 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      619 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5534 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4116 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35316 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33693 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2341 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/nlp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.233937 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6499 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12729 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1121 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1093 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40804 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      626 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8422 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19392 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)      259 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      633 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6392 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2406 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       25 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1074 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      670 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9103 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1139 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6830 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      182 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1938 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7556 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/requirements.txt
+-rwxr-xr-x   0 runner    (1000) runner    (1000)      649 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      588 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3398 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      538 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8306 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1743 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      319 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/apache_doris_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1933 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      909 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/aqicn.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3216 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12837 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3304 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/icon.png
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.237937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6352 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      690 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      131 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1188 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      956 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      560 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5618 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      693 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      710 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15729 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      584 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2303 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       50 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      914 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      484 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5334 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7458 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1020 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      475 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23890 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4454 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1645 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14968 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1353 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14733 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4199 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1950 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15883 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      472 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3515 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8453 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6583 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      387 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1445 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.241937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      555 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3157 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1759 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      669 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7521 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    75313 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1592 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      366 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5153 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27975 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)      195 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1157 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1857 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1187 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      542 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3248 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1163 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      577 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6043 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1658 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1909 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      522 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2768 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7031 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2500 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2163 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8067 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1683 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1237 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7007 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      634 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1484 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2136 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       68 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1687 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6919 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2675 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.245937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1231 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      685 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1000) runner    (1000)    86110 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    58645 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    35986 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    21694 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)    62078 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8455 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      618 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1302 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      544 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      327 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      445 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       65 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8885 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56094 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1439 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8768 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2278 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1513 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5600 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/discord_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5899 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/discord_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1330 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2172 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2277 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4222 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16832 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3562 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2899 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       66 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7312 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5946 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1109 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      362 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7665 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2823 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1084 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.249937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dummy_data_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      228 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dummy_data_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      491 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dummy_data_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2740 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dummy_data_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      638 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6618 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1929 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      617 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1869 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      742 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8374 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3383 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1120 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2734 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_ingestor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5209 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32416 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1632 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      399 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      615 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7739 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   328372 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1843 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3267 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18318 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7954 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9086 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2404 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10364 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      807 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1144 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14717 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/file_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      185 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.253937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/data/
+-rw-r--r--   0 runner    (1000) runner    (1000)      570 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/data/test.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    12750 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9639 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4207 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       41 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1243 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1617 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3096 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4374 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7988 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2648 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      920 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4645 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30742 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1198 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2587 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15320 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1995 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      528 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20489 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      862 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1479 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1332 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      532 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4718 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10179 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1815 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      379 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6268 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      962 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11062 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8111 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1915 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      110 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2215 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      424 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16267 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14279 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2651 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.257937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2436 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      358 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      495 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6631 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1511 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      581 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2647 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8089 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7375 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3303 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2178 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3722 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5281 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11129 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2135 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      592 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5972 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17076 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1638 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7519 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41120 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2796 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19979 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1453 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      381 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      536 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      112 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8782 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      128 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      549 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8085 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/finetune.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13592 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9064 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       77 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/requirements_cpu.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      984 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      761 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7598 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.261937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1013 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3532 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5655 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1559 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      514 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2681 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3065 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3019 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3200 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9626 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       89 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1702 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      389 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      627 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2321 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7607 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       79 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1817 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      987 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4076 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15203 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3716 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3738 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4953 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      508 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1246 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3225 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5472 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      758 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1986 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      661 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3475 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    14420 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       37 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      561 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7473 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.265936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1989 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/constants.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73222 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    13763 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2737 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1704 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      259 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    11201 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/tools.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    99151 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1387 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6271 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      540 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18709 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11253 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     3186 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20193 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5263 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1678 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6788 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      143 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9139 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    23643 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       91 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10985 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2242 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      534 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6694 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      341 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37122 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     4899 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2488 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2269 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12609 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    11554 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      535 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      414 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2395 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      250 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6041 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     1939 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/luma.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2434 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/luma_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5495 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/luma_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.269936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2843 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      315 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      501 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2689 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1285 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1774 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      612 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1573 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6895 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1776 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2141 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7528 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1905 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18250 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2182 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3299 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2721 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8696 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4456 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4330 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8498 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2657 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8238 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1117 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    20322 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1154 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3802 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      611 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8134 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1622 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1134 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      573 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9693 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3890 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.273937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6960 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14734 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      357 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3934 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7981 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5389 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22215 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    10638 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11944 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4830 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4382 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4136 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    10843 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      587 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6374 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements_extra.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      662 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2790 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     7178 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3188 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      575 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2157 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7537 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/notion_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12946 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/notion_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2037 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      328 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      516 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      786 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      674 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1651 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/npm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9036 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/npm_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9850 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1626 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2615 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1293 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1741 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.277937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      658 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1695 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3389 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6516 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   113588 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     6030 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1190 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/constants.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5771 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2625 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    36366 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       34 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      373 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      525 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11289 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       33 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      613 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1758 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1390 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1379 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2669 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7765 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1228 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      537 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7078 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1064 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      810 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1307 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1747 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1485 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    16725 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/palm_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1833 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3815 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9866 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13760 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    11463 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       76 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43812 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     8788 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.281937 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1037 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      666 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2683 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    14972 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      353 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      602 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10555 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8603 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1132 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      380 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      695 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54926 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     8203 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      492 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1389 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     8103 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5151 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      149 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      621 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      391 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1327 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      388 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      562 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3114 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13757 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    10782 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5815 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      564 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10283 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     4759 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       24 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/test/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/test/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10377 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4258 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18842 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1907 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7043 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1629 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    19040 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      485 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2029 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1172 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.285936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1289 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3395 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13384 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      337 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2542 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5873 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/ingest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4758 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/rag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4978 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/rag_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      250 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    15414 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      595 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1990 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2661 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3986 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     3265 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6558 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        4 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      636 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      765 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7618 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1212 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      550 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.289936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/
+-rw-r--r--   0 runner    (1000) runner    (1000)   355320 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png
+-rw-r--r--   0 runner    (1000) runner    (1000)  1314584 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/groot.png
+-rw-r--r--   0 runner    (1000) runner    (1000)  1556534 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6893 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      499 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2492 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5293 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6298 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      539 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1362 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   194064 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1000) runner    (1000)   108141 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      591 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1930 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     7336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1249 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2168 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5407 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    59422 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/tests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9670 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8412 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1290 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2730 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2601 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10852 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      394 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2691 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       61 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2686 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      276 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/settings.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)    20746 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4175 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17973 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1896 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5229 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      356 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5628 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5785 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1059 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.293936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2452 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     4954 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31708 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2064 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1446 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      334 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      518 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2005 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    17306 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      882 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4088 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     4746 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1309 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      354 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      480 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      152 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5647 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/solace_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      332 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      599 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       15 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     6928 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1215 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      487 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3544 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5829 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       27 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     7023 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      623 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3379 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     6000 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1033 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19052 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     6297 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1434 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1284 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     6901 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7274 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      493 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1945 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1301 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1746 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.297936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      374 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      515 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       21 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/requirements_extra.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8220 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      529 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5441 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4803 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1904 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      628 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3433 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8188 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      507 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      704 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2858 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16193 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1174 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      326 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1408 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      376 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      607 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1449 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     7492 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1891 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      632 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3586 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18160 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4903 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5370 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1564 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      345 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      608 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      465 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8286 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      329 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      593 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      470 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1334 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1338 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      390 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      590 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     9845 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.301936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      355 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      497 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6197 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1552 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1242 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      335 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      526 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   114250 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3335 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      457 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9363 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1630 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      359 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6813 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      363 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      527 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)     9888 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10822 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14054 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      352 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      559 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2110 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     9351 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16821 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10747 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      496 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1547 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    13129 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      500 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      471 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    16111 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/api_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       43 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/api_utilities/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/
+-rw-r--r--   0 runner    (1000) runner    (1000)       56 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3086 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)      123 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/exceptions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/
+-rw-r--r--   0 runner    (1000) runner    (1000)      150 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2412 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_service_account_oauth_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4230 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/
+-rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4114 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)      279 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1555 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      432 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3110 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4239 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2557 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/validation_utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       72 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/validation_utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      678 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.305936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      498 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23708 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/icon.png
+-rw-r--r--   0 runner    (1000) runner    (1000)       32 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/requirements.txt
+-rwxr-xr-x   0 runner    (1000) runner    (1000)     3942 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/vertex_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3924 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      604 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1482 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1663 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6038 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      481 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2834 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1727 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1277 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      343 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   115913 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    25567 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1385 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1046 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/tests/example_data.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1516 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10860 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3161 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/web_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      521 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1042 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       84 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5777 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/webz_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6219 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/webz_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      533 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3521 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        6 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)    14477 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      545 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12498 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/evaluate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1814 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/ingest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      409 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/rag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      149 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     2878 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6883 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      646 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2726 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)        5 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16519 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/xata_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      954 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       48 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     5294 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16797 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      350 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      490 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3292 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1000) runner    (1000)       67 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.309936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1612 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1969 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      349 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/__about__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      656 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1113 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/tests/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2043 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3953 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15080 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1375 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5252 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_client/db_grpc_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7869 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      565 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5549 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1098 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1000) runner    (1000)       99 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10701 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      236 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/api_handler_exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12851 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      407 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1931 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/handler_helpers.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/libs/llm/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/llm/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2869 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/llm/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22181 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/llm/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16707 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_exec_base.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/
+-rw-r--r--   0 runner    (1000) runner    (1000)      663 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      444 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/create_validation_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4225 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/describe_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      771 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6671 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/learn_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1346 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/predict_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      784 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/update_process.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      966 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14566 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/process_cache.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1171 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/realtime_chat_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3119 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/storage_handler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15599 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/libs/vectordatabase_handler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1665 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/dataset.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/question_answering/
+-rw-r--r--   0 runner    (1000) runner    (1000)     6906 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv
+-rw-r--r--   0 runner    (1000) runner    (1000)   104035 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv
+-rw-r--r--   0 runner    (1000) runner    (1000)     2769 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2113 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/handler_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2095 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      384 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5928 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      684 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8312 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      972 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/interfaces/agents/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/agents/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11433 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/agents/agents_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11171 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/chatbot_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6514 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/chatbot_executor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3790 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/chatbot_task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5550 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/memory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3473 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/model_executor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4292 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/polling.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      929 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/types.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4063 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28097 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11064 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/database/log.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11134 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3737 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4629 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.313936 MindsDB-24.4.2.0/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14357 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3602 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/knowledge_base/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/knowledge_base/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13849 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/knowledge_base/controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4590 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20365 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/query_context/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/query_context/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9331 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/query_context/context_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7156 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/query_context/last_query.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/skills/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/skills/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4240 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/skills/skill_tool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5414 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/skills/skills_controller.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7268 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/skills/sql_agent.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17504 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20045 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2925 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8267 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/tabs/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/tabs/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8761 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/tabs/tabs_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/tasks/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/tasks/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      401 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/tasks/task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3863 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/tasks/task_monitor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1666 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/tasks/task_thread.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/interfaces/triggers/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/triggers/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2911 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/triggers/trigger_task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5376 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/interfaces/triggers/triggers_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/metrics/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/metrics/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1819 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/metrics/metrics.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      985 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/metrics/server.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2327 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12845 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3565 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14810 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1263 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      159 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2170 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5430 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.317936 MindsDB-24.4.2.0/mindsdb/migrations/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2193 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1000) runner    (1000)     2218 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1769 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5871 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1050 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10817 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6163 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2788 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      849 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      998 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1000 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1045 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2330 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2146 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1957 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1789 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2384 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3486 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1802 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3487 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      799 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2035 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1115 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      836 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      930 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1567 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1180 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      730 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      856 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1138 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1940 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1222 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      596 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      983 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      605 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2519 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      701 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1023 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      824 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1323 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      837 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1419 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/mindsdb/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7245 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6450 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1450 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      610 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/context_executor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1034 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/exception.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5458 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7184 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1000) runner    (1000)      796 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2262 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2336 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1039 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2810 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      453 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/base.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      578 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/const.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9413 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/consumer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2702 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/producer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3166 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3177 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      251 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3936 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2339 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      751 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/security.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1377 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1708 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      122 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/requirements/
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/requirements/requirements-grpc.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      799 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-10 21:13:20.321936 MindsDB-24.4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     5998 2024-04-10 21:13:02.000000 MindsDB-24.4.2.0/setup.py
```

### Comparing `MindsDB-24.3.5.0/LICENSE` & `MindsDB-24.4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/MindsDB.egg-info/PKG-INFO` & `MindsDB-24.4.2.0/MindsDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 24.3.5.0
+Version: 24.4.2.0
 Summary: MindsDB's AI SQL Server enables developers to build AI tools that need access to real-time data to perform their tasks
 Home-page: https://github.com/mindsdb/mindsdb
 Download-URL: https://pypi.org/project/mindsdb/
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: ELv2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MindsDB-24.3.5.0/MindsDB.egg-info/SOURCES.txt` & `MindsDB-24.4.2.0/MindsDB.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -736,14 +736,15 @@
 mindsdb/integrations/handlers/langchain_embedding_handler/__about__.py
 mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py
 mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg
 mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py
 mindsdb/integrations/handlers/langchain_embedding_handler/requirements.txt
 mindsdb/integrations/handlers/langchain_handler/__about__.py
 mindsdb/integrations/handlers/langchain_handler/__init__.py
+mindsdb/integrations/handlers/langchain_handler/constants.py
 mindsdb/integrations/handlers/langchain_handler/icon.svg
 mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
 mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py
 mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
 mindsdb/integrations/handlers/langchain_handler/requirements.txt
 mindsdb/integrations/handlers/langchain_handler/tools.py
 mindsdb/integrations/handlers/leonardoai_handler/__about__.py
@@ -1391,15 +1392,16 @@
 mindsdb/integrations/handlers/utilities/__init__.py
 mindsdb/integrations/handlers/utilities/api_utilities/__init__.py
 mindsdb/integrations/handlers/utilities/api_utilities/microsoft/__init__.py
 mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py
 mindsdb/integrations/handlers/utilities/auth_utilities/__init__.py
 mindsdb/integrations/handlers/utilities/auth_utilities/exceptions.py
 mindsdb/integrations/handlers/utilities/auth_utilities/google/__init__.py
-mindsdb/integrations/handlers/utilities/auth_utilities/google/google_oauth_utilities.py
+mindsdb/integrations/handlers/utilities/auth_utilities/google/google_service_account_oauth_utilities.py
+mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py
 mindsdb/integrations/handlers/utilities/auth_utilities/google/requirements.txt
 mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/__init__.py
 mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py
 mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/requirements.txt
 mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
 mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py
 mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py
@@ -1499,22 +1501,24 @@
 mindsdb/integrations/handlers_wrapper/ml_handler_service.py
 mindsdb/integrations/libs/__init__.py
 mindsdb/integrations/libs/api_handler.py
 mindsdb/integrations/libs/api_handler_exceptions.py
 mindsdb/integrations/libs/base.py
 mindsdb/integrations/libs/const.py
 mindsdb/integrations/libs/handler_helpers.py
-mindsdb/integrations/libs/llm_utils.py
 mindsdb/integrations/libs/ml_exec_base.py
 mindsdb/integrations/libs/net_helpers.py
 mindsdb/integrations/libs/process_cache.py
 mindsdb/integrations/libs/realtime_chat_handler.py
 mindsdb/integrations/libs/response.py
 mindsdb/integrations/libs/storage_handler.py
 mindsdb/integrations/libs/vectordatabase_handler.py
+mindsdb/integrations/libs/llm/__init__.py
+mindsdb/integrations/libs/llm/config.py
+mindsdb/integrations/libs/llm/utils.py
 mindsdb/integrations/libs/ml_handler_process/__init__.py
 mindsdb/integrations/libs/ml_handler_process/create_engine_process.py
 mindsdb/integrations/libs/ml_handler_process/create_validation_process.py
 mindsdb/integrations/libs/ml_handler_process/describe_process.py
 mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py
 mindsdb/integrations/libs/ml_handler_process/learn_process.py
 mindsdb/integrations/libs/ml_handler_process/predict_process.py
```

### Comparing `MindsDB-24.3.5.0/MindsDB.egg-info/requires.txt` & `MindsDB-24.4.2.0/MindsDB.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 sqlalchemy<3.0.0,>=2.0.0
 psycopg2-binary
 alembic>=1.3.3
 redis<6.0.0,>=5.0.0
 walrus==0.9.3
 flask-compress>=1.0.0
 appdirs>=1.0.0
-mindsdb-sql~=0.11.0
+mindsdb-sql~=0.12.0
 mindsdb-evaluator<0.1.0,>=0.0.7
 checksumdir>=1.2.0
 duckdb==0.9.1
 requests>=2.30.0
 pydateinfer==0.3.0
 dataprep_ml==0.0.22
 dill==0.3.6
@@ -35,21 +35,22 @@
 protobuf==3.20.3
 hierarchicalforecast~=0.4.0
 google-auth-oauthlib
 msal
 langchain>=0.1.9
 langchain-core>=0.1.28
 prometheus-client==0.20.0
+pydantic
 binance-connector
 virtualenv
 pyarrow==11.0.0
 scylla-driver
 langchain-community
-pymupdf
 openpyxl
+pymupdf
 charset-normalizer
 python-magic>=0.4.27
 mysql-connector-python
 certifi
 mysql-connector-python
 tiktoken>=0.3.0
 openai==1.6.1
@@ -63,234 +64,230 @@
 sqlalchemy-access
 pyodbc
 
 [aerospike]
 aerospike~=13.0.0
 
 [all_extras]
+docker>=5.0.3
+pytest<8.0.0,>=7.3.0
 black==24.3.0
+pytest-lazy-fixture~=0.6.3
+netifaces>=0.11.0
 flake8==5.0.4
-hierarchicalforecast
-wheel
+twine
 locust
-pytest-subtests
-responses
-openai==1.6.1
-docker>=5.0.3
-isort==5.10.1
-coveralls
-watchfiles==0.19.0
-grpcio-tools
-ollama>=0.1.7
-netifaces>=0.11.0
+pytest-cov
 lightwood==23.12.4.0
-pytest<8.0.0,>=7.3.0
-twine
-pytest-lazy-fixture~=0.6.3
+wheel
+hierarchicalforecast
+ollama>=0.1.7
 deptry==0.12.0
+anthropic>=0.21.3
 setuptools
-pytest-cov
+responses
+coveralls
+grpcio-tools
+openai==1.6.1
+watchfiles==0.19.0
+pytest-subtests
 pre-commit>=2.16.0
+isort==5.10.1
 
 [all_handlers_extras]
-langfuse
-type_infer==0.0.18
+tiktoken~=0.4.0
+langchain-community
+pillow
+couchbase==4.0.2
+tzlocal
+sqlalchemy-vertica-python
+sqlalchemy-access
+sqlalchemy-hana
 redshift_connector
-hubspot-api-client
-vertica-python
+pyodbc
 sqlalchemy-spanner
-mlflow
-notion-client
-stravalib
 autokeras
-paypalrestsdk
-nltk>=3.8.1
-weaviate-client~=3.24.2
-ibm-db-sa
-tiktoken>=0.3.0
-openai==1.6.1
-writerai~=1.1.0
-auto-sklearn
-python-gitlab
-pyarrow~=10.0.1
+ray==2.0.1
 ShopifyAPI
-pgvector
-snowflake-sqlalchemy@ git+https://github.com/ea-rus/snowflake-sqlalchemy
-stripe
-langchain-community
-pysurrealdb
-charset-normalizer
-scipy
-google-cloud-spanner
-impyla
-openbb-core==1.0.1
-crate[sqlalchemy]
-google-api-python-client
-pycaret
-atlassian-python-api
-anthropic==0.3.5
-databend-sqlalchemy
-sqlalchemy_dremio
-pydantic>=1.10.8
-html2text
-chromadb~=0.4.8
-databricks-sql-connector
-rockset
-virtualenv
-taospy
-pyodbc
-anthropic==0.18.1
+pymysql
+vertica-python
 stability-sdk
-oracledb==1.0.2
-autogluon
-ibm-db
+pymssql>=2.1.4
+sqlalchemy-databricks
+sqlalchemy_dremio
 ludwig[distributed]>=0.5.2
-ray==2.0.1
-llama-hub==0.0.62
-pymonetdb
-polars
-sib_api_v3_sdk
-snowflake-connector-python>=2.7.12
-lightwood[xai]==24.3.3.1
-bs4
-pyignite
-nltk
-bs4==0.0.2
-couchbase==4.0.2
-sqlalchemy-bigquery
-monkeylearn==3.6.0
-sentence-transformers
-overpy
-elasticsearch-dbapi
-tweepy
-qdrant-client
-langchain-experimental
-chardet
-slack_sdk==3.21.3
-nixtlats>=0.1.10
-openbb==4.0.1
+plaid-python
+faiss-cpu
+flaml<=1.2.3
+google-auth-httplib2
+praw
+python-magic>=0.4.27
 webzio==1.0.2
-pillow
-statsforecast==1.6.0
-trino~=0.313.0
-qbosdk
-lancedb~=0.3.1
-libsql-experimental
-huggingface-hub
-lance
-sqlalchemy-firebird<3.0.0,>=2.0.0
+sqlalchemy-solr
+evaluate
 requests_toolbelt
-twilio
-sqlalchemy-vertica-python
 hdbcli
-lightwood==24.3.3.1
-salesforce-merlion<=1.3.1,>=1.2.0
-pyod>=1.1
-xata
-sqlalchemy-redshift
-binance-connector
-sqlalchemy-informix
-spacy
-pyphoenix
-pyodbc==4.0.34
-sqlalchemy-access
-lightfm==1.17
-pysqream_sqlalchemy>=0.8
-torch==2.0.1+cpu
+langfuse
+ibm-db-sa
+pygithub
+google-generativeai==0.3.1
+nltk
+openai==1.6.1
 llama-index==0.9.23
-pymupdf
-newsapi-python
-pydruid
-praw
-pycaret[models]
-pydantic==2.5.1
-teradatasqlalchemy
+pymonetdb
+oracledb==1.0.2
+sqlanydb
+neuralforecast<1.7.0,>=1.6.0
+pyarrow==11.0.0
+hubspot-api-client
+influxdb3-python
+slack_sdk==3.21.3
 rocketchat_API
-scylla-driver
-google
+transformers<5.0.0,>=4.34.0
+litellm==1.23.2
+dask
+crate[sqlalchemy]
+elasticsearch
+pyphoenix
+faunadb
+taospy
+sentence-transformers
+IfxPy@ git+https://github.com/OpenInformix/IfxPy#subdirectory=IfxPy
+openbb-core==1.0.1
+lightwood[xai]==24.3.3.1
 lightwood[extra]==24.3.3.1
-google-cloud-aiplatform>=1.35.0
-mendeley
-pymilvus==2.3
-catboost>=1.2
-flaml<=1.2.3
-replicate
-ingres_sa_dialect@ git+https://github.com/ActianCorp/ingres_sa_dialect
-pygithub
-ray[tune]>=2.2.0
-pinotdb
-cohere==4.5.1
-phoenixdb
-xgboost
-torch
-pydantic>=1.10.7
-hugging_py_face
+pyarrow~=10.0.1
+pyignite
+torch==2.0.1+cpu
+paypalrestsdk
+sqlalchemy-sqlany
+tiktoken>=0.3.0
+databricks-sql-connector
+scipy
 mysql-connector-python
+salesforce-merlion<=1.3.1,>=1.2.0
+dotty-dict==1.3.1
+monkeylearn==3.6.0
+lancedb~=0.3.1
+autogluon
 tensorflow
-pymysql
-sqlalchemy-hana
-solace-pubsubplus
-teradatasql
-sqlalchemy-databricks
-pyarrow==11.0.0
-google-generativeai>=0.1.0
-evaluate
-google-generativeai==0.3.1
-IfxPy@ git+https://github.com/OpenInformix/IfxPy#subdirectory=IfxPy
+ray[tune]>=2.2.0
+sqlalchemy-redshift
+youtube-transcript-api
+impyla
+lance
+pgvector
 aerospike~=13.0.0
-tiktoken~=0.4.0
-mediawikiapi
-faunadb
-google-analytics-admin
+replicate
+anthropic==0.3.5
+huggingface-hub
+pydruid
+charset-normalizer
+ingres_sa_dialect@ git+https://github.com/ActianCorp/ingres_sa_dialect
+google-cloud-aiplatform>=1.35.0
 fdb
-pyhive
+google-generativeai>=0.1.0
+databend-sqlalchemy
+catboost>=1.2
+solace-pubsubplus
+scylla-driver
+tweepy
 eventbrite-python
-tzlocal
+pinecone-client
+hugging_py_face
+google-cloud-bigquery[pandas]
+openpyxl
+sqlalchemy-monetdb
+sqlalchemy-firebird<3.0.0,>=2.0.0
+qbosdk
 joblib
-neuralforecast<1.7.0,>=1.6.0
-python-magic>=0.4.27
+pyhive
+openbb==4.0.1
+writerai~=1.1.0
+qdrant-client
+overpy
+anthropic==0.18.1
 symbl
-google-auth-httplib2
-wikipedia==1.4.0
-sqlalchemy-monetdb
-pydantic
-ckanapi
-sqlalchemy-solr
-litellm==1.23.2
-tpot<=0.11.7
-certifi
-rouge-score>=0.1.2
-openpyxl
-influxdb3-python
-dotty-dict==1.3.1
 litellm
-elasticsearch
+cohere==4.5.1
+bs4==0.0.2
+mendeley
+torch
+notion-client
+ckanapi
 clickhouse-sqlalchemy>=0.3.1
-google-cloud-bigquery[pandas]
-dask
-sqlalchemy-sqlany
+google-analytics-admin
+snowflake-connector-python>=2.7.12
+atlassian-python-api
+pinotdb
+sib_api_v3_sdk
+snowflake-sqlalchemy@ git+https://github.com/ea-rus/snowflake-sqlalchemy
+chardet
+lightfm==1.17
+certifi
+google-cloud-spanner
 datasets
+ibm-db
+chromadb~=0.4.8
+xata
+rouge-score>=0.1.2
+binance-connector
+sqlalchemy-informix
+bs4
+pymupdf
+auto-sklearn
+wikipedia==1.4.0
+libsql-experimental
+polars
+pycaret
+pysurrealdb
+type_infer==0.0.18
+teradatasql
 jaydebeapi
-plaid-python
-pymssql>=2.1.4
-pinecone-client
-sqlanydb
-youtube-transcript-api
-faiss-cpu
+langchain-experimental
+lightwood==24.3.3.1
+python-gitlab
 pysqream>=3.2.5
-transformers<5.0.0,>=4.34.0
+spacy
+pyod>=1.1
+mediawikiapi
+virtualenv
+teradatasqlalchemy
+stripe
+newsapi-python
+xgboost
+google
+tpot<=0.11.7
+elasticsearch-dbapi
+pyodbc==4.0.34
+statsforecast==1.6.0
+pymilvus==2.3
+weaviate-client~=3.24.2
+sqlalchemy-bigquery
+mlflow
+trino~=0.313.0
+phoenixdb
+nltk>=3.8.1
+html2text
+pysqream_sqlalchemy>=0.8
+pycaret[models]
+twilio
+nixtlats>=0.1.10
+google-api-python-client
+llama-hub==0.0.62
+stravalib
 
 [altibase]
 jaydebeapi
 
 [anomaly_detection]
-pyod>=1.1
 catboost>=1.2
-joblib
 xgboost
+pyod>=1.1
+joblib
 
 [anthropic]
 anthropic==0.18.1
 
 [anyscale_endpoints]
 tiktoken>=0.3.0
 openai==1.6.1
@@ -310,30 +307,29 @@
 autokeras
 
 [autosklearn]
 auto-sklearn
 type_infer==0.0.18
 
 [bigquery]
-sqlalchemy-bigquery
 google-cloud-bigquery[pandas]
+sqlalchemy-bigquery
 
 [binance]
 binance-connector
 
 [byom]
 virtualenv
 pyarrow==11.0.0
 
 [cassandra]
 scylla-driver
 
 [chromadb]
 chromadb~=0.4.8
-pydantic
 
 [ckan]
 ckanapi
 
 [clickhouse]
 clickhouse-sqlalchemy>=0.3.1
 
@@ -364,16 +360,16 @@
 [d0lt]
 pymysql
 
 [databend]
 databend-sqlalchemy
 
 [databricks]
-sqlalchemy-databricks
 databricks-sql-connector
+sqlalchemy-databricks
 
 [datastax]
 scylla-driver
 
 [db2]
 ibm-db-sa
 ibm-db
@@ -409,35 +405,34 @@
 [elasticsearch]
 elasticsearch-dbapi
 elasticsearch
 
 [email]
 bs4==0.0.2
 chardet
-pydantic
 
 [empress]
 pyodbc
 
 [eventbrite]
 eventbrite-python
 
 [faunadb]
 faunadb
 
 [file]
 langchain-community
-pymupdf
 openpyxl
+pymupdf
 charset-normalizer
 python-magic>=0.4.27
 
 [firebird]
-sqlalchemy-firebird<3.0.0,>=2.0.0
 fdb
+sqlalchemy-firebird<3.0.0,>=2.0.0
 
 [flaml]
 flaml<=1.2.3
 type_infer==0.0.18
 
 [frappe]
 
@@ -448,33 +443,33 @@
 python-gitlab
 
 [gmail]
 google-auth-httplib2
 google-api-python-client
 
 [google_analytics]
-google-api-python-client
 google-analytics-admin
+google-api-python-client
 
 [google_books]
 google-auth-httplib2
 google-api-python-client
 
 [google_calendar]
 google-auth-httplib2
 google-api-python-client
 
 [google_content_shopping]
 google-auth-httplib2
 google-api-python-client
 
 [google_fit]
-tzlocal
-google-api-python-client
 google
+google-api-python-client
+tzlocal
 
 [google_gemini]
 google-generativeai==0.3.1
 
 [google_search]
 google-auth-httplib2
 google-api-python-client
@@ -492,105 +487,103 @@
 [hsqldb]
 pyodbc==4.0.34
 
 [hubspot]
 hubspot-api-client
 
 [huggingface]
-datasets
 evaluate
-torch
-huggingface-hub
 nltk
 transformers<5.0.0,>=4.34.0
+torch
+huggingface-hub
+datasets
 
 [huggingface-cpu]
-datasets
 evaluate
-huggingface-hub
 nltk
 transformers<5.0.0,>=4.34.0
+huggingface-hub
 torch==2.0.1+cpu
+datasets
 
 [huggingface_api]
-hugging_py_face
 huggingface-hub
+hugging_py_face
 
 [ignite]
 pyignite
 
 [impala]
 impyla
 
 [influxdb]
 influxdb3-python
 
 [informix]
-sqlalchemy-informix
 IfxPy@ git+https://github.com/OpenInformix/IfxPy#subdirectory=IfxPy
+sqlalchemy-informix
 
 [ingres]
-pyodbc
 ingres_sa_dialect@ git+https://github.com/ActianCorp/ingres_sa_dialect
+pyodbc
 
 [jira]
 atlassian-python-api
 
 [kinetica]
 
 [lancedb]
 lancedb~=0.3.1
-pyarrow~=10.0.1
 lance
+pyarrow~=10.0.1
 
 [langchain]
-wikipedia==1.4.0
-langfuse
-litellm==1.23.2
-langchain-community
 tiktoken>=0.3.0
+langchain-community
 langchain-experimental
+langfuse
+litellm==1.23.2
 openai==1.6.1
 anthropic==0.3.5
+wikipedia==1.4.0
 
 [langchain_embedding]
 tiktoken~=0.4.0
 openai==1.6.1
 
 [leonardoai]
 
 [libsql]
 libsql-experimental
 
 [lightfm]
-pydantic>=1.10.7
 lightfm==1.17
 
 [lightwood]
-lightwood[extra]==24.3.3.1
-type_infer==0.0.18
-lightwood==24.3.3.1
 lightwood[xai]==24.3.3.1
+lightwood==24.3.3.1
+type_infer==0.0.18
+lightwood[extra]==24.3.3.1
 
 [lindorm]
-phoenixdb
 pyphoenix
+phoenixdb
 
 [litellm]
 litellm
-pydantic
 
 [llama_index]
 llama-hub==0.0.62
-llama-index==0.9.23
 openai==1.6.1
+llama-index==0.9.23
 
 [ludwig]
-ray==2.0.1
 dask
+ray==2.0.1
 ludwig[distributed]>=0.5.2
 
 [luma]
 
 [mariadb]
 mysql-connector-python
 
@@ -615,25 +608,24 @@
 [milvus]
 pymilvus==2.3
 
 [mlflow]
 mlflow
 
 [monetdb]
-sqlalchemy-monetdb
 pymonetdb
+sqlalchemy-monetdb
 
 [mongodb]
 certifi
 
 [monkeylearn]
 monkeylearn==3.6.0
 
 [ms_teams]
-pydantic
 
 [mssql]
 pymssql>=2.1.4
 
 [mysql]
 mysql-connector-python
 
@@ -659,40 +651,38 @@
 
 [openai]
 tiktoken>=0.3.0
 openai==1.6.1
 
 [openbb]
 openbb==4.0.1
-pydantic==2.5.1
 openbb-core==1.0.1
 
 [opengauss]
 
 [openstreetmap]
 overpy
 
 [oracle]
 oracledb==1.0.2
 
 [orioledb]
 
 [palm]
 google-generativeai>=0.1.0
-pydantic
 
 [paypal]
 paypalrestsdk
 
 [pgvector]
 pgvector
 
 [phoenix]
-phoenixdb
 pyphoenix
+phoenixdb
 
 [pinecone]
 pinecone-client
 
 [pinot]
 pinotdb
 
@@ -714,22 +704,21 @@
 
 [questdb]
 
 [quickbooks]
 qbosdk
 
 [rag]
-html2text
 sentence-transformers
-chromadb~=0.4.8
-pydantic
 langchain-community
-faiss-cpu
 openai==1.6.1
+faiss-cpu
+html2text
 writerai~=1.1.0
+chromadb~=0.4.8
 
 [reddit]
 praw
 
 [redshift]
 sqlalchemy-redshift
 redshift_connector
@@ -738,31 +727,29 @@
 replicate
 
 [rocket_chat]
 rocketchat_API
 
 [rockset]
 mysql-connector-python
-rockset
 
 [scylla]
 scylla-driver
 
 [sendinblue]
 sib_api_v3_sdk
 
 [sentence_transformers]
-html2text
 sentence-transformers
-chromadb~=0.4.8
-pydantic
 langchain-community
+openai==1.6.1
 faiss-cpu
+html2text
 writerai~=1.1.0
-openai==1.6.1
+chromadb~=0.4.8
 
 [shopify]
 ShopifyAPI
 
 [singlestore]
 mysql-connector-python
 
@@ -834,80 +821,78 @@
 pytest-subtests
 lightwood==23.12.4.0
 responses
 pytest-cov
 coveralls
 locust
 ollama>=0.1.7
+anthropic>=0.21.3
 
 [tidb]
 mysql-connector-python
 
 [timegpt]
 nixtlats>=0.1.10
 
 [timescaledb]
 
 [tpot]
 tpot<=0.11.7
 type_infer==0.0.18
 
 [trino]
-pyhive
 trino~=0.313.0
+pyhive
 
 [twelve_labs]
 requests_toolbelt
-pydantic
 
 [twilio]
 twilio
 
 [twitter]
 tweepy
 
 [vertex]
 google-cloud-aiplatform>=1.35.0
 
 [vertica]
-sqlalchemy-vertica-python
 vertica-python
+sqlalchemy-vertica-python
 
 [vitess]
 mysql-connector-python
 
 [weaviate]
 weaviate-client~=3.24.2
 
 [web]
 pymupdf
 bs4
 
 [webz]
-dotty-dict==1.3.1
 webzio==1.0.2
+dotty-dict==1.3.1
 
 [whatsapp]
 twilio
 
 [writer]
-pydantic>=1.10.8
-html2text
 sentence-transformers
-chromadb~=0.4.8
-pydantic
+rouge-score>=0.1.2
 langchain-community
-nltk>=3.8.1
-faiss-cpu
 openai==1.6.1
-rouge-score>=0.1.2
-writerai~=1.1.0
 scipy
+faiss-cpu
+nltk>=3.8.1
+html2text
+writerai~=1.1.0
+chromadb~=0.4.8
 
 [xata]
 xata
 
 [youtube]
-youtube-transcript-api
 google-api-python-client
+youtube-transcript-api
 
 [yugabyte]
```

### Comparing `MindsDB-24.3.5.0/PKG-INFO` & `MindsDB-24.4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 24.3.5.0
+Version: 24.4.2.0
 Summary: MindsDB's AI SQL Server enables developers to build AI tools that need access to real-time data to perform their tasks
 Home-page: https://github.com/mindsdb/mindsdb
 Download-URL: https://pypi.org/project/mindsdb/
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: ELv2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MindsDB-24.3.5.0/README.md` & `MindsDB-24.4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/__main__.py` & `MindsDB-24.4.2.0/mindsdb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from mindsdb.api.mongo.start import start as start_mongo
 from mindsdb.api.postgres.start import start as start_postgres
 from mindsdb.interfaces.tasks.task_monitor import start as start_tasks
 from mindsdb.utilities.ml_task_queue.consumer import start as start_ml_task_queue
 from mindsdb.interfaces.jobs.scheduler import start as start_scheduler
 from mindsdb.utilities.config import Config
 from mindsdb.utilities.ps import is_pid_listen_port, get_child_pids
-from mindsdb.utilities.functions import args_parse, get_versions_where_predictors_become_obsolete
+from mindsdb.utilities.functions import args_parse, get_handler_install_message, get_versions_where_predictors_become_obsolete
 from mindsdb.interfaces.database.integrations import integration_controller
 import mindsdb.interfaces.storage.db as db
 from mindsdb.integrations.utilities.install import install_dependencies
 from mindsdb.utilities.fs import create_dirs_recursive, clean_process_marks, clean_unlinked_process_marks
 from mindsdb.utilities.telemetry import telemetry_file_exists, disable_telemetry
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities.auth import register_oauth_client, get_aws_meta_data
@@ -217,19 +217,17 @@
         handler_name,
         handler_meta,
     ) in integration_controller.get_handlers_import_status().items():
         import_meta = handler_meta.get("import", {})
         dependencies = import_meta.get("dependencies")
         if import_meta.get("success", False) is not True:
             logger.debug(
-                f"Dependencies for the handler '{handler_name}' are not installed by default."
-            )
-            logger.debug(
-                f'If you want to use "{handler_name}" please "pip install mindsdb[{handler_name}]"'
+                f"Dependencies for the handler '{handler_name}' are not installed."
             )
+            logger.debug(get_handler_install_message(handler_name))
 
     # from mindsdb.utilities.fs import get_marked_processes_and_threads
     # marks = get_marked_processes_and_threads()
 
     if not is_cloud:
         # region creating permanent integrations
         for (
```

### Comparing `MindsDB-24.3.5.0/mindsdb/api/common/check_auth.py` & `MindsDB-24.4.2.0/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/command_executor.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/command_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     SERVER_VARIABLES,
     TYPES,
 )
 
 from .exceptions import (
     ExecutorException,
     BadDbError,
-    BadTableError,
     NotSupportedYet,
     WrongArgumentError,
     TableNotExistError,
 )
 from mindsdb.api.executor.utilities.functions import download_file
 from mindsdb.api.executor.utilities.sql import query_df
 from mindsdb.integrations.libs.const import (
@@ -99,15 +98,15 @@
     get_model_record,
     get_model_records,
     get_predictor_integration,
 )
 from mindsdb.interfaces.query_context.context_controller import query_context_controller
 from mindsdb.interfaces.triggers.triggers_controller import TriggersController
 from mindsdb.utilities.context import context as ctx
-from mindsdb.utilities.functions import mark_process, resolve_model_identifier
+from mindsdb.utilities.functions import mark_process, resolve_model_identifier, get_handler_install_message
 from mindsdb.utilities.exception import EntityExistsError, EntityNotExistsError
 from mindsdb.utilities import log
 
 logger = log.getLogger(__name__)
 
 
 def _get_show_where(
@@ -607,21 +606,14 @@
         elif type(statement) is CreateView:
             return self.answer_create_view(statement, database_name)
         elif type(statement) is DropView:
             return self.answer_drop_view(statement, database_name)
         elif type(statement) is Delete:
             if statement.table.parts[-1].lower() == "models_versions":
                 return self.answer_delete_model_version(statement, database_name)
-            if (
-                database_name != "mindsdb"
-                and statement.table.parts[0] != "mindsdb"
-            ):
-                raise BadTableError(
-                    "Only 'DELETE' from database 'mindsdb' is possible at this moment"
-                )
 
             SQLQuery(statement, session=self.session, execute=True, database=database_name)
             return ExecuteAnswer(ANSWER_TYPE.OK)
 
         elif type(statement) is Insert:
             SQLQuery(statement, session=self.session, execute=True, database=database_name)
             return ExecuteAnswer(ANSWER_TYPE.OK)
@@ -1043,15 +1035,15 @@
         storage = None
         try:
             handlers_meta = (
                 self.session.integration_controller.get_handlers_import_status()
             )
             handler_meta = handlers_meta[engine]
             if handler_meta.get("import", {}).get("success") is not True:
-                raise ExecutorException(f"Handler '{engine}' can not be used")
+                raise ExecutorException(f"The '{engine}' handler isn't installed.\n" + get_handler_install_message(engine))
 
             accept_connection_args = handler_meta.get("connection_args")
             if accept_connection_args is not None and connection_args is not None:
                 for arg_name, arg_value in connection_args.items():
                     if arg_name == "as_service":
                         continue
                     if arg_name not in accept_connection_args:
@@ -1135,30 +1127,21 @@
                 name=name, engine=statement.handler, connection_args=params
             )
         except Exception as e:
             msg = str(e)
             if type(e) in (ImportError, ModuleNotFoundError):
                 msg = dedent(
                     f"""\
-                    Handler '{handler_module_meta['name']}' cannot be used. Reason is:
+                    The '{handler_module_meta['name']}' handler cannot be used. Reason is:
                         {handler_module_meta['import']['error_message']}
                 """
                 )
                 is_cloud = self.session.config.get("cloud", False)
-                if is_cloud is False:
-                    msg += dedent(
-                        f"""
-
-                    If the error is related to missing dependencies, then try to run one of the following commands in a shell and restart mindsdb:
-                        If you have cloned the github repo, run "pip install '.[{handler_module_meta['name']}]'"
-                        If you have installed via pip, run "pip install 'mindsdb[{handler_module_meta['name']}]'"
-                        If you are using docker, run "docker exec <container_name> pip install 'mindsdb[{handler_module_meta['name']}]'"
-                    """
-                    )
-                logger.info(msg)
+                if is_cloud is False and "No module named" in handler_module_meta['import']['error_message']:
+                    logger.info(get_handler_install_message(handler_module_meta['name']))
             ast_drop = DropMLEngine(name=statement.name)
             self.answer_drop_ml_engine(ast_drop)
             logger.info(msg)
             raise ExecutorException(msg)
 
         return ExecuteAnswer(ANSWER_TYPE.OK)
```

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/controllers/session_controller.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/data_types/answer.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/data_types/answer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/datahub/classes/tables_row.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/integration_datanode.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/integration_datanode.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 raise Exception(result.error_message)
             is_create = True
 
         if is_create:
             create_table_ast = CreateTable(
                 name=table_name,
                 columns=columns,
-                is_replace=True
+                is_replace=is_replace
             )
             result = self._query(create_table_ast)
             if result.type == RESPONSE_TYPE.ERROR:
                 raise Exception(result.error_message)
 
         if result_set is None:
             # it is just a 'create table'
```

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/datahub/datanodes/project_datanode.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/exceptions.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/result_set.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/result_set.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/sql_query.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/__init__.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/apply_predictor_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/delete_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/delete_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/fetch_dataframe.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/insert_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/insert_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/join_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/join_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/map_reduce_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/map_reduce_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/multiple_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/multiple_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/prepare_steps.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/prepare_steps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/project_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/project_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/sql_steps.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/sql_steps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/subselect_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/subselect_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/union_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/union_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/sql_query/steps/update_step.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/sql_query/steps/update_step.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/utilities/functions.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/executor/utilities/sql.py` & `MindsDB-24.4.2.0/mindsdb/api/executor/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/gui.py` & `MindsDB-24.4.2.0/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-24.4.2.0/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/initialize.py` & `MindsDB-24.4.2.0/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/agents.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/agents.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/auth.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/chatbots.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/chatbots.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/config.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/databases.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/default.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/file.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 import multipart
 import requests
 from flask import current_app as ca
 from flask import request
 from flask_restx import Resource
 
 from mindsdb.api.http.namespaces.configs.files import ns_conf
-from mindsdb.api.http.utils import http_error, safe_extract
+from mindsdb.api.http.utils import http_error
 from mindsdb.metrics.metrics import api_endpoint_metrics
 from mindsdb.utilities.config import Config
 from mindsdb.utilities.context import context as ctx
 from mindsdb.utilities import log
 from mindsdb.utilities.security import is_private_url, clear_filename
+from mindsdb.utilities.fs import safe_extract
 
 logger = log.getLogger(__name__)
 
 
 @ns_conf.route("/")
 class FilesList(Resource):
     @ns_conf.doc("get_files_list")
```

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/models.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/models.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/projects.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/skills.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/skills.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/sql.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/tab.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/tree.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/util.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/namespaces/views.py` & `MindsDB-24.4.2.0/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/http/start.py` & `MindsDB-24.4.2.0/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/classes/responder.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/classes/scram.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/classes/session.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/delete.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/find.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/insert.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/server.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-24.4.2.0/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/executor/mysql_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-24.4.2.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-24.4.2.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/aerospike_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aerospike_handler/tests/test_aerospike_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/anomaly_detection_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anomaly_detection_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anthropic_handler/anthropic_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/anyscale_endpoints_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import contextlib
 from typing import Optional, Dict
 
 import pandas as pd
 
 from mindsdb.integrations.handlers.openai_handler.openai_handler import OpenAIHandler
 from mindsdb.integrations.handlers.openai_handler.constants import OPENAI_API_BASE
+from mindsdb.integrations.libs.llm.utils import ft_jsonl_validation, ft_formatter
 from mindsdb.integrations.utilities.handler_utils import get_api_key
-from mindsdb.integrations.libs.llm_utils import ft_jsonl_validation, ft_formatter
 from mindsdb.utilities import log
 
 logger = log.getLogger(__name__)
 
 
 ANYSCALE_API_BASE = 'https://api.endpoints.anyscale.com/v1'
 MIN_FT_VAL_LEN = 20  # anyscale checks for at least 20 validation chats
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/anyscale_endpoints_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/apache_doris_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/apache_doris_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/aqicn.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/aqicn.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/aqicn_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aqicn_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aqicn_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/autogluon_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autogluon_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autogluon_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autokeras_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autokeras_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/autosklearn_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/autosklearn_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from mindsdb.utilities.config import Config
 from mindsdb.interfaces.storage import db
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.libs.const import PREDICTOR_STATUS
 from mindsdb.integrations.utilities.utils import format_exception_error
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 import mindsdb.utilities.profiler as profiler
+from mindsdb.utilities.fs import safe_extract
+
 
 from .proc_wrapper import (
     pd_decode, pd_encode, encode, decode, BYOM_METHOD,
     import_string, find_model_class
 )
 from .__about__ import __version__
 
@@ -471,15 +473,15 @@
             if self.is_cloud:
                 bese_env_path = Path(tempfile.gettempdir()) / 'mindsdb' / 'venv'
                 bese_env_path.mkdir(parents=True, exist_ok=True)
                 self.env_path = bese_env_path / env_folder_name
                 tar_path = self.env_storage_path.with_suffix('.tar')
                 if self.env_path.exists() is False and tar_path.exists() is True:
                     with tarfile.open(tar_path) as tar:
-                        tar.extractall(path=bese_env_path)
+                        safe_extract(tar, path=bese_env_path)
             else:
                 self.env_path = self.env_storage_path
 
             if sys.platform in ('win32', 'cygwin'):
                 exectable_folder_name = 'Scripts'
             else:
                 exectable_folder_name = 'bin'
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/chromadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/chromadb_handler/tests/test_chromadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/clipdrop_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/clipdrop_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/clipdrop_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/cohere_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/cohere_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/coinbase_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/coinbase_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/coinbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/confluence_handler/tests/test_confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/discord_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/discord_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/discord_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/discord_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/discord_handler/tests/test_discord.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/dockerhub_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dockerhub_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dockerhub_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/documentdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/documentdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/documentdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dummy_data_handler/dummy_data_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_client.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_ingestor.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/email_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/email_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/email_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/email_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/eventbrite_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventbrite_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventbrite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/faunadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/faunadb_handler/tests/test_faunadb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/data/test.txt` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/data/test.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/file_handler/tests/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/flaml_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/flaml_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/gmail_handler/utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/gmail_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/google_analytics_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_analytics_handler/tests/test_google_analytics_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_fit_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_fit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_gemini_handler/google_gemini_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/hubspot_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/hubspot_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/hubspot_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_api_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/finetune.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/finetune.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/huggingface_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/huggingface_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/instatus_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/instatus_handler/instatus_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/intercom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/intercom_handler/intercom_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/kinetica_handler/kinetica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/lancedb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lancedb_handler/tests/test_lancedb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_embedding_handler/langchain_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/log_callback_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/langchain_handler/tools.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/langchain_handler/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,29 +98,28 @@
     return mdb_write_call
 
 def _setup_standard_tools(tools, llm, model_kwargs):
     executor = skill_tool.get_command_executor()
 
     all_standard_tools = []
     langchain_tools = []
-    for tool in tools:
-        if tool == 'mdb_read':
-            mdb_tool = Tool(
-                name="MindsDB",
-                func=get_exec_call_tool(llm, executor, model_kwargs),
-                description="useful to read from databases or tables connected to the mindsdb machine learning package. the action must be a valid simple SQL query, always ending with a semicolon. For example, you can do `show databases;` to list the available data sources, and `show tables;` to list the available tables within each data source."  # noqa
-            )
+    mdb_tool = Tool(
+        name="MindsDB",
+        func=get_exec_call_tool(llm, executor, model_kwargs),
+        description="useful to read from databases or tables connected to the mindsdb machine learning package. the action must be a valid simple SQL query, always ending with a semicolon. For example, you can do `show databases;` to list the available data sources, and `show tables;` to list the available tables within each data source."  # noqa
+    )
 
-            mdb_meta_tool = Tool(
-                name="MDB-Metadata",
-                func=get_exec_metadata_tool(llm, executor, model_kwargs),
-                description="useful to get column names from a mindsdb table or metadata from a mindsdb data source. the command should be either 1) a data source name, to list all available tables that it exposes, or 2) a string with the format `data_source_name.table_name` (for example, `files.my_table`), to get the table name, table type, column names, data types per column, and amount of rows of the specified table."  # noqa
-            )
-            all_standard_tools.append(mdb_tool)
-            all_standard_tools.append(mdb_meta_tool)
+    mdb_meta_tool = Tool(
+        name="MDB-Metadata",
+        func=get_exec_metadata_tool(llm, executor, model_kwargs),
+        description="useful to get column names from a mindsdb table or metadata from a mindsdb data source. the command should be either 1) a data source name, to list all available tables that it exposes, or 2) a string with the format `data_source_name.table_name` (for example, `files.my_table`), to get the table name, table type, column names, data types per column, and amount of rows of the specified table."  # noqa
+    )
+    all_standard_tools.append(mdb_tool)
+    all_standard_tools.append(mdb_meta_tool)
+    for tool in tools:
         if tool == 'mindsdb_write':
             mdb_write_tool = Tool(
                 name="MDB-Write",
                 func=get_mdb_write_tool(executor),
                 description="useful to write into data sources connected to mindsdb. command must be a valid SQL query with syntax: `INSERT INTO data_source_name.table_name (column_name_1, column_name_2, [...]) VALUES (column_1_value_row_1, column_2_value_row_1, [...]), (column_1_value_row_2, column_2_value_row_2, [...]), [...];`. note the command always ends with a semicolon. order of column names and values for each row must be a perfect match. If write fails, try casting value with a function, passing the value without quotes, or truncating string as needed.`."  # noqa
             )
             all_standard_tools.append(mdb_write_tool)
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/leonardoai_handler/leonardo_ai_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import requests
 import time
 from typing import Dict, Optional
-from mindsdb.integrations.libs.llm_utils import get_completed_prompts
 
 import pandas as pd
 
 from mindsdb.integrations.libs.base import BaseMLEngine
+from mindsdb.integrations.libs.llm.utils import get_completed_prompts
 from mindsdb.utilities import log
 from mindsdb.interfaces.storage.model_fs import HandlerStorage
 from mindsdb.utilities.config import Config
 
 logger = log.getLogger(__name__)
 
 LEONARDO_API_BASE = 'https://cloud.leonardo.ai/api/rest/v1'
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/libsql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/libsql_handler/tests/test_libsql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/api.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightdash_handler/lightdash_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/functions.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lightwood_handler/utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/lindorm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/lindorm_handler/tests/test_lindorm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/litellm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/litellm_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/litellm_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/config.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/github_loader_helper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/luma.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/luma.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/luma_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/luma_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/luma_handler/luma_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/luma_handler/luma_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/milvus_handler/milvus_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/tests/test_mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/ms_graph_api_teams_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/ms_teams_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ms_teams_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ms_teams_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,21 @@
         if self.is_connected is True:
             return self.connection
 
         self.connection = pymssql.connect(**self.connection_data)
         self.is_connected = True
 
         return self.connection
+    
+    def disconnect(self):
+        if self.is_connected is False:
+            return
+        self.connection.close()
+        self.is_connected = False
+        return
 
     def check_connection(self) -> StatusResponse:
         """
         Check the connection of the SQL Server database
         :return: success status and error message if error occurs
         """
         response = StatusResponse(False)
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 import pytest
+import pymssql
 import pandas as pd
 from unittest.mock import MagicMock
 from mindsdb.integrations.handlers.mssql_handler.mssql_handler import SqlServerHandler
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb.api.executor.data_types.response_type import RESPONSE_TYPE
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE,
 )
 
-
-@pytest.fixture(scope="class")
-def sql_server_handler():
-    HANDLER_KWARGS = {
-        "connection_data": {
-            "host": "localhost",
-            "port": "1433",
-            "user": "sa",
-            "password": "admin5678@",
-            "database": "master",
-        }
+HANDLER_KWARGS = {
+    "connection_data": {
+        "host": "localhost",
+        "port": "1433",
+        "user": "sa",
+        "password": "admin5678@",
+        "database": "mdb_db_handler_test",
     }
-    handler = SqlServerHandler("test_sqlserver_handler", **HANDLER_KWARGS)
-    yield handler
-    handler.disconnect()
-
-
-@pytest.fixture(scope="class")
-def database_connection_and_cursor():
-    connection = MagicMock()
-    cursor = MagicMock()
-    connection.cursor.return_value = cursor
-    return connection, cursor
-
+}
 
 expected_columns = {
     "Field": ["col_one", "col_two", "col_three", "col_four"],
-    "Type": ["int", "int", "float", "text"],
+    "Type": ["int", "int", "float", "varchar"],
 }
 
 expected_data = {
     "col_one": [1, 2, 3],
     "col_two": [-1, -2, -3],
     "col_three": [0.1, 0.2, 0.3],
     "col_four": ["A", "B", "C"],
 }
 
+def seed_db():
+    """Seed the test DB with some data"""
+    
+    # Connect to 'master' while we create our test DB
+    conn_info = HANDLER_KWARGS["connection_data"].copy()
+    conn_info["database"] = "master"
+    db = pymssql.connect(**conn_info, autocommit=True)
+    cursor = db.cursor()
+
+    with open("mindsdb/integrations/handlers/mssql_handler/tests/seed.sql", "r") as f:
+        for line in f.readlines():
+            cursor.execute(line)
+    cursor.close()
+    db.close()
+
+@pytest.fixture(scope="class")
+def sql_server_handler():
+    seed_db()
+    handler = SqlServerHandler("test_sqlserver_handler", **HANDLER_KWARGS)
+    yield handler
+    handler.disconnect()
+
+@pytest.fixture(scope="class")
+def database_connection_and_cursor():
+    connection = MagicMock()
+    cursor = MagicMock()
+    connection.cursor.return_value = cursor
+    return connection, cursor
 
 def check_valid_response(res):
     if res.resp_type == RESPONSE_TYPE.TABLE:
         assert res.data_frame is not None, "expected to have some data, but got None"
     assert (
         res.error_code == 0
     ), f"expected to have zero error_code, but got {res.error_code}"
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/notion_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/notion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/notion_table.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/notion_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/notion_handler/tests/test_notion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/api.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/npm_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/npm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/npm_handler/npm_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/npm_handler/npm_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oilpriceapi_handler/oilpriceapi_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ollama_handler/ollama_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 from typing import Dict, Optional
 
 import pandas as pd
 
 from mindsdb.integrations.libs.base import BaseMLEngine
-from mindsdb.integrations.libs.llm_utils import get_completed_prompts
+from mindsdb.integrations.libs.llm.utils import get_completed_prompts
 
 
 class OllamaHandler(BaseMLEngine):
     name = "ollama"
     DEFAULT_SERVE_URL = "http://localhost:11434"
 
     @staticmethod
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/constants.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/constants.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -137,16 +137,21 @@
         return num_tokens
     else:
         raise NotImplementedError(
             f"""_count_tokens() is not presently implemented for model {model_name}."""
         )
 
 
-def get_available_models(api_key: str) -> List[str]:
-    """
-    Returns a list of available openai models for the given API key.
+def get_available_models(api_key: str, base_url: str) -> List[str]:
     """
+    Returns a list of all available OpenAI models for the given API key.
+
+    Args:
+        api_key (str): The API key used for authenticating with the OpenAI API. 
+        base_url (str): The base URL of the OpenAI API.
 
-    api_base = os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
-    res = OpenAI(api_key=api_key, base_url=api_base).models.list()
+    Returns:
+        List[str]: A list of string identifiers, each representing a model that is available with the provided OpenAI key.
+    """
+    res = OpenAI(api_key=api_key, base_url=base_url).models.list()
 
     return [models.id for models in res.data]
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 )
 from mindsdb.integrations.handlers.openai_handler.constants import (
     CHAT_MODELS,
     IMAGE_MODELS,
     FINETUNING_MODELS,
     OPENAI_API_BASE,
 )
+from mindsdb.integrations.libs.llm.utils import get_completed_prompts
 from mindsdb.integrations.utilities.handler_utils import get_api_key
-from mindsdb.integrations.libs.llm_utils import get_completed_prompts
 
 logger = log.getLogger(__name__)
 
 
 class OpenAIHandler(BaseMLEngine):
     name = 'openai'
 
@@ -60,16 +60,16 @@
 
     def create_engine(self, connection_args):
         '''check api key if provided
         '''
         connection_args = {k.lower(): v for k, v in connection_args.items()}
         api_key = connection_args.get('openai_api_key')
         if api_key is not None:
-            api_base = connection_args.get('api_base', os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE))
             org = connection_args.get('api_organization')
+            api_base = connection_args.get('api_base') or os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
             client = self._get_client(api_key=api_key, base_url=api_base, org=org)
             OpenAIHandler._check_client_connection(client)
 
     @staticmethod
     def _check_client_connection(client: OpenAI):
         '''try to connect to api
 
@@ -159,26 +159,29 @@
         if unknown_args:
             # return a list of unknown args as a string
             raise Exception(
                 f"Unknown arguments: {', '.join(unknown_args)}.\n Known arguments are: {', '.join(known_args)}"
             )
 
         engine_storage = kwargs['handler_storage']
+        connection_args = engine_storage.get_connection_args()
         api_key = get_api_key('openai', args, engine_storage=engine_storage)
-        api_base = args.get('api_base', os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE))
+        api_base = connection_args.get('api_base') or args.get('api_base') or os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
         org = args.get('api_organization')
         client = OpenAIHandler._get_client(api_key=api_key, base_url=api_base, org=org)
         OpenAIHandler._check_client_connection(client)
 
     def create(self, target, args=None, **kwargs):
         args = args['using']
         args['target'] = target
         try:
             api_key = get_api_key(self.name, args, self.engine_storage)
-            available_models = get_available_models(api_key)
+            connection_args = self.engine_storage.get_connection_args()
+            api_base = connection_args.get('api_base') or args.get('api_base') or os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
+            available_models = get_available_models(api_key, api_base)
 
             if not args.get('mode'):
                 args['mode'] = self.default_mode
             elif args['mode'] not in self.supported_modes:
                 raise Exception(
                     f"Invalid operation mode. Please use one of {self.supported_modes}"
                 )
@@ -197,19 +200,19 @@
         """
         If there is a prompt template, we use it. Otherwise, we use the concatenation of `context_column` (optional) and `question_column` to ask for a completion.
         """  # noqa
         # TODO: support for edits, embeddings and moderation
 
         pred_args = args['predict_params'] if args else {}
         args = self.model_storage.json_get('args')
-        args['api_base'] = pred_args.get(
-                    'api_base',
-                    args.get(
-                        'api_base', os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE)
-                    ))
+        connection_args = self.engine_storage.get_connection_args()
+        args['api_base'] = (pred_args.get('api_base') or
+                            connection_args.get('api_base') or
+                            args.get('api_base') or
+                            os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE))
         if pred_args.get('api_organization'):
             args['api_organization'] = pred_args['api_organization']
         df = df.reset_index(drop=True)
 
         if pred_args.get('mode'):
             if pred_args['mode'] in self.supported_modes:
                 args['mode'] = pred_args['mode']
@@ -579,16 +582,14 @@
                 ]
 
             completions = [
                 client.images.generate(**{'prompt': p, **kwargs, **api_args}).data[0]
                 for p in prompts
             ]
             return _tidy(completions)
-        
-
         client = self._get_client(
             api_key=api_key,
             base_url=args.get('api_base'),
             org=args.pop('api_organization') if 'api_organization' in args else None,
             )
         try:
             # check if simple completion works
@@ -689,16 +690,14 @@
         """  # noqa
 
         args = args if args else {}
 
         api_key = get_api_key(self.name, args, self.engine_storage)
 
         using_args = args.pop('using') if 'using' in args else {}
-        prompt_col = using_args.get('prompt_column', 'prompt')
-        completion_col = using_args.get('completion_column', 'completion')
         
         api_base = using_args.get('api_base', os.environ.get('OPENAI_API_BASE', OPENAI_API_BASE))
         org = using_args.get('api_organization')
         client = self._get_client(api_key=api_key, base_url=api_base, org=org)
 
 
         args = {**using_args, **args}
@@ -875,9 +874,9 @@
         result_file_id = client.fine_tuning.jobs.retrieve(fine_tuning_job_id=ft_result.id).result_files[0]
         if hasattr(result_file_id, 'id'):
             result_file_id = result_file_id.id  # legacy endpoint
 
         return ft_stats, result_file_id
     
     @staticmethod
-    def _get_client(api_key, base_url=OPENAI_API_BASE, org=None):
+    def _get_client(api_key, base_url, org=None):
         return OpenAI(api_key=api_key, base_url=base_url, organization=org)
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/openbb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openbb_handler/openbb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/openstreetmap_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/openstreetmap_handler/tests/test_openstreetmap_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/palm_handler/palm_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/palm_handler/palm_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import google.generativeai as palm
 import numpy as np
 import pandas as pd
 
 from mindsdb.utilities.hooks import before_palm_query, after_palm_query
 from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import BaseMLEngine
+from mindsdb.integrations.libs.llm.utils import get_completed_prompts
 
 from mindsdb.integrations.utilities.handler_utils import get_api_key
-from mindsdb.integrations.libs.llm_utils import get_completed_prompts
 
 CHAT_MODELS = (
     "models/chat-bison-001",
     "models/embedding-gecko-001",
     "models/text-bison-001",
 )
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pgvector_handler/pgvector_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinecone_handler/pinecone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pirateweather_handler/pirateweather_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/postgres_handler/tests/test_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/pycaret_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pycaret_handler/test/test_pycaret.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/api.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/pypi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/pypi_handler/pypi_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/qdrant_handler/qdrant_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/ingest.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/ingest.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/rag.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/rag.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/rag_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/rag_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rag_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rag_handler/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
 
         elif vector_store == "faiss":
 
             return FAISS.load_local(
                 folder_path=self.config.persist_directory,
                 embeddings=self.config.embeddings_model,
                 index_name=self.config.collection_name,
+                allow_dangerous_deserialization=True
             )
 
         else:
             raise NotImplementedError(f"{vector_store} client is not yet supported")
 
     def load_vector_store(self) -> VectorStore:
         """Load vector store from the persisted vector store"""
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/Arjuna.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/groot.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/groot.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/assets/warrior.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/replicate_handler/replicate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/rockset_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from collections import OrderedDict
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
 from mindsdb.integrations.handlers.mysql_handler import Handler as MySQLHandler
-import rockset
-from rockset import Client
+
 
 class RocksetHandler(MySQLHandler):
     """
     This handler handles connection and execution of the Rockset integration
     """
     name = 'rockset'
 
     def __init__(self, name, **kwargs):
         super().__init__(name, **kwargs)
 
 
 connection_args = OrderedDict(
     user = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.STR,
         'description': 'Rockset user name'
     },
     password = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.STR,
         'description': 'Rockset password'
     },
     api_key = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.STR,
         'description': 'Rockset API key'
     },
     api_server = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.STR,
         'description': 'Rockset API server'
     },
     host = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.STR,
         'description': 'Rockset host'
     },
     port = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.INT,
         'description': 'Rockset port'
     },
     database = {
-        'type': ARG_TYPE.STRING,
+        'type': ARG_TYPE.STR,
         'description': 'Rockset database'
     }
 )
 connection_args_example = OrderedDict(
     user = 'rockset',
     password = 'rockset',
     api_key = "adkjf234rksjfa23waejf2",
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/rockset_handler/tests/test_rockset_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/api.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sap_erp_handler/sap_erp_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sentence_transformers_handler/sentence_transformers_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/sharepoint_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/tests/test_sharepoint_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sharepoint_handler/utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sharepoint_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/solace_handler/solace_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/solace_handler/solace_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/spacy_handler/spacy_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stabilityai_handler/stabilityai_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/strapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/strapi_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strapi_handler/tests/test_strapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/symbl_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/symbl_handler/symbl_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/timegpt_handler/timegpt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_api.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/tripadvisor_handler/tripadvisor_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_api_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twelve_labs_handler/twelve_labs_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twilio_handler/twilio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/api_utilities/microsoft/ms_graph_api_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_oauth_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/google/google_user_oauth_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from google.oauth2.credentials import Credentials
 from google.auth.transport.requests import Request
 
 logger = log.getLogger(__name__)
 
 
-class GoogleOAuth2Manager:
+class GoogleUserOAuth2Manager:
     def __init__(self, handler_stroage: str, scopes: list, credentials_file: str = None, credentials_url: str = None, code: str = None):
         self.handler_storage = handler_stroage
         self.scopes = scopes
         self.credentials_file = credentials_file
         self.credentials_url = credentials_url
         self.code = code
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/auth_utilities/microsoft/ms_graph_api_auth_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/base_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/delete_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/query_utilities/update_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/utilities/validation_utilities/parameter_validation_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/icon.png` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/vertex_client.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/vertex_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from mindsdb.utilities import log
 from google.cloud import aiplatform
-from google.oauth2 import service_account
 import pandas as pd
 
+from mindsdb.integrations.handlers.utilities.auth_utilities import GoogleServiceAccountOAuth2Manager
+
 logger = log.getLogger(__name__)
 
 
 class VertexClient:
     """A class to interact with Vertex AI"""
 
-    def __init__(self, credentials_info, args_json):
-        credentials = service_account.Credentials.from_service_account_info(credentials_info)
+    def __init__(self, args_json, credentials_url=None, credentials_file=None, credentials_json=None):
+        google_sa_oauth2_manager = GoogleServiceAccountOAuth2Manager(
+            credentials_url=credentials_url,
+            credentials_file=credentials_file,
+            credentials_json=credentials_json,
+        )
+        credentials = google_sa_oauth2_manager.get_oauth2_credentials()
+
         aiplatform.init(
             credentials=credentials,
             project=args_json["project_id"],
             location=args_json["location"],
             staging_bucket=args_json["staging_bucket"],
             # the name of the experiment to use to track
             # logged metrics and parameters
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertex_handler/vertex_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import json
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.handlers.vertex_handler.vertex_client import VertexClient
 from mindsdb.utilities import log
 
 logger = log.getLogger(__name__)
 
 
@@ -22,21 +21,22 @@
         """
         assert "using" in args, "Must provide USING arguments for this handler"
         args = args["using"]
 
         model_name = args.pop("model_name")
         custom_model = args.pop("custom_model", False)
 
-        service_account_info = self.engine_storage.json_get('service_account')
+        # get credentials from engine
+        credentials_url, credentials_file, credentials_json = self._get_credentials_from_engine()
 
         # get vertex args from handler then update args from model
         vertex_args = self.engine_storage.json_get('args')
         vertex_args.update(args)
 
-        vertex = VertexClient(service_account_info, vertex_args)
+        vertex = VertexClient(vertex_args, credentials_url, credentials_file, credentials_json)
 
         model = vertex.get_model_by_display_name(model_name)
         if not model:
             raise Exception(f"Vertex model {model_name} not found")
         endpoint_name = model_name + "_endpoint"
         if vertex.get_endpoint_by_display_name(endpoint_name):
             logger.info(f"Endpoint {endpoint_name} already exists, skipping deployment")
@@ -58,30 +58,30 @@
         """Predict using the deployed model by calling the endpoint."""
 
         if "__mindsdb_row_id" in df.columns:
             df.drop("__mindsdb_row_id", axis=1, inplace=True)  # TODO is this required?
 
         predict_args = self.model_storage.json_get("predict_args")
         vertex_args = self.model_storage.json_get("vertex_args")
-        service_account_info = self.engine_storage.json_get('service_account')
 
-        vertex = VertexClient(service_account_info, vertex_args)
+        # get credentials from engine
+        credentials_url, credentials_file, credentials_json = self._get_credentials_from_engine()
+
+        vertex = VertexClient(vertex_args, credentials_url, credentials_file, credentials_json)
         results = vertex.predict_from_df(predict_args["endpoint_name"], df, custom_model=predict_args["custom_model"])
 
         if predict_args["custom_model"]:
             return pd.DataFrame(results.predictions, columns=[predict_args["target"]])
         else:
             return pd.DataFrame(results.predictions)
 
     def create_engine(self, connection_args):
-        if 'service_account' not in connection_args:
-            raise KeyError('"service_account" parameter is required')
-        service_account = connection_args.pop('service_account')
-        if isinstance(service_account, str):
-            # convert to json
-            service_account = json.loads(service_account)
-        else:
-            # unescape new lines in private_key
-            service_account['private_key'] = service_account['private_key'].replace('\\n', '\n')
+        # check if one of credentials_url, credentials_file, or credentials_json is provided
+        if 'service_account_key_url' not in connection_args and 'service_account_key_file' not in connection_args and 'service_account_key_json' not in connection_args:
+            raise KeyError('Either service_account_key_url, service_account_key_file, or service_account_key_json must be provided')
 
         self.engine_storage.json_set('args', connection_args)
-        self.engine_storage.json_set('service_account', service_account)
+
+    def _get_credentials_from_engine(self):
+        engine_args = self.engine_storage.json_get('args')
+
+        return engine_args.get('service_account_key_url'), engine_args.get('service_account_key_file'), engine_args.get('service_account_key_json')
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/weaviate_handler/weaviate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/tests/example_data.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/tests/example_data.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/web_handler/web_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/web_handler/web_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/webz_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/webz_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/webz_handler/webz_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/webz_handler/webz_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/whatsapp_handler/whatsapp_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/evaluate.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/evaluate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/settings.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/xata_handler/xata_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/xata_handler/xata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from collections import OrderedDict
 from mindsdb.utilities.config import Config
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
 from googleapiclient.discovery import build
 
-from mindsdb.integrations.handlers.utilities.auth_utilities import GoogleOAuth2Manager
+from mindsdb.integrations.handlers.utilities.auth_utilities import GoogleUserOAuth2Manager
 
 DEFAULT_SCOPES = [
 	'https://www.googleapis.com/auth/youtube',
 	'https://www.googleapis.com/auth/youtube.force-ssl',
 	'https://www.googleapis.com/auth/youtubepartner'
 ]
 
@@ -82,15 +82,15 @@
         -------
         StatusResponse
             connection object
         """
         if self.is_connected is True:
             return self.connection
         
-        google_oauth2_manager = GoogleOAuth2Manager(self.handler_storage, self.scopes, self.credentials_file, self.credentials_url, self.connection_data.get('code'))
+        google_oauth2_manager = GoogleUserOAuth2Manager(self.handler_storage, self.scopes, self.credentials_file, self.credentials_url, self.connection_data.get('code'))
         creds = google_oauth2_manager.get_oauth2_credentials()
 
         youtube = build(
             "youtube", "v3", developerKey=self.youtube_api_token, credentials=creds
         )
         self.connection = youtube
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers/zipcodebase_handler/zipcodebase_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-24.4.2.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/api_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/base.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/llm_utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/llm/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,39 @@
-import re
+from typing import Optional, Dict, List, Tuple
 import json
 import itertools
-from typing import Optional, Dict, List, Tuple
+import re
 
 import numpy as np
 import pandas as pd
 from langchain.text_splitter import (
     Language,
     RecursiveCharacterTextSplitter,
 )
 
+from mindsdb.integrations.libs.llm.config import AnthropicConfig, AnyscaleConfig, BaseLLMConfig, LiteLLMConfig, OllamaConfig, OpenAIConfig
+
+# Default to latest GPT-4 model (https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo)
+DEFAULT_OPENAI_MODEL = 'gpt-4-0125-preview'
+# Requires more than vanilla OpenAI due to ongoing summarization and 3rd party input.
+DEFAULT_OPENAI_MAX_TOKENS = 2048
+DEFAULT_OPENAI_MAX_RETRIES = 3
+
+DEFAULT_ANTHROPIC_MODEL = 'claude-3-haiku-20240307'
+
+DEFAULT_ANYSCALE_MODEL = 'meta-llama/Llama-2-7b-chat-hf'
+DEFAULT_ANYSCALE_BASE_URL = 'https://api.endpoints.anyscale.com/v1'
+
+DEFAULT_LITELLM_MODEL = 'gpt-3.5-turbo'
+DEFAULT_LITELLM_PROVIDER = 'openai'
+DEFAULT_LITELLM_BASE_URL = 'https://ai.dev.mindsdb.com'
+
+DEFAULT_OLLAMA_BASE_URL = 'http://localhost:11434'
+DEFAULT_OLLAMA_MODEL = 'llama2'
+
 
 def get_completed_prompts(base_template: str, df: pd.DataFrame) -> Tuple[List[str], np.ndarray]:
     """
         Helper method that produces formatted prompts given a template and data in a Pandas DataFrame.
         It also returns the ID of any empty templates that failed to be filled due to missing data.
         
         :param base_template: string with placeholders for each column in the DataFrame. Placeholders should follow double curly braces format, e.g. `{{column_name}}`. All placeholders should have matching columns in `df`.
@@ -52,14 +72,97 @@
         else:
             df['__mdb_prompt'] = df['__mdb_prompt'].apply(lambda x: x + atom)
     prompts = list(df['__mdb_prompt'])
 
     return prompts, empty_prompt_ids
 
 
+def get_llm_config(provider: str, config: Dict) -> BaseLLMConfig:
+    """
+        Helper method that returns the configuration for a given LLM provider.
+
+        :param provider: string with the name of the provider.
+        :param config: dictionary with the configuration for the provider.
+
+        :return: LLMConfig object with the configuration for the provider.
+    """
+    temperature = min(1.0, max(0.0, config.get('temperature', 0.0)))
+    if provider == 'openai':
+        return OpenAIConfig(
+            model_name=config.get('model_name', DEFAULT_OPENAI_MODEL),
+            temperature=temperature,
+            max_retries=config.get('max_retries', DEFAULT_OPENAI_MAX_RETRIES),
+            max_tokens=config.get('max_tokens', DEFAULT_OPENAI_MAX_TOKENS),
+            openai_api_base=config.get('base_url', None),
+            openai_api_key=config['api_keys'].get('openai', None),
+            openai_organization=config.get('api_organization', None),
+            request_timeout=config.get('request_timeout', None),
+        )
+    if provider == 'anthropic':
+        return AnthropicConfig(
+            model=config.get('model_name', DEFAULT_ANTHROPIC_MODEL),
+            temperature=temperature,
+            max_tokens=config.get('max_tokens', None),
+            top_p=config.get('top_p', None),
+            top_k=config.get('top_k', None),
+            default_request_timeout=config.get('default_request_timeout', None),
+            anthropic_api_key=config['api_keys'].get('anthropic', None),
+            anthropic_api_url=config.get('base_url', None),
+        )
+    if provider == 'anyscale':
+        return AnyscaleConfig(
+            model_name=config.get('model_name', DEFAULT_ANYSCALE_MODEL),
+            temperature=temperature,
+            max_retries=config.get('max_retries', DEFAULT_OPENAI_MAX_RETRIES),
+            max_tokens=config.get('max_tokens', DEFAULT_OPENAI_MAX_TOKENS),
+            anyscale_api_base=config.get('base_url', DEFAULT_ANYSCALE_BASE_URL),
+            anyscale_api_key=config['api_keys'].get('anyscale', None),
+            anyscale_proxy=config.get('proxy', None),
+            request_timeout=config.get('request_timeout', None),
+        )
+    if provider == 'litellm':
+        model_kwargs = {
+            'api_key': config['api_keys'].get('litellm', None),
+            'top_p': config.get('top_p', None),
+            'request_timeout': config.get('request_timeout', None),
+            'frequency_penalty': config.get('frequency_penalty', None),
+            'presence_penalty': config.get('presence_penalty', None),
+            'logit_bias': config.get('logit_bias', None),
+        }
+        return LiteLLMConfig(
+            model_name=config.get('model_name', DEFAULT_LITELLM_MODEL),
+            temperature=temperature,
+            api_base=config.get('base_url', DEFAULT_LITELLM_BASE_URL),
+            max_retries=config.get('max_retries', DEFAULT_OPENAI_MAX_RETRIES),
+            max_tokens=config.get('max_tokens', DEFAULT_OPENAI_MAX_TOKENS),
+            top_p=config.get('top_p', None),
+            top_k=config.get('top_k', None),
+            custom_llm_provider=config.get('custom_llm_provider', DEFAULT_LITELLM_PROVIDER),
+            model_kwargs=model_kwargs
+        )
+    if provider == 'ollama':
+        return OllamaConfig(
+            base_url=config.get('base_url', DEFAULT_OLLAMA_BASE_URL),
+            model=config.get('model_name', DEFAULT_OLLAMA_MODEL),
+            temperature=temperature,
+            top_p=config.get('top_p', None),
+            top_k=config.get('top_k', None),
+            timeout=config.get('request_timeout', None),
+            format=config.get('format', None),
+            headers=config.get('headers', None),
+            num_predict=config.get('num_predict', None),
+            num_ctx=config.get('num_ctx', None),
+            num_gpu=config.get('num_gpu', None),
+            repeat_penalty=config.get('repeat_penalty', None),
+            stop=config.get('stop', None),
+            template=config.get('template', None),
+        )
+    raise ValueError(f'Provider {provider} is not supported.')
+
+
 def ft_jsonl_validation(
         items: list,  # read from a JSONL file
         messages_col: str = "messages",
 
         # valid keys for each chat message
         role_key: str = "role",
         content_key: str = "content",
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/__init__.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/create_engine_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/describe_process.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/describe_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/handlers_cacher.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/learn_process.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/learn_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,18 @@
             predictor_record = db.Predictor.query.with_for_update().get(model_id)
             predictor_record.training_data_columns_count = training_data_columns_count
             predictor_record.training_data_rows_count = training_data_rows_count
             db.session.commit()
 
             module = importlib.import_module(module_path)
 
+            # check if module is imported successfully and raise exception if not
+            if module.import_error is not None:
+                raise module.import_error
+
             handlerStorage = HandlerStorage(integration_id)
             modelStorage = ModelStorage(model_id)
             modelStorage.fileStorage.push()     # FIXME
 
             kwargs = {}
             if base_model_id is not None:
                 kwargs['base_model_storage'] = ModelStorage(base_model_id)
```

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/predict_process.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/predict_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/update_engine_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/ml_handler_process/update_process.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/ml_handler_process/update_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/process_cache.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/process_cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/realtime_chat_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/realtime_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/response.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/libs/vectordatabase_handler.py` & `MindsDB-24.4.2.0/mindsdb/integrations/libs/vectordatabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/dataset.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/question_answering/fda_style_qa.csv`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/datasets/question_answering/squad_v2_val_100_sample.csv`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/handler_utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/handler_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/integrations/utilities/utils.py` & `MindsDB-24.4.2.0/mindsdb/integrations/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/agents/agents_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/agents/agents_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/chatbot_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/chatbot_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/chatbot_executor.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/chatbot_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/chatbot_task.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/chatbot_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/memory.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/memory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/model_executor.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/model_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/polling.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/polling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/chatbot/types.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/chatbot/types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/database/database.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/database/integrations.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/database/log.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/database/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/database/projects.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/database/views.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/file/file_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/knowledge_base/controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/knowledge_base/controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/model/functions.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/model/model_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/model/model_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/query_context/context_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/query_context/context_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,27 @@
                 query=query,
                 session=session
             )
 
             if len(data) == 0:
                 value = None
             else:
-                value = data[0][0]
+                row = data[0]
+
+                idx = None
+                for i, col in enumerate(columns_info):
+                    if col['name'].upper() == info['column_name'].upper():
+                        idx = i
+                        break
+
+                if idx is None or len(row) == 1:
+                    value = row[0]
+                else:
+                    value = row[idx]
+
             if value is not None:
                 last_values[info['table_name']] = {info['column_name']: value}
 
         return last_values
 
     # Context
```

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/query_context/last_query.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/query_context/last_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/skills/skill_tool.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/skills/skill_tool.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/skills/skills_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/skills/skills_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/skills/sql_agent.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/skills/sql_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/storage/db.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/storage/fs.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/storage/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     pass
 
 
 from mindsdb.utilities.config import Config
 from mindsdb.utilities.context import context as ctx
 import mindsdb.utilities.profiler as profiler
 from mindsdb.utilities import log
+from mindsdb.utilities.fs import safe_extract
 
 logger = log.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class RESOURCE_GROUP:
     PREDICTOR = 'predictor'
@@ -295,15 +296,15 @@
             Key=remote_ziped_name,
             ObjectAttributes=['ObjectSize']
         )['ObjectSize']
         if (remote_size * 2) > psutil.virtual_memory().available:
             fh = io.BytesIO()
             self.s3.download_fileobj(self.bucket, remote_ziped_name, fh)
             with tarfile.open(fileobj=fh) as tar:
-                tar.extractall(path=base_dir)
+                safe_extract(tar, path=base_dir)
         else:
             self.s3.download_file(self.bucket, remote_ziped_name, local_ziped_path)
             shutil.unpack_archive(local_ziped_path, base_dir)
             os.remove(local_ziped_path)
 
         # os.system(f'chmod -R 777 {base_dir}')
```

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/storage/json.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/tabs/tabs_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/tabs/tabs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/tasks/task_monitor.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/tasks/task_monitor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/tasks/task_thread.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/tasks/task_thread.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/triggers/trigger_task.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/triggers/trigger_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/interfaces/triggers/triggers_controller.py` & `MindsDB-24.4.2.0/mindsdb/interfaces/triggers/triggers_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/metrics/metrics.py` & `MindsDB-24.4.2.0/mindsdb/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/metrics/server.py` & `MindsDB-24.4.2.0/mindsdb/metrics/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-24.4.2.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/alembic.ini` & `MindsDB-24.4.2.0/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/env.py` & `MindsDB-24.4.2.0/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/migrate.py` & `MindsDB-24.4.2.0/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-07-13_a57506731839_triggers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-07-19_ad04ee0bd385_chatbot_to_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-08-29_b0382f5be48d_predictor_hostname.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-08-31_4c26ad04eeaa_add_skills_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-06_d44ab65a6a35_add_agents_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-06_e187961e844a_add_agent_skills_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-18_011e6f2dd9c2_backfill_agent_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-18_f16d4ab03091_add_agent_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-09-20_309db3d07cf4_add_knowledge_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-10-03_6cb02dfd7f61_query_context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-11-01_c67822e96833_jobs_active.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2023-12-25_4b3c9d63e89c_predictor_index.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2024-02-02_5a5c49313e52_job_condition.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py` & `MindsDB-24.4.2.0/mindsdb/migrations/versions/2024-02-12_9461892bd889_llm_log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/auth.py` & `MindsDB-24.4.2.0/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/cache.py` & `MindsDB-24.4.2.0/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/config.py` & `MindsDB-24.4.2.0/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/context.py` & `MindsDB-24.4.2.0/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/context_executor.py` & `MindsDB-24.4.2.0/mindsdb/utilities/context_executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/exception.py` & `MindsDB-24.4.2.0/mindsdb/utilities/exception.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/fs.py` & `MindsDB-24.4.2.0/mindsdb/utilities/fs.py`

 * *Files 9% similar despite different names*

```diff
@@ -158,7 +158,28 @@
                 continue
 
             except psutil.NoSuchProcess:
                 logger.warning(
                     f"We have mark for process/thread {process_id}/{thread_id} but it does not exists"
                 )
                 file.unlink()
+
+
+def __is_within_directory(directory, target):
+    abs_directory = os.path.abspath(directory)
+    abs_target = os.path.abspath(target)
+    prefix = os.path.commonprefix([abs_directory, abs_target])
+    return prefix == abs_directory
+
+
+def safe_extract(tarfile, path=".", members=None, *, numeric_owner=False):
+    # for py >= 3.12
+    if hasattr(tarfile, 'data_filter'):
+        tarfile.extractall(path, members=members, numeric_owner=numeric_owner, filter='data')
+        return
+
+    # for py < 3.12
+    for member in tarfile.getmembers():
+        member_path = os.path.join(path, member.name)
+        if not __is_within_directory(path, member_path):
+            raise Exception("Attempted Path Traversal in Tar File")
+    tarfile.extractall(path, members=members, numeric_owner=numeric_owner)
```

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/functions.py` & `MindsDB-24.4.2.0/mindsdb/utilities/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import argparse
 import datetime
 from functools import wraps
 import hashlib
 import base64
+import os
+import textwrap
 from cryptography.fernet import Fernet
 from collections.abc import Callable
 
 import requests
 from mindsdb_sql import get_lexer_parser
 from mindsdb_sql.parser.ast import Identifier
 
 from mindsdb.utilities.fs import create_process_mark, delete_process_mark, set_process_mark
 from mindsdb.utilities import log
+from mindsdb.utilities.config import Config
+
 
 logger = log.getLogger(__name__)
 
 
 def args_parse():
     parser = argparse.ArgumentParser(description='CL argument for mindsdb server')
     parser.add_argument('--api', type=str, default=None)
@@ -24,14 +28,30 @@
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('--no_studio', action='store_true')
     parser.add_argument('-v', '--version', action='store_true')
     parser.add_argument('--ml_task_queue_consumer', action='store_true', default=None)
     return parser.parse_args()
 
 
+def get_handler_install_message(handler_name):
+    if Config().use_docker_env:
+        container_id = os.environ.get("HOSTNAME", "<container_id>")
+        return textwrap.dedent(f"""\
+            To install the {handler_name} handler, run the following in your terminal outside the docker container
+            ({container_id} is the ID of this container):
+
+                docker exec {container_id} pip install 'mindsdb[{handler_name}]'""")
+    else:
+        return textwrap.dedent(f"""\
+            To install the {handler_name} handler, run the following in your terminal:
+
+                pip install 'mindsdb[{handler_name}]'  # If you installed mindsdb via pip
+                pip install '.[{handler_name}]'        # If you installed mindsdb from source""")
+
+
 def cast_row_types(row, field_types):
     '''
     '''
     keys = [x for x in row.keys() if x in field_types]
     for key in keys:
         t = field_types[key]
         if t == 'Timestamp' and isinstance(row[key], (int, float)):
```

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/hooks/__init__.py` & `MindsDB-24.4.2.0/mindsdb/utilities/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/hooks/profiling.py` & `MindsDB-24.4.2.0/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/json_encoder.py` & `MindsDB-24.4.2.0/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/log.py` & `MindsDB-24.4.2.0/mindsdb/utilities/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             "__main__": {
                 "level": mindsdb_level,
             },
             "mindsdb": {
                 "level": mindsdb_level,
             },
             "alembic": {
-                "level": logging.DEBUG,
+                "level": mindsdb_level,
             },
         },
     )
     dictConfig(logging_config)
 
 
 # I would prefer to leave code to use logging.getLogger(), but there are a lot of complicated situations
```

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/log_controller.py` & `MindsDB-24.4.2.0/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/__init__.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/const.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/const.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/consumer.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/consumer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/producer.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/producer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/task.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ml_task_queue/utils.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ml_task_queue/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/profiler/profiler.py` & `MindsDB-24.4.2.0/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/ps.py` & `MindsDB-24.4.2.0/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/security.py` & `MindsDB-24.4.2.0/mindsdb/utilities/security.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/telemetry.py` & `MindsDB-24.4.2.0/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/mindsdb/utilities/wizards.py` & `MindsDB-24.4.2.0/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-24.3.5.0/requirements/requirements.txt` & `MindsDB-24.4.2.0/requirements/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 sqlalchemy >= 2.0.0, < 3.0.0
 psycopg2-binary  # This is required for using sqlalchemy with postgres
 alembic >= 1.3.3
 redis >=5.0.0, < 6.0.0
 walrus==0.9.3
 flask-compress >= 1.0.0
 appdirs >= 1.0.0
-mindsdb-sql ~= 0.11.0
+mindsdb-sql ~= 0.12.0
 mindsdb-evaluator >= 0.0.7, < 0.1.0
 checksumdir >= 1.2.0
 duckdb == 0.9.1
 requests >= 2.30.0
 pydateinfer==0.3.0
 dataprep_ml==0.0.22
 dill == 0.3.6
@@ -34,8 +34,9 @@
 scikit-learn==1.3.2
 protobuf==3.20.3
 hierarchicalforecast~=0.4.0
 google-auth-oauthlib
 msal
 langchain>=0.1.9
 langchain-core>=0.1.28
-prometheus-client==0.20.0
+prometheus-client==0.20.0
+pydantic
```

### Comparing `MindsDB-24.3.5.0/setup.py` & `MindsDB-24.4.2.0/setup.py`

 * *Files identical despite different names*

