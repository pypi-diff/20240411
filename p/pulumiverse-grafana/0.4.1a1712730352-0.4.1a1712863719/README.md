# Comparing `tmp/pulumiverse_grafana-0.4.1a1712730352.tar.gz` & `tmp/pulumiverse_grafana-0.4.1a1712863719.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_grafana-0.4.1a1712730352.tar", last modified: Wed Apr 10 06:31:25 2024, max compression
+gzip compressed data, was "pulumiverse_grafana-0.4.1a1712863719.tar", last modified: Thu Apr 11 19:34:17 2024, max compression
```

## Comparing `pulumiverse_grafana-0.4.1a1712730352.tar` & `pulumiverse_grafana-0.4.1a1712863719.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:31:25.576253 pulumiverse_grafana-0.4.1a1712730352/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 06:31:25.576253 pulumiverse_grafana-0.4.1a1712730352/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:31:25.576253 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   381605 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    21810 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    21514 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_access_policy_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_plugin_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)    58137 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack_service_account_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:31:25.576253 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    68822 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/contact_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/dashboard_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/dashboard_public.py
--rw-r--r--   0 runner    (1001) docker     (127)    44410 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/data_source_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    18208 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/folder_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_cloud_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_cloud_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_cloud_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_library_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_on_call_slack_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_escalation_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_outgoing_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_organization_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_slos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_synthetic_monitoring_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_synthetic_monitoring_probes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/library_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/machine_learning_holiday.py
--rw-r--r--   0 runner    (1001) docker     (127)    30294 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/machine_learning_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/machine_learning_outlier_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/message_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/mute_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    31101 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_escalation_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    40193 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_on_call_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)    38049 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_outgoing_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    23349 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/organization_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)   361617 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    36890 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    29510 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/rule_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/service_account_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/service_account_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    24513 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/sso_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    63441 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/synthetic_monitoring_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    22004 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/synthetic_monitoring_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/synthetic_monitoring_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)    25601 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/team_external_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:31:25.576253 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:31:25.576253 pulumiverse_grafana-0.4.1a1712730352/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-10 06:31:25.000000 pulumiverse_grafana-0.4.1a1712730352/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:34:17.044369 pulumiverse_grafana-0.4.1a1712863719/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-11 19:34:17.044369 pulumiverse_grafana-0.4.1a1712863719/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:34:17.040369 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   381605 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21810 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21514 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_access_policy_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_plugin_installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58137 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack_service_account_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:34:17.044369 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68822 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/contact_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/dashboard_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/dashboard_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44410 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/data_source_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18208 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14313 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/folder_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_cloud_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_cloud_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_cloud_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_library_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_on_call_slack_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_escalation_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_outgoing_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_organization_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_slos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_synthetic_monitoring_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_synthetic_monitoring_probes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/library_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/machine_learning_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30294 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/machine_learning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/machine_learning_outlier_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/message_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/mute_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31101 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_escalation_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40193 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_on_call_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38049 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_outgoing_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23349 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/organization_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)   361617 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36890 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29510 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/rule_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/service_account_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/service_account_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24513 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/sso_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63441 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/synthetic_monitoring_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22004 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/synthetic_monitoring_installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/synthetic_monitoring_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25601 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/team_external_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:34:17.044369 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:34:17.044369 pulumiverse_grafana-0.4.1a1712863719/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-11 19:34:16.000000 pulumiverse_grafana-0.4.1a1712863719/setup.py
```

### Comparing `pulumiverse_grafana-0.4.1a1712730352/PKG-INFO` & `pulumiverse_grafana-0.4.1a1712863719/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_grafana
-Version: 0.4.1a1712730352
+Version: 0.4.1a1712863719
 Summary: A Pulumi package for creating and managing grafana.
 Home-page: https://grafana.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-grafana
 Keywords: pulumi grafana pulumiverse
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_grafana-0.4.1a1712730352/README.md` & `pulumiverse_grafana-0.4.1a1712863719/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/__init__.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/_inputs.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/_utilities.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/annotation.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/annotation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/api_key.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_access_policy.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_access_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_access_policy_token.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_access_policy_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_api_key.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_plugin_installation.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_plugin_installation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack_api_key.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack_service_account.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/cloud_stack_service_account_token.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/cloud_stack_service_account_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/config/vars.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/contact_point.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/contact_point.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/dashboard.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/dashboard_permission.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/dashboard_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/dashboard_public.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/dashboard_public.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/data_source.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/data_source.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/data_source_permission.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/data_source_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/folder.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/folder.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/folder_permission.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/folder_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_cloud_ips.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_cloud_ips.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_cloud_organization.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_cloud_organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_cloud_stack.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_cloud_stack.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_dashboard.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_dashboards.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_dashboards.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_data_source.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_data_source.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_folder.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_folder.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_folders.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_folders.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_library_panel.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_library_panel.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_on_call_slack_channel.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_on_call_slack_channel.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_action.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_action.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_escalation_chain.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_escalation_chain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_outgoing_webhook.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_outgoing_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_schedule.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_team.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_user.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_oncall_user_group.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_oncall_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_organization.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_organization_preferences.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_organization_preferences.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_role.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_service_account.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_slos.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_slos.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_synthetic_monitoring_probe.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_synthetic_monitoring_probe.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_synthetic_monitoring_probes.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_synthetic_monitoring_probes.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_team.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_user.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/get_users.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/library_panel.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/library_panel.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/machine_learning_holiday.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/machine_learning_holiday.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/machine_learning_job.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/machine_learning_job.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/machine_learning_outlier_detector.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/machine_learning_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/message_template.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/message_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/mute_timing.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/mute_timing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/notification_policy.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_escalation.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_escalation_chain.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_escalation_chain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_integration.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_integration.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_on_call_shift.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_on_call_shift.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_outgoing_webhook.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_outgoing_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_route.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_route.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/oncall_schedule.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/oncall_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/organization.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/organization_preference.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/organization_preference.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/outputs.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/playlist.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/playlist.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/provider.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/report.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/report.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/role.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/role_assignment.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/rule_group.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/rule_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/service_account.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/service_account_permission.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/service_account_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/service_account_token.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/service_account_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/slo.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/slo.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/sso_settings.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/sso_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/synthetic_monitoring_check.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/synthetic_monitoring_check.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/synthetic_monitoring_installation.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/synthetic_monitoring_installation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/synthetic_monitoring_probe.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/synthetic_monitoring_probe.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/team.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/team_external_group.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/team_external_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana/user.py` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana/user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/PKG-INFO` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-grafana
-Version: 0.4.1a1712730352
+Version: 0.4.1a1712863719
 Summary: A Pulumi package for creating and managing grafana.
 Home-page: https://grafana.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-grafana
 Keywords: pulumi grafana pulumiverse
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_grafana-0.4.1a1712730352/pulumiverse_grafana.egg-info/SOURCES.txt` & `pulumiverse_grafana-0.4.1a1712863719/pulumiverse_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_grafana-0.4.1a1712730352/setup.py` & `pulumiverse_grafana-0.4.1a1712863719/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.1a1712730352"
+VERSION = "0.4.1a1712863719"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "grafana Pulumi Package - Development Version"
```

