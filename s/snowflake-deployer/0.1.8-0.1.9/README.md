# Comparing `tmp/snowflake-deployer-0.1.8.tar.gz` & `tmp/snowflake-deployer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-deployer-0.1.8.tar", last modified: Thu Oct  5 04:12:26 2023, max compression
+gzip compressed data, was "snowflake-deployer-0.1.9.tar", last modified: Fri Oct  6 21:06:17 2023, max compression
```

## Comparing `snowflake-deployer-0.1.8.tar` & `snowflake-deployer-0.1.9.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.518757 snowflake-deployer-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-05 04:12:26.518757 snowflake-deployer-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-05 04:12:26.518757 snowflake-deployer-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.502757 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-05 04:12:26.000000 snowflake-deployer-0.1.8/snowflake_deployer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.502757 snowflake-deployer-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.502757 snowflake-deployer-0.1.8/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/common/processing_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.502757 snowflake-deployer-0.1.8/src/configurator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11475 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.506757 snowflake-deployer-0.1.8/src/deploy_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deploy_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deploy_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.506757 snowflake-deployer-0.1.8/src/deployer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.506757 snowflake-deployer-0.1.8/src/deployer/object_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_masking_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_row_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/deployer/object_types/deploy_warehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.506757 snowflake-deployer-0.1.8/src/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/snowflake/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/column_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/columns_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/current_role_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/database_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/database_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/database_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/databases_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/deploy_code_hash_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/deploy_code_hash_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/deploy_db_check_installed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/deploy_db_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/deploy_hash_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/deploy_hash_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/function_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/function_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/function_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/functions_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/grants_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/masking_policies_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/masking_policy_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/masking_policy_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/masking_policy_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/network_policies_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/object_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/object_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/object_row_access_policy_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/objects_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/ownership_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/procedure_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/procedure_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/procedure_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/procedures_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_check_assigned.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_grant_to_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_handle_ownership.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/role_parent_grants_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/roles_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policies_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policy_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policy_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policy_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/schema_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/schema_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/schema_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/schemas_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tag_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tag_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tag_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tag_masking_policy_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tag_references_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tags_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/task_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/task_check_exist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/task_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/tasks_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/warehouse_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/warehouse_check_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/warehouse_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/functions/warehouses_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake/snowflake_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30393 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake_generate_rsa_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    21842 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/snowflake_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/validator/object_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_masking_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_row_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/object_types/validate_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/wrangler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/wrangler/object_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_masking_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_network_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_row_access_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/wrangler/wrangler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/yaml_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_reader/yaml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.514757 snowflake-deployer-0.1.8/src/yaml_writer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:26.518757 snowflake-deployer-0.1.8/src/yaml_writer/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_database_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_function_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_masking_policy_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_object_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_procedure_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_role_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_row_access_policy_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_schema_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_tag_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_task_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/functions/write_warehouse_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    18661 2023-10-05 04:12:18.000000 snowflake-deployer-0.1.8/src/yaml_writer/yaml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:17.001863 snowflake-deployer-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-06 21:06:17.001863 snowflake-deployer-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-06 21:06:17.001863 snowflake-deployer-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-06 21:06:16.000000 snowflake-deployer-0.1.9/snowflake_deployer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/common/processing_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/deploy_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deploy_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deploy_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/deployer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/deployer/object_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_masking_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_row_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/deployer/object_types/deploy_warehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.989863 snowflake-deployer-0.1.9/src/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/snowflake/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/column_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/columns_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/current_role_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/database_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/database_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/database_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/databases_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/deploy_code_hash_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/deploy_code_hash_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/deploy_db_check_installed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/deploy_db_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/deploy_hash_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/deploy_hash_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/function_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/function_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/function_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/functions_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/grants_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/masking_policies_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/masking_policy_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/masking_policy_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/masking_policy_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/network_policies_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/object_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/object_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/object_row_access_policy_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/objects_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/ownership_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/procedure_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/procedure_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/procedure_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/procedures_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_check_assigned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_grant_to_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_handle_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/role_parent_grants_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/roles_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policies_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policy_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policy_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policy_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/schema_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/schema_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/schema_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/schemas_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tag_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tag_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tag_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tag_masking_policy_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tag_references_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tags_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/task_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/task_check_exist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/task_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/tasks_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/warehouse_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/warehouse_check_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/warehouse_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/functions/warehouses_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake/snowflake_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30393 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake_generate_rsa_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21860 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/snowflake_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/validator/object_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_masking_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_row_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/object_types/validate_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/wrangler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/wrangler/object_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_masking_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_network_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_row_access_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/wrangler/wrangler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/yaml_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_reader/yaml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:16.997863 snowflake-deployer-0.1.9/src/yaml_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:17.001863 snowflake-deployer-0.1.9/src/yaml_writer/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_database_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_function_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_masking_policy_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_object_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_procedure_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_role_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_row_access_policy_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_schema_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_tag_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_task_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/functions/write_warehouse_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18661 2023-10-06 21:06:09.000000 snowflake-deployer-0.1.9/src/yaml_writer/yaml_writer.py
```

### Comparing `snowflake-deployer-0.1.8/LICENSE` & `snowflake-deployer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/setup.py` & `snowflake-deployer-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #        for requirement
 #        in pkg_resources.parse_requirements(requirements_txt)
 #    ]
 
 
 setup(
     name='snowflake-deployer',
-    version='0.1.8',
+    version='0.1.9',
     description='Snowflake state based deployer',
     long_description='Deploy objects to Snowflake instance in a stateful manner.  See Project Docs for details.',
     long_description_content_type="text/markdown",
     author='Justin Hanson, Jernej Plankelj',
     entry_points = {
         'console_scripts': ['snowflake-deployer=src.cli:cli'],
         #'console_scripts': ['snowflake_deployer=src.command_line:cli'],
@@ -27,8 +27,8 @@
     include_package_data=True,
     packages=find_packages(),
     keywords = ['SNOWFLAKE','DATAOPS','DEVOPS','DATA','DEPLOYMENT'],
     project_urls = {
         'Project Docs': 'https://metaopslabs.github.io/snowflake_deployer/'
     }
 
-) 
+)
```

### Comparing `snowflake-deployer-0.1.8/snowflake_deployer.egg-info/SOURCES.txt` & `snowflake-deployer-0.1.9/snowflake_deployer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/cli.py` & `snowflake-deployer-0.1.9/src/cli.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/common/common.py` & `snowflake-deployer-0.1.9/src/common/common.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/common/exceptions.py` & `snowflake-deployer-0.1.9/src/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/configurator/configurator.py` & `snowflake-deployer-0.1.9/src/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deploy_logger/logger.py` & `snowflake-deployer-0.1.9/src/deploy_logger/logger.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/deployer.py` & `snowflake-deployer-0.1.9/src/deployer/deployer.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_database.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_database.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_function.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_masking_policy.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_masking_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_object.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_object.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_procedure.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_role.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_role.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_row_access_policy.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_row_access_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_schema.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_schema.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_tag.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_tag.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_task.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_task.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/deployer/object_types/deploy_warehouse.py` & `snowflake-deployer-0.1.9/src/deployer/object_types/deploy_warehouse.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/column_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/column_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/columns_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/columns_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/database_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/database_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/database_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/database_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/database_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/database_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/databases_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/databases_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/deploy_code_hash_apply.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/deploy_code_hash_apply.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/deploy_code_hash_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/deploy_code_hash_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/deploy_db_install.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/deploy_db_install.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/deploy_hash_apply.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/deploy_hash_apply.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/deploy_hash_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/deploy_hash_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/function_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/function_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/function_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/function_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/function_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/function_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/functions_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/functions_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/grants_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/grants_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/masking_policies_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/masking_policies_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/masking_policy_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/masking_policy_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/masking_policy_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/masking_policy_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/masking_policy_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/masking_policy_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/network_policies_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/network_policies_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/object_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/object_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/object_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/object_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/object_row_access_policy_reference.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/object_row_access_policy_reference.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/objects_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/objects_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/procedure_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/procedure_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/procedure_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/procedure_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/procedure_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/procedure_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/procedures_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/procedures_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_check_assigned.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_check_assigned.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_grant_to_role.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_grant_to_role.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_handle_ownership.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_handle_ownership.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/role_parent_grants_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/role_parent_grants_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/roles_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/roles_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policies_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policies_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policy_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policy_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policy_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policy_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/row_access_policy_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/row_access_policy_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/schema_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/schema_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/schema_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/schema_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/schema_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/schema_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/schemas_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/schemas_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tag_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tag_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tag_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tag_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tag_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tag_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tag_masking_policy_reference.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tag_masking_policy_reference.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tag_references_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tag_references_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tags_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tags_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/task_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/task_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/task_check_exist.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/task_check_exist.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/task_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/task_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/tasks_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/tasks_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/warehouse_alter.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/warehouse_alter.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/warehouse_check_exists.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/warehouse_check_exists.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/warehouse_create.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/warehouse_create.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/functions/warehouses_get.py` & `snowflake-deployer-0.1.9/src/snowflake/functions/warehouses_get.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake/snowflake_client.py` & `snowflake-deployer-0.1.9/src/snowflake/snowflake_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake_deploy.py` & `snowflake-deployer-0.1.9/src/snowflake_deploy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake_generate_rsa_keys.py` & `snowflake-deployer-0.1.9/src/snowflake_generate_rsa_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/snowflake_import.py` & `snowflake-deployer-0.1.9/src/snowflake_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         threads = []
 
         #####################################################
         # DATA START
         
         # Databases
         #dbs = sf.databases_get(excluded_databases,config['DEPLOY_DATABASE_NAME'],config['ENV_DATABASE_PREFIX'], ignore_roles_list)
-        dbs = wrangler.wrangle_database(config['ENV_DATABASE_PREFIX'], config['ENV_ROLE_PREFIX'], excluded_databases, config['DEPLOY_DATABASE_NAME'], ignore_roles_list, config['DEPLOY_TAGS'],config['DEPLOY_ROLE'], available_roles, config['HANDLE_OWNERSHIP'])
+        dbs = wrangler.wrangle_database(config['ENV_DATABASE_PREFIX'], config['ENV_ROLE_PREFIX'], excluded_databases, config['DEPLOY_DATABASE_NAME'], ignore_roles_list, config['DEPLOY_TAGS'],config['DEPLOY_ROLE'], available_roles, config['HANDLE_OWNERSHIP'], import_databases)
         for db in dbs:
             if db['DATABASE_NAME'] not in excluded_databases:
                 if import_databases == [] or db['DATABASE_NAME'] in import_databases:
                     tn =  db['DATABASE_NAME'] + ' [database]'
                     t = threading.Thread(target=task_db, name=tn, args=(semaphore, writer, sf, config, tn, db, current_role, available_roles, logger))
                     threads.append(t)
```

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_database.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_database.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_function.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_masking_policy.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_masking_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_object.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_object.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_procedure.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_role.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_role.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_row_access_policy.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_row_access_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_schema.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_schema.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_tag.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_tag.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_task.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_task.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/object_types/validate_warehouse.py` & `snowflake-deployer-0.1.9/src/validator/object_types/validate_warehouse.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/validator/validator.py` & `snowflake-deployer-0.1.9/src/validator/validator.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_column.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_column.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_database.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 from src.util.util import remove_prefix
-def wrangle_database(self, env_database_prefix:str, env_role_prefix:str, excluded_databases:list[str], deploy_db_name:str, ignore_roles_list:str, deploy_tag_list:list[str], current_role:str, available_roles:list[str], handle_ownership)->dict:
+def wrangle_database(self, env_database_prefix:str, env_role_prefix:str, excluded_databases:list[str], deploy_db_name:str, ignore_roles_list:str, deploy_tag_list:list[str], current_role:str, available_roles:list[str], handle_ownership, import_databases:list[str])->dict:
     if env_database_prefix is None:
         env_database_prefix = ''
     if env_role_prefix is None:
         env_role_prefix = ''
         
     dbs = self._sf.databases_get(env_database_prefix)  
     
     data = []
     for db in dbs:
         if db['DATABASE_NAME'] not in excluded_databases and db['DATABASE_NAME'] != deploy_db_name:
-            db['DATABASE_NAME_SANS_ENV'] = remove_prefix(db['DATABASE_NAME'],env_database_prefix)   
-            
-            db['OWNER'] = self._handle_ownership(handle_ownership, db['OWNER'], 'database', db['DATABASE_NAME'], current_role, available_roles)
+            if import_databases == [] or db['DATABASE_NAME'] in import_databases:
+                db['DATABASE_NAME_SANS_ENV'] = remove_prefix(db['DATABASE_NAME'],env_database_prefix)   
+                
+                db['OWNER'] = self._handle_ownership(handle_ownership, db['OWNER'], 'database', db['DATABASE_NAME'], current_role, available_roles)
 
-            if db['OWNER'] not in ignore_roles_list: # if role managed by deployer (not out of the box) then add the jinja reference
-                db['OWNER'] = self.create_jinja_role_instance(db['OWNER'])
-            
-            tags = []
-            tags_raw = self._sf.tag_references_get(db['DATABASE_NAME'], db['DATABASE_NAME'], 'database')
-            for t in tags_raw:
-                if not (t['TAG_DATABASE'] == deploy_db_name and t['TAG_SCHEMA'] == 'TAG' and t['TAG_NAME'] in deploy_tag_list):
-                    tv = {}
-                    db_name = remove_prefix(t['TAG_DATABASE'],env_database_prefix)
-                    #tv['name'] = self.create_jinja_ref(db_name, t['TAG_SCHEMA'], t['TAG_NAME'])
-                    #tv['value'] = t['TAG_VALUE']
-                    tag_name = self.create_jinja_ref(db_name, t['TAG_SCHEMA'], t['TAG_NAME'])
-                    tv[tag_name] = t['TAG_VALUE']
-                    tags.append(tv)
-            db['TAGS'] = tags
-            
-            grants_raw = self._sf.grants_get(db['DATABASE_NAME'], 'database')
-            grants = []
-            for g in grants_raw:
-                if g['PRIVILEGE'] != 'OWNERSHIP' and g['GRANTEE_NAME'] != current_role and g['GRANT_TYPE'] == 'ROLE':
-                    grant = {}
-                    role_name = remove_prefix(g['GRANTEE_NAME'],env_role_prefix)
-                    grant_to = self.create_jinja_role_instance(role_name) if role_name not in ignore_roles_list else role_name
-                    grant[grant_to] = g['PRIVILEGE']
-                    if g['GRANT_OPTION'] is True:
-                        grant['GRANT_OPTION'] = True
-                    grants.append(grant)
-            grants_combined = self._combine_grants(grants)
-            db['GRANTS'] = grants_combined
+                if db['OWNER'] not in ignore_roles_list: # if role managed by deployer (not out of the box) then add the jinja reference
+                    db['OWNER'] = self.create_jinja_role_instance(db['OWNER'])
+                
+                tags = []
+                tags_raw = self._sf.tag_references_get(db['DATABASE_NAME'], db['DATABASE_NAME'], 'database')
+                for t in tags_raw:
+                    if not (t['TAG_DATABASE'] == deploy_db_name and t['TAG_SCHEMA'] == 'TAG' and t['TAG_NAME'] in deploy_tag_list):
+                        tv = {}
+                        db_name = remove_prefix(t['TAG_DATABASE'],env_database_prefix)
+                        #tv['name'] = self.create_jinja_ref(db_name, t['TAG_SCHEMA'], t['TAG_NAME'])
+                        #tv['value'] = t['TAG_VALUE']
+                        tag_name = self.create_jinja_ref(db_name, t['TAG_SCHEMA'], t['TAG_NAME'])
+                        tv[tag_name] = t['TAG_VALUE']
+                        tags.append(tv)
+                db['TAGS'] = tags
+                
+                grants_raw = self._sf.grants_get(db['DATABASE_NAME'], 'database')
+                grants = []
+                for g in grants_raw:
+                    if g['PRIVILEGE'] != 'OWNERSHIP' and g['GRANTEE_NAME'] != current_role and g['GRANT_TYPE'] == 'ROLE':
+                        grant = {}
+                        role_name = remove_prefix(g['GRANTEE_NAME'],env_role_prefix)
+                        grant_to = self.create_jinja_role_instance(role_name) if role_name not in ignore_roles_list else role_name
+                        grant[grant_to] = g['PRIVILEGE']
+                        if g['GRANT_OPTION'] is True:
+                            grant['GRANT_OPTION'] = True
+                        grants.append(grant)
+                grants_combined = self._combine_grants(grants)
+                db['GRANTS'] = grants_combined
 
-            data.append(db)      
+                data.append(db)      
 
     return data
```

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_function.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_masking_policy.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_masking_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_network_policy.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_network_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_object.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_object.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_procedure.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_role.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_role.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_row_access_policy.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_row_access_policy.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_schema.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_schema.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_tag.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_tag.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_task.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_task.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/object_types/wrangle_warehouse.py` & `snowflake-deployer-0.1.9/src/wrangler/object_types/wrangle_warehouse.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/wrangler/wrangler.py` & `snowflake-deployer-0.1.9/src/wrangler/wrangler.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_database_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_database_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_function_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_function_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_masking_policy_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_masking_policy_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_object_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_object_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_procedure_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_procedure_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_role_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_role_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_row_access_policy_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_row_access_policy_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_schema_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_schema_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_tag_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_tag_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_task_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_task_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/functions/write_warehouse_file.py` & `snowflake-deployer-0.1.9/src/yaml_writer/functions/write_warehouse_file.py`

 * *Files identical despite different names*

### Comparing `snowflake-deployer-0.1.8/src/yaml_writer/yaml_writer.py` & `snowflake-deployer-0.1.9/src/yaml_writer/yaml_writer.py`

 * *Files identical despite different names*

