# Comparing `tmp/dagster-cloud-1.6.9.tar.gz` & `tmp/dagster-cloud-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.6.9.tar", last modified: Fri Mar  8 00:31:56 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.0.tar", last modified: Thu Apr  4 19:55:52 2024, max compression
```

## Comparing `dagster-cloud-1.6.9.tar` & `dagster-cloud-1.7.0.tar`

### file list

```diff
@@ -1,133 +1,140 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.762329 dagster-cloud-1.6.9/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-03-08 00:31:56.762329 dagster-cloud-1.6.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.570331 dagster-cloud-1.6.9/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      160 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.582331 dagster-cloud-1.6.9/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)      796 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.586331 dagster-cloud-1.6.9/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46069 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1770 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.590331 dagster-cloud-1.6.9/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18910 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.598331 dagster-cloud-1.6.9/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/auth/constants.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.610330 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.618330 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
--rw-r--r--   0 root         (0) root         (0)     6941 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3234 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/errors.py
--rw-r--r--   0 root         (0) root         (0)     2375 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/insights_utils.py
--rw-r--r--   0 root         (0) root         (0)    10824 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/metrics_utils.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.626330 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 root         (0) root         (0)     5145 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7064 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/definitions.py
--rw-r--r--   0 root         (0) root         (0)     9358 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 root         (0) root         (0)     3808 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.630330 dagster-cloud-1.6.9/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.630330 dagster-cloud-1.6.9/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.638330 dagster-cloud-1.6.9/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    17256 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.646330 dagster-cloud-1.6.9/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.646330 dagster-cloud-1.6.9/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    20441 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.654330 dagster-cloud-1.6.9/dagster_cloud/metrics/
--rw-r--r--   0 root         (0) root         (0)    10117 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/metrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.658330 dagster-cloud-1.6.9/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.666330 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.674330 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3907 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9301 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.678330 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.682330 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     2115 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17843 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)    12797 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.686330 dagster-cloud-1.6.9/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.698330 dagster-cloud-1.6.9/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4565 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.702329 dagster-cloud-1.6.9/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1619 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.706329 dagster-cloud-1.6.9/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4742 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.714329 dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16065 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    44444 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.718329 dagster-cloud-1.6.9/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6445 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19029 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.726329 dagster-cloud-1.6.9/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7726 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.738329 dagster-cloud-1.6.9/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2427 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/util/container_resources.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.738329 dagster-cloud-1.6.9/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.746329 dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)    10918 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6405 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.746329 dagster-cloud-1.6.9/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12535 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.754329 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28413 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    27667 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2766 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.754329 dagster-cloud-1.6.9/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25531 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11618 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/kubernetes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.762329 dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14157 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    79489 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:56.570331 dagster-cloud-1.6.9/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-03-08 00:31:56.000000 dagster-cloud-1.6.9/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4069 2024-03-08 00:31:56.000000 dagster-cloud-1.6.9/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:31:56.000000 dagster-cloud-1.6.9/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-03-08 00:31:56.000000 dagster-cloud-1.6.9/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-08 00:31:56.000000 dagster-cloud-1.6.9/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 00:31:56.762329 dagster-cloud-1.6.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3078 2024-03-08 00:18:12.000000 dagster-cloud-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.204191 dagster-cloud-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-04-04 19:55:52.204191 dagster-cloud-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.128191 dagster-cloud-1.7.0/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.132191 dagster-cloud-1.7.0/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.132191 dagster-cloud-1.7.0/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45467 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.136191 dagster-cloud-1.7.0/dagster_cloud/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      190 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9288 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.140191 dagster-cloud-1.7.0/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.140191 dagster-cloud-1.7.0/dagster_cloud/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.140191 dagster-cloud-1.7.0/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.144191 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.148191 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10835 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.152191 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     9358 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.152191 dagster-cloud-1.7.0/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.156191 dagster-cloud-1.7.0/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.156191 dagster-cloud-1.7.0/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17256 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.156191 dagster-cloud-1.7.0/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.156191 dagster-cloud-1.7.0/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    21080 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.160191 dagster-cloud-1.7.0/dagster_cloud/metrics/
+-rw-r--r--   0 root         (0) root         (0)    10090 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/metrics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.160191 dagster-cloud-1.7.0/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.160191 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.164191 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.168191 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.168191 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17843 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.168191 dagster-cloud-1.7.0/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.172191 dagster-cloud-1.7.0/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.172191 dagster-cloud-1.7.0/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.176191 dagster-cloud-1.7.0/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.180191 dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16297 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46114 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.180191 dagster-cloud-1.7.0/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6446 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    18839 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.184191 dagster-cloud-1.7.0/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.184191 dagster-cloud-1.7.0/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.188191 dagster-cloud-1.7.0/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.188191 dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.192191 dagster-cloud-1.7.0/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12977 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.196191 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28818 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28623 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.200191 dagster-cloud-1.7.0/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26248 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9825 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.204191 dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14248 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    82607 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:52.128191 dagster-cloud-1.7.0/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-04-04 19:55:51.000000 dagster-cloud-1.7.0/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4274 2024-04-04 19:55:51.000000 dagster-cloud-1.7.0/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:51.000000 dagster-cloud-1.7.0/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-04 19:55:51.000000 dagster-cloud-1.7.0/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-04 19:55:51.000000 dagster-cloud-1.7.0/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 19:55:52.204191 dagster-cloud-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-04 19:44:30.000000 dagster-cloud-1.7.0/setup.py
```

### Comparing `dagster-cloud-1.6.9/PKG-INFO` & `dagster-cloud-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.6.9
+Version: 1.7.0
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.6.9/README.md` & `dagster-cloud-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/agent/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/agent/cli/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster-cloud-1.7.0/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import logging
 import os
 import sys
-import tempfile
 import time
-import zlib
 from collections import deque
 from concurrent.futures import Future, ThreadPoolExecutor
 from contextlib import ExitStack
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union, cast
 
 import dagster._check as check
 import pendulum
 from dagster import DagsterInstance
-from dagster._core.host_representation import (
+from dagster._core.launcher.base import LaunchRunContext
+from dagster._core.remote_representation import (
     CodeLocationOrigin,
 )
-from dagster._core.host_representation.origin import RegisteredCodeLocationOrigin
-from dagster._core.launcher.base import LaunchRunContext
+from dagster._core.remote_representation.origin import RegisteredCodeLocationOrigin
 from dagster._core.utils import FuturesAwareThreadPoolExecutor
 from dagster._grpc.client import DagsterGrpcClient
 from dagster._grpc.types import CancelExecutionRequest
 from dagster._serdes import (
     deserialize_value,
     serialize_value,
 )
 from dagster._utils.container import (
     retrieve_containerized_utilization_metrics,
 )
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.interrupts import raise_interrupts_as
 from dagster._utils.merger import merge_dicts
 from dagster._utils.typed_dict import init_optional_typeddict
-from dagster_cloud_cli.core.errors import GraphQLStorageError, raise_http_error
+from dagster_cloud_cli.core.errors import raise_http_error
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 
 from dagster_cloud.api.dagster_cloud_api import (
     AgentHeartbeat,
     AgentUtilizationMetrics,
     DagsterCloudApi,
     DagsterCloudApiErrorResponse,
@@ -50,15 +48,15 @@
 )
 from dagster_cloud.instance import DagsterCloudAgentInstance
 from dagster_cloud.workspace.user_code_launcher import (
     DagsterCloudUserCodeLauncher,
     UserCodeLauncherEntry,
 )
 
-from ..util import SERVER_HANDLE_TAG, is_isolated_run
+from ..util import SERVER_HANDLE_TAG, compressed_namedtuple_upload_file, is_isolated_run
 from ..version import __version__
 from .queries import (
     ADD_AGENT_HEARTBEATS_MUTATION,
     DEPLOYMENTS_QUERY,
     GET_USER_CLOUD_REQUESTS_QUERY,
     WORKSPACE_ENTRIES_QUERY,
 )
@@ -264,31 +262,27 @@
                 pass
 
             if user_code_launcher.ready_to_serve_requests:
                 try:
                     self._check_add_heartbeat(instance, agent_uuid, heartbeat_interval_seconds)
                 except Exception:
                     self._logger.error(
-                        "Failed to add heartbeat: \n{}".format(
-                            serializable_error_info_from_exc_info(sys.exc_info())
-                        )
+                        f"Failed to add heartbeat: \n{serializable_error_info_from_exc_info(sys.exc_info())}"
                     )
 
             # Check for any received interrupts
             with raise_interrupts_as(KeyboardInterrupt):
                 pass
 
             try:
                 self._check_update_workspace(instance, user_code_launcher, upload_all=False)
 
             except Exception:
                 self._logger.error(
-                    "Failed to check for workspace updates: \n{}".format(
-                        serializable_error_info_from_exc_info(sys.exc_info())
-                    )
+                    f"Failed to check for workspace updates: \n{serializable_error_info_from_exc_info(sys.exc_info())}"
                 )
 
             # Check for any received interrupts
             with raise_interrupts_as(KeyboardInterrupt):
                 time.sleep(SLEEP_INTERVAL_SECONDS)
 
     def _check_update_workspace(self, instance, user_code_launcher, upload_all):
@@ -370,25 +364,22 @@
             ]
             self._logger.info(
                 f"Current agent threadpool utilization: {num_running_requests}/{max_concurrent_requests} threads"
             )
 
         self._last_heartbeat_time = curr_time
 
-        res = instance.organization_scoped_graphql_client().execute(
+        instance.organization_scoped_graphql_client().execute(
             ADD_AGENT_HEARTBEATS_MUTATION,
             variable_values={
                 "serializedAgentHeartbeats": serialized_agent_heartbeats,
             },
             idempotent_mutation=True,
         )
 
-        if "errors" in res:
-            raise GraphQLStorageError(res)
-
     @property
     def executor(self) -> ThreadPoolExecutor:
         return self._executor
 
     @property
     def request_ids_to_futures(self) -> Dict[str, Future]:
         return self._request_ids_to_futures
@@ -616,15 +607,15 @@
         """Derive the location from the specific argument passed in to a dagster_cloud_api call."""
         api_name = request.request_api
         if api_name in {
             DagsterCloudApi.GET_EXTERNAL_EXECUTION_PLAN,
             DagsterCloudApi.GET_SUBSET_EXTERNAL_PIPELINE_RESULT,
         }:
             external_pipeline_origin = request.request_args.job_origin
-            return external_pipeline_origin.external_repository_origin.code_location_origin
+            return external_pipeline_origin.repository_origin.code_location_origin
         elif api_name in {
             DagsterCloudApi.GET_EXTERNAL_PARTITION_CONFIG,
             DagsterCloudApi.GET_EXTERNAL_PARTITION_TAGS,
             DagsterCloudApi.GET_EXTERNAL_PARTITION_NAMES,
             DagsterCloudApi.GET_EXTERNAL_PARTITION_SET_EXECUTION_PARAM_DATA,
             DagsterCloudApi.GET_EXTERNAL_SCHEDULE_EXECUTION_DATA,
             DagsterCloudApi.GET_EXTERNAL_SENSOR_EXECUTION_DATA,
@@ -783,15 +774,15 @@
                         f"Launching {run.run_id} without an isolated run environment.",
                         run,
                         cls=self.__class__,
                     )
 
                     run_location_name = cast(
                         str,
-                        run.external_job_origin.external_repository_origin.code_location_origin.location_name,
+                        run.external_job_origin.repository_origin.code_location_origin.location_name,
                     )
 
                     server = user_code_launcher.get_grpc_server(deployment_name, run_location_name)
 
                     # Record the server handle that we launched it on to for run monitoring
                     scoped_instance.add_run_tags(
                         run.run_id, new_tags={SERVER_HANDLE_TAG: str(server.server_handle)}
@@ -827,15 +818,15 @@
                     )
                     if is_isolated_run(run):
                         launcher = scoped_instance.get_run_launcher_for_run(run)  # type: ignore  # (instance subclass)
                         launcher.terminate(run.run_id)
                     else:
                         run_location_name = cast(
                             str,
-                            run.external_job_origin.external_repository_origin.code_location_origin.location_name,
+                            run.external_job_origin.repository_origin.code_location_origin.location_name,
                         )
 
                         server = user_code_launcher.get_grpc_server(
                             deployment_name, run_location_name
                         )
                         client = server.server_endpoint.create_client()
 
@@ -868,16 +859,16 @@
         request: Union[str, DagsterCloudApiRequest] = DagsterCloudApiRequest.format_request(
             request_id, request_api
         )
 
         if request_api not in DagsterCloudApi.__members__:
             api_result = DagsterCloudApiUnknownCommandResponse(request_api)
             self._logger.warning(
-                "Ignoring request {request}: Unknown command. This is likely due to running an "
-                "older version of the agent.".format(request=json_request)
+                f"Ignoring request {json_request}: Unknown command. This is likely due to running an "
+                "older version of the agent."
             )
         else:
             try:
                 request = deserialize_value(request_body, DagsterCloudApiRequest)
                 self._logger.info(f"Received request {request}.")
                 api_result = self._handle_api_request(
                     request, deployment_name, is_branch_deployment, instance, user_code_launcher
@@ -952,19 +943,16 @@
                 f"Iteration #{self._iteration}: Adding {len(json_requests)} requests to be"
                 f" processed. Currently {num_pending_requests} waiting for server to be ready"
             )
             self._pending_requests.extend(json_requests)
 
         else:
             self._logger.warning(
-                "Iteration #{iteration}: Waiting to pull requests from the queue since there are"
-                " already {num_pending_requests} in the queue".format(
-                    iteration=self._iteration,
-                    num_pending_requests=len(self._pending_requests),
-                )
+                f"Iteration #{self._iteration}: Waiting to pull requests from the queue since there are"
+                f" already {len(self._pending_requests)} in the queue"
             )
 
         invalid_requests = []
         self._locations_with_pending_requests = set()
 
         # Determine which pending requests are now ready (their locations have been loaded, or the
         # request does not correspond to a particular location)
@@ -1041,21 +1029,16 @@
 
 
 def upload_api_response(
     instance: DagsterCloudAgentInstance,
     deployment_name: str,
     upload_response: DagsterCloudUploadApiResponse,
 ):
-    with tempfile.TemporaryDirectory() as temp_dir:
-        dst = os.path.join(temp_dir, "api_response.tmp")
-        with open(dst, "wb") as f:
-            f.write(zlib.compress(serialize_value(upload_response).encode("utf-8")))
-
-        with open(dst, "rb") as f:
-            resp = instance.rest_requests_session.put(
-                instance.dagster_cloud_upload_api_response_url,
-                headers=instance.headers_for_deployment(deployment_name),
-                files={"api_response.tmp": f},
-                timeout=instance.dagster_cloud_api_timeout,
-                proxies=instance.dagster_cloud_api_proxies,
-            )
-            raise_http_error(resp)
+    with compressed_namedtuple_upload_file(upload_response) as f:
+        resp = instance.requests_managed_retries_session.put(
+            instance.dagster_cloud_upload_api_response_url,
+            headers=instance.headers_for_deployment(deployment_name),
+            files={"api_response.tmp": f},
+            timeout=instance.dagster_cloud_api_timeout,
+            proxies=instance.dagster_cloud_api_proxies,
+        )
+        raise_http_error(resp)
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/agent/queries.py` & `dagster-cloud-1.7.0/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/api/dagster_cloud_api.py` & `dagster-cloud-1.7.0/dagster_cloud/api/dagster_cloud_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from enum import Enum
 from typing import Any, List, Mapping, NamedTuple, Optional, Sequence, TypedDict, Union, cast
 
 import dagster._check as check
 import pendulum
 from dagster._core.code_pointer import CodePointer
 from dagster._core.definitions.selector import JobSelector
-from dagster._core.host_representation import (
+from dagster._core.events.log import EventLogEntry
+from dagster._core.remote_representation import (
     CodeLocationOrigin,
     ExternalRepositoryData,
 )
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.utils import RequestUtilizationMetrics
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.container import ContainerUtilizationMetrics
@@ -399,14 +400,22 @@
     DagsterCloudApiGrpcResponse,
     DagsterCloudApiErrorResponse,
     DagsterCloudApiUnknownCommandResponse,
 )
 
 
 @whitelist_for_serdes
+class StoreEventBatchRequest(
+    NamedTuple("_StoreEventBatchRequest", [("event_log_entries", Sequence[EventLogEntry])])
+):
+    def __new__(cls, event_log_entries: Sequence[EventLogEntry]):
+        return super().__new__(cls, event_log_entries=event_log_entries)
+
+
+@whitelist_for_serdes
 class DagsterCloudUploadApiResponse(
     NamedTuple(
         "_DagsterCloudUploadApiResponse",
         [
             ("request_id", str),
             ("request_api", str),
             ("response", DagsterCloudApiResponse),
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/auth/constants.py` & `dagster-cloud-1.7.0/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
-    Any,
     Iterable,
     Iterator,
     Optional,
     Union,
 )
 
-import dagster._check as check
+import yaml
 from dagster import (
     AssetCheckResult,
     AssetExecutionContext,
     AssetKey,
     AssetMaterialization,
     AssetObservation,
-    MetadataValue,
     OpExecutionContext,
     Output,
 )
-from dagster._core.definitions.metadata import MetadataMapping
-from google.cloud import bigquery
+from dagster_dbt import DbtCliInvocation
+from dagster_dbt.version import __version__ as dagster_dbt_version
+from packaging import version
 
 from ..insights_utils import extract_asset_info_from_event
 from .bigquery_utils import build_bigquery_cost_metadata, marker_asset_key_for_job
 
 if TYPE_CHECKING:
-    from dagster_dbt import DbtCliInvocation
+    from dbt.adapters.base.impl import BaseAdapter
+    from google.cloud import bigquery
+
+OPAQUE_ID_SQL_SIGIL = "bigquery_dagster_dbt_v1_opaque_id"
+DEFAULT_BQ_REGION = "region-us"
+MIN_DAGSTER_DBT_VERSION = "1.7.0"
 
 
 @dataclass
 class BigQueryCostInfo:
     asset_key: AssetKey
     partition: Optional[str]
     job_id: Optional[str]
@@ -43,39 +47,22 @@
         return (
             f"{self.asset_key.to_string()}:{self.partition}"
             if self.partition
             else self.asset_key.to_string()
         )
 
 
-def _extract_metadata_value(value: Optional[MetadataValue], default_value: Any = None) -> Any:
-    return value.value if value else default_value
-
-
-def _extract_bigquery_info_from_metadata(metadata: MetadataMapping):
-    job_id = _extract_metadata_value(metadata.get("job_id"))
-    bytes_billed = _extract_metadata_value(metadata.get("bytes_billed"), 0)
-    slots_ms = _extract_metadata_value(metadata.get("slots_ms"), 0)
-    return job_id, bytes_billed, slots_ms
-
-
-def _asset_partition_key(asset_key: AssetKey, partition_key: Optional[str]) -> str:
-    return f"{asset_key.to_string()}:{partition_key}" if partition_key else asset_key.to_string()
-
-
 def dbt_with_bigquery_insights(
     context: Union[OpExecutionContext, AssetExecutionContext],
-    dbt_cli_invocation: "DbtCliInvocation",
+    dbt_cli_invocation: DbtCliInvocation,
     dagster_events: Optional[
         Iterable[Union[Output, AssetMaterialization, AssetObservation, AssetCheckResult]]
     ] = None,
+    skip_config_check=False,
     record_observation_usage: bool = True,
-    explicitly_query_information_schema: bool = False,
-    bigquery_client: Optional[bigquery.Client] = None,
-    bigquery_location: Optional[str] = None,
 ) -> Iterator[Union[Output, AssetMaterialization, AssetObservation, AssetCheckResult]]:
     """Wraps a dagster-dbt invocation to associate each BigQuery query with the produced
     asset materializations. This allows the cost of each query to be associated with the asset
     materialization that it produced.
 
     If called in the context of an op (rather than an asset), filters out any Output events
     which do not correspond with any output of the op.
@@ -98,68 +85,105 @@
         def jaffle_shop_dbt_assets(
             context: AssetExecutionContext,
             dbt: DbtCliResource,
         ):
             dbt_cli_invocation = dbt.cli(["build"], context=context)
             yield from dbt_with_bigquery_insights(context, dbt_cli_invocation)
     """
-    if explicitly_query_information_schema:
-        check.inst_param(bigquery_client, "bigquery_client", bigquery.Client)
-        check.str_param(bigquery_location, "bigquery_location")
+    if not skip_config_check:
+        adapter_type = dbt_cli_invocation.manifest["metadata"]["adapter_type"]
+        if adapter_type != "bigquery":
+            raise RuntimeError(
+                f"The 'bigquery' adapter must be used but instead found '{adapter_type}'"
+            )
+        dbt_project_config = yaml.safe_load(
+            (dbt_cli_invocation.project_dir / "dbt_project.yml").open("r")
+        )
+        # sanity check that the sigil is present somewhere in the query comment
+        query_comment = dbt_project_config.get("query-comment")
+        if query_comment is None:
+            raise RuntimeError("query-comment is required in dbt_project.yml but it was missing")
+        comment = query_comment.get("comment")
+        if comment is None:
+            raise RuntimeError(
+                "query-comment.comment is required in dbt_project.yml but it was missing"
+            )
+        if OPAQUE_ID_SQL_SIGIL not in comment:
+            raise RuntimeError(
+                "query-comment.comment in dbt_project.yml must contain the string"
+                f" '{OPAQUE_ID_SQL_SIGIL}'. Read the Dagster Insights docs for more info."
+            )
 
     if dagster_events is None:
         dagster_events = dbt_cli_invocation.stream()
 
-    asset_info_by_job_id = {}
-    cost_by_asset = defaultdict(list)
+    asset_info_by_unique_id = {}
     for dagster_event in dagster_events:
-        if isinstance(dagster_event, (AssetMaterialization, AssetObservation, Output)):
+        if isinstance(
+            dagster_event, (AssetMaterialization, AssetObservation, Output, AssetCheckResult)
+        ):
+            unique_id = dagster_event.metadata["unique_id"].value
             asset_key, partition = extract_asset_info_from_event(
                 context, dagster_event, record_observation_usage
             )
             if not asset_key:
                 asset_key = marker_asset_key_for_job(context.job_def)
-            job_id, bytes_billed, slots_ms = _extract_bigquery_info_from_metadata(
-                dagster_event.metadata
-            )
-            if bytes_billed or slots_ms:
-                asset_info_by_job_id[job_id] = (asset_key, partition)
-                cost_info = BigQueryCostInfo(asset_key, partition, job_id, slots_ms, bytes_billed)
-                cost_by_asset[cost_info.asset_partition_key].append(cost_info)
+            asset_info_by_unique_id[unique_id] = (asset_key, partition)
 
         yield dagster_event
 
-    if explicitly_query_information_schema and bigquery_client:
-        marker_asset_key = marker_asset_key_for_job(context.job_def)
-        run_results_json = dbt_cli_invocation.get_artifact("run_results.json")
-        invocation_id = run_results_json["metadata"]["invocation_id"]
-        assert bigquery_client
-        try:
-            cost_query = f"""
-                SELECT job_id, SUM(total_bytes_billed) AS bytes_billed, SUM(total_slot_ms) AS slots_ms
-                FROM `{bigquery_location}`.INFORMATION_SCHEMA.JOBS
-                WHERE query like '%{invocation_id}%'
-                GROUP BY job_id
-            """
-            context.log.info(f"Querying INFORMATION_SCHEMA.JOBS for bytes billed: {cost_query}")
-            query_result = bigquery_client.query(cost_query)
+    marker_asset_key = marker_asset_key_for_job(context.job_def)
+    run_results_json = dbt_cli_invocation.get_artifact("run_results.json")
+    invocation_id = run_results_json["metadata"]["invocation_id"]
+
+    # backcompat-proof in case the invocation does not have an instantiated adapter on it
+    adapter: Optional["BaseAdapter"] = getattr(dbt_cli_invocation, "adapter", None)
+    if not adapter:
+        if version.parse(dagster_dbt_version) < version.parse(MIN_DAGSTER_DBT_VERSION):
+            upgrade_message = f" Extracting cost information requires dagster_dbt>={MIN_DAGSTER_DBT_VERSION} (found {dagster_dbt_version}). "
+        else:
+            upgrade_message = ""
+
+        context.log.error(
+            "Could not find a BigQuery adapter on the dbt CLI invocation. Skipping cost analysis."
+            + upgrade_message
+        )
+        return
 
-            # overwrite cost_by_asset that is computed from the metadata
-            cost_by_asset = defaultdict(list)
+    cost_by_asset = defaultdict(list)
+    try:
+        with adapter.connection_named("dagster_insights:bigquery_cost"):
+            client: "bigquery.Client" = adapter.connections.get_thread_connection().handle
+            dataset = client.get_dataset(adapter.config.credentials.schema)
+            region = f"region-{dataset.location.lower()}" if dataset.location else DEFAULT_BQ_REGION
+            query_result = client.query(
+                rf"""
+                    SELECT
+                    job_id,
+                    regexp_extract(query, r"{OPAQUE_ID_SQL_SIGIL}\[\[\[(.*?):{invocation_id}\]\]\]") as unique_id,
+                    total_bytes_billed AS bytes_billed,
+                    total_slot_ms AS slots_ms
+                    FROM `{dataset.project}`.`{region}`.INFORMATION_SCHEMA.JOBS
+                    WHERE query like '%{invocation_id}%'
+                """
+            )
             for row in query_result:
-                asset_key, partition = asset_info_by_job_id.get(
-                    row.job_id, (marker_asset_key, None)
+                if not row.unique_id:
+                    continue
+                asset_key, partition = asset_info_by_unique_id.get(
+                    row.unique_id, (marker_asset_key, None)
                 )
                 if row.bytes_billed or row.slots_ms:
                     cost_info = BigQueryCostInfo(
                         asset_key, partition, row.job_id, row.bytes_billed, row.slots_ms
                     )
                     cost_by_asset[cost_info.asset_partition_key].append(cost_info)
-        except:
-            context.log.exception("Could not query information_schema.jobs for bytes billed")
+    except:
+        context.log.exception("Could not query information_schema for BigQuery cost information")
+        return
 
     for cost_info_list in cost_by_asset.values():
         bytes_billed = sum(item.bytes_billed for item in cost_info_list)
         slots_ms = sum(item.slots_ms for item in cost_info_list)
         job_ids = [item.job_id for item in cost_info_list]
         asset_key = cost_info_list[0].asset_key
         partition = cost_info_list[0].partition
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/insights_utils.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/insights_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Tuple, Union
 
 import dagster._check as check
 from dagster import (
+    AssetCheckResult,
     AssetExecutionContext,
     AssetKey,
     AssetMaterialization,
     AssetObservation,
     DagsterInvariantViolationError,
     OpExecutionContext,
     Output,
@@ -38,18 +39,19 @@
     return asset_info.key
 
 
 def extract_asset_info_from_event(context, dagster_event, record_observation_usage):
     if isinstance(dagster_event, AssetMaterialization):
         return dagster_event.asset_key, dagster_event.partition
 
-    if isinstance(dagster_event, AssetObservation) and record_observation_usage:
-        return dagster_event.asset_key, dagster_event.partition
+    if isinstance(dagster_event, (AssetCheckResult, AssetObservation)) and record_observation_usage:
+        partition = dagster_event.partition if isinstance(dagster_event, AssetObservation) else None
+        return dagster_event.asset_key, partition
 
-    if isinstance(dagster_event, AssetObservation):
+    if isinstance(dagster_event, (AssetCheckResult, AssetObservation)):
         return None, None
 
     if isinstance(dagster_event, Output):
         asset_key = get_asset_key_for_output(context, dagster_event.output_name)
         partition_key = None
         if asset_key and context._step_execution_context.has_asset_partitions_for_output(  # noqa: SLF001
             dagster_event.output_name
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/metrics_utils.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/metrics_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 def get_post_request_params(
     instance: DagsterInstance,
 ) -> Tuple[requests.Session, str, Dict[str, str], int, Optional[Dict[str, str]]]:
     if not isinstance(instance, DagsterCloudAgentInstance):
         raise RuntimeError("This asset only functions in a running Dagster Cloud instance")
 
     return (
-        instance.rest_requests_session,
+        instance.requests_managed_retries_session,
         instance.dagster_cloud_gen_insights_url_url,
         instance.dagster_cloud_api_headers(DagsterCloudInstanceScope.DEPLOYMENT),
         instance.dagster_cloud_api_timeout,
         instance.dagster_cloud_api_proxies,
     )
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/query.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/query.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
                 )
 
     if dagster_events is None:
         dagster_events = dbt_cli_invocation.stream()
 
     asset_and_partition_key_to_unique_id: List[Tuple[AssetKey, Optional[str], Any]] = []
     for dagster_event in dagster_events:
-        if isinstance(dagster_event, (AssetMaterialization, AssetObservation, Output)):
+        if isinstance(
+            dagster_event, (AssetMaterialization, AssetObservation, Output, AssetCheckResult)
+        ):
             unique_id = dagster_event.metadata["unique_id"].value
             asset_key, partition = extract_asset_info_from_event(
                 context, dagster_event, record_observation_usage
             )
             if not asset_key:
                 asset_key = marker_asset_key_for_job(context.job_def)
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/definitions.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py` & `dagster-cloud-1.7.0/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster-cloud-1.7.0/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/execution/monitoring/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/execution/utils/process.py` & `dagster-cloud-1.7.0/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/instance/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/instance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from dagster._core.instance import DagsterInstance
 from dagster._core.instance.config import config_field_for_configurable_class
 from dagster._core.instance.ref import InstanceRef, configurable_class_data
 from dagster._core.launcher import DefaultRunLauncher, RunLauncher
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._serdes import ConfigurableClassData
 from dagster_cloud_cli.core.graphql_client import (
+    create_agent_graphql_client,
+    create_agent_http_client,
     create_graphql_requests_session,
-    create_proxy_client,
     get_agent_headers,
 )
 from dagster_cloud_cli.core.headers.auth import DagsterCloudInstanceScope
 from requests import Session
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
@@ -87,14 +88,15 @@
 
         self._exit_stack = ExitStack()
 
         self._user_code_launcher = None
         self._graphql_requests_session: Optional[Session] = None
         self._rest_requests_session: Optional[Session] = None
         self._graphql_client = None
+        self._http_client = None
 
         assert self.dagster_cloud_url
 
         # Handle backcompat between isolated_agents and agent_replicas
         if isolated_agents and agent_replicas:
             raise Exception(
                 "Cannot provide both isolated_agents and agent_replicas configuration. Please only"
@@ -153,60 +155,60 @@
         my_ref = self.get_ref()
         my_custom_instance_class_data = my_ref.custom_instance_class_data
         new_class_data = _cached_inject_deployment(my_custom_instance_class_data, deployment_name)
 
         return my_ref._replace(custom_instance_class_data=new_class_data)
 
     def organization_scoped_graphql_client(self):
-        return create_proxy_client(
-            self.graphql_requests_session,
+        return create_agent_graphql_client(
+            self.client_managed_retries_requests_session,
             self.dagster_cloud_graphql_url,
             self._dagster_cloud_api_config_for_deployment(None),
             scope=DagsterCloudInstanceScope.ORGANIZATION,
         )
 
     def graphql_client_for_deployment(self, deployment_name: Optional[str]):
-        return create_proxy_client(
-            self.graphql_requests_session,
+        return create_agent_graphql_client(
+            self.client_managed_retries_requests_session,
             self.dagster_cloud_graphql_url,
             self._dagster_cloud_api_config_for_deployment(deployment_name),
             scope=DagsterCloudInstanceScope.DEPLOYMENT,
         )
 
     def headers_for_deployment(self, deployment_name: str):
         return get_agent_headers(
             self._dagster_cloud_api_config_for_deployment(deployment_name),
             DagsterCloudInstanceScope.DEPLOYMENT,
         )
 
     def create_graphql_client(
         self, scope: DagsterCloudInstanceScope = DagsterCloudInstanceScope.DEPLOYMENT
     ):
-        return create_proxy_client(
-            self.graphql_requests_session,
+        return create_agent_graphql_client(
+            self.client_managed_retries_requests_session,
             self.dagster_cloud_graphql_url,
             self._dagster_cloud_api_config,
             scope=scope,
         )
 
     @property
-    def graphql_requests_session(self):
+    def client_managed_retries_requests_session(self):
         """A shared requests Session to use between GraphQL clients.
 
         Retries handled in GraphQL client layer.
         """
         if self._graphql_requests_session is None:
             self._graphql_requests_session = self._exit_stack.enter_context(
                 create_graphql_requests_session()
             )
 
         return self._graphql_requests_session
 
     @property
-    def rest_requests_session(self):
+    def requests_managed_retries_session(self):
         """A requests session to use for non-GraphQL Rest API requests.
 
         Retries handled by requests.
         """
         if self._rest_requests_session is None:
             self._rest_requests_session = self._exit_stack.enter_context(Session())
             adapter = HTTPAdapter(
@@ -225,14 +227,25 @@
             self._graphql_client = self.create_graphql_client(
                 scope=DagsterCloudInstanceScope.DEPLOYMENT
             )
 
         return self._graphql_client
 
     @property
+    def http_client(self):
+        if self._http_client is None:
+            self._http_client = create_agent_http_client(
+                self.client_managed_retries_requests_session,
+                self._dagster_cloud_api_config,
+                scope=DagsterCloudInstanceScope.DEPLOYMENT,
+            )
+
+        return self._http_client
+
+    @property
     def dagster_cloud_url(self):
         if "url" in self._dagster_cloud_api_config:
             return self._dagster_cloud_api_config["url"]
 
         organization = get_organization_name_from_agent_token(self.dagster_cloud_agent_token)
         if not organization:
             raise DagsterInvariantViolationError(
@@ -281,14 +294,18 @@
         return f"https://{organization}.dagster.cloud/" + (f"{deployment}/" if deployment else "")
 
     @property
     def dagster_cloud_graphql_url(self):
         return f"{self.dagster_cloud_url}/graphql"
 
     @property
+    def dagster_cloud_store_events_url(self):
+        return f"{self.dagster_cloud_url}/store_events"
+
+    @property
     def dagster_cloud_upload_logs_url(self):
         return f"{self.dagster_cloud_url}/upload_logs"
 
     @property
     def dagster_cloud_gen_logs_url_url(self):
         return f"{self.dagster_cloud_url}/gen_logs_url"
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/metrics/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/metrics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         for selected_asset_keys in _chunks(list(context.selected_asset_keys), 5):
             metric_graphql_inputs.append(
                 {
                     "runId": context.run_id,
                     "stepKey": context.get_step_execution_context().step.key,
                     "codeLocationName": context.dagster_run.external_job_origin.location_name,
                     "repositoryName": (
-                        context.dagster_run.external_job_origin.external_repository_origin.repository_name
+                        context.dagster_run.external_job_origin.repository_origin.repository_name
                     ),
                     "assetMetricDefinitions": [
                         {
                             "assetKey": selected_asset_key.to_python_identifier(),
                             "assetGroup": context.assets_def.group_names_by_key.get(
                                 selected_asset_key, None
                             ),
@@ -90,15 +90,15 @@
     else:
         metric_graphql_inputs.append(
             {
                 "runId": context.run_id,
                 "stepKey": context.get_step_execution_context().step.key,
                 "codeLocationName": context.dagster_run.external_job_origin.location_name,
                 "repositoryName": (
-                    context.dagster_run.external_job_origin.external_repository_origin.repository_name
+                    context.dagster_run.external_job_origin.repository_origin.repository_name
                 ),
                 "jobMetricDefinitions": [
                     {
                         "metricValues": [
                             {
                                 "metricValue": metric_def.metric_value,
                                 "metricName": metric_def.metric_name,
@@ -215,15 +215,15 @@
     for assetMetricDefinitions in _chunks(assetMetricDefinitions, 5):
         metric_graphql_inputs.append(
             {
                 "runId": context.run_id,
                 "stepKey": context.get_step_execution_context().step.key,
                 "codeLocationName": context.dagster_run.external_job_origin.location_name,
                 "repositoryName": (
-                    context.dagster_run.external_job_origin.external_repository_origin.repository_name
+                    context.dagster_run.external_job_origin.repository_origin.repository_name
                 ),
                 "assetMetricDefinitions": assetMetricDefinitions,
             }
         )
     for metric_graphql_inputs in _chunks(metric_graphql_inputs, 5):
         try:
             result = client.execute(
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/client.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/compile.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/manager.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/registry.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/server/server.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/pex/grpc/types.py` & `dagster-cloud-1.7.0/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/secrets/loader.py` & `dagster-cloud-1.7.0/dagster_cloud/secrets/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,24 @@
         secretName
         secretValue
         locationNames
     }
 }
 """
 
-from dagster_cloud_cli.core.errors import GraphQLStorageError
-
 
 class DagsterCloudSecretsLoader(SecretsLoader, ConfigurableClass):
     def __init__(
         self,
         inst_data=None,
     ):
         self._inst_data = inst_data
 
     def _execute_query(self, query, variables=None):
-        res = self._instance.graphql_client.execute(query, variable_values=variables)
-        if "errors" in res:
-            raise GraphQLStorageError(res)
-        return res
+        return self._instance.graphql_client.execute(query, variable_values=variables)
 
     def get_secrets_for_environment(self, location_name: Optional[str]) -> Dict[str, str]:
         res = self._execute_query(
             SECRETS_QUERY,
             variables={"locationName": location_name},
         )
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/serverless/io_manager.py` & `dagster-cloud-1.7.0/dagster_cloud/serverless/io_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,21 +55,14 @@
 
         return "/".join([self._s3_prefix, *path])
 
     def has_output(self, context):
         key = self._get_path(context)
         return self._has_object(key)
 
-    def _rm_object(self, key):
-        check.str_param(key, "key")
-        check.param_invariant(len(key) > 0, "key")
-
-        # delete_object wont fail even if the item has been deleted.
-        self._s3.delete_object(Bucket=self._bucket, Key=key)
-
     def _has_object(self, key):
         check.str_param(key, "key")
         check.param_invariant(len(key) > 0, "key")
 
         found_object = False
 
         try:
@@ -97,17 +90,14 @@
                 "Output had Nothing type or 'None' annotation, but handle_output received"
                 f" value that was not None and was of type {type(obj)}.",
             )
             return None
 
         key = self._get_path(context)
 
-        if self._has_object(key):
-            self._rm_object(key)
-
         pickled_obj = pickle.dumps(obj, PICKLE_PROTOCOL)
         pickled_obj_bytes = io.BytesIO(pickled_obj)
         self._s3.upload_fileobj(
             pickled_obj_bytes,
             self._bucket,
             key,
         )
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/client.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             "io_type": io_type.value,
             # for back-compat
             "run_id": log_key[0],
             "key": log_key[-1],
         }
         if partial:
             params["partial"] = True
-        resp = self._instance.rest_requests_session.post(
+        resp = self._instance.requests_managed_retries_session.post(
             self._instance.dagster_cloud_gen_logs_url_url,
             params=params,
             headers=self._instance.dagster_cloud_api_headers(DagsterCloudInstanceScope.DEPLOYMENT),
             timeout=self._instance.dagster_cloud_api_timeout,
             proxies=self._instance.dagster_cloud_api_proxies,
         )
         raise_http_error(resp)
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/queries.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -349,15 +349,25 @@
     mutation StoreEvent($eventRecord: EventLogEntryInput!) {
         eventLogs {
             StoreEvent(eventRecord: $eventRecord) {
                 ok
             }
         }
     }
-    """
+"""
+
+STORE_EVENT_BATCH_MUTATION = """
+    mutation StoreEventBatch($eventRecords: [EventLogEntryInput!]!) {
+        eventLogs {
+            StoreEventBatch(eventRecords: $eventRecords) {
+                ok
+            }
+        }
+    }
+"""
 
 DELETE_EVENTS_MUTATION = """
     mutation DeleteEvents($runId: String!) {
         eventLogs {
             DeleteEvents(runId: $runId) {
                 ok
             }
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/storage.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
+import os
 from collections import defaultdict
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Mapping,
     Optional,
@@ -53,18 +55,24 @@
     ConcurrencyClaimStatus,
     ConcurrencyKeyInfo,
     ConcurrencySlotStatus,
     PendingStepInfo,
 )
 from dagster._utils.error import SerializableErrorInfo
 from dagster._utils.merger import merge_dicts
-from dagster_cloud_cli.core.errors import GraphQLStorageError
+from dagster_cloud_cli.core.errors import DagsterCloudAgentServerError
 from typing_extensions import Self
 
+from dagster_cloud.api.dagster_cloud_api import StoreEventBatchRequest
 from dagster_cloud.storage.event_logs.utils import truncate_event
+from dagster_cloud.util import compressed_namedtuple_upload_file
+
+if TYPE_CHECKING:
+    from dagster_cloud.instance import DagsterCloudAgentInstance
+
 
 from .queries import (
     ADD_DYNAMIC_PARTITIONS_MUTATION,
     CHECK_CONCURRENCY_CLAIM_QUERY,
     CLAIM_CONCURRENCY_SLOT_MUTATION,
     DELETE_CONCURRENCY_LIMIT_MUTATION,
     DELETE_DYNAMIC_PARTITION_MUTATION,
@@ -96,23 +104,38 @@
     HAS_ASSET_KEY_QUERY,
     HAS_DYNAMIC_PARTITION_QUERY,
     INITIALIZE_CONCURRENCY_LIMIT_MUTATION,
     IS_ASSET_AWARE_QUERY,
     IS_PERSISTENT_QUERY,
     REINDEX_MUTATION,
     SET_CONCURRENCY_SLOTS_MUTATION,
+    STORE_EVENT_BATCH_MUTATION,
     STORE_EVENT_MUTATION,
     UPDATE_ASSET_CACHED_STATUS_DATA_MUTATION,
     UPGRADE_EVENT_LOG_STORAGE_MUTATION,
     WIPE_ASSET_CACHED_STATUS_DATA_MUTATION,
     WIPE_ASSET_MUTATION,
     WIPE_EVENT_LOG_STORAGE_MUTATION,
 )
 
 
+def _input_for_event(event: EventLogEntry):
+    event = truncate_event(event)
+    return {
+        "errorInfo": _input_for_serializable_error_info(event.error_info),
+        "level": event.level,
+        "userMessage": event.user_message,
+        "runId": event.run_id,
+        "timestamp": event.timestamp,
+        "stepKey": event.step_key,
+        "pipelineName": event.job_name,
+        "dagsterEvent": _input_for_dagster_event(event.dagster_event),
+    }
+
+
 def _input_for_serializable_error_info(serializable_error_info: Optional[SerializableErrorInfo]):
     check.opt_inst_param(serializable_error_info, "serializable_error_info", SerializableErrorInfo)
 
     if serializable_error_info is None:
         return None
 
     return {
@@ -391,24 +414,27 @@
     def _graphql_client(self):
         return (
             self._override_graphql_client
             if self._override_graphql_client
             else self._instance.graphql_client
         )
 
+    @property
+    def agent_instance(self) -> "DagsterCloudAgentInstance":
+        from dagster_cloud.instance import DagsterCloudAgentInstance
+
+        return cast(DagsterCloudAgentInstance, self._instance)
+
     def _execute_query(self, query, variables=None, headers=None, idempotent_mutation=False):
-        res = self._graphql_client.execute(
+        return self._graphql_client.execute(
             query,
             variable_values=variables,
             headers=headers,
             idempotent_mutation=idempotent_mutation,
         )
-        if "errors" in res:
-            raise GraphQLStorageError(res)
-        return res
 
     def get_records_for_run(
         self,
         run_id: str,
         cursor: Optional[str] = None,
         of_type: Optional[Union[DagsterEventType, Set[DagsterEventType]]] = None,
         limit: Optional[int] = None,
@@ -505,37 +531,52 @@
                     deserialize_value(marker, RunStepMarker)
                     for marker in check.opt_list_elem(stats, "markers", of_type=str)
                 ],
             )
             for stats in step_stats
         ]
 
+    def _store_events_http(self, headers, events: Sequence[EventLogEntry]):
+        batch_request = StoreEventBatchRequest(event_log_entries=events)
+        with compressed_namedtuple_upload_file(batch_request) as f:
+            self.agent_instance.http_client.post(
+                url=self.agent_instance.dagster_cloud_store_events_url,
+                headers=headers,
+                files={"store_events.tmp": f},
+            )
+
     def store_event(self, event: EventLogEntry):
         check.inst_param(event, "event", EventLogEntry)
+        headers = {"Idempotency-Key": str(uuid4())}
 
-        event = truncate_event(event)
+        if os.getenv("DAGSTER_CLOUD_STORE_EVENT_OVER_HTTP"):
+            self._store_events_http(headers, [event])
+        else:
+            self._execute_query(
+                STORE_EVENT_MUTATION,
+                variables={
+                    "eventRecord": _input_for_event(event),
+                },
+                headers=headers,
+            )
 
+    def store_event_batch(self, events: Sequence[EventLogEntry]):
+        check.sequence_param(events, "events", of_type=EventLogEntry)
         headers = {"Idempotency-Key": str(uuid4())}
 
-        self._execute_query(
-            STORE_EVENT_MUTATION,
-            variables={
-                "eventRecord": {
-                    "errorInfo": _input_for_serializable_error_info(event.error_info),
-                    "level": event.level,
-                    "userMessage": event.user_message,
-                    "runId": event.run_id,
-                    "timestamp": event.timestamp,
-                    "stepKey": event.step_key,
-                    "pipelineName": event.job_name,
-                    "dagsterEvent": _input_for_dagster_event(event.dagster_event),
-                }
-            },
-            headers=headers,
-        )
+        if os.getenv("DAGSTER_CLOUD_STORE_EVENT_OVER_HTTP"):
+            self._store_events_http(headers, events)
+        else:
+            self._execute_query(
+                STORE_EVENT_BATCH_MUTATION,
+                variables={
+                    "eventRecords": [_input_for_event(event) for event in events],
+                },
+                headers=headers,
+            )
 
     def delete_events(self, run_id: str):
         self._execute_query(
             DELETE_EVENTS_MUTATION, variables={"runId": check.str_param(run_id, "run_id")}
         )
         return
 
@@ -798,18 +839,21 @@
         res = self._execute_query(
             GET_LATEST_ASSET_PARTITION_MATERIALIZATION_ATTEMPTS_WITHOUT_MATERIALIZATIONS,
             variables={
                 "assetKey": asset_key.to_string(),
                 "afterStorageId": after_storage_id,
             },
         )
-        return res["data"]["eventLogs"][
+        result = res["data"]["eventLogs"][
             "getLatestAssetPartitionMaterializationAttemptsWithoutMaterializations"
         ]
 
+        # Translate list to tuple
+        return {key: tuple(val) for key, val in result.items()}
+
     def get_event_tags_for_asset(
         self,
         asset_key: AssetKey,
         filter_tags: Optional[Mapping[str, str]] = None,
         filter_event_id: Optional[int] = None,
     ) -> Sequence[Mapping[str, str]]:
         check.inst_param(asset_key, "asset_key", AssetKey)
@@ -894,15 +938,15 @@
         result = res["data"]["eventLogs"]["InitializeConcurrencyLimit"]
         error = result.get("error")
 
         if error:
             if error["className"] == "DagsterInvalidInvocationError":
                 raise DagsterInvalidInvocationError(error["message"])
             else:
-                raise GraphQLStorageError(res)
+                raise DagsterCloudAgentServerError(res)
         return result.get("success")
 
     def set_concurrency_slots(self, concurrency_key: str, num: int) -> None:
         check.str_param(concurrency_key, "concurrency_key")
         check.int_param(num, "num")
         res = self._execute_query(
             SET_CONCURRENCY_SLOTS_MUTATION,
@@ -911,30 +955,30 @@
         result = res["data"]["eventLogs"]["SetConcurrencySlots"]
         error = result.get("error")
 
         if error:
             if error["className"] == "DagsterInvalidInvocationError":
                 raise DagsterInvalidInvocationError(error["message"])
             else:
-                raise GraphQLStorageError(res)
+                raise DagsterCloudAgentServerError(res)
         return res
 
     def delete_concurrency_limit(self, concurrency_key: str) -> None:
         check.str_param(concurrency_key, "concurrency_key")
         res = self._execute_query(
             DELETE_CONCURRENCY_LIMIT_MUTATION,
             variables={"concurrencyKey": concurrency_key},
         )
         result = res["data"]["eventLogs"]["DeleteConcurrencyLimit"]
         error = result.get("error")
         if error:
             if error["className"] == "DagsterInvalidInvocationError":
                 raise DagsterInvalidInvocationError(error["message"])
             else:
-                raise GraphQLStorageError(res)
+                raise DagsterCloudAgentServerError(res)
 
     def get_concurrency_keys(self) -> Set[str]:
         res = self._execute_query(GET_CONCURRENCY_KEYS_QUERY)
         return set(res["data"]["eventLogs"]["getConcurrencyKeys"])
 
     def get_concurrency_info(self, concurrency_key: str) -> ConcurrencyKeyInfo:
         check.str_param(concurrency_key, "concurrency_key")
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/event_logs/utils.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/runs/queries.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/runs/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             }
         }
     }
 """
 )
 
 GET_RUN_TAGS_QUERY = """
-    query getRunTagsQuery($jsonTagKeys: JSONString, $valuePrefix: String, $limit: Int) {
+    query getRunTagsQuery($jsonTagKeys: JSONString!, $valuePrefix: String, $limit: Int) {
         runs {
             getRunTags(jsonTagKeys: $jsonTagKeys, valuePrefix: $valuePrefix, limit: $limit) {
                 key
                 values
             }
         }
     }
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/runs/storage.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/runs/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     DagsterInvariantViolationError,
     DagsterRunAlreadyExists,
     DagsterRunNotFoundError,
     DagsterSnapshotDoesNotExist,
 )
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
-from dagster._core.host_representation.origin import ExternalJobOrigin
+from dagster._core.remote_representation.origin import RemoteJobOrigin
 from dagster._core.snap import (
     ExecutionPlanSnapshot,
     JobSnapshot,
     create_execution_plan_snapshot_id,
     create_job_snapshot_id,
 )
 from dagster._core.storage.dagster_run import (
@@ -43,15 +43,15 @@
     ConfigurableClass,
     ConfigurableClassData,
     deserialize_value,
     serialize_value,
 )
 from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.merger import merge_dicts
-from dagster_cloud_cli.core.errors import GraphQLStorageError
+from dagster_cloud_cli.core.errors import DagsterCloudAgentServerError
 from typing_extensions import Self
 
 from .queries import (
     ADD_BACKFILL_MUTATION,
     ADD_DAEMON_HEARTBEAT_MUTATION,
     ADD_EXECUTION_PLAN_SNAPSHOT_MUTATION,
     ADD_PIPELINE_SNAPSHOT_MUTATION,
@@ -168,20 +168,17 @@
         return (
             self._override_graphql_client
             if self._override_graphql_client
             else self._instance.graphql_client
         )
 
     def _execute_query(self, query, variables=None, idempotent_mutation=False):
-        res = self._graphql_client.execute(
+        return self._graphql_client.execute(
             query, variable_values=variables, idempotent_mutation=idempotent_mutation
         )
-        if "errors" in res:
-            raise GraphQLStorageError(res)
-        return res
 
     def add_run(self, dagster_run: DagsterRun):
         check.inst_param(dagster_run, "dagster_run", DagsterRun)
         res = self._execute_query(
             ADD_RUN_MUTATION,
             variables={"serializedPipelineRun": serialize_value(dagster_run)},
         )
@@ -192,15 +189,15 @@
         # Special-case some errors to match the RunStorage API
         if error:
             if error["className"] == "DagsterRunAlreadyExists":
                 raise DagsterRunAlreadyExists(error["message"])
             if error["className"] == "DagsterSnapshotDoesNotExist":
                 raise DagsterSnapshotDoesNotExist(error["message"])
             else:
-                raise GraphQLStorageError(res)
+                raise DagsterCloudAgentServerError(res)
 
         return dagster_run
 
     def handle_run_event(self, run_id: str, event: DagsterEvent):
         # no-op, handled by store_event
         pass
 
@@ -301,26 +298,22 @@
                 "bucketBy": _get_bucket_input(bucket_by),
             },
         )
         return [_run_record_from_graphql(record) for record in res["data"]["runs"]["getRunRecords"]]
 
     def get_run_tags(
         self,
-        tag_keys: Optional[Sequence[str]] = None,
+        tag_keys: Sequence[str],
         value_prefix: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> Sequence[Tuple[str, Set[str]]]:
         res = self._execute_query(
             GET_RUN_TAGS_QUERY,
             variables={
-                "jsonTagKeys": (
-                    json.dumps(check.list_param(tag_keys, "tag_keys", of_type=str))
-                    if tag_keys
-                    else None
-                ),
+                "jsonTagKeys": (json.dumps(check.list_param(tag_keys, "tag_keys", of_type=str))),
                 "valuePrefix": check.opt_str_param(value_prefix, "value_prefix"),
                 "limit": check.opt_int_param(limit, "limit"),
             },
         )
         return [
             (run_tag["key"], set(run_tag["values"]))
             for run_tag in res["data"]["runs"]["getRunTags"]
@@ -513,15 +506,15 @@
     def get_cursor_values(self, keys: Set[str]):
         return NotImplementedError("KVS is not supported from the user cloud")
 
     def set_cursor_values(self, pairs: Mapping[str, str]):
         return NotImplementedError("KVS is not supported from the user cloud")
 
     # Migrating run history
-    def replace_job_origin(self, run: DagsterRun, job_origin: ExternalJobOrigin):
+    def replace_job_origin(self, run: DagsterRun, job_origin: RemoteJobOrigin):
         self._execute_query(
             MUTATE_JOB_ORIGIN,
             variables={
                 "runId": run.run_id,
                 "serializedJobOrigin": serialize_value(job_origin),
             },
         )
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/schedules/queries.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/storage/schedules/storage.py` & `dagster-cloud-1.7.0/dagster_cloud/storage/schedules/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from dagster._core.storage.schedules.base import ScheduleStorage
 from dagster._serdes import (
     ConfigurableClass,
     ConfigurableClassData,
     deserialize_value,
     serialize_value,
 )
-from dagster_cloud_cli.core.errors import GraphQLStorageError
 from typing_extensions import Self
 
 from .queries import (
     ADD_JOB_STATE_MUTATION,
     ALL_STORED_JOB_STATE_QUERY,
     CREATE_JOB_TICK_MUTATION,
     GET_JOB_STATE_QUERY,
@@ -63,18 +62,15 @@
         return (
             self._override_graphql_client
             if self._override_graphql_client
             else self._instance.graphql_client
         )
 
     def _execute_query(self, query, variables=None):
-        res = self._graphql_client.execute(query, variable_values=variables)
-        if "errors" in res:
-            raise GraphQLStorageError(res)
-        return res
+        return self._graphql_client.execute(query, variable_values=variables)
 
     def wipe(self):
         raise Exception("Not allowed to wipe from user cloud")
 
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/util/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import zlib
 from collections import namedtuple
-from typing import Any, Dict, List, Mapping
+from contextlib import contextmanager
+from io import BytesIO
+from typing import Any, Dict, List, Mapping, NamedTuple
 
 from dagster import (
     Field,
     _check as check,
 )
 from dagster._config import BoolSourceType, IntSourceType, StringSourceType
+from dagster._serdes import serialize_value
 from dagster._serdes.utils import create_snapshot_id
 
 
 class SerializableNamedtupleMapDiff(
     namedtuple(
         "_SerializableNamedtupleMapDiff",
         "to_add to_update to_remove",
@@ -77,7 +81,14 @@
 
 
 def keys_not_none(
     keys: List[str],
     dictionary: Mapping[str, Any],
 ) -> bool:
     return all(key in dictionary and dictionary[key] is not None for key in keys)
+
+
+@contextmanager
+def compressed_namedtuple_upload_file(to_serialize: NamedTuple):
+    compressed_data = zlib.compress(serialize_value(to_serialize).encode("utf-8"))
+    with BytesIO(compressed_data) as f:
+        yield f
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/util/container_resources.py` & `dagster-cloud-1.7.0/dagster_cloud/util/container_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/docker.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/ecs.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,19 @@
                 "key": Field(StringSource, is_required=True),
                 "value": Field(StringSource, is_required=False),
             }
         ),
         is_required=False,
         description="Additional tags to apply to the launched ECS task for a code server.",
     ),
+    "server_health_check": Field(
+        Permissive(),
+        is_required=False,
+        description="Health check to include in code server task definitions.",
+    ),
 }
 
 
 ECS_CONTAINER_CONTEXT_CONFIG = {
     "secrets": Field(
         Noneable(Array(Shape({"name": StringSource, "valueFrom": StringSource}))),
         is_required=False,
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/docker/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/docker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     _check as check,
 )
 from dagster._core.utils import parse_env_var
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
 from dagster._utils import find_free_port
 from dagster._utils.merger import merge_dicts
-from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 from dagster_docker import DockerRunLauncher
 from dagster_docker.container_context import DockerContainerContext
+from dateutil.parser import parse
 from docker.models.containers import Container
 from typing_extensions import Self
 
 from dagster_cloud.api.dagster_cloud_api import UserCodeDeploymentType
 from dagster_cloud.execution.monitoring import CloudContainerResourceLimits
 from dagster_cloud.workspace.user_code_launcher.user_code_launcher import UserCodeLauncherEntry
 
@@ -34,14 +34,16 @@
 )
 from ..user_code_launcher.utils import deterministic_label_for_location
 from .utils import unique_docker_resource_name
 
 GRPC_SERVER_LABEL = "dagster_grpc_server"
 MULTIPEX_SERVER_LABEL = "dagster_multipex_server"
 AGENT_LABEL = "dagster_agent_id"
+SERVER_TIMESTAMP_LABEL = "dagster_server_timestamp"
+
 
 IMAGE_PULL_LOG_INTERVAL = 15
 
 
 class DagsterDockerContainer(NamedTuple):
     """We use __str__ on server handles to serialize them to the run tags. Wrap the docker container
     object so that we can serialize it to a string.
@@ -257,16 +259,17 @@
         # Empty because we don't currently internally monitor docker deployment resource usage.
         return {}
 
     def _start_new_server_spinup(
         self,
         deployment_name: str,
         location_name: str,
-        metadata: CodeDeploymentMetadata,
+        desired_entry: UserCodeLauncherEntry,
     ) -> DagsterCloudGrpcServer:
+        metadata = desired_entry.code_deployment_metadata
         container_name = unique_docker_resource_name(deployment_name, location_name)
 
         container_context = DockerContainerContext(
             registry=None,
             env_vars=self.env_vars
             + [f"{k}={v}" for k, v in (metadata.cloud_context_env or {}).items()],
             networks=self._networks,
@@ -290,26 +293,28 @@
                 metrics_enabled=self._instance.user_code_launcher.code_server_metrics_enabled,
             )
             environment = metadata.get_multipex_server_env()
             labels = {
                 MULTIPEX_SERVER_LABEL: "",
                 deterministic_label_for_location(deployment_name, location_name): "",
                 AGENT_LABEL: self._instance.instance_uuid,
+                SERVER_TIMESTAMP_LABEL: str(desired_entry.update_timestamp),
             }
         else:
             command = metadata.get_grpc_server_command(
                 metrics_enabled=self._instance.user_code_launcher.code_server_metrics_enabled
             )
             environment = metadata.get_grpc_server_env(
                 grpc_port, location_name, self._instance.ref_for_deployment(deployment_name)
             )
             labels = {
                 GRPC_SERVER_LABEL: "",
                 deterministic_label_for_location(deployment_name, location_name): "",
                 AGENT_LABEL: self._instance.instance_uuid,
+                SERVER_TIMESTAMP_LABEL: str(desired_entry.update_timestamp),
             }
 
         container, server_endpoint = self._launch_container(
             deployment_name,
             location_name,
             container_name,
             hostname,
@@ -347,14 +352,18 @@
             self._logger.error(f"Failure stopping container {container.id}: {sys.exc_info()}")
         container.remove(force=True)
         self._logger.info(f"Removed container {container.id}")
 
     def get_agent_id_for_server(self, handle: DagsterDockerContainer) -> Optional[str]:
         return handle.container.labels.get(AGENT_LABEL)
 
+    def get_server_create_timestamp(self, handle: DagsterDockerContainer) -> Optional[float]:
+        created_time_str = handle.container.attrs["Created"]
+        return parse(created_time_str).timestamp()
+
     def _list_server_handles(self) -> List[DagsterDockerContainer]:
         client = docker.client.from_env()
         return [
             DagsterDockerContainer(container=container)
             for container in client.containers.list(all=True, filters={"label": GRPC_SERVER_LABEL})
         ] + [
             DagsterDockerContainer(container=container)
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/client.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 from dagster_cloud.workspace.ecs.service import Service
 
 DEFAULT_ECS_TIMEOUT = 300
 DEFAULT_ECS_GRACE_PERIOD = 30
 
 STOPPED_TASK_GRACE_PERIOD = 30
 
+
+ECS_EXEC_LINUX_PARAMETERS = {
+    "capabilities": {"add": ["SYS_PTRACE"]},
+    "initProcessEnabled": True,
+}
+
 config = Config(retries={"max_attempts": 50, "mode": "standard"})
 
 
 def get_debug_ecs_prompt(cluster: str, task_arn: str) -> str:
     return (
         "For more information about the failure, check the ECS console for logs for task"
         f" {task_arn} in cluster {cluster}."
@@ -137,14 +143,16 @@
         cpu=None,
         memory=None,
         ephemeral_storage=None,
         repository_credentials=None,
         runtime_platform=None,
         mount_points=None,
         volumes=None,
+        linux_parameters=None,
+        health_check=None,
     ):
         container_name = container_name or family
 
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
         env = env or {}
         environment = [{"name": key, "value": value} for key, value in env.items()]
@@ -175,14 +183,16 @@
             cpu=cpu,
             memory=memory,
             ephemeral_storage=ephemeral_storage,
             repository_credentials=repository_credentials,
             runtime_platform=runtime_platform,
             mount_points=mount_points,
             volumes=volumes,
+            linux_parameters=linux_parameters,
+            health_check=health_check,
         )
 
         try:
             existing_task_definition = self.ecs.describe_task_definition(taskDefinition=family)[
                 "taskDefinition"
             ]
         except ClientError:
@@ -227,14 +237,15 @@
         ephemeral_storage=None,
         replica_count=None,
         repository_credentials=None,
         allow_ecs_exec=False,
         runtime_platform=None,
         mount_points=None,
         volumes=None,
+        health_check=None,
     ):
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
         service_name = name
         family = family or name
 
         logger.info(f"Checking if task definition {family} for {name} can be re-used...")
@@ -253,14 +264,16 @@
             cpu=cpu,
             memory=memory,
             ephemeral_storage=ephemeral_storage,
             repository_credentials=repository_credentials,
             runtime_platform=runtime_platform,
             mount_points=mount_points,
             volumes=volumes,
+            linux_parameters=ECS_EXEC_LINUX_PARAMETERS if allow_ecs_exec else None,
+            health_check=health_check,
         )
 
         service_registry_arn = None
         # Configure service discovery
         if register_service_discovery:
             logger.info(f"Creating service registry for {service_name}...")
             service_registry_arn = self._create_service_registry(
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/launcher.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,29 @@
     StringSource,
     _check as check,
 )
 from dagster._serdes import ConfigurableClass, ConfigurableClassData
 from dagster._utils.merger import merge_dicts
 from dagster_aws.ecs.container_context import EcsContainerContext
 from dagster_aws.secretsmanager import get_secrets_from_arns
-from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 
 from dagster_cloud.api.dagster_cloud_api import (
     UserCodeDeploymentType,
 )
 from dagster_cloud.execution.monitoring import CloudContainerResourceLimits
 from dagster_cloud.pex.grpc.types import (
     GetCrashedPexServersArgs,
 )
 from dagster_cloud.workspace.config_schema import SHARED_ECS_CONFIG
-from dagster_cloud.workspace.ecs.client import DEFAULT_ECS_GRACE_PERIOD, DEFAULT_ECS_TIMEOUT, Client
+from dagster_cloud.workspace.ecs.client import (
+    DEFAULT_ECS_GRACE_PERIOD,
+    DEFAULT_ECS_TIMEOUT,
+    ECS_EXEC_LINUX_PARAMETERS,
+    Client,
+)
 from dagster_cloud.workspace.ecs.service import Service
 from dagster_cloud.workspace.ecs.utils import get_ecs_human_readable_label, unique_ecs_resource_name
 from dagster_cloud.workspace.user_code_launcher import (
     DEFAULT_SERVER_PROCESS_STARTUP_TIMEOUT,
     SHARED_USER_CODE_LAUNCHER_CONFIG,
     DagsterCloudGrpcServer,
     DagsterCloudUserCodeLauncher,
@@ -74,14 +78,15 @@
         runtime_platform: Optional[Mapping[str, Any]] = None,
         mount_points: Optional[Sequence[Mapping[str, Any]]] = None,
         volumes: Optional[Sequence[Mapping[str, Any]]] = None,
         server_sidecar_containers: Optional[Sequence[Mapping[str, Any]]] = None,
         run_sidecar_containers: Optional[Sequence[Mapping[str, Any]]] = None,
         server_ecs_tags: Optional[Sequence[Mapping[str, Optional[str]]]] = None,
         run_ecs_tags: Optional[Sequence[Mapping[str, Optional[str]]]] = None,
+        server_health_check: Optional[Mapping[str, Any]] = None,
         **kwargs,
     ):
         self.ecs = boto3.client("ecs")
         self.logs = boto3.client("logs")
         self.service_discovery = boto3.client("servicediscovery")
         self.secrets_manager = boto3.client("secretsmanager")
 
@@ -134,14 +139,18 @@
         self.run_sidecar_containers = check.opt_sequence_param(
             run_sidecar_containers, "run_sidecar_containers"
         )
 
         self.server_ecs_tags = check.opt_sequence_param(server_ecs_tags, "server_ecs_tags")
         self.run_ecs_tags = check.opt_sequence_param(run_ecs_tags, "run_ecs_tags")
 
+        self.server_health_check = check.opt_mapping_param(
+            server_health_check, "server_health_check"
+        )
+
         self.client = Client(
             cluster_name=self.cluster,
             subnet_ids=self.subnets,
             security_group_ids=security_group_ids,
             service_discovery_namespace_id=self.service_discovery_namespace_id,
             log_group=self.log_group,
             show_debug_cluster_info=self.show_debug_cluster_info,
@@ -333,33 +342,43 @@
             "ecs": {
                 "cpu_limit": resources.get("cpu"),
                 "memory_limit": resources.get("memory"),
             }
         }
 
     def _start_new_server_spinup(
-        self, deployment_name: str, location_name: str, metadata: CodeDeploymentMetadata
+        self,
+        deployment_name: str,
+        location_name: str,
+        desired_entry: UserCodeLauncherEntry,
     ) -> DagsterCloudGrpcServer:
+        metadata = desired_entry.code_deployment_metadata
+
         if metadata.pex_metadata:
             command = metadata.get_multipex_server_command(
                 PORT, metrics_enabled=self._instance.user_code_launcher.code_server_metrics_enabled
             )
             additional_env = metadata.get_multipex_server_env()
             tags = {
                 "dagster/multipex_server": "1",
                 "dagster/agent_id": self._instance.instance_uuid,
+                "dagster/server_timestamp": str(desired_entry.update_timestamp),
             }
         else:
             command = metadata.get_grpc_server_command(
                 metrics_enabled=self._instance.user_code_launcher.code_server_metrics_enabled
             )
             additional_env = metadata.get_grpc_server_env(
                 PORT, location_name, self._instance.ref_for_deployment(deployment_name)
             )
-            tags = {"dagster/grpc_server": "1", "dagster/agent_id": self._instance.instance_uuid}
+            tags = {
+                "dagster/grpc_server": "1",
+                "dagster/agent_id": self._instance.instance_uuid,
+                "dagster/server_timestamp": str(desired_entry.update_timestamp),
+            }
 
         container_context = EcsContainerContext(
             secrets=self.secrets,
             secrets_tags=[self.secrets_tag] if self.secrets_tag else [],
             env_vars=self.env_vars
             + [f"{k}={v}" for k, v in (metadata.cloud_context_env or {}).items()],
             server_resources=self.server_resources,
@@ -369,14 +388,15 @@
             runtime_platform=self.runtime_platform,
             mount_points=self.mount_points,
             volumes=self.volumes,
             server_sidecar_containers=self.server_sidecar_containers,
             run_sidecar_containers=self.run_sidecar_containers,
             server_ecs_tags=self.server_ecs_tags,
             run_ecs_tags=self.run_ecs_tags,
+            server_health_check=self.server_health_check,
         ).merge(EcsContainerContext.create_from_config(metadata.container_context))
 
         # disallow multiple replicas for code locations acting as pex servers
         if metadata.pex_metadata:
             replica_count = (
                 metadata.container_context.get("ecs", {})
                 .get("server_resources", {})
@@ -439,19 +459,18 @@
             repository_credentials=self._get_service_repository_credentials_override(
                 container_context
             ),
             allow_ecs_exec=self._get_enable_ecs_exec(),
             runtime_platform=container_context.runtime_platform,
             mount_points=container_context.mount_points,
             volumes=container_context.volumes,
+            health_check=container_context.server_health_check,
         )
         self._logger.info(
-            "Created a new service at hostname {} for {}:{}, waiting for server to be ready...".format(
-                service.hostname, deployment_name, location_name
-            )
+            f"Created a new service at hostname {service.hostname} for {deployment_name}:{location_name}, waiting for server to be ready..."
         )
 
         endpoint = ServerEndpoint(
             host=service.hostname,
             port=PORT,
             socket=None,
         )
@@ -623,14 +642,17 @@
             if "dagster/location_name" in service.tags.keys()
         ]
 
     def get_agent_id_for_server(self, handle: EcsServerHandleType) -> Optional[str]:
         # Need to get container for server handle, then get the agent tag from that.
         return handle.tags.get("dagster/agent_id")
 
+    def get_server_create_timestamp(self, handle: EcsServerHandleType) -> Optional[float]:
+        return handle.create_timestamp
+
     def _run_launcher_kwargs(self) -> Dict[str, Any]:
         return dict(
             task_definition={
                 "log_group": self.log_group,
                 "execution_role_arn": self.execution_role_arn,
                 "requires_compatibilities": [self.launch_type],
                 **({"task_role_arn": self.task_role_arn} if self.task_role_arn else {}),
@@ -638,23 +660,29 @@
                     {"sidecar_containers": self.run_sidecar_containers}
                     if self.run_sidecar_containers
                     else {}
                 ),
                 **({"runtime_platform": self.runtime_platform} if self.runtime_platform else {}),
                 **({"mount_points": self.mount_points} if self.mount_points else {}),
                 **({"volumes": self.volumes} if self.volumes else {}),
+                **(
+                    {"linux_parameters": ECS_EXEC_LINUX_PARAMETERS}
+                    if self._get_enable_ecs_exec()
+                    else {}
+                ),
             },
             secrets=self.secrets,
             secrets_tag=self.secrets_tag,
             env_vars=self.env_vars,
             use_current_ecs_task_config=False,
             run_task_kwargs={
                 "cluster": self.cluster,
                 "networkConfiguration": self.client.network_configuration,
                 "launchType": self.launch_type,
+                **({"enableExecuteCommand": True} if self._get_enable_ecs_exec() else {}),
             },
             run_ecs_tags=self.run_ecs_tags,
             container_name=CONTAINER_NAME,
             run_resources=self.run_resources,
         )
 
     def run_launcher(self) -> CloudEcsRunLauncher:
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/service.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Optional
 
 from dagster._utils.cached_method import cached_method
 
 
 class Service:
     def __init__(self, client, arn):
         self.client = client
@@ -72,27 +73,23 @@
                 eni_id = detail.get("value")
                 eni = self.client.ec2.NetworkInterface(eni_id)
                 if eni.association_attribute:
                     return eni.association_attribute.get("PublicIp")
 
     @property
     @cached_method
-    def created_at(self):
-        task_arns = self.client.ecs.list_tasks(
-            cluster=self.client.cluster_name,
-            serviceName=self.name,
-        ).get("taskArns")
+    def create_timestamp(self) -> Optional[float]:
+        response = self.client.ecs.describe_services(
+            cluster=self.client.cluster_name, services=[self.name]
+        )
 
-        # Assume there's only one task per service
-        task = self.client.ecs.describe_tasks(
-            cluster=self.client.cluster_name,
-            tasks=task_arns,
-        ).get("tasks")[0]
+        service_description = response["services"][0]
 
-        return task.get("createdAt")
+        # Extract the creation timestamp
+        return service_description["createdAt"].timestamp()
 
     @property
     @cached_method
     def environ(self):
         task_arns = self.client.ecs.list_tasks(
             cluster=self.client.cluster_name,
             serviceName=self.name,
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/ecs/utils.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/ecs/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
 import re
 from typing import Optional
 
-from dagster._core.host_representation.origin import ExternalJobOrigin
+from dagster._core.remote_representation.origin import RemoteJobOrigin
 from dagster_aws.ecs.utils import sanitize_family
 
 from ..user_code_launcher.utils import get_human_readable_label, unique_resource_name
 
 
 def unique_ecs_resource_name(deployment_name, location_name):
     return unique_resource_name(
@@ -51,22 +51,22 @@
 
     return sanitize_family(final_family)
 
 
 def get_run_task_definition_family(
     organization_name: Optional[str],
     deployment_name: str,
-    job_origin: ExternalJobOrigin,
+    job_origin: RemoteJobOrigin,
 ) -> str:
     # Truncate the location name if it's too long (but add a unique suffix at the end so that no matter what it's unique)
     # Relies on the fact that org name and deployment name are always <= 64 characters long to
     # stay well underneath the 255 character limit imposed by ECS
     job_name = job_origin.job_name
-    repo_name = job_origin.external_repository_origin.repository_name
-    location_name = job_origin.external_repository_origin.code_location_origin.location_name
+    repo_name = job_origin.repository_origin.repository_name
+    location_name = job_origin.repository_origin.code_location_origin.location_name
 
     assert len(str(organization_name)) <= 64
     assert len(deployment_name) <= 64
 
     # '{16}_{64}_{64}_{32}_{32}_{32}': max 245 characters
 
     final_family = f"run_{organization_name}_{deployment_name}_{_get_family_hash(location_name)}_{_get_family_hash(repo_name)}_{_get_family_hash(job_name)}"
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from collections import defaultdict
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Collection, Dict, List, NamedTuple, Optional, Set, Tuple, cast
+from typing import Any, Collection, Dict, List, Mapping, NamedTuple, Optional, Set, Tuple
 
 import kubernetes
 import kubernetes.client as client
 from dagster import (
     Array,
     Field,
     IntSource,
@@ -20,15 +20,14 @@
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
 from dagster._utils.merger import merge_dicts
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 from dagster_k8s.container_context import K8sContainerContext
 from dagster_k8s.job import UserDefinedDagsterK8sConfig
 from dagster_k8s.models import k8s_snake_case_dict
-from kubernetes.client.models.v1_deployment_list import V1DeploymentList
 from kubernetes.client.rest import ApiException
 from typing_extensions import Self
 
 from dagster_cloud.api.dagster_cloud_api import (
     UserCodeDeploymentType,
 )
 from dagster_cloud.constants import RESERVED_ENV_VAR_NAMES
@@ -58,14 +57,16 @@
 
 from ..config_schema.kubernetes import SHARED_K8S_CONFIG
 
 
 class K8sHandle(NamedTuple):
     namespace: str
     name: str
+    labels: Mapping[str, str]
+    creation_timestamp: Optional[float]
 
     def __str__(self):
         return f"{self.namespace}/{self.name}"
 
 
 class K8sUserCodeLauncher(DagsterCloudUserCodeLauncher[K8sHandle], ConfigurableClass):
     def __init__(
@@ -392,67 +393,73 @@
                 "cpu_request": resources.get("requests", {}).get("cpu"),
                 "memory_limit": resources.get("limits", {}).get("memory"),
                 "memory_request": resources.get("requests", {}).get("memory"),
             }
         }
 
     def _start_new_server_spinup(
-        self, deployment_name: str, location_name: str, metadata: CodeDeploymentMetadata
+        self,
+        deployment_name: str,
+        location_name: str,
+        desired_entry: UserCodeLauncherEntry,
     ) -> DagsterCloudGrpcServer:
+        metadata = desired_entry.code_deployment_metadata
+
         args = metadata.get_grpc_server_command(
             metrics_enabled=self._instance.user_code_launcher.code_server_metrics_enabled
         )
 
         resource_name = unique_k8s_resource_name(deployment_name, location_name)
 
         container_context = self._resolve_container_context(metadata)
 
+        deployment_reponse = None
+
         try:
             with self._get_apps_api_instance() as api_instance:
-                api_response = api_instance.create_namespaced_deployment(
+                deployment_reponse = api_instance.create_namespaced_deployment(
                     container_context.namespace,
                     body=construct_code_location_deployment(
                         self._instance,
                         deployment_name,
                         location_name,
                         resource_name,
                         metadata,
                         container_context,
                         args=args,
+                        server_timestamp=desired_entry.update_timestamp,
                     ),
                 )
             self._logger.info(
-                "Created deployment {} in namespace {}".format(
-                    api_response.metadata.name,
-                    container_context.namespace,
-                )
+                f"Created deployment {deployment_reponse.metadata.name} in namespace {container_context.namespace}"
             )
         except ApiException as e:
             self._logger.error(
                 "Exception when calling AppsV1Api->create_namespaced_deployment: %s\n" % e
             )
             raise e
 
         namespace = check.not_none(container_context.namespace)
 
         self._used_namespaces[(deployment_name, location_name)].add(namespace)
 
         try:
-            api_response = self._get_core_api_client().create_namespaced_service(
+            service_response = self._get_core_api_client().create_namespaced_service(
                 namespace,
                 construct_code_location_service(
                     deployment_name,
                     location_name,
                     resource_name,
                     container_context,
                     self._instance,
+                    server_timestamp=desired_entry.update_timestamp,
                 ),
             )
             self._logger.info(
-                f"Created service {api_response.metadata.name} in namespace {namespace}"
+                f"Created service {service_response.metadata.name} in namespace {namespace}"
             )
         except ApiException as e:
             self._logger.error(
                 "Exception when calling AppsV1Api->create_namespaced_service: %s\n" % e
             )
             raise e
 
@@ -462,15 +469,24 @@
         endpoint = ServerEndpoint(
             host=host,
             port=SERVICE_PORT,
             socket=None,
         )
 
         return DagsterCloudGrpcServer(
-            K8sHandle(namespace=namespace, name=resource_name), endpoint, metadata
+            K8sHandle(
+                namespace=namespace,
+                name=resource_name,
+                labels=deployment_reponse.metadata.labels,
+                creation_timestamp=deployment_reponse.metadata.creation_timestamp.timestamp()
+                if deployment_reponse.metadata.creation_timestamp
+                else None,
+            ),
+            endpoint,
+            metadata,
         )
 
     def _get_timeout_debug_info(
         self,
         server_handle,
     ):
         core_api = self._get_core_api_client()
@@ -536,15 +552,24 @@
                 deployments = api_instance.list_namespaced_deployment(
                     namespace,
                     label_selector=(
                         f"location_hash={deterministic_label_for_location(deployment_name, location_name)},agent_id={self._instance.instance_uuid}"
                     ),
                 ).items
                 for deployment in deployments:
-                    handles.append(K8sHandle(namespace=namespace, name=deployment.metadata.name))
+                    handles.append(
+                        K8sHandle(
+                            namespace=namespace,
+                            name=deployment.metadata.name,
+                            labels=deployment.metadata.labels,
+                            creation_timestamp=deployment.metadata.creation_timestamp.timestamp()
+                            if deployment.metadata.creation_timestamp
+                            else None,
+                        )
+                    )
 
         return handles
 
     def _list_server_handles(self) -> List[K8sHandle]:
         namespaces: Set[str] = set()
         if self._namespace:
             namespaces.add(self._namespace)
@@ -555,35 +580,32 @@
         with self._get_apps_api_instance() as api_instance:
             for namespace in namespaces:
                 deployments = api_instance.list_namespaced_deployment(
                     namespace,
                     label_selector="managed_by=K8sUserCodeLauncher",
                 ).items
                 for deployment in deployments:
-                    handles.append(K8sHandle(namespace, deployment.metadata.name))
+                    handles.append(
+                        K8sHandle(
+                            namespace,
+                            deployment.metadata.name,
+                            deployment.metadata.labels,
+                            deployment.metadata.creation_timestamp.timestamp()
+                            if deployment.metadata.creation_timestamp
+                            else None,
+                        )
+                    )
         self._logger.info(f"Listing server handles: {handles}")
         return handles
 
     def get_agent_id_for_server(self, handle: K8sHandle) -> Optional[str]:
-        with self._get_apps_api_instance() as api_instance:
-            deployments = cast(
-                V1DeploymentList,
-                api_instance.list_namespaced_deployment(
-                    handle.namespace,
-                    label_selector="managed_by=K8sUserCodeLauncher",
-                    field_selector=f"metadata.name={handle.name}",
-                ),
-            ).items
-            if not deployments:
-                self._logger.warning(
-                    f"Attempted to retrieve agent_id for server with handle {handle}; but no"
-                    " deployments found."
-                )
-                return None
-            return deployments.pop().metadata.labels.get("agent_id")
+        return handle.labels.get("agent_id")
+
+    def get_server_create_timestamp(self, handle: K8sHandle) -> Optional[float]:
+        return handle.creation_timestamp
 
     def _remove_server_handle(self, server_handle: K8sHandle) -> None:
         # Since we track which servers to delete by listing the k8s deployments,
         # delete the k8s service first to ensure that it can't be left dangling
         try:
             self._get_core_api_client().delete_namespaced_service(
                 server_handle.name, server_handle.namespace
@@ -606,17 +628,15 @@
                     self._logger.exception(
                         f"Tried to delete deployment {server_handle.name} but it was not found"
                     )
                 else:
                     raise
 
         self._logger.info(
-            "Removed deployment and service {} in namespace {}".format(
-                server_handle.name, server_handle.namespace
-            )
+            f"Removed deployment and service {server_handle.name} in namespace {server_handle.namespace}"
         )
 
     def __exit__(self, exception_type, exception_value, traceback):
         super().__exit__(exception_value, exception_value, traceback)
         self._launcher.dispose()
 
     def run_launcher(self):
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/kubernetes/utils.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import copy
 import re
 import time
 from typing import Mapping, Optional
 
 import kubernetes
-from dagster._utils.merger import merge_dicts
 from dagster_k8s.client import DagsterKubernetesClient
 from dagster_k8s.models import k8s_model_from_dict
 from kubernetes import client
 
 from dagster_cloud.instance import DagsterCloudAgentInstance
 
 from ..user_code_launcher.utils import (
@@ -18,22 +17,26 @@
 )
 
 MANAGED_RESOURCES_LABEL = {"managed_by": "K8sUserCodeLauncher"}
 SERVICE_PORT = 4000
 
 
 def _get_dagster_k8s_labels(
-    deployment_name: str, location_name: str, instance: DagsterCloudAgentInstance
+    deployment_name: str,
+    location_name: str,
+    instance: DagsterCloudAgentInstance,
+    server_timestamp: float,
 ) -> Mapping[str, str]:
     return {
         **MANAGED_RESOURCES_LABEL,
         "location_hash": deterministic_label_for_location(deployment_name, location_name),
         "location_name": get_k8s_human_readable_label(location_name),
         "deployment_name": get_k8s_human_readable_label(deployment_name),
         "agent_id": instance.instance_uuid,
+        "server_timestamp": str(server_timestamp),
     }
 
 
 def _sanitize_k8s_resource_name(name):
     filtered_name = re.sub("[^a-z0-9-]", "", name.lower())
 
     # ensure it doesn't start with a non-alpha character
@@ -69,24 +72,31 @@
         sanitize_fn=lambda name: (
             re.sub("[^a-zA-Z0-9-_.]", "", name).strip("-").strip("_").strip(".")
         ),
     )
 
 
 def construct_code_location_service(
-    deployment_name, location_name, service_name, container_context, instance
+    deployment_name,
+    location_name,
+    service_name,
+    container_context,
+    instance,
+    server_timestamp: float,
 ):
     labels = container_context.labels
 
     return client.V1Service(
         metadata=client.V1ObjectMeta(
             name=service_name,
             labels={
                 **labels,
-                **_get_dagster_k8s_labels(deployment_name, location_name, instance),
+                **_get_dagster_k8s_labels(
+                    deployment_name, location_name, instance, server_timestamp
+                ),
             },
         ),
         spec=client.V1ServiceSpec(
             selector={"user-deployment": service_name},
             ports=[client.V1ServicePort(name="grpc", protocol="TCP", port=SERVICE_PORT)],
         ),
     )
@@ -96,107 +106,71 @@
     instance,
     deployment_name,
     location_name,
     k8s_deployment_name,
     metadata,
     container_context,
     args,
+    server_timestamp: float,
 ):
-    pull_policy = container_context.image_pull_policy
-    env_config_maps = container_context.env_config_maps
-    env_secrets = container_context.env_secrets
-    service_account_name = container_context.service_account_name
-    image_pull_secrets = container_context.image_pull_secrets
-    volume_mounts = container_context.volume_mounts
-
-    volumes = container_context.volumes
-    resources = container_context.resources
-
-    scheduler_name = container_context.scheduler_name
-    security_context = container_context.security_context
-
-    env = merge_dicts(
-        metadata.get_grpc_server_env(
-            SERVICE_PORT, location_name, instance.ref_for_deployment(deployment_name)
-        ),
-        container_context.get_environment_dict(),
+    env = metadata.get_grpc_server_env(
+        SERVICE_PORT, location_name, instance.ref_for_deployment(deployment_name)
     )
 
     user_defined_config = container_context.server_k8s_config
 
     container_config = copy.deepcopy(user_defined_config.container_config)
 
-    container_config["args"] = args
-
-    if pull_policy:
-        container_config["image_pull_policy"] = pull_policy
-
     user_defined_env_vars = container_config.pop("env", [])
-    user_defined_env_from = container_config.pop("env_from", [])
-    user_defined_volume_mounts = container_config.pop("volume_mounts", [])
-    user_defined_resources = container_config.pop("resources", {})
-    user_defined_security_context = container_config.pop("security_context", None)
-
-    container_name = container_config.get("name", "dagster")
+    container_name = container_config.pop("name", "dagster")
 
     container_config = {
         **container_config,
+        "args": args,
         "name": container_name,
         "image": metadata.image,
-        "env": [{"name": key, "value": value} for key, value in env.items()]
-        + user_defined_env_vars,
-        "env_from": (
-            [{"config_map_ref": {"name": config_map}} for config_map in env_config_maps]
-            + [{"secret_ref": {"name": secret_name}} for secret_name in env_secrets]
-            + user_defined_env_from
+        "env": (
+            [{"name": key, "value": value} for key, value in env.items()] + user_defined_env_vars
         ),
-        "volume_mounts": volume_mounts + user_defined_volume_mounts,
-        "resources": user_defined_resources or resources,
-        "security_context": user_defined_security_context or security_context,
     }
 
     pod_spec_config = copy.deepcopy(user_defined_config.pod_spec_config)
 
-    user_defined_image_pull_secrets = pod_spec_config.pop("image_pull_secrets", [])
-    user_defined_service_account_name = pod_spec_config.pop("service_account_name", None)
     user_defined_containers = pod_spec_config.pop("containers", [])
-    user_defined_volumes = pod_spec_config.pop("volumes", [])
-    user_defined_scheduler_name = pod_spec_config.pop("scheduler_name", None)
 
     pod_spec_config = {
         **pod_spec_config,
-        "image_pull_secrets": [{"name": x["name"]} for x in image_pull_secrets]
-        + user_defined_image_pull_secrets,
-        "service_account_name": user_defined_service_account_name or service_account_name,
         "containers": [container_config] + user_defined_containers,
-        "volumes": volumes + user_defined_volumes,
-        "scheduler_name": user_defined_scheduler_name or scheduler_name,
     }
 
     pod_template_spec_metadata = copy.deepcopy(user_defined_config.pod_template_spec_metadata)
     user_defined_pod_template_labels = pod_template_spec_metadata.pop("labels", {})
 
     deployment_dict = {
         "metadata": {
             "name": k8s_deployment_name,
             "labels": {
                 **container_context.labels,
-                **_get_dagster_k8s_labels(deployment_name, location_name, instance),
+                **_get_dagster_k8s_labels(
+                    deployment_name, location_name, instance, server_timestamp
+                ),
             },
         },
         "spec": {  # DeploymentSpec
             "selector": {"match_labels": {"user-deployment": k8s_deployment_name}},
             "template": {  # PodTemplateSpec
                 "metadata": {
                     **pod_template_spec_metadata,
                     "labels": {
                         "user-deployment": k8s_deployment_name,
                         **container_context.labels,
                         **user_defined_pod_template_labels,
-                        **_get_dagster_k8s_labels(deployment_name, location_name, instance),
+                        **_get_dagster_k8s_labels(
+                            deployment_name, location_name, instance, server_timestamp
+                        ),
                     },
                 },
                 "spec": pod_spec_config,
             },
         },
     }
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 )
 from dagster._core.errors import DagsterUserCodeUnreachableError
 from dagster._grpc.client import DagsterGrpcClient, client_heartbeat_thread
 from dagster._serdes import ConfigurableClass, ConfigurableClassData
 from dagster._serdes.ipc import open_ipc_subprocess
 from dagster._utils import find_free_port, safe_tempfile_path_unmanaged
 from dagster._utils.merger import merge_dicts
-from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 from typing_extensions import Self
 
 from dagster_cloud.api.dagster_cloud_api import (
     UserCodeDeploymentType,
 )
 from dagster_cloud.execution.cloud_run_launcher.process import CloudProcessRunLauncher
 from dagster_cloud.execution.monitoring import CloudContainerResourceLimits
@@ -219,16 +218,18 @@
     ) -> Self:
         return cls(inst_data=inst_data, **config_value)
 
     def _start_new_server_spinup(
         self,
         deployment_name: str,
         location_name: str,
-        metadata: CodeDeploymentMetadata,
+        desired_entry: UserCodeLauncherEntry,
     ) -> DagsterCloudGrpcServer:
+        metadata = desired_entry.code_deployment_metadata
+
         key = (deployment_name, location_name)
 
         client: Union[MultiPexGrpcClient, DagsterGrpcClient]
 
         port: Optional[int] = None
         socket: Optional[str] = None
 
@@ -387,13 +388,16 @@
 
     def _list_server_handles(self) -> List[int]:
         return list(self._process_entries.keys())
 
     def get_agent_id_for_server(self, handle: int) -> Optional[str]:
         return self._instance.instance_uuid
 
+    def get_server_create_timestamp(self, handle: int) -> Optional[float]:
+        return None
+
     def __exit__(self, exception_type, exception_value, traceback):
         super().__exit__(exception_value, exception_value, traceback)
 
         if self._cleanup_zombies_thread:
             self._cleanup_zombies_shutdown_event.set()
             self._cleanup_zombies_thread.join()
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 import tempfile
 import threading
 import time
 import zlib
 from abc import abstractmethod, abstractproperty
-from concurrent.futures import ThreadPoolExecutor, wait
+from concurrent.futures import ThreadPoolExecutor, as_completed, wait
 from contextlib import AbstractContextManager
 from typing import (
     Any,
     Callable,
     Collection,
     DefaultDict,
     Dict,
@@ -27,32 +27,34 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 import dagster._check as check
+import grpc
+import pendulum
 from dagster import BoolSource, Field, IntSource
 from dagster._api.list_repositories import sync_list_repositories_grpc
 from dagster._core.definitions.selector import JobSelector
 from dagster._core.errors import DagsterUserCodeUnreachableError
-from dagster._core.host_representation import ExternalRepositoryOrigin
-from dagster._core.host_representation.origin import (
+from dagster._core.instance import MayHaveInstanceWeakref
+from dagster._core.launcher import RunLauncher
+from dagster._core.remote_representation import RemoteRepositoryOrigin
+from dagster._core.remote_representation.origin import (
     CodeLocationOrigin,
     RegisteredCodeLocationOrigin,
 )
-from dagster._core.instance import MayHaveInstanceWeakref
-from dagster._core.launcher import RunLauncher
 from dagster._grpc.client import DagsterGrpcClient
 from dagster._grpc.types import GetCurrentImageResult
 from dagster._serdes import deserialize_value, serialize_value, whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.merger import merge_dicts
 from dagster._utils.typed_dict import init_optional_typeddict
-from dagster_cloud_cli.core.errors import GraphQLStorageError, raise_http_error
+from dagster_cloud_cli.core.errors import raise_http_error
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 from typing_extensions import Self, TypeAlias
 
 from dagster_cloud.agent.queries import GET_AGENTS_QUERY
 from dagster_cloud.api.dagster_cloud_api import (
     DagsterCloudUploadLocationData,
     DagsterCloudUploadRepositoryData,
@@ -87,16 +89,18 @@
 
 USER_CODE_LAUNCHER_RECONCILE_SLEEP_SECONDS = 1
 USER_CODE_LAUNCHER_RECONCILE_METRICS_SLEEP_SECONDS = 60
 
 # Check on pending delete servers every 30th reconcile
 PENDING_DELETE_SERVER_CHECK_INTERVAL = 30
 
-# How often to sync actual_entries with pex server liveness
-MULTIPEX_ACTUAL_ENTRIES_REFRESH_INTERVAL = 30
+# How often to sync actual_entries with server liveness
+ACTUAL_ENTRIES_REFRESH_INTERVAL = 30
+
+CLEANUP_SERVER_GRACE_PERIOD_SECONDS = 3600
 
 ServerHandle = TypeVar("ServerHandle")
 
 DEPLOYMENT_INFO_QUERY = """
     query DeploymentInfo {
          deploymentInfo {
              deploymentType
@@ -311,14 +315,16 @@
         requires_healthcheck: bool = False,
         code_server_metrics: Optional[Mapping[str, Any]] = None,
         agent_metrics: Optional[Mapping[str, Any]] = None,
     ):
         self._grpc_servers: Dict[
             DeploymentAndLocation, Union[DagsterCloudGrpcServer, SerializableErrorInfo]
         ] = {}
+        self._first_unavailable_times: Dict[DeploymentAndLocation, float] = {}
+
         self._pending_delete_grpc_server_handles: Set[ServerHandle] = set()
         self._grpc_servers_lock = threading.Lock()
         self._per_location_metrics: Dict[
             DeploymentAndLocation, CloudCodeServerUtilizationMetrics
         ] = DefaultDict(lambda: init_optional_typeddict(CloudCodeServerUtilizationMetrics))
 
         self._multipex_servers: Dict[DeploymentAndLocation, DagsterCloudGrpcServer] = {}
@@ -380,19 +386,16 @@
             )
         except:
             self._logger.exception(
                 "Could not connect to graphql server to "
                 "retrieve active agent_ids. Just returning this agent as an active ID."
             )
             return set([self._instance.instance_uuid])
-        if "errors" in result:
-            raise GraphQLStorageError(result["errors"])
-        else:
-            self._logger.info(f"Active agent ids response: {result}")
-            return set(agent_data["id"] for agent_data in result["data"]["agents"])
+        self._logger.info(f"Active agent ids response: {result}")
+        return set(agent_data["id"] for agent_data in result["data"]["agents"])
 
     @property
     def code_server_metrics_enabled(self) -> bool:
         return (
             self._code_server_metrics_config["enabled"]
             if self._code_server_metrics_config
             else False
@@ -547,22 +550,18 @@
         with tempfile.TemporaryDirectory() as temp_dir:
             dst = os.path.join(temp_dir, "workspace_entry.tmp")
             with open(dst, "wb") as f:
                 f.write(zlib.compress(serialize_value(workspace_entry).encode("utf-8")))
 
             with open(dst, "rb") as f:
                 self._logger.info(
-                    "Uploading workspace entry for {deployment_name}:{location_name} ({size} bytes)".format(
-                        deployment_name=deployment_name,
-                        location_name=workspace_entry.location_name,
-                        size=os.path.getsize(dst),
-                    )
+                    f"Uploading workspace entry for {deployment_name}:{workspace_entry.location_name} ({os.path.getsize(dst)} bytes)"
                 )
 
-                resp = self._instance.rest_requests_session.put(
+                resp = self._instance.requests_managed_retries_session.put(
                     self._instance.dagster_cloud_upload_workspace_entry_url,
                     headers=self._instance.headers_for_deployment(deployment_name),
                     data={},
                     files={"workspace_entry.tmp": f},
                     timeout=self._instance.dagster_cloud_api_timeout,
                     proxies=self._instance.dagster_cloud_api_proxies,
                 )
@@ -595,15 +594,15 @@
                     for job_selector in missing
                 ]
                 wait(futures)
                 # trigger any exceptions to throw
                 _ = [f.result() for f in futures]
 
             with open(dst, "rb") as f:
-                resp = self._instance.rest_requests_session.put(
+                resp = self._instance.requests_managed_retries_session.put(
                     self._instance.dagster_cloud_upload_workspace_entry_url,
                     headers=self._instance.headers_for_deployment(deployment_name),
                     data={},
                     files={"workspace_entry.tmp": f},
                     timeout=self._instance.dagster_cloud_api_timeout,
                     proxies=self._instance.dagster_cloud_api_proxies,
                 )
@@ -638,15 +637,15 @@
 
         for (
             repository_name,
             code_pointer,
         ) in list_repositories_response.repository_code_pointer_dict.items():
             external_repository_chunks = list(
                 client.streaming_external_repository(
-                    external_repository_origin=ExternalRepositoryOrigin(
+                    external_repository_origin=RemoteRepositoryOrigin(
                         location_origin,
                         repository_name,
                     ),
                     defer_snapshots=self._defer_job_snapshots,
                 )
             )
 
@@ -679,20 +678,16 @@
         self,
         deployment_name: str,
         location_name: str,
         error_info: SerializableErrorInfo,
         metadata: CodeDeploymentMetadata,
     ):
         self._logger.error(
-            "Unable to update {deployment_name}:{location_name}. Updating location with error data:"
-            " {error_info}.".format(
-                deployment_name=deployment_name,
-                location_name=location_name,
-                error_info=str(error_info),
-            )
+            f"Unable to update {deployment_name}:{location_name}. Updating location with error data:"
+            f" {error_info!s}."
         )
 
         # Update serialized error
         errored_workspace_entry = DagsterCloudUploadWorkspaceEntry(
             location_name=location_name,
             deployment_metadata=metadata,
             upload_location_data=None,
@@ -810,15 +805,15 @@
         return []
 
     @abstractmethod
     def _start_new_server_spinup(
         self,
         deployment_name: str,
         location_name: str,
-        metadata: CodeDeploymentMetadata,
+        desired_entry: UserCodeLauncherEntry,
     ) -> DagsterCloudGrpcServer:
         """Create a new server for the given location using the given metadata as configuration
         and return a ServerHandle indicating where it can be found. Any waiting for the server
         to happen should happen in _wait_for_new_server_ready.
         """
 
     def _wait_for_new_multipex_server(
@@ -921,27 +916,51 @@
     def _list_server_handles(self) -> List[ServerHandle]:
         """Return a list of all server handles across all deployments and locations."""
 
     @abstractmethod
     def get_agent_id_for_server(self, handle: ServerHandle) -> Optional[str]:
         """Returns the agent_id that created a particular GRPC server."""
 
+    @abstractmethod
+    def get_server_create_timestamp(self, handle: ServerHandle) -> Optional[float]:
+        """Returns the update_timestamp value from the given code server."""
+
     def _can_cleanup_server(self, handle: ServerHandle, active_agent_ids: Set[str]) -> bool:
         """Returns true if we can clean up the server identified by the handle without issues (server was started by this agent, or agent is no longer active)."""
         agent_id_for_server = self.get_agent_id_for_server(handle)
         self._logger.info(
             f"For server {handle}; agent_id is {agent_id_for_server} while current agent_id is"
             f" {self._instance.instance_uuid}."
         )
         self._logger.info(f"All active agent ids: {active_agent_ids}")
-        return (
-            not agent_id_for_server
-            or self._instance.instance_uuid == agent_id_for_server
-            or agent_id_for_server not in cast(Set[str], active_agent_ids)
-        )
+
+        # If this server was created by the current agent, it can always be cleaned up
+        # (or if its a legacy server that never set an agent ID)
+        if not agent_id_for_server or self._instance.instance_uuid == agent_id_for_server:
+            return True
+
+        try:
+            update_timestamp_for_server = self.get_server_create_timestamp(handle)
+        except:
+            self._logger.exception(f"Failure fetching service creation timestamp for {handle}")
+            return False
+
+        # Clean up servers that were created more than CLEANUP_SERVER_GRACE_PERIOD_SECONDS
+        # seconds ago (to avoid race conditions) and were created by some agent that is now
+        # inactive, to ensure that servers are eventually cleaned up by the next agent
+        # when an agent crashes
+        if (
+            update_timestamp_for_server
+            and update_timestamp_for_server
+            >= pendulum.now("UTC").timestamp() - CLEANUP_SERVER_GRACE_PERIOD_SECONDS
+        ):
+            self._logger.info("Not cleaning up server since it was recently created")
+            return False
+
+        return agent_id_for_server not in cast(Set[str], active_agent_ids)
 
     def _graceful_cleanup_servers(self):  # ServerHandles
         active_agent_ids = self.get_active_agent_ids()
         if not self.supports_get_current_runs_for_server_handle:
             return self._cleanup_servers(active_agent_ids)
 
         handles = self._list_server_handles()
@@ -1055,40 +1074,37 @@
             if shutdown_event.is_set():
                 break
 
             try:
                 self.reconcile()
             except Exception:
                 self._logger.error(
-                    "Failure updating user code servers: {exc_info}".format(
-                        exc_info=serializable_error_info_from_exc_info(sys.exc_info()),
-                    )
+                    f"Failure updating user code servers: {serializable_error_info_from_exc_info(sys.exc_info())}"
                 )
 
     def reconcile(self) -> None:
         with self._metadata_lock:
             desired_entries = (
                 self._desired_entries.copy() if self._desired_entries is not None else None
             )
             upload_locations = self._upload_locations.copy()
             self._upload_locations = set()
 
         if desired_entries is None:
             # Wait for the first time the desired metadata is set before reconciling
             return
 
-        if (
-            time.time() - self._last_refreshed_actual_entries
-            > MULTIPEX_ACTUAL_ENTRIES_REFRESH_INTERVAL
-        ):
+        now = pendulum.now("UTC").timestamp()
+
+        if now - self._last_refreshed_actual_entries > ACTUAL_ENTRIES_REFRESH_INTERVAL:
             try:
                 self._refresh_actual_entries()
             except:
                 self._logger.exception("Failed to refresh actual entries.")
-            self._last_refreshed_actual_entries = time.time()
+            self._last_refreshed_actual_entries = now
 
         self._reconcile(
             desired_entries,
             upload_locations,
             check_on_pending_delete_servers=self._reconcile_count % self._reconcile_interval == 0,
         )
         if self._reconcile_count == 0 and self._requires_healthcheck:
@@ -1114,53 +1130,132 @@
                 self.record_resource_limit_metrics_all_locations()
                 self.update_utilization_metrics_all_locations()
                 self._logger.info(
                     f"Current code server utilization metrics: {self._per_location_metrics}"
                 )
             except Exception:
                 self._logger.error(
-                    "Failure updating user code server metrics: {exc_info}".format(
-                        exc_info=serializable_error_info_from_exc_info(sys.exc_info()),
-                    )
+                    f"Failure updating user code server metrics: {serializable_error_info_from_exc_info(sys.exc_info())}"
                 )
 
     @property
     def ready_to_serve_requests(self) -> bool:
         # thread-safe since reconcile_count is an integer
         return self._reconcile_count > 0
 
+    def _make_check_on_running_server_endpoint(self, server_endpoint: ServerEndpoint):
+        # Ensure that server_endpoint is bound correctly
+        return lambda: server_endpoint.create_client().ping("")
+
     def _refresh_actual_entries(self) -> None:
         for deployment_location, server in self._multipex_servers.items():
             if deployment_location in self._actual_entries:
                 # If a multipex server exists, we query it over gRPC
                 # to make sure the pex server is still available.
 
                 # First verify that the multipex server is running
                 try:
                     server.server_endpoint.create_multipex_client().ping("")
                 except:
                     # If it isn't, this is expected if ECS is currently spinning up this service
                     # after it crashed. In this case, we want to wait for it to fully come up
                     # before we remove actual entries. This ensures the recon loop uses the ECS
-                    # replacement multiplex server and not try to spin up a new multipex server.
+                    # replacement multipex server and not try to spin up a new multipex server.
                     self._logger.info(
                         "Multipex server entry exists but server is not running. "
                         "Will wait for server to come up."
                     )
                     return
                 deployment_name, location_name = deployment_location
                 if not self._get_existing_pex_servers(deployment_name, location_name):
                     self._logger.warning(
-                        "Pex servers disappeared for %s, %s. Removing actual entries to"
+                        "Pex servers disappeared for %s:%s. Removing actual entries to"
                         " activate reconciliation logic.",
                         deployment_name,
                         location_name,
                     )
                     del self._actual_entries[deployment_location]
 
+        # Check to see if any servers have become unresponsive
+        unavailable_server_timeout = int(
+            os.getenv(
+                "DAGSTER_CLOUD_CODE_SERVER_HEALTH_CHECK_REDEPLOY_TIMEOUT",
+                str(self._server_process_startup_timeout),
+            )
+        )
+
+        if unavailable_server_timeout < 0:
+            return
+
+        running_locations = {
+            deployment_location: endpoint_or_error
+            for deployment_location, endpoint_or_error in self.get_grpc_endpoints().items()
+            if (
+                isinstance(endpoint_or_error, ServerEndpoint)
+                and deployment_location in self._actual_entries
+            )
+        }
+
+        if not running_locations:
+            return
+
+        with ThreadPoolExecutor(
+            max_workers=max(
+                len(running_locations),
+                int(os.getenv("DAGSTER_CLOUD_CODE_SERVER_HEALTH_CHECK_MAX_WORKERS", "8")),
+            ),
+            thread_name_prefix="dagster_cloud_agent_server_health_check",
+        ) as executor:
+            futures = {}
+            for deployment_location, endpoint_or_error in running_locations.items():
+                deployment_name, location_name = deployment_location
+
+                futures[
+                    executor.submit(self._make_check_on_running_server_endpoint(endpoint_or_error))
+                ] = deployment_location
+
+            for future in as_completed(futures):
+                deployment_location = futures[future]
+
+                deployment_name, location_name = deployment_location
+                try:
+                    future.result()
+
+                    # Successful ping resets the tracked last unavailable time for this code server, if set
+                    self._first_unavailable_times.pop(deployment_location, None)
+                except Exception as e:
+                    if (
+                        isinstance(e, DagsterUserCodeUnreachableError)
+                        and isinstance(e.__cause__, grpc.RpcError)
+                        and cast(grpc.RpcError, e.__cause__).code() == grpc.StatusCode.UNAVAILABLE
+                    ):
+                        first_unavailable_time = self._first_unavailable_times.get(
+                            deployment_location
+                        )
+
+                        now = pendulum.now("UTC").timestamp()
+
+                        if not first_unavailable_time:
+                            self._logger.warning(
+                                f"Code server for {deployment_name}:{location_name} failed a health check. If it continues failing for more than {unavailable_server_timeout} seconds, a replacement code server will be deployed."
+                            )
+                            # Initialize the first unavailable time if set
+                            self._first_unavailable_times[deployment_location] = now
+                        elif now > first_unavailable_time + unavailable_server_timeout:
+                            self._logger.warning(
+                                f"Code server for {deployment_name}:{location_name} has been unresponsive for more than {unavailable_server_timeout} seconds. Deploying a new code server."
+                            )
+                            del self._actual_entries[deployment_location]
+                            del self._first_unavailable_times[deployment_location]
+                    else:
+                        self._logger.exception(
+                            f"Code server for {deployment_name}:{location_name} health check failed, but the error did not indicate that the server was unavailable."
+                        )
+                        self._first_unavailable_times.pop(deployment_location, None)
+
     def _write_liveness_sentinel(self) -> None:
         """Write a sentinel file to indicate that the agent is alive and grpc servers have been spun up."""
         pass
 
     def _check_for_image(self, metadata: CodeDeploymentMetadata):
         if self.requires_images and not self._resolve_image(metadata):
             raise Exception(
@@ -1297,18 +1392,18 @@
                         desired_pex_metadata.python_version if desired_pex_metadata else None
                     )
                     multipex_server_repr = f"{deployment_name}:{location_name} image={desired_entry.code_deployment_metadata.image} python_version={desired_python_version}"
                     if not multipex_server:
                         self._logger.info(
                             f"Creating new multipex server for {multipex_server_repr}"
                         )
-                        # confirm it's a valid image since _create_multipex_server will launch a container
+                        # confirm it's a valid image since _start_new_server_spinup will launch a container
                         self._check_for_image(desired_entry.code_deployment_metadata)
-                        multipex_server = self._create_multipex_server(
-                            deployment_name, location_name, desired_entry.code_deployment_metadata
+                        multipex_server = self._start_new_server_spinup(
+                            deployment_name, location_name, desired_entry
                         )
                         self._multipex_servers[to_update_key] = multipex_server
                         assert self._get_multipex_server(
                             deployment_name,
                             location_name,
                             desired_entry.code_deployment_metadata,
                         )
@@ -1345,20 +1440,16 @@
                     multipex_server.server_handle,
                     multipex_server.server_endpoint,
                 )
             except Exception:
                 error_info = serializable_error_info_from_exc_info(sys.exc_info())
 
                 self._logger.error(
-                    "Error while waiting for multipex server for {deployment_name}:{location_name}:"
-                    " {error_info}".format(
-                        deployment_name=deployment_name,
-                        location_name=location_name,
-                        error_info=error_info,
-                    )
+                    f"Error while waiting for multipex server for {deployment_name}:{location_name}:"
+                    f" {error_info}"
                 )
                 new_dagster_servers[to_update_key] = error_info
                 # Clear out this multipex server so we don't try to use it again
                 del self._multipex_servers[to_update_key]
 
         # Now that any needed multipex servers have been created, spin up dagster servers
         # (either as standalone servers or within a multipex server)
@@ -1423,21 +1514,16 @@
                         desired_entries[to_update_key],
                         server_or_error.server_handle,
                         server_or_error.server_endpoint,
                     )
                 except Exception:
                     error_info = serializable_error_info_from_exc_info(sys.exc_info())
                     self._logger.error(
-                        "Error while waiting for server for {deployment_name}:{location_name} for {deployment_info} to be"
-                        " ready: {error_info}".format(
-                            deployment_name=deployment_name,
-                            location_name=location_name,
-                            error_info=error_info,
-                            deployment_info=deployment_info,
-                        )
+                        f"Error while waiting for server for {deployment_name}:{location_name} for {deployment_info} to be"
+                        f" ready: {error_info}"
                     )
                     server_or_error = error_info
 
             # If needed, upload snapshot information to Dagster Cloud
             if to_update_key in upload_locations:
                 upload_locations.remove(to_update_key)
                 try:
@@ -1456,43 +1542,36 @@
                         f" {error_info}"
                     )
 
             # Once we've verified that the new server has uploaded its data successfully, swap in
             # the server to start serving new requests
             with self._grpc_servers_lock:
                 self._grpc_servers[to_update_key] = server_or_error
+                self._first_unavailable_times.pop(to_update_key, None)
 
         for to_update_key in to_update_keys:
             deployment_name, location_name = to_update_key
 
             # Remove any old standalone grpc server containers
             server_handles = existing_standalone_dagster_server_handles.get(to_update_key, [])
             removed_any_servers = False
 
             if server_handles:
                 removed_any_servers = True
                 self._logger.info(
-                    "Removing {num_servers} existing servers for {deployment_name}:{location_name}".format(
-                        num_servers=len(server_handles),
-                        location_name=location_name,
-                        deployment_name=deployment_name,
-                    )
+                    f"Removing {len(server_handles)} existing servers for {deployment_name}:{location_name}"
                 )
 
             for server_handle in server_handles:
                 try:
                     self._graceful_remove_server_handle(server_handle)
                 except Exception:
                     self._logger.error(
                         "Error while cleaning up after updating server for"
-                        " {deployment_name}:{location_name}: {error_info}".format(
-                            deployment_name=deployment_name,
-                            location_name=location_name,
-                            error_info=serializable_error_info_from_exc_info(sys.exc_info()),
-                        )
+                        f" {deployment_name}:{location_name}: {serializable_error_info_from_exc_info(sys.exc_info())}"
                     )
 
             # Remove any existing multipex servers other than the current one for each location
             multipex_server_handles = existing_multipex_server_handles.get(to_update_key, [])
 
             current_multipex_server = self._get_multipex_server(
                 deployment_name,
@@ -1514,19 +1593,15 @@
                     )
 
                     try:
                         self._graceful_remove_server_handle(multipex_server_handle)
                     except Exception:
                         self._logger.error(
                             "Error while cleaning up old multipex server for"
-                            " {deployment_name}:{location_name}: {error_info}".format(
-                                deployment_name=deployment_name,
-                                location_name=location_name,
-                                error_info=serializable_error_info_from_exc_info(sys.exc_info()),
-                            )
+                            f" {deployment_name}:{location_name}: {serializable_error_info_from_exc_info(sys.exc_info())}"
                         )
 
             # On the current multipex server, shut down any old pex servers
             pex_server_handles = existing_pex_server_handles.get(to_update_key)
             if current_multipex_server and pex_server_handles:
                 removed_any_servers = True
                 self._logger.info(
@@ -1541,19 +1616,15 @@
                             current_multipex_server.server_handle,
                             current_multipex_server.server_endpoint,
                             pex_server_handle,
                         )
                     except Exception:
                         self._logger.error(
                             "Error while cleaning up after updating server for"
-                            " {deployment_name}:{location_name}: {error_info}".format(
-                                deployment_name=deployment_name,
-                                location_name=location_name,
-                                error_info=serializable_error_info_from_exc_info(sys.exc_info()),
-                            )
+                            f" {deployment_name}:{location_name}: {serializable_error_info_from_exc_info(sys.exc_info())}"
                         )
 
             if removed_any_servers:
                 self._logger.info(
                     f"Removed all previous servers for {deployment_name}:{location_name}"
                 )
 
@@ -1637,22 +1708,14 @@
                 == code_deployment_metadata.container_context
             )
         ):
             return cand_server
 
         return None
 
-    def _create_multipex_server(self, deployment_name, location_name, code_deployment_metadata):
-        multipex_server = self._start_new_server_spinup(
-            deployment_name,
-            location_name,
-            code_deployment_metadata,
-        )
-        return multipex_server
-
     def _create_pex_server(
         self,
         deployment_name: str,
         location_name: str,
         desired_entry: UserCodeLauncherEntry,
         multipex_server: DagsterCloudGrpcServer,
     ):
@@ -1695,17 +1758,15 @@
                         ("location", location_name),
                         ("timestamp", str(int(desired_entry.update_timestamp))),
                     ],
                 ),
                 desired_entry.code_deployment_metadata,
             )
         else:
-            return self._start_new_server_spinup(
-                deployment_name, location_name, desired_entry.code_deployment_metadata
-            )
+            return self._start_new_server_spinup(deployment_name, location_name, desired_entry)
 
     def get_grpc_endpoint(
         self,
         deployment_name: str,
         location_name: str,
     ) -> ServerEndpoint:
         with self._grpc_servers_lock:
@@ -1814,15 +1875,15 @@
             self._graceful_remove_server_handle(server_handle)
 
     def _wait_for_dagster_server_process(
         self,
         client: DagsterGrpcClient,
         timeout,
         additional_check: Optional[Callable[[], None]] = None,
-        get_timeout_debug_info: Optional[Callable[[], None]] = None,
+        get_timeout_debug_info: Optional[Callable[[], Any]] = None,
     ) -> None:
         self._wait_for_server_process(
             client, timeout, additional_check, get_timeout_debug_info=get_timeout_debug_info
         )
         # Call a method that raises an exception if there was an error importing the code
         sync_list_repositories_grpc(client)
 
@@ -1877,15 +1938,15 @@
         job_selector: JobSelector,
         server: DagsterCloudGrpcServer,
     ):
         with tempfile.TemporaryDirectory() as temp_dir:
             client = server.server_endpoint.create_client()
             location_origin = self._get_code_location_origin(job_selector.location_name)
             response = client.external_job(
-                ExternalRepositoryOrigin(location_origin, job_selector.repository_name),
+                RemoteRepositoryOrigin(location_origin, job_selector.repository_name),
                 job_selector.job_name,
             )
             if not response.serialized_job_data:
                 error = (
                     deserialize_value(response.serialized_error, SerializableErrorInfo)
                     if response.serialized_error
                     else "no captured error"
@@ -1893,15 +1954,15 @@
                 raise Exception(f"Error fetching job data in code server:\n{error}")
 
             dst = os.path.join(temp_dir, "job.tmp")
             with open(dst, "wb") as f:
                 f.write(zlib.compress(response.serialized_job_data.encode("utf-8")))
 
             with open(dst, "rb") as f:
-                resp = self._instance.rest_requests_session.put(
+                resp = self._instance.requests_managed_retries_session.put(
                     self._instance.dagster_cloud_upload_job_snap_url,
                     headers=self._instance.headers_for_deployment(deployment_name),
                     data={},
                     files={"job.tmp": f},
                     timeout=self._instance.dagster_cloud_api_timeout,
                     proxies=self._instance.dagster_cloud_api_proxies,
                 )
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster-cloud-1.7.0/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.6.9/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.0/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.6.9
+Version: 1.7.0
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.6.9/dagster_cloud.egg-info/SOURCES.txt` & `dagster-cloud-1.7.0/dagster_cloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 dagster_cloud.egg-info/dependency_links.txt
 dagster_cloud.egg-info/requires.txt
 dagster_cloud.egg-info/top_level.txt
 dagster_cloud/agent/__init__.py
 dagster_cloud/agent/dagster_cloud_agent.py
 dagster_cloud/agent/queries.py
 dagster_cloud/agent/cli/__init__.py
+dagster_cloud/anomaly_detection/__init__.py
+dagster_cloud/anomaly_detection/defs.py
+dagster_cloud/anomaly_detection/mutation.py
+dagster_cloud/anomaly_detection/types.py
 dagster_cloud/api/__init__.py
 dagster_cloud/api/dagster_cloud_api.py
+dagster_cloud/artifacts/__init__.py
 dagster_cloud/auth/__init__.py
 dagster_cloud/auth/constants.py
 dagster_cloud/dagster_insights/__init__.py
 dagster_cloud/dagster_insights/errors.py
 dagster_cloud/dagster_insights/insights_utils.py
 dagster_cloud/dagster_insights/metrics_utils.py
 dagster_cloud/dagster_insights/query.py
```

### Comparing `dagster-cloud-1.6.9/setup.py` & `dagster-cloud-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.6.9",
-        "dagster-cloud-cli==1.6.9",
+        "dagster==1.7.0",
+        "dagster-cloud-cli==1.7.0",
         "pex>=2.1.132,<3",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -62,21 +62,21 @@
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
             "dbt-core",
             "dbt-snowflake",
             "dbt-postgres",
             "dbt-duckdb",
-            "dagster-dbt==0.22.9",
-            "dagster_k8s==0.22.9",
+            "dagster-dbt==0.23.0",
+            "dagster_k8s==0.23.0",
         ],
         "insights": ["pyarrow"],
-        "docker": ["docker", "dagster_docker==0.22.9"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.22.9"],
-        "ecs": ["dagster_aws==0.22.9", "boto3"],
+        "docker": ["docker", "dagster_docker==0.23.0"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.0"],
+        "ecs": ["dagster_aws==0.23.0", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

