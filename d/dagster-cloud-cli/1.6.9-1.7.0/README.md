# Comparing `tmp/dagster-cloud-cli-1.6.9.tar.gz` & `tmp/dagster-cloud-cli-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.6.9.tar", last modified: Fri Mar  8 00:32:07 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.0.tar", last modified: Thu Apr  4 19:55:58 2024, max compression
```

## Comparing `dagster-cloud-cli-1.6.9.tar` & `dagster-cloud-cli-1.7.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.442223 dagster-cloud-cli-1.6.9/
--rw-r--r--   0 root         (0) root         (0)      132 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-08 00:32:07.442223 dagster-cloud-cli-1.6.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.390223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.398223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.406223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4947 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.410223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    26608 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4090 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8598 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.414223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.414223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    10963 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.414223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.414223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.418223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.418223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.426223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18361 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.430223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11826 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.430223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9448 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.430223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.438223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.438223 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13814 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6014 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     7106 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    20448 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.394223 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-08 00:32:07.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2950 2024-03-08 00:32:07.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:32:07.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-08 00:32:07.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-03-08 00:32:07.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-03-08 00:32:07.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:32:07.442223 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16130 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      659 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 00:32:07.442223 dagster-cloud-cli-1.6.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1139 2024-03-08 00:18:12.000000 dagster-cloud-cli-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.640234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.644234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.644234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4947 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    26640 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17056 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.652234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.652234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.656234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18361 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.656234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12434 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.660234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    12940 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.660234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.664234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.672234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13814 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    21075 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.644234 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16130 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/setup.py
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 ):
     state_store = state.FileStore(statedir=statedir)
     location_states = state_store.list_locations()
 
     source = metrics.get_source()
     if source == CliEventTags.source.github:
         event = github_context.get_github_event(project_dir)
-        msg = "Your pull request is automatically being deployed to Dagster Cloud."
+        msg = f"Your pull request at commit `{event.github_sha}` is automatically being deployed to Dagster Cloud."
         event.update_pr_comment(
             msg + "\n\n" + report.markdown_report(location_states),
             orig_author="github-actions[bot]",
             orig_text=msg,
         )
     else:
         raise ui.error("'dagster-cloud ci notify' is only available within Github actions.")
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/checks.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/report.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/ci/state.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/config.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 app = Typer(help="Configure the Dagster Cloud CLI.")
 
 
 @app.command()
 @dagster_cloud_options()
 def set_deployment(
-    ctx: Context, deployment: str = Argument(..., autocompletion=available_deployment_names)
+    ctx: Context,
+    deployment: str = Argument(..., autocompletion=available_deployment_names),
 ):
     """Set the default deployment for CLI commands."""
     deployments = available_deployment_names(ctx=ctx)
     if not deployment or deployment not in deployments:
         raise ui.error(f"Deployment {ui.as_code(deployment)} not found")
 
     config = read_config()
@@ -38,15 +39,18 @@
 
     ui.print(f"Default deployment changed to {ui.as_code(deployment)}")
 
 
 @app.command()
 def view(
     show_token: bool = Option(
-        False, "--show-token", "-s", help="Whether to display the user token in plaintext."
+        False,
+        "--show-token",
+        "-s",
+        help="Whether to display the user token in plaintext.",
     ),
 ):
     """View the current CLI configuration."""
     config = read_config()
     if not show_token and config.user_token:
         config = config._replace(user_token=ui.censor_token(config.user_token))
     config_to_display = {k: v for k, v in config._asdict().items() if v is not None}
@@ -194,15 +198,15 @@
         ui.print(f"Authorized for organization {ui.as_code(str(new_org))}\n")
     else:
         new_org = ui.input("Dagster Cloud organization:", default=organization or "") or None
         if not api_token:
             deployment_name = deployment if deployment else "prod"
             ui.print(
                 "\nTo create a new user token or find an existing token, visit"
-                f" https://dagster.cloud/{new_org}/{deployment_name}/cloud-settings/tokens"
+                f" https://dagster.cloud/{new_org}/{deployment_name}/org-settings/tokens"
             )
         new_api_token = (
             ui.password_input("Dagster Cloud user token:", default=api_token or "") or None
         )
 
     # Attempt to fetch deployment names from server, fallback to a text input upon failure
     deployment_names = []
@@ -228,15 +232,17 @@
         if new_deployment == "None":
             new_deployment = None
     else:
         new_deployment = ui.input("Default deployment:", default=deployment or "") or None
 
     write_config(
         DagsterCloudCliConfig(
-            organization=new_org, default_deployment=new_deployment, user_token=new_api_token
+            organization=new_org,
+            default_deployment=new_deployment,
+            user_token=new_api_token,
         )
     )
 
 
 @app.command()
 @dagster_cloud_options(allow_empty=True)
 def setup(organization: str, deployment: str, api_token: str):
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from pathlib import Path
 
 import yaml
 from typer import Argument, Typer
+from typing_extensions import Annotated
 
 from ... import gql, ui
 from ...config_utils import dagster_cloud_options
+from ...core.artifacts import download_artifact, upload_artifact
+from ...core.headers.auth import DagsterCloudInstanceScope
 from ...utils import create_stub_app
 
 try:
     from .alert_policies.commands import app as alert_policies_app
 except ImportError:
     alert_policies_app = create_stub_app("dagster-cloud")
 
@@ -39,7 +42,63 @@
     api_token: str,
     url: str,
 ):
     """Get the Dagster Cloud deployment settings."""
     with gql.graphql_client_from_url(url, api_token) as client:
         settings = gql.get_deployment_settings(client)
     ui.print_yaml(settings)
+
+
+@app.command(name="upload-artifact")
+@dagster_cloud_options(allow_empty=True, requires_url=True)
+def upload_artifact_command(
+    key: Annotated[
+        str,
+        Argument(
+            help="The key for the artifact being uploaded.",
+        ),
+    ],
+    path: Annotated[
+        str,
+        Argument(
+            help="The path to the file to upload.",
+        ),
+    ],
+    api_token: str,
+    url: str,
+):
+    """Upload a deployment scoped artifact."""
+    upload_artifact(
+        url=url,
+        scope=DagsterCloudInstanceScope.DEPLOYMENT,
+        api_token=api_token,
+        key=key,
+        path=path,
+    )
+
+
+@app.command(name="download-artifact")
+@dagster_cloud_options(allow_empty=True, requires_url=True)
+def download_artifact_command(
+    key: Annotated[
+        str,
+        Argument(
+            help="The key for the artifact to download.",
+        ),
+    ],
+    path: Annotated[
+        str,
+        Argument(
+            help="Path to the file that the contents should be written to.",
+        ),
+    ],
+    api_token: str,
+    url: str,
+):
+    """Download a deployment scoped artifact."""
+    download_artifact(
+        url=url,
+        scope=DagsterCloudInstanceScope.DEPLOYMENT,
+        api_token=api_token,
+        key=key,
+        path=path,
+    )
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import yaml
 from typer import Option, Typer
 
 from .... import gql, ui
 from ....config_utils import dagster_cloud_options
-from .config_schema import process_alert_policies_config
+from .config_schema import INSIGHTS_ALERT_POLICIES_SCHEMA, process_alert_policies_config
 
 DEFAULT_ALERT_POLICIES_YAML_FILENAME = "alert_policies.yaml"
 
 app = Typer(help="Interact with your alert policies.")
 
 
 @app.command(name="list")
@@ -40,14 +40,14 @@
 ):
     """Sync your YAML configured alert policies to Dagster Cloud."""
     with gql.graphql_client_from_url(url, api_token) as client:
         with open(str(alert_policies_file), "r", encoding="utf8") as f:
             config = yaml.load(f.read(), Loader=yaml.SafeLoader)
 
         try:
-            process_alert_policies_config(config)
+            process_alert_policies_config(config, INSIGHTS_ALERT_POLICIES_SCHEMA)
 
             alert_policies = gql.reconcile_alert_policies(client, config)
 
             ui.print(f"Synced alert policies: {', '.join(alert_policies)}")
         except Exception as e:
             raise ui.error(str(e))
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+from typing import Any
+
 import dagster._check as check
 from dagster import Array, Enum, EnumValue, Field, Selector, Shape
 from dagster._config import validate_config
 from dagster._core.definitions.repository_definition.valid_definitions import (
     SINGLETON_REPOSITORY_NAME,
 )
 
+from dagster_cloud_cli.core.alert_types import InsightsAlertComparisonOperator
 
-def validate_alert_policy_config(alert_policy_config):
-    validation = validate_config(ALERT_POLICY_SCHEMA, alert_policy_config)
-    return [error.message for error in validation.errors]
 
+def validate_alert_policy_config(alert_policy_config, schema: Any):
+    validation = validate_config(schema, alert_policy_config)
+    return [error.message for error in validation.errors] if validation.errors else []
 
-def validate_alert_policies_config(alert_policies_config):
-    validation = validate_config(ALERT_POLICIES_SCHEMA, alert_policies_config)
-    return [error.message for error in validation.errors]
 
+def validate_alert_policies_config(alert_policies_config, schema: Any):
+    validation = validate_config(schema, alert_policies_config)
+    return [error.message for error in validation.errors] if validation.errors else []
 
-def process_alert_policies_config(alert_policies_config):
+
+def process_alert_policies_config(alert_policies_config, schema: Any):
     validation = validate_config(ALERT_POLICIES_SCHEMA, alert_policies_config)
 
     check.invariant(
         validation.success,
-        ", ".join([error.message for error in validation.errors]),
+        ", ".join([error.message for error in validation.errors] if validation.errors else []),
     )
 
     # Validate each individual alert policy
     for alert_policy_config in alert_policies_config["alert_policies"]:
         check.invariant(
             "tags" not in alert_policy_config or len(alert_policy_config["tags"]) > 0,
             "When setting tags for an alert policy, the configuration "
@@ -39,217 +43,393 @@
             check.invariant(
                 len(email_notification_service["email_addresses"]) > 0,
                 "When creating an alert policy to send email alerts, "
                 "the configuration must contain at least one email address.",
             )
 
 
-ALERT_POLICY_SCHEMA = Shape(
-    fields={
-        "name": Field(
-            config=str,
-            is_required=True,
-            description="Alert policy name.",
-        ),
-        "description": Field(
-            config=str,
-            default_value="",
-            description="Description of alert policy",
-        ),
-        "tags": Field(
-            config=Array(
-                Shape(
+TARGET_TYPES_SCHEMA = {
+    "asset_group_target": Field(
+        config=Shape(
+            fields={
+                "asset_group": Field(
+                    config=str,
+                    is_required=True,
+                    description="The name of the asset group.",
+                ),
+                "location_name": Field(
+                    config=str,
+                    is_required=True,
+                    description=("The name of the code location that contains the asset" " group."),
+                ),
+                "repo_name": Field(
+                    config=str,
+                    is_required=False,
+                    description=(
+                        "The name of the repository that contains the asset"
+                        " group. Only required if there are multiple"
+                        " repositories with the same code location."
+                    ),
+                    default_value=SINGLETON_REPOSITORY_NAME,
+                ),
+            }
+        )
+    ),
+    "asset_key_target": Field(
+        config=Shape(
+            fields={
+                "asset_key": Field(
+                    config=Array(str),
+                    is_required=True,
+                    description="The key of the asset.",
+                )
+            }
+        )
+    ),
+}
+
+
+insights_operator_enum = Enum.from_python_enum(InsightsAlertComparisonOperator)
+
+
+INSIGHTS_TARGET_TYPES_SCHEMA = {
+    **TARGET_TYPES_SCHEMA,
+    "insights_deployment_threshold_target": Field(
+        config=Shape(
+            fields={
+                "metric_name": Field(
+                    config=str,
+                    is_required=True,
+                    description="The name of the metric to target.",
+                ),
+                "threshold": Field(
+                    config=float,
+                    is_required=True,
+                    description="The threshold value to alert if exceeded.",
+                ),
+                "selection_period_days": Field(
+                    config=int,
+                    is_required=True,
+                    description="The number of days to use for the selection period.",
+                ),
+                "operator": Field(
+                    config=insights_operator_enum,
+                    is_required=True,
+                    description="The operator to use for the threshold comparison.",
+                ),
+            }
+        )
+    ),
+    "insights_asset_group_threshold_target": Field(
+        config=Shape(
+            fields={
+                "metric_name": Field(
+                    config=str,
+                    is_required=True,
+                    description="The name of the metric to target.",
+                ),
+                "threshold": Field(
+                    config=float,
+                    is_required=True,
+                    description="The threshold value to alert if exceeded.",
+                ),
+                "selection_period_days": Field(
+                    config=int,
+                    is_required=True,
+                    description="The number of days to use for the selection period.",
+                ),
+                "operator": Field(
+                    config=insights_operator_enum,
+                    is_required=True,
+                    description="The operator to use for the threshold comparison.",
+                ),
+                "asset_group": Shape(
                     fields={
-                        "key": Field(
+                        "location_name": Field(
                             config=str,
                             is_required=True,
-                            description="Specify a tag key.",
+                            description="The name of the code location that contains the asset group.",
                         ),
-                        "value": Field(
+                        "asset_group_name": Field(
                             config=str,
                             is_required=True,
-                            description="Specify a tag value.",
-                        ),
-                    },
-                    description="A tag key-value pair.",
-                )
-            ),
-            description=(
-                "The alert policy will apply to code artifacts that have all the specified tags."
-                " When tags are explicitly omitted, this alert policy will apply to all code"
-                " artifacts."
-            ),
-            is_required=False,
-        ),
-        "event_types": Field(
-            config=Array(
-                Enum(
-                    name="AlertPolicyEventType",
-                    enum_values=[
-                        EnumValue("JOB_FAILURE", description="Alert on job failure."),
-                        EnumValue("JOB_SUCCESS", description="Alert on job success."),
-                        EnumValue("TICK_FAILURE", description="Alert on schedule/sensor failure."),
-                        EnumValue("AGENT_UNAVAILABLE", description="Alert on agent downtime."),
-                        EnumValue(
-                            "CODE_LOCATION_ERROR", description="Alert on code location error."
-                        ),
-                        EnumValue(
-                            "ASSET_MATERIALIZATION_SUCCESS",
-                            description="Alert when an asset successfully materializes.",
+                            description="The name of the asset group.",
                         ),
-                        EnumValue(
-                            "ASSET_MATERIALIZATION_FAILURE",
+                        "repo_name": Field(
+                            config=str,
+                            is_required=False,
                             description=(
-                                "Alert when a planned asset materialization fails to occur."
+                                "The name of the repository that contains the asset group."
                             ),
+                            default_value=SINGLETON_REPOSITORY_NAME,
                         ),
-                        EnumValue(
-                            "ASSET_CHECK_PASSED", description="Alert on asset check success."
+                    }
+                ),
+            }
+        )
+    ),
+    "insights_asset_threshold_target": Field(
+        config=Shape(
+            fields={
+                "metric_name": Field(
+                    config=str,
+                    is_required=True,
+                    description="The name of the metric to target.",
+                ),
+                "threshold": Field(
+                    config=float,
+                    is_required=True,
+                    description="The threshold value to alert if exceeded.",
+                ),
+                "selection_period_days": Field(
+                    config=int,
+                    is_required=True,
+                    description="The number of days to use for the selection period.",
+                ),
+                "operator": Field(
+                    config=insights_operator_enum,
+                    is_required=True,
+                    description="The operator to use for the threshold comparison.",
+                ),
+                "asset_key": Field(
+                    config=Array(str),
+                    is_required=True,
+                    description="The key of the asset.",
+                ),
+            }
+        )
+    ),
+    "insights_job_threshold_target": Field(
+        config=Shape(
+            fields={
+                "metric_name": Field(
+                    config=str,
+                    is_required=True,
+                    description="The name of the metric to target.",
+                ),
+                "threshold": Field(
+                    config=float,
+                    is_required=True,
+                    description="The threshold value to alert if exceeded.",
+                ),
+                "selection_period_days": Field(
+                    config=int,
+                    is_required=True,
+                    description="The number of days to use for the selection period.",
+                ),
+                "operator": Field(
+                    config=insights_operator_enum,
+                    is_required=True,
+                    description="The operator to use for the threshold comparison.",
+                ),
+                "job": Shape(
+                    fields={
+                        "job_name": Field(
+                            config=str,
+                            is_required=True,
+                            description="The name of the job.",
                         ),
-                        EnumValue(
-                            "ASSET_CHECK_EXECUTION_FAILURE",
-                            description=(
-                                "Alert when a planned asset check fails before it evaluates."
-                            ),
+                        "location_name": Field(
+                            config=str,
+                            is_required=True,
+                            description="The name of the code location that contains the job.",
                         ),
-                        EnumValue(
-                            "ASSET_CHECK_SEVERITY_WARN",
-                            description=(
-                                "Alert when a planned asset check fails with severity warn."
-                            ),
+                        "repo_name": Field(
+                            config=str,
+                            is_required=False,
+                            description=("The name of the repository that contains the job."),
+                            default_value=SINGLETON_REPOSITORY_NAME,
                         ),
-                        EnumValue(
-                            "ASSET_CHECK_SEVERITY_ERROR",
-                            description=(
-                                "Alert when a planned asset check fails with severity error."
+                    }
+                ),
+            }
+        )
+    ),
+}
+
+ALERT_EVENT_TYPES = [
+    EnumValue("JOB_FAILURE", description="Alert on job failure."),
+    EnumValue("JOB_SUCCESS", description="Alert on job success."),
+    EnumValue("TICK_FAILURE", description="Alert on schedule/sensor failure."),
+    EnumValue("AGENT_UNAVAILABLE", description="Alert on agent downtime."),
+    EnumValue("CODE_LOCATION_ERROR", description="Alert on code location error."),
+    EnumValue(
+        "ASSET_MATERIALIZATION_SUCCESS",
+        description="Alert when an asset successfully materializes.",
+    ),
+    EnumValue(
+        "ASSET_MATERIALIZATION_FAILURE",
+        description=("Alert when a planned asset materialization fails to occur."),
+    ),
+    EnumValue("ASSET_CHECK_PASSED", description="Alert on asset check success."),
+    EnumValue(
+        "ASSET_CHECK_EXECUTION_FAILURE",
+        description=("Alert when a planned asset check fails before it evaluates."),
+    ),
+    EnumValue(
+        "ASSET_CHECK_SEVERITY_WARN",
+        description=("Alert when a planned asset check fails with severity warn."),
+    ),
+    EnumValue(
+        "ASSET_CHECK_SEVERITY_ERROR",
+        description=("Alert when a planned asset check fails with severity error."),
+    ),
+    EnumValue(
+        "ASSET_OVERDUE",
+        description="Alert when an asset is overdue, based on its freshness policy.",
+    ),
+]
+
+INSIGHTS_ALERT_EVENT_TYPES = [
+    *ALERT_EVENT_TYPES,
+    EnumValue(
+        "INSIGHTS_CONSUMPTION_EXCEEDED",
+        description="Alert when insights consumption exceeds the threshold.",
+    ),
+]
+
+ALERT_POLICY_SCHEMA, INSIGHTS_ALERT_POLICY_SCHEMA = [
+    Shape(
+        fields={
+            "name": Field(
+                config=str,
+                is_required=True,
+                description="Alert policy name.",
+            ),
+            "description": Field(
+                config=str,
+                default_value="",
+                description="Description of alert policy",
+            ),
+            "tags": Field(
+                config=Array(
+                    Shape(
+                        fields={
+                            "key": Field(
+                                config=str,
+                                is_required=True,
+                                description="Specify a tag key.",
                             ),
-                        ),
-                        EnumValue(
-                            "ASSET_OVERDUE",
-                            description="Alert when an asset is overdue, based on its freshness policy.",
-                        ),
-                    ],
-                )
+                            "value": Field(
+                                config=str,
+                                is_required=True,
+                                description="Specify a tag value.",
+                            ),
+                        },
+                        description="A tag key-value pair.",
+                    )
+                ),
+                description=(
+                    "The alert policy will apply to code artifacts that have all the specified tags."
+                    " When tags are explicitly omitted, this alert policy will apply to all code"
+                    " artifacts."
+                ),
+                is_required=False,
             ),
-            description="The selected system event types that will trigger the alert policy.",
-        ),
-        "notification_service": Field(
-            Selector(
-                fields={
-                    "email": Field(
-                        config=Shape(
-                            fields={
-                                "email_addresses": Field(
-                                    config=Array(str),
-                                    is_required=True,
-                                    description="Email addresses to send alerts to.",
-                                )
-                            }
-                        ),
-                        description=(
-                            "Details to customize email notifications for this alert policy."
-                        ),
-                    ),
-                    "slack": Field(
-                        config=Shape(
-                            fields={
-                                "slack_workspace_name": Field(
-                                    config=str,
-                                    is_required=True,
-                                    description="The name of your slack workspace.",
-                                ),
-                                "slack_channel_name": Field(
-                                    config=str,
-                                    is_required=True,
-                                    description=(
-                                        "The name of the slack channel in which to post alerts."
-                                    ),
-                                ),
-                            }
-                        )
-                    ),
-                    "email_owners": Field(config=Shape(fields={})),
-                    "microsoft_teams": Field(
-                        config=Shape(
-                            fields={
-                                "webhook_url": Field(
-                                    config=str,
-                                    is_required=True,
-                                    description="The incoming webhook URL for your Microsoft Team connector. "
-                                    "Must match the form https://xxxxx.webhook.office.com/xxxxx",
-                                )
-                            }
-                        )
-                    ),
-                }
+            "event_types": Field(
+                config=Array(
+                    Enum(
+                        name="AlertPolicyEventType",
+                        enum_values=event_types,
+                    )
+                ),
+                description="The selected system event types that will trigger the alert policy.",
             ),
-            is_required=True,
-            description="Configure how the alert policy should send a notification.",
-        ),
-        "enabled": Field(
-            config=bool,
-            default_value=True,
-            description="Whether the alert policy is active or not.",
-        ),
-        "alert_targets": Field(
-            config=Array(
+            "notification_service": Field(
                 Selector(
                     fields={
-                        "asset_group_target": Field(
+                        "email": Field(
                             config=Shape(
                                 fields={
-                                    "asset_group": Field(
+                                    "email_addresses": Field(
+                                        config=Array(str),
+                                        is_required=True,
+                                        description="Email addresses to send alerts to.",
+                                    )
+                                }
+                            ),
+                            description=(
+                                "Details to customize email notifications for this alert policy."
+                            ),
+                        ),
+                        "slack": Field(
+                            config=Shape(
+                                fields={
+                                    "slack_workspace_name": Field(
                                         config=str,
                                         is_required=True,
-                                        description="The name of the asset group.",
+                                        description="The name of your slack workspace.",
                                     ),
-                                    "location_name": Field(
+                                    "slack_channel_name": Field(
                                         config=str,
                                         is_required=True,
                                         description=(
-                                            "The name of the code location that contains the asset"
-                                            " group."
+                                            "The name of the slack channel in which to post alerts."
                                         ),
                                     ),
-                                    "repo_name": Field(
+                                }
+                            )
+                        ),
+                        "email_owners": Field(config=Shape(fields={})),
+                        "microsoft_teams": Field(
+                            config=Shape(
+                                fields={
+                                    "webhook_url": Field(
                                         config=str,
-                                        is_required=False,
-                                        description=(
-                                            "The name of the repository that contains the asset"
-                                            " group. Only required if there are multiple"
-                                            " repositories with the same code location."
-                                        ),
-                                        default_value=SINGLETON_REPOSITORY_NAME,
-                                    ),
+                                        is_required=True,
+                                        description="The incoming webhook URL for your Microsoft Team connector. "
+                                        "Must match the form https://xxxxx.webhook.office.com/xxxxx",
+                                    )
                                 }
                             )
                         ),
-                        "asset_key_target": Field(
+                        "pagerduty": Field(
                             config=Shape(
                                 fields={
-                                    "asset_key": Field(
-                                        config=Array(str),
+                                    "integration_key": Field(
+                                        config=str,
                                         is_required=True,
-                                        description="The key of the asset.",
+                                        description="The integration key for your PagerDuty app.",
                                     )
                                 }
                             )
                         ),
-                    },
-                    description=(
-                        "Information for targeting events for this alert policy. If no target is"
-                        " specified, the alert policy will apply to all events of a particular"
-                        " type."
+                    }
+                ),
+                is_required=True,
+                description="Configure how the alert policy should send a notification.",
+            ),
+            "enabled": Field(
+                config=bool,
+                default_value=True,
+                description="Whether the alert policy is active or not.",
+            ),
+            "alert_targets": Field(
+                config=Array(
+                    Selector(
+                        fields=target_types_schema,
+                        description=(
+                            "Information for targeting events for this alert policy. If no target is"
+                            " specified, the alert policy will apply to all events of a particular"
+                            " type."
+                        ),
                     ),
                 ),
+                is_required=False,
             ),
-            is_required=False,
-        ),
-    },
-    description="Details to customize an alert policy in Dagster Cloud.",
-)
+        },
+        description="Details to customize an alert policy in Dagster Cloud.",
+    )
+    for target_types_schema, event_types in (
+        (TARGET_TYPES_SCHEMA, ALERT_EVENT_TYPES),
+        (INSIGHTS_TARGET_TYPES_SCHEMA, INSIGHTS_ALERT_EVENT_TYPES),
+    )
+]
 
-ALERT_POLICIES_SCHEMA = Shape(
-    fields={
-        "alert_policies": Array(ALERT_POLICY_SCHEMA),
-    }
-)
+INSIGHTS_ALERT_POLICIES_SCHEMA, ALERT_POLICIES_SCHEMA = [
+    Shape(
+        fields={
+            "alert_policies": Array(alert_policy_schema),
+        }
+    )
+    for alert_policy_schema in (INSIGHTS_ALERT_POLICY_SCHEMA, ALERT_POLICY_SCHEMA)
+]
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/job/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/metrics.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/run/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Mapping, Optional
 
 import dagster._check as check
 import yaml
 from dagster._serdes.serdes import deserialize_value
 from dagster._utils import DEFAULT_WORKSPACE_YAML_FILENAME
 from typer import Argument, Option, Typer
 
 from dagster_cloud_cli import gql, ui
 from dagster_cloud_cli.config_utils import (
     DEFAULT_LOCATION_LOAD_TIMEOUT,
     DEPLOYMENT_CLI_OPTIONS,
     dagster_cloud_options,
     get_location_document,
 )
-from dagster_cloud_cli.core.graphql_client import GqlShimClient
+from dagster_cloud_cli.core.graphql_client import DagsterCloudGraphQLClient
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 from dagster_cloud_cli.utils import add_options
 
 DEFAULT_LOCATIONS_YAML_FILENAME = "locations.yaml"
 
 app = Typer(help="Manage your Dagster Cloud workspace.")
 
@@ -40,15 +40,15 @@
             kwargs["git"].get("commit_hash") if "git" in kwargs else kwargs.get("commit_hash")
         ),
         url=kwargs["git"].get("url") if "git" in kwargs else kwargs.get("git_url"),
     )
 
 
 def _add_or_update_location(
-    client: GqlShimClient,
+    client: DagsterCloudGraphQLClient,
     location_document: Dict[str, Any],
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     url: Optional[str] = None,
 ) -> None:
     try:
         gql.add_or_update_code_location(client, location_document)
@@ -116,14 +116,32 @@
             location_document,
             location_load_timeout=location_load_timeout,
             agent_heartbeat_timeout=agent_heartbeat_timeout,
             url=url,
         )
 
 
+def _format_error(load_error: Mapping[str, Any]):
+    result = [
+        load_error["message"],
+        "".join(load_error["stack"]),
+    ]
+
+    for chain_link in load_error["errorChain"]:
+        result.append(
+            "The above exception was caused by the following exception:"
+            if chain_link["isExplicitLink"]
+            else "The above exception occurred during handling of the following exception:"
+        )
+
+        result.extend([chain_link["error"]["message"], "".join(chain_link["error"]["stack"])])
+
+    return "\n".join(result)
+
+
 def wait_for_load(
     client,
     locations,
     location_load_timeout=DEFAULT_LOCATION_LOAD_TIMEOUT,
     agent_heartbeat_timeout=DEFAULT_LOCATION_LOAD_TIMEOUT,
     url: Optional[str] = None,
 ):
@@ -175,16 +193,16 @@
             ]
 
             if error_locations:
                 error_string = (
                     "Some locations failed to load after being synced by the agent:\n"
                     + "\n".join(
                         [
-                            f"Error loading {error_location}:"
-                            f" {nodes_by_location[error_location]['locationOrLoadError']}"
+                            f"Error loading {error_location}:\n"
+                            f"{_format_error(nodes_by_location[error_location]['locationOrLoadError'])}"
                             for error_location in error_locations
                         ]
                     )
                 )
                 raise ui.error(error_string)
             else:
                 ui.print(
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/config_utils.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/docker_runner.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/graphql_client.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/graphql_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,228 @@
 import logging
 import re
 import time
-from contextlib import ExitStack, contextmanager
+from contextlib import contextmanager
 from email.utils import mktime_tz, parsedate_tz
-from typing import Any, Dict, Mapping, Optional
+from typing import Any, Callable, Dict, Mapping, Optional
 
 import dagster._check as check
 import requests
 from requests.exceptions import (
     ConnectionError as RequestsConnectionError,
     HTTPError,
     ReadTimeout as RequestsReadTimeout,
 )
 
-from .errors import DagsterCloudHTTPError, DagsterCloudMaintenanceException, GraphQLStorageError
+from .errors import (
+    DagsterCloudAgentServerError,
+    DagsterCloudHTTPError,
+    DagsterCloudMaintenanceException,
+)
 from .headers.auth import DagsterCloudInstanceScope
 from .headers.impl import get_dagster_cloud_api_headers
 
 DEFAULT_RETRIES = 6
 DEFAULT_BACKOFF_FACTOR = 0.5
 DEFAULT_TIMEOUT = 60
 
 logger = logging.getLogger("dagster_cloud")
 
 
 RETRY_STATUS_CODES = [
-    # retry on server errors to recover on transient issue
-    500,
     502,
     503,
     504,
     429,
 ]
 
 
-class GqlShimClient:
-    """Adapter for gql.Client that wraps errors in human-readable format."""
+class DagsterCloudAgentHttpClient:
+    def __init__(
+        self,
+        session: requests.Session,
+        headers: Optional[Dict[str, Any]] = None,
+        verify: bool = True,
+        timeout: int = DEFAULT_TIMEOUT,
+        cookies: Optional[Dict[str, Any]] = None,
+        proxies: Optional[Dict[str, Any]] = None,
+        max_retries: int = 0,
+        backoff_factor: float = DEFAULT_BACKOFF_FACTOR,
+    ):
+        self.headers = headers or {}
+        self.verify = verify
+        self.timeout = timeout
+        self.cookies = cookies
+        self._session = session
+        self._proxies = proxies
+        self._max_retries = max_retries
+        self._backoff_factor = backoff_factor
+
+    @property
+    def session(self) -> requests.Session:
+        return self._session
+
+    def post(self, *args, **kwargs):
+        return self.execute("POST", *args, **kwargs)
+
+    def get(self, *args, **kwargs):
+        return self.execute("GET", *args, **kwargs)
+
+    def put(self, *args, **kwargs):
+        return self.execute("PUT", *args, **kwargs)
+
+    def execute(
+        self,
+        method: str,
+        url: str,
+        headers: Optional[Mapping[str, str]] = None,
+        idempotent: bool = False,
+        **kwargs,
+    ):
+        retry_on_read_timeout = idempotent or bool(
+            headers.get("Idempotency-Key") if headers else False
+        )
+
+        return _retry_loop(
+            lambda: self._execute_retry(method, url, headers, **kwargs),
+            max_retries=self._max_retries,
+            backoff_factor=self._backoff_factor,
+            retry_on_read_timeout=retry_on_read_timeout,
+        )
+
+    def _execute_retry(
+        self,
+        method: str,
+        url: str,
+        headers: Optional[Mapping[str, Any]],
+        **kwargs,
+    ):
+        response = self._session.request(
+            method,
+            url,
+            headers={
+                **(self.headers if self.headers is not None else {}),
+                **(headers if headers is not None else {}),
+            },
+            cookies=self.cookies,
+            timeout=self.timeout,
+            verify=self.verify,
+            proxies=self._proxies,
+            **kwargs,
+        )
+        try:
+            result = response.json()
+            if not isinstance(result, dict):
+                result = {}
+        except ValueError:
+            result = {}
+
+        if "maintenance" in result:
+            maintenance_info = result["maintenance"]
+            raise DagsterCloudMaintenanceException(
+                message=maintenance_info.get("message"),
+                timeout=maintenance_info.get("timeout"),
+                retry_interval=maintenance_info.get("retry_interval"),
+            )
+
+        if "errors" in result:
+            raise DagsterCloudAgentServerError(f"Error in GraphQL response: {result['errors']}")
+
+        response.raise_for_status()
+
+        return result
 
+
+def _retry_loop(
+    execute_retry: Callable,
+    max_retries: int,
+    backoff_factor: float,
+    retry_on_read_timeout: bool,
+):
+    start_time = time.time()
+    retry_number = 0
+    error_msg_set = set()
+    requested_sleep_time = None
+    while True:
+        try:
+            return execute_retry()
+        except (HTTPError, RequestsConnectionError, RequestsReadTimeout) as e:
+            retryable_error = False
+            if isinstance(e, HTTPError):
+                retryable_error = e.response.status_code in RETRY_STATUS_CODES
+                error_msg = e.response.status_code
+                requested_sleep_time = _get_retry_after_sleep_time(e.response.headers)
+            elif isinstance(e, RequestsReadTimeout):
+                retryable_error = retry_on_read_timeout
+                error_msg = str(e)
+            else:
+                retryable_error = True
+                error_msg = str(e)
+
+            error_msg_set.add(error_msg)
+            if retryable_error and retry_number < max_retries:
+                retry_number += 1
+                sleep_time = 0
+                if requested_sleep_time:
+                    sleep_time = requested_sleep_time
+                elif retry_number > 1:
+                    sleep_time = backoff_factor * (2 ** (retry_number - 1))
+
+                if sleep_time > 0:
+                    logger.warning(
+                        f"Error in Dagster Cloud request ({error_msg}). Retrying in"
+                        f" {sleep_time} seconds..."
+                    )
+                    time.sleep(sleep_time)
+                else:
+                    logger.warning(f"Error in Dagster Cloud request ({error_msg}). Retrying now.")
+            else:
+                # Throw the error straight if no retries were involved
+                if max_retries == 0 or not retryable_error:
+                    if isinstance(e, HTTPError):
+                        raise DagsterCloudHTTPError(e) from e
+                    else:
+                        raise
+                else:
+                    if len(error_msg_set) == 1:
+                        status_code_msg = str(next(iter(error_msg_set)))
+                    else:
+                        status_code_msg = str(error_msg_set)
+                    raise DagsterCloudAgentServerError(
+                        f"Max retries ({max_retries}) exceeded, too many"
+                        f" {status_code_msg} error responses."
+                    ) from e
+        except DagsterCloudMaintenanceException as e:
+            if time.time() - start_time > e.timeout:
+                raise
+
+            logger.warning(
+                "Dagster Cloud is currently unavailable due to scheduled maintenance. Retrying"
+                f" in {e.retry_interval} seconds..."
+            )
+            time.sleep(e.retry_interval)
+        except DagsterCloudAgentServerError:
+            raise
+        except Exception as e:
+            raise DagsterCloudAgentServerError(str(e)) from e
+
+
+class DagsterCloudGraphQLClient:
     def __init__(
         self,
         url: str,
         session: requests.Session,
         headers: Optional[Dict[str, Any]] = None,
         verify: bool = True,
         timeout: int = DEFAULT_TIMEOUT,
         cookies: Optional[Dict[str, Any]] = None,
         proxies: Optional[Dict[str, Any]] = None,
         max_retries: int = 0,
         backoff_factor: float = DEFAULT_BACKOFF_FACTOR,
     ):
-        self._exit_stack = ExitStack()
-
         self.url = url
         self.headers = headers
         self.verify = verify
         self.timeout = timeout
         self.cookies = cookies
         self._session = session
         self._proxies = proxies
@@ -68,89 +236,28 @@
     def execute(
         self,
         query: str,
         variable_values: Optional[Mapping[str, Any]] = None,
         headers: Optional[Mapping[str, str]] = None,
         idempotent_mutation: bool = False,
     ):
-        start_time = time.time()
-        retry_number = 0
-        error_msg_set = set()
-        requested_sleep_time = None
-        while True:
-            try:
-                return self._execute_retry(query, variable_values, headers)
-            except (HTTPError, RequestsConnectionError, RequestsReadTimeout) as e:
-                retryable_error = False
-                if isinstance(e, HTTPError):
-                    retryable_error = e.response.status_code in RETRY_STATUS_CODES
-                    error_msg = e.response.status_code
-                    requested_sleep_time = _get_retry_after_sleep_time(e.response.headers)
-                elif isinstance(e, RequestsReadTimeout):
-                    # "mutation " must appear in the document if its a mutation
-                    if "mutation " in query and not idempotent_mutation:
-                        # mutations can be made idempotent if they use Idempotency-Key header
-                        retryable_error = (
-                            bool(headers.get("Idempotency-Key")) if headers is not None else False
-                        )
-                    # otherwise assume its a query that is naturally idempotent
-                    else:
-                        retryable_error = True
-
-                    error_msg = str(e)
-                else:
-                    retryable_error = True
-                    error_msg = str(e)
+        if "mutation " in query and not idempotent_mutation:
+            # mutations can be made idempotent if they use Idempotency-Key header
+            retry_on_read_timeout = (
+                bool(headers.get("Idempotency-Key")) if headers is not None else False
+            )
+        else:
+            retry_on_read_timeout = True
 
-                error_msg_set.add(error_msg)
-                if retryable_error and retry_number < self._max_retries:
-                    retry_number += 1
-                    sleep_time = 0
-                    if requested_sleep_time:
-                        sleep_time = requested_sleep_time
-                    elif retry_number > 1:
-                        sleep_time = self._backoff_factor * (2 ** (retry_number - 1))
-
-                    if sleep_time > 0:
-                        logger.warning(
-                            f"Error in Dagster Cloud request ({error_msg}). Retrying in"
-                            f" {sleep_time} seconds..."
-                        )
-                        time.sleep(sleep_time)
-                    else:
-                        logger.warning(
-                            f"Error in Dagster Cloud request ({error_msg}). Retrying now."
-                        )
-                else:
-                    # Throw the error straight if no retries were involved
-                    if self._max_retries == 0 or not retryable_error:
-                        if isinstance(e, HTTPError):
-                            raise DagsterCloudHTTPError(e) from e
-                        else:
-                            raise GraphQLStorageError(str(e)) from e
-                    else:
-                        if len(error_msg_set) == 1:
-                            status_code_msg = str(next(iter(error_msg_set)))
-                        else:
-                            status_code_msg = str(error_msg_set)
-                        raise GraphQLStorageError(
-                            f"Max retries ({self._max_retries}) exceeded, too many"
-                            f" {status_code_msg} error responses."
-                        ) from e
-            except DagsterCloudMaintenanceException as e:
-                if time.time() - start_time > e.timeout:
-                    raise
-
-                logger.warning(
-                    "Dagster Cloud is currently unavailable due to scheduled maintenance. Retrying"
-                    f" in {e.retry_interval} seconds..."
-                )
-                time.sleep(e.retry_interval)
-            except Exception as e:
-                raise GraphQLStorageError(str(e)) from e
+        return _retry_loop(
+            lambda: self._execute_retry(query, variable_values, headers),
+            max_retries=self._max_retries,
+            backoff_factor=self._backoff_factor,
+            retry_on_read_timeout=retry_on_read_timeout,
+        )
 
     def _execute_retry(
         self,
         query: str,
         variable_values: Optional[Mapping[str, Any]],
         headers: Optional[Mapping[str, Any]],
     ):
@@ -186,17 +293,17 @@
             raise DagsterCloudMaintenanceException(
                 message=maintenance_info.get("message"),
                 timeout=maintenance_info.get("timeout"),
                 retry_interval=maintenance_info.get("retry_interval"),
             )
 
         if "errors" in result:
-            raise GraphQLStorageError(f"Error in GraphQL response: {result['errors']}")
-        else:
-            return result
+            raise DagsterCloudAgentServerError(f"Error in GraphQL response: {result['errors']}")
+
+        return result
 
 
 def get_agent_headers(config_value: Dict[str, Any], scope: DagsterCloudInstanceScope):
     return get_dagster_cloud_api_headers(
         config_value["agent_token"],
         scope=scope,
         deployment_name=config_value.get("deployment"),
@@ -206,21 +313,41 @@
 
 @contextmanager
 def create_graphql_requests_session():
     with requests.Session() as session:
         yield session
 
 
-def create_proxy_client(
+def create_agent_http_client(
+    session: requests.Session,
+    config_value: Dict[str, Any],
+    scope: DagsterCloudInstanceScope = DagsterCloudInstanceScope.DEPLOYMENT,
+):
+    return DagsterCloudAgentHttpClient(
+        headers=get_agent_headers(config_value, scope=scope),
+        verify=config_value.get("verify", True),
+        timeout=config_value.get("timeout", DEFAULT_TIMEOUT),
+        cookies=config_value.get("cookies", {}),
+        # Requests library modifies proxies dictionary so create a copy
+        proxies=(
+            check.is_dict(config_value.get("proxies")).copy() if config_value.get("proxies") else {}
+        ),
+        session=session,
+        max_retries=config_value.get("retries", DEFAULT_RETRIES),
+        backoff_factor=config_value.get("backoff_factor", DEFAULT_BACKOFF_FACTOR),
+    )
+
+
+def create_agent_graphql_client(
     session: requests.Session,
     url: str,
     config_value: Dict[str, Any],
     scope: DagsterCloudInstanceScope = DagsterCloudInstanceScope.DEPLOYMENT,
 ):
-    return GqlShimClient(
+    return DagsterCloudGraphQLClient(
         url=url,
         headers=get_agent_headers(config_value, scope=scope),
         verify=config_value.get("verify", True),
         timeout=config_value.get("timeout", DEFAULT_TIMEOUT),
         cookies=config_value.get("cookies", {}),
         # Requests library modifies proxies dictionary so create a copy
         proxies=(
@@ -250,15 +377,15 @@
 
     return max(seconds, 0)
 
 
 @contextmanager
 def create_cloud_webserver_client(url: str, api_token: str, retries=3):
     with create_graphql_requests_session() as session:
-        yield GqlShimClient(
+        yield DagsterCloudGraphQLClient(
             session=session,
             url=f"{url}/graphql",
             headers=get_dagster_cloud_api_headers(
                 api_token, scope=DagsterCloudInstanceScope.DEPLOYMENT
             ),
             max_retries=retries,
         )
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/headers/impl.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/impl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import platform
 from typing import Dict, Optional
 
 from ...version import __version__
-from .._utils import merge_dicts
 from .auth import (
     API_TOKEN_HEADER,
     DAGSTER_CLOUD_SCOPE_HEADER,
     DEPLOYMENT_NAME_HEADER,
     DagsterCloudInstanceScope,
 )
 from .versioning.constants import DAGSTER_CLOUD_VERSION_HEADER, PYTHON_VERSION_HEADER
@@ -14,17 +13,17 @@
 
 def get_dagster_cloud_api_headers(
     agent_token: str,
     scope: DagsterCloudInstanceScope,
     deployment_name: Optional[str] = None,
     additional_headers: Optional[Dict[str, str]] = None,
 ) -> Dict[str, str]:
-    return merge_dicts(
-        {
+    return {
+        **{
             API_TOKEN_HEADER: agent_token,
             PYTHON_VERSION_HEADER: platform.python_version(),
             DAGSTER_CLOUD_VERSION_HEADER: __version__,
             DAGSTER_CLOUD_SCOPE_HEADER: scope.value,
         },
-        {DEPLOYMENT_NAME_HEADER: deployment_name} if deployment_name else {},
-        additional_headers if additional_headers else {},
-    )
+        **({DEPLOYMENT_NAME_HEADER: deployment_name} if deployment_name else {}),
+        **(additional_headers if additional_headers else {}),
+    }
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/source.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pex_builder/util.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,21 @@
     version_tag = f"{python_version.major}{python_version.minor}"  # eg '38'
     # Resolves dependencies using the local interpreter, effectively allowing source distributions
     # to work (since they get built by the local interpreter).
     # If build_sdists is false and a binary distribution matching the platform below is not
     # available for a dependency, then the build will fail.
     # see also https://linear.app/elementl/issue/CLOUD-2023/pex-builds-fail-for-dbt-core-dependency
     resolve_local = ["--resolve-local-platforms"] if build_sdists else []
+    # This is mainly useful in local mac test environments
+    include_current = ["--platform=current"] if os.getenv("PEX_INCLUDE_CURRENT_PLATFORM") else []
     return [
         # this platform matches what can run on our serverless base images
         # the version tag is a major/minor string like "38"
         f"--platform=manylinux2014_x86_64-cp-{version_tag}-cp{version_tag}",
+        *include_current,
         # this ensures PEX_PATH is not cleared and any subprocess invoked can also use this.
         # this is important for running console scripts that use the pex environment (eg dbt)
         "--no-strip-pex-env",
         # use the latest version of pip bundled with pex - this will typically provide
         # the best dependency resolution logic. added in
         # https://github.com/pantsbuild/pex/releases/tag/v2.1.132
         "--pip-version=latest",
@@ -76,15 +79,15 @@
     requirements_filepaths: passed to the pex -r flag (aka --requirement)
 
     Platform:
     For the pex --platform tag used below, see pex --help and
     https://peps.python.org/pep-0425/
     https://peps.python.org/pep-0427/
 
-    Packages for the current platform are always included. (--platform=current)
+    Packages for the current platform are only included if requested with PEX_INCLUDE_CURRENT_PLATFORM
     The manylinux platform ensures pexes built on local machines (macos, windows) are compatible
     with linux on cloud.
 
     The python_version tuple eg ('3', '9') determines the target runtime environment. In theory
     we can build a pex in an environment without the target python version present.
     """
     flags = pex_flags.copy()
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/core/workspace.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/docker_utils.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/entrypoint.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/gql.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/gql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from contextlib import contextmanager, suppress
 from typing import Any, Dict, Generator, List, Optional, Sequence, cast
 
 from dagster_cloud_cli.types import (
     CliEventType,
 )
 
-from .core.graphql_client import GqlShimClient, create_cloud_webserver_client
+from .core.graphql_client import DagsterCloudGraphQLClient, create_cloud_webserver_client
 
 
 @contextmanager
 def graphql_client_from_url(
     url: str, token: str, retries: int = 3
-) -> Generator[GqlShimClient, None, None]:
+) -> Generator[DagsterCloudGraphQLClient, None, None]:
     with create_cloud_webserver_client(url.rstrip("/"), token, retries) as client:
         yield client
 
 
 def url_from_config(organization: str, deployment: Optional[str] = None) -> str:
     """Gets the Cloud webserver base url for a given organization and API token.
     Uses the default deployment if none is specified.
@@ -34,15 +34,15 @@
         deploymentId
         deploymentType
     }
 }
 """
 
 
-def fetch_full_deployments(client: GqlShimClient) -> List[Any]:
+def fetch_full_deployments(client: DagsterCloudGraphQLClient) -> List[Any]:
     return client.execute(FULL_DEPLOYMENTS_QUERY)["data"]["fullDeployments"]
 
 
 class CliInputCodeLocation:
     def __init__(
         self,
         name: str,
@@ -108,15 +108,15 @@
             }
         }
     }
 }
 """
 
 
-def fetch_agent_status(client: GqlShimClient) -> List[Any]:
+def fetch_agent_status(client: DagsterCloudGraphQLClient) -> List[Any]:
     return client.execute(AGENT_STATUS_QUERY)["data"]["agents"]
 
 
 WORKSPACE_ENTRIES_QUERY = """
 query CliWorkspaceEntries {
     workspace {
         workspaceEntries {
@@ -124,15 +124,15 @@
             serializedDeploymentMetadata
         }
     }
 }
 """
 
 
-def fetch_workspace_entries(client: GqlShimClient) -> List[Any]:
+def fetch_workspace_entries(client: DagsterCloudGraphQLClient) -> List[Any]:
     return client.execute(WORKSPACE_ENTRIES_QUERY)["data"]["workspace"]["workspaceEntries"]
 
 
 REPOSITORY_LOCATIONS_QUERY = """
 query CliLocationsQuery {
   workspaceOrError {
     __typename
@@ -145,28 +145,35 @@
                 __typename
                 ... on RepositoryLocation {
                     name
                 }
                 ... on PythonError {
                     message
                     stack
+                    errorChain {
+                        isExplicitLink
+                        error {
+                            message
+                            stack
+                        }
+                    }
                 }
             }
         }
     }
     ... on PythonError {
         message
         stack
     }
   }
 }
 """
 
 
-def fetch_code_locations(client: GqlShimClient) -> List[Any]:
+def fetch_code_locations(client: DagsterCloudGraphQLClient) -> List[Any]:
     result = client.execute(REPOSITORY_LOCATIONS_QUERY)["data"]["workspaceOrError"]
     if result["__typename"] != "Workspace":
         raise Exception("Unable to query code locations: ", result["message"])
     return result["locationEntries"]
 
 
 ADD_OR_UPDATE_LOCATION_FROM_DOCUMENT_MUTATION = """
@@ -184,15 +191,17 @@
             errors
         }
     }
 }
 """
 
 
-def add_or_update_code_location(client: GqlShimClient, location_document: Dict[str, Any]) -> None:
+def add_or_update_code_location(
+    client: DagsterCloudGraphQLClient, location_document: Dict[str, Any]
+) -> None:
     result = client.execute(
         ADD_OR_UPDATE_LOCATION_FROM_DOCUMENT_MUTATION,
         variable_values={"document": location_document},
     )["data"]["addOrUpdateLocationFromDocument"]
     if result["__typename"] == "InvalidLocationError":
         raise Exception("Error in location config:\n" + "\n".join(result["errors"]))
     elif result["__typename"] != "WorkspaceEntry":
@@ -211,15 +220,15 @@
             stack
         }
     }
 }
 """
 
 
-def delete_code_location(client: GqlShimClient, location_name: str) -> None:
+def delete_code_location(client: DagsterCloudGraphQLClient, location_name: str) -> None:
     result = client.execute(
         DELETE_LOCATION_MUTATION, variable_values={"locationName": location_name}
     )
 
     if result["data"]["deleteLocation"]["__typename"] != "DeleteLocationSuccess":
         raise Exception(f"Unable to delete location: {result['data']['deleteLocation']}")
 
@@ -242,15 +251,15 @@
         }
     }
 }
 """
 
 
 def reconcile_code_locations(
-    client: GqlShimClient, locations_document: Dict[str, Any]
+    client: DagsterCloudGraphQLClient, locations_document: Dict[str, Any]
 ) -> List[str]:
     result = client.execute(
         RECONCILE_LOCATIONS_FROM_DOCUMENT_MUTATION,
         variable_values={"document": locations_document},
     )
 
     if (
@@ -275,15 +284,15 @@
         __typename
         document
     }
 }
 """
 
 
-def fetch_locations_as_document(client: GqlShimClient) -> Dict[str, Any]:
+def fetch_locations_as_document(client: DagsterCloudGraphQLClient) -> Dict[str, Any]:
     result = client.execute(GET_LOCATIONS_AS_DOCUMENT_QUERY)
 
     return result["data"]["locationsAsDocument"]["document"]
 
 
 SET_DEPLOYMENT_SETTINGS_MUTATION = """
     mutation CliSetDeploymentSettings($deploymentSettings: DeploymentSettingsInput!) {
@@ -300,15 +309,17 @@
                 stack
             }
         }
     }
 """
 
 
-def set_deployment_settings(client: GqlShimClient, deployment_settings: Dict[str, Any]) -> None:
+def set_deployment_settings(
+    client: DagsterCloudGraphQLClient, deployment_settings: Dict[str, Any]
+) -> None:
     result = client.execute(
         SET_DEPLOYMENT_SETTINGS_MUTATION,
         variable_values={"deploymentSettings": deployment_settings},
     )
 
     if result["data"]["setDeploymentSettings"]["__typename"] != "DeploymentSettings":
         raise Exception(f"Unable to set deployment settings: {result}")
@@ -319,15 +330,15 @@
         deploymentSettings {
             settings
         }
     }
 """
 
 
-def get_deployment_settings(client: GqlShimClient) -> Dict[str, Any]:
+def get_deployment_settings(client: DagsterCloudGraphQLClient) -> Dict[str, Any]:
     result = client.execute(DEPLOYMENT_SETTINGS_QUERY)
 
     if result.get("data", {}).get("deploymentSettings", {}).get("settings") is None:
         raise Exception(f"Unable to get deployment settings: {result}")
 
     return result["data"]["deploymentSettings"]["settings"]
 
@@ -349,22 +360,25 @@
                 ... on SlackAlertPolicyNotification {
                     slackWorkspaceName
                     slackChannelName
                 }
                 ... on MicrosoftTeamsAlertPolicyNotification {
                     webhookUrl
                 }
+                ... on PagerdutyAlertPolicyNotification {
+                    integrationKey
+                }
             }
             enabled
         }
     }
 """
 
 
-def get_alert_policies(client: GqlShimClient) -> Dict[str, Any]:
+def get_alert_policies(client: DagsterCloudGraphQLClient) -> Dict[str, Any]:
     result = client.execute(ALERT_POLICIES_QUERY)
 
     if result.get("data", {}).get("alertPolicies", {}) is None:
         raise Exception(f"Unable to get deployment settings: {result}")
 
     return result["data"]["alertPolicies"]
 
@@ -390,15 +404,15 @@
             }
         }
     }
 """
 
 
 def reconcile_alert_policies(
-    client: GqlShimClient, alert_policy_inputs: Sequence[dict]
+    client: DagsterCloudGraphQLClient, alert_policy_inputs: Sequence[dict]
 ) -> Sequence[str]:
     result = client.execute(
         RECONCILE_ALERT_POLICIES_FROM_DOCUMENT_MUTATION,
         variable_values={"document": alert_policy_inputs},
     )
 
     if (
@@ -428,15 +442,17 @@
                 stack
             }
         }
     }
 """
 
 
-def set_organization_settings(client: GqlShimClient, organization_settings: Dict[str, Any]) -> None:
+def set_organization_settings(
+    client: DagsterCloudGraphQLClient, organization_settings: Dict[str, Any]
+) -> None:
     result = client.execute(
         SET_ORGANIZATION_SETTINGS_MUTATION,
         variable_values={"organizationSettings": organization_settings},
     )
 
     if result["data"]["setOrganizationSettings"]["__typename"] != "OrganizationSettings":
         raise Exception(f"Unable to set organization settings: {result}")
@@ -447,15 +463,15 @@
         organizationSettings {
             settings
         }
     }
 """
 
 
-def get_organization_settings(client: GqlShimClient) -> Dict[str, Any]:
+def get_organization_settings(client: DagsterCloudGraphQLClient) -> Dict[str, Any]:
     result = client.execute(ORGANIZATION_SETTINGS_QUERY)
 
     if result.get("data", {}).get("organizationSettings", {}).get("settings") is None:
         raise Exception(f"Unable to get organization settings: {result}")
 
     return result["data"]["organizationSettings"]["settings"]
 
@@ -476,15 +492,15 @@
         }
     }
 }
 """
 
 
 def create_or_update_branch_deployment(
-    client: GqlShimClient,
+    client: DagsterCloudGraphQLClient,
     repo_name: str,
     branch_name: str,
     commit_hash: str,
     timestamp: float,
     branch_url: Optional[str] = None,
     pull_request_url: Optional[str] = None,
     pull_request_status: Optional[str] = None,
@@ -551,15 +567,15 @@
             }
         }
     }
 """
 
 
 def launch_run(
-    client: GqlShimClient,
+    client: DagsterCloudGraphQLClient,
     location_name: str,
     repo_name: str,
     job_name: str,
     tags: Dict[str, Any],
     config: Dict[str, Any],
     asset_keys: Optional[List[str]],
 ) -> str:
@@ -594,15 +610,15 @@
         registryAllowCustomBase
         registryUrl
     }
 }
 """
 
 
-def get_ecr_info(client: GqlShimClient) -> Any:
+def get_ecr_info(client: DagsterCloudGraphQLClient) -> Any:
     data = client.execute(GET_ECR_CREDS_QUERY)["data"]
     return {
         "registry_url": data["serverless"]["registryUrl"],
         "aws_region": data["serverless"]["awsRegion"],
         "aws_auth_token": data["serverless"]["awsAuthToken"],
         "allow_custom_base": data["serverless"]["registryAllowCustomBase"],
     }
@@ -617,15 +633,15 @@
 			status
 		}
     }
 }
 """
 
 
-def run_status(client: GqlShimClient, run_id: str) -> Any:
+def run_status(client: DagsterCloudGraphQLClient, run_id: str) -> Any:
     data = client.execute(
         GET_RUN_STATUS_QUERY,
         variable_values={"runId": run_id},
     )["data"]
     if data["runOrError"]["__typename"] != "Run":
         return None
 
@@ -643,15 +659,15 @@
  ) {
    markCliEvent(eventType: $eventType, durationSeconds: $durationSeconds, success: $success, tags: $tags, message: $message)
  }
  """
 
 
 def mark_cli_event(
-    client: GqlShimClient,
+    client: DagsterCloudGraphQLClient,
     event_type: CliEventType,
     duration_seconds: float,
     success: bool = True,
     tags: Optional[List[str]] = None,
     message: Optional[str] = None,
 ) -> Any:
     with suppress(Exception):
@@ -693,26 +709,26 @@
             stack
         }
     }
 }
 """
 
 
-def get_deployment_by_name(client: GqlShimClient, deployment: str) -> Dict[str, Any]:
+def get_deployment_by_name(client: DagsterCloudGraphQLClient, deployment: str) -> Dict[str, Any]:
     result = client.execute(
         GET_DEPLOYMENT_BY_NAME_QUERY, variable_values={"deploymentName": deployment}
     )["data"]["deploymentByName"]
     if not result["__typename"] == "DagsterCloudDeployment":
         raise Exception(f"Unable to find deployment {deployment}")
 
     return result
     raise Exception(f"Unable to find deployment {deployment}")
 
 
-def delete_branch_deployment(client: GqlShimClient, deployment: str) -> Any:
+def delete_branch_deployment(client: DagsterCloudGraphQLClient, deployment: str) -> Any:
     deployment_info = get_deployment_by_name(client, deployment)
     if not deployment_info["deploymentType"] == "BRANCH":
         raise Exception(f"Deployment {deployment} is not a branch deployment")
 
     result = client.execute(
         DELETE_DEPLOYMENT_MUTATION,
         variable_values={"deploymentId": deployment_info["deploymentId"]},
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/pex_utils.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/types.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/ui.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli/utils.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 dagster_cloud_cli/commands/organization/saml/commands.py
 dagster_cloud_cli/commands/run/__init__.py
 dagster_cloud_cli/commands/serverless/Dockerfile
 dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
 dagster_cloud_cli/commands/serverless/__init__.py
 dagster_cloud_cli/commands/workspace/__init__.py
 dagster_cloud_cli/core/__init__.py
-dagster_cloud_cli/core/_utils.py
+dagster_cloud_cli/core/alert_types.py
+dagster_cloud_cli/core/artifacts.py
 dagster_cloud_cli/core/docker_runner.py
 dagster_cloud_cli/core/errors.py
 dagster_cloud_cli/core/graphql_client.py
 dagster_cloud_cli/core/pydantic_yaml.py
 dagster_cloud_cli/core/workspace.py
 dagster_cloud_cli/core/headers/__init__.py
 dagster_cloud_cli/core/headers/auth.py
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_check.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_gql.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_gql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from unittest.mock import MagicMock
 
-from dagster_cloud_cli.core.graphql_client import GqlShimClient
+from dagster_cloud_cli.core.graphql_client import DagsterCloudGraphQLClient
 from dagster_cloud_cli.gql import graphql_client_from_url, mark_cli_event
 
 
 def test_graphql_client_from_url_doesnt_raise():
     with graphql_client_from_url(str(None), str(None)):
         pass
 
     with graphql_client_from_url("bad-url", "bad-token"):
         pass
 
 
 def test_mark_cli_event_doesnt_raise():
-    client = MagicMock(GqlShimClient, autospec=True)
+    client = MagicMock(DagsterCloudGraphQLClient, autospec=True)
     client.execute.side_effect = Exception("boom")
 
     mark_cli_event(
         client=client,
         event_type=MagicMock(),
         duration_seconds=MagicMock(),
         tags=MagicMock(),
```

### Comparing `dagster-cloud-cli-1.6.9/dagster_cloud_cli_tests/test_metrics.py` & `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.6.9/setup.py` & `dagster-cloud-cli-1.7.0/setup.py`

 * *Files identical despite different names*

