# Comparing `tmp/data-repo-client-2.37.0.tar.gz` & `tmp/data-repo-client-2.38.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-rvp1idct/data-repo-client-2.37.0.tar", last modified: Wed Apr 10 17:11:44 2024, max compression
+gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-8p2iskgi/data-repo-client-2.38.0.tar", last modified: Wed Apr 10 23:42:25 2024, max compression
```

## Comparing `data-repo-client-2.37.0.tar` & `data-repo-client-2.38.0.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:11:44.000000 data-repo-client-2.37.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-10 17:11:44.000000 data-repo-client-2.37.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    42643 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   261657 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   453780 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   146221 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/api/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/api/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:11:44.000000 data-repo-client-2.37.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/data_repo_client/models/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/enumerate_snapshot_access_request_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_get_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/data_repo_client/models/workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/data_repo_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 17:11:43.000000 data-repo-client-2.37.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 17:11:44.000000 data-repo-client-2.37.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:11:44.000000 data-repo-client-2.37.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-10 17:11:38.000000 data-repo-client-2.37.0/test/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_enumerate_snapshot_access_request_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_get_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/test/test_unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-10 17:11:40.000000 data-repo-client-2.37.0/test/test_upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-10 17:11:39.000000 data-repo-client-2.37.0/test/test_workspace_policy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    42643 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   261657 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   453780 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146221 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api/upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/enumerate_snapshot_access_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_get_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/models/workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/data_repo_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:42:25.000000 data-repo-client-2.38.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_enumerate_snapshot_access_request_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_get_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-10 23:42:16.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-10 23:42:17.000000 data-repo-client-2.38.0/test/test_workspace_policy_model.py
```

### Comparing `data-repo-client-2.37.0/PKG-INFO` & `data-repo-client-2.38.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.37.0
+Version: 2.38.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.37.0/README.md` & `data-repo-client-2.38.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 2.37.0
+- Package version: 2.38.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `data-repo-client-2.37.0/data_repo_client/__init__.py` & `data-repo-client-2.38.0/data_repo_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.37.0"
+__version__ = "2.38.0"
 
 # import apis into sdk package
 from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
 from data_repo_client.api.admin_api import AdminApi
 from data_repo_client.api.configs_api import ConfigsApi
 from data_repo_client.api.datasets_api import DatasetsApi
 from data_repo_client.api.duos_api import DuosApi
```

### Comparing `data-repo-client-2.37.0/data_repo_client/api/__init__.py` & `data-repo-client-2.38.0/data_repo_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/admin_api.py` & `data-repo-client-2.38.0/data_repo_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/configs_api.py` & `data-repo-client-2.38.0/data_repo_client/api/configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/data_repository_service_api.py` & `data-repo-client-2.38.0/data_repo_client/api/data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/datasets_api.py` & `data-repo-client-2.38.0/data_repo_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/duos_api.py` & `data-repo-client-2.38.0/data_repo_client/api/duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/jobs_api.py` & `data-repo-client-2.38.0/data_repo_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/journal_api.py` & `data-repo-client-2.38.0/data_repo_client/api/journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/profiles_api.py` & `data-repo-client-2.38.0/data_repo_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/register_api.py` & `data-repo-client-2.38.0/data_repo_client/api/register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/repository_api.py` & `data-repo-client-2.38.0/data_repo_client/api/repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/resources_api.py` & `data-repo-client-2.38.0/data_repo_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/search_api.py` & `data-repo-client-2.38.0/data_repo_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/snapshots_api.py` & `data-repo-client-2.38.0/data_repo_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/unauthenticated_api.py` & `data-repo-client-2.38.0/data_repo_client/api/unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api/upgrade_api.py` & `data-repo-client-2.38.0/data_repo_client/api/upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/api_client.py` & `data-repo-client-2.38.0/data_repo_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.37.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.38.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `data-repo-client-2.37.0/data_repo_client/configuration.py` & `data-repo-client-2.38.0/data_repo_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 2.37.0".\
+               "SDK Package Version: 2.38.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `data-repo-client-2.37.0/data_repo_client/exceptions.py` & `data-repo-client-2.38.0/data_repo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/__init__.py` & `data-repo-client-2.38.0/data_repo_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/access_info_big_query_model.py` & `data-repo-client-2.38.0/data_repo_client/models/access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/access_info_big_query_model_table.py` & `data-repo-client-2.38.0/data_repo_client/models/access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/access_info_model.py` & `data-repo-client-2.38.0/data_repo_client/models/access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/access_info_parquet_model.py` & `data-repo-client-2.38.0/data_repo_client/models/access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/access_info_parquet_model_table.py` & `data-repo-client-2.38.0/data_repo_client/models/access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/add_auth_domain_response_model.py` & `data-repo-client-2.38.0/data_repo_client/models/add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/asset_model.py` & `data-repo-client-2.38.0/data_repo_client/models/asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/asset_table_model.py` & `data-repo-client-2.38.0/data_repo_client/models/asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/billing_profile_model.py` & `data-repo-client-2.38.0/data_repo_client/models/billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/billing_profile_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/billing_profile_update_model.py` & `data-repo-client-2.38.0/data_repo_client/models/billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_array_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_array_result_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_file_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_file_result_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_file_state.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_history_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_history_model_list.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/bulk_load_result_model.py` & `data-repo-client-2.38.0/data_repo_client/models/bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/cloud_platform.py` & `data-repo-client-2.38.0/data_repo_client/models/cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_model.py` & `data-repo-client-2.38.0/data_repo_client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_double_model.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_double_model_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_int_model.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_int_model_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_model.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_text_model.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_text_model_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/column_statistics_text_value.py` & `data-repo-client-2.38.0/data_repo_client/models/column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_enable_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_fault_counted_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_fault_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_group_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_list_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/config_parameter_model.py` & `data-repo-client-2.38.0/data_repo_client/models/config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/data_deletion_gcs_file_model.py` & `data-repo-client-2.38.0/data_repo_client/models/data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/data_deletion_json_array_model.py` & `data-repo-client-2.38.0/data_repo_client/models/data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/data_deletion_request.py` & `data-repo-client-2.38.0/data_repo_client/models/data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/data_deletion_table_model.py` & `data-repo-client-2.38.0/data_repo_client/models/data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_data_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_patch_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_request_access_include_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_request_model_policies.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_schema_column_update_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_schema_update_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_schema_update_model_changes.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_specification_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/dataset_summary_model.py` & `data-repo-client-2.38.0/data_repo_client/models/dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/date_partition_options_model.py` & `data-repo-client-2.38.0/data_repo_client/models/date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/delete_response_model.py` & `data-repo-client-2.38.0/data_repo_client/models/delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/directory_detail_model.py` & `data-repo-client-2.38.0/data_repo_client/models/directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_access_method.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_access_url.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_alias_model.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_authorizations.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_checksum.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_contents_object.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_error.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_object.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_passport_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/drs_service_info.py` & `data-repo-client-2.38.0/data_repo_client/models/drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/duos_firecloud_group_model.py` & `data-repo-client-2.38.0/data_repo_client/models/duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/duos_firecloud_groups_sync_response.py` & `data-repo-client-2.38.0/data_repo_client/models/duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/enumerate_billing_profile_model.py` & `data-repo-client-2.38.0/data_repo_client/models/enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/enumerate_dataset_model.py` & `data-repo-client-2.38.0/data_repo_client/models/enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/enumerate_snapshot_access_request.py` & `data-repo-client-2.38.0/data_repo_client/models/enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/enumerate_snapshot_access_request_item.py` & `data-repo-client-2.38.0/data_repo_client/models/enumerate_snapshot_access_request_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/enumerate_snapshot_model.py` & `data-repo-client-2.38.0/data_repo_client/models/enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/enumerate_sort_by_param.py` & `data-repo-client-2.38.0/data_repo_client/models/enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/error_model.py` & `data-repo-client-2.38.0/data_repo_client/models/error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/file_detail_model.py` & `data-repo-client-2.38.0/data_repo_client/models/file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/file_load_model.py` & `data-repo-client-2.38.0/data_repo_client/models/file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/file_model.py` & `data-repo-client-2.38.0/data_repo_client/models/file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/file_model_type.py` & `data-repo-client-2.38.0/data_repo_client/models/file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/iam_resource_type_enum.py` & `data-repo-client-2.38.0/data_repo_client/models/iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/inaccessible_workspace_policy_model.py` & `data-repo-client-2.38.0/data_repo_client/models/inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/ingest_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/ingest_response_model.py` & `data-repo-client-2.38.0/data_repo_client/models/ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/int_partition_options_model.py` & `data-repo-client-2.38.0/data_repo_client/models/int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/job_model.py` & `data-repo-client-2.38.0/data_repo_client/models/job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/journal_entry_model.py` & `data-repo-client-2.38.0/data_repo_client/models/journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/policy_member_request.py` & `data-repo-client-2.38.0/data_repo_client/models/policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/policy_model.py` & `data-repo-client-2.38.0/data_repo_client/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/policy_response.py` & `data-repo-client-2.38.0/data_repo_client/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/query_column_statistics_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/query_data_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/relationship_model.py` & `data-repo-client-2.38.0/data_repo_client/models/relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/relationship_term_model.py` & `data-repo-client-2.38.0/data_repo_client/models/relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/repository_configuration_model.py` & `data-repo-client-2.38.0/data_repo_client/models/repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/repository_status_model.py` & `data-repo-client-2.38.0/data_repo_client/models/repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/repository_status_model_systems.py` & `data-repo-client-2.38.0/data_repo_client/models/repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/resource_locks.py` & `data-repo-client-2.38.0/data_repo_client/models/resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/resource_policy_model.py` & `data-repo-client-2.38.0/data_repo_client/models/resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/sam_policy_model.py` & `data-repo-client-2.38.0/data_repo_client/models/sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_access_request.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_access_request_response.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_access_request_status.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_cohort.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_concept.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_count_request.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_count_response.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_count_response_result.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_criteria.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_criteria_group.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_criteria.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_option.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_feature_value_group.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_get_concepts_response.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_get_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_option.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_parent_concept.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_item.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_option.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_option.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_option.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_request.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_builder_settings.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_ids_and_roles_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_link_duos_dataset_response.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_patch_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_preview_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_asset_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_contents_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_model_policies.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_query_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_row_id_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_request_row_id_table_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_retrieve_include_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_source_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/snapshot_summary_model.py` & `data-repo-client-2.38.0/data_repo_client/models/snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/sql_sort_direction_asc_default.py` & `data-repo-client-2.38.0/data_repo_client/models/sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/sql_sort_direction_desc_default.py` & `data-repo-client-2.38.0/data_repo_client/models/sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/storage_resource_model.py` & `data-repo-client-2.38.0/data_repo_client/models/storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/table_data_type.py` & `data-repo-client-2.38.0/data_repo_client/models/table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/table_model.py` & `data-repo-client-2.38.0/data_repo_client/models/table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/tag_count.py` & `data-repo-client-2.38.0/data_repo_client/models/tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/tag_count_result_model.py` & `data-repo-client-2.38.0/data_repo_client/models/tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/tag_update_request_model.py` & `data-repo-client-2.38.0/data_repo_client/models/tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/transaction_close_model.py` & `data-repo-client-2.38.0/data_repo_client/models/transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/transaction_create_model.py` & `data-repo-client-2.38.0/data_repo_client/models/transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/transaction_model.py` & `data-repo-client-2.38.0/data_repo_client/models/transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/unlock_resource_request.py` & `data-repo-client-2.38.0/data_repo_client/models/unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/upgrade_model.py` & `data-repo-client-2.38.0/data_repo_client/models/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/upgrade_response_model.py` & `data-repo-client-2.38.0/data_repo_client/models/upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/user_status_info.py` & `data-repo-client-2.38.0/data_repo_client/models/user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/models/workspace_policy_model.py` & `data-repo-client-2.38.0/data_repo_client/models/workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client/rest.py` & `data-repo-client-2.38.0/data_repo_client/rest.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/data_repo_client.egg-info/PKG-INFO` & `data-repo-client-2.38.0/data_repo_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.37.0
+Version: 2.38.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.37.0/data_repo_client.egg-info/SOURCES.txt` & `data-repo-client-2.38.0/data_repo_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/setup.py` & `data-repo-client-2.38.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "data-repo-client"
-VERSION = "2.37.0"
+VERSION = "2.38.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `data-repo-client-2.37.0/test/test_access_info_big_query_model.py` & `data-repo-client-2.38.0/test/test_access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_access_info_big_query_model_table.py` & `data-repo-client-2.38.0/test/test_access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_access_info_model.py` & `data-repo-client-2.38.0/test/test_access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_access_info_parquet_model.py` & `data-repo-client-2.38.0/test/test_access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_access_info_parquet_model_table.py` & `data-repo-client-2.38.0/test/test_access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_add_auth_domain_response_model.py` & `data-repo-client-2.38.0/test/test_add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_admin_api.py` & `data-repo-client-2.38.0/test/test_admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_asset_model.py` & `data-repo-client-2.38.0/test/test_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_asset_table_model.py` & `data-repo-client-2.38.0/test/test_asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_billing_profile_model.py` & `data-repo-client-2.38.0/test/test_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_billing_profile_request_model.py` & `data-repo-client-2.38.0/test/test_billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_billing_profile_update_model.py` & `data-repo-client-2.38.0/test/test_billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_array_request_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_array_result_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_file_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_file_result_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_file_state.py` & `data-repo-client-2.38.0/test/test_bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_history_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_history_model_list.py` & `data-repo-client-2.38.0/test/test_bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_request_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_bulk_load_result_model.py` & `data-repo-client-2.38.0/test/test_bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_cloud_platform.py` & `data-repo-client-2.38.0/test/test_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_model.py` & `data-repo-client-2.38.0/test/test_column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_double_model.py` & `data-repo-client-2.38.0/test/test_column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_double_model_all_of.py` & `data-repo-client-2.38.0/test/test_column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_int_model.py` & `data-repo-client-2.38.0/test/test_column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_int_model_all_of.py` & `data-repo-client-2.38.0/test/test_column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_model.py` & `data-repo-client-2.38.0/test/test_column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_text_model.py` & `data-repo-client-2.38.0/test/test_column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_text_model_all_of.py` & `data-repo-client-2.38.0/test/test_column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_column_statistics_text_value.py` & `data-repo-client-2.38.0/test/test_column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_enable_model.py` & `data-repo-client-2.38.0/test/test_config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_fault_counted_model.py` & `data-repo-client-2.38.0/test/test_config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_fault_model.py` & `data-repo-client-2.38.0/test/test_config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_group_model.py` & `data-repo-client-2.38.0/test/test_config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_list_model.py` & `data-repo-client-2.38.0/test/test_config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_model.py` & `data-repo-client-2.38.0/test/test_config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_config_parameter_model.py` & `data-repo-client-2.38.0/test/test_config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_configs_api.py` & `data-repo-client-2.38.0/test/test_configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_data_deletion_gcs_file_model.py` & `data-repo-client-2.38.0/test/test_data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_data_deletion_json_array_model.py` & `data-repo-client-2.38.0/test/test_data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_data_deletion_request.py` & `data-repo-client-2.38.0/test/test_data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_data_deletion_table_model.py` & `data-repo-client-2.38.0/test/test_data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_data_repository_service_api.py` & `data-repo-client-2.38.0/test/test_data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_data_model.py` & `data-repo-client-2.38.0/test/test_dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_model.py` & `data-repo-client-2.38.0/test/test_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_patch_request_model.py` & `data-repo-client-2.38.0/test/test_dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_request_access_include_model.py` & `data-repo-client-2.38.0/test/test_dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_request_model.py` & `data-repo-client-2.38.0/test/test_dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_request_model_policies.py` & `data-repo-client-2.38.0/test/test_dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_schema_column_update_model.py` & `data-repo-client-2.38.0/test/test_dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_schema_update_model.py` & `data-repo-client-2.38.0/test/test_dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_schema_update_model_changes.py` & `data-repo-client-2.38.0/test/test_dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_specification_model.py` & `data-repo-client-2.38.0/test/test_dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_dataset_summary_model.py` & `data-repo-client-2.38.0/test/test_dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_datasets_api.py` & `data-repo-client-2.38.0/test/test_datasets_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_date_partition_options_model.py` & `data-repo-client-2.38.0/test/test_date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_delete_response_model.py` & `data-repo-client-2.38.0/test/test_delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_directory_detail_model.py` & `data-repo-client-2.38.0/test/test_directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_access_method.py` & `data-repo-client-2.38.0/test/test_drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_access_url.py` & `data-repo-client-2.38.0/test/test_drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_alias_model.py` & `data-repo-client-2.38.0/test/test_drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_authorizations.py` & `data-repo-client-2.38.0/test/test_drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_checksum.py` & `data-repo-client-2.38.0/test/test_drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_contents_object.py` & `data-repo-client-2.38.0/test/test_drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_error.py` & `data-repo-client-2.38.0/test/test_drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_object.py` & `data-repo-client-2.38.0/test/test_drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_passport_request_model.py` & `data-repo-client-2.38.0/test/test_drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_drs_service_info.py` & `data-repo-client-2.38.0/test/test_drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_duos_api.py` & `data-repo-client-2.38.0/test/test_duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_duos_firecloud_group_model.py` & `data-repo-client-2.38.0/test/test_duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_duos_firecloud_groups_sync_response.py` & `data-repo-client-2.38.0/test/test_duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_enumerate_billing_profile_model.py` & `data-repo-client-2.38.0/test/test_enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_enumerate_dataset_model.py` & `data-repo-client-2.38.0/test/test_enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_enumerate_snapshot_access_request.py` & `data-repo-client-2.38.0/test/test_enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_enumerate_snapshot_access_request_item.py` & `data-repo-client-2.38.0/test/test_enumerate_snapshot_access_request_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_enumerate_snapshot_model.py` & `data-repo-client-2.38.0/test/test_enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_enumerate_sort_by_param.py` & `data-repo-client-2.38.0/test/test_enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_error_model.py` & `data-repo-client-2.38.0/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_file_detail_model.py` & `data-repo-client-2.38.0/test/test_file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_file_load_model.py` & `data-repo-client-2.38.0/test/test_file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_file_model.py` & `data-repo-client-2.38.0/test/test_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_file_model_type.py` & `data-repo-client-2.38.0/test/test_file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_iam_resource_type_enum.py` & `data-repo-client-2.38.0/test/test_iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_inaccessible_workspace_policy_model.py` & `data-repo-client-2.38.0/test/test_inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_ingest_request_model.py` & `data-repo-client-2.38.0/test/test_ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_ingest_response_model.py` & `data-repo-client-2.38.0/test/test_ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_int_partition_options_model.py` & `data-repo-client-2.38.0/test/test_int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_job_model.py` & `data-repo-client-2.38.0/test/test_job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_jobs_api.py` & `data-repo-client-2.38.0/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_journal_api.py` & `data-repo-client-2.38.0/test/test_journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_journal_entry_model.py` & `data-repo-client-2.38.0/test/test_journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_policy_member_request.py` & `data-repo-client-2.38.0/test/test_policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_policy_model.py` & `data-repo-client-2.38.0/test/test_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_policy_response.py` & `data-repo-client-2.38.0/test/test_policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_profiles_api.py` & `data-repo-client-2.38.0/test/test_profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_query_column_statistics_request_model.py` & `data-repo-client-2.38.0/test/test_query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_query_data_request_model.py` & `data-repo-client-2.38.0/test/test_query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_register_api.py` & `data-repo-client-2.38.0/test/test_register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_relationship_model.py` & `data-repo-client-2.38.0/test/test_relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_relationship_term_model.py` & `data-repo-client-2.38.0/test/test_relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_repository_api.py` & `data-repo-client-2.38.0/test/test_repository_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_repository_configuration_model.py` & `data-repo-client-2.38.0/test/test_repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_repository_status_model.py` & `data-repo-client-2.38.0/test/test_repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_repository_status_model_systems.py` & `data-repo-client-2.38.0/test/test_repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_resource_locks.py` & `data-repo-client-2.38.0/test/test_resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_resource_policy_model.py` & `data-repo-client-2.38.0/test/test_resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_resources_api.py` & `data-repo-client-2.38.0/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_sam_policy_model.py` & `data-repo-client-2.38.0/test/test_sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_search_api.py` & `data-repo-client-2.38.0/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_access_request.py` & `data-repo-client-2.38.0/test/test_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_access_request_response.py` & `data-repo-client-2.38.0/test/test_snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_access_request_status.py` & `data-repo-client-2.38.0/test/test_snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_cohort.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_concept.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_count_request.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_count_response.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_count_response_result.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_criteria.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_criteria_group.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_domain_criteria.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_domain_option.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_feature_value_group.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_get_concepts_response.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_get_concepts_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_option.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_parent_concept.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_item.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_option.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_option.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_option.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_request.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_builder_settings.py` & `data-repo-client-2.38.0/test/test_snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_export_response_model.py` & `data-repo-client-2.38.0/test/test_snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_export_response_model_format.py` & `data-repo-client-2.38.0/test/test_snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.38.0/test/test_snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_ids_and_roles_model.py` & `data-repo-client-2.38.0/test/test_snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_link_duos_dataset_response.py` & `data-repo-client-2.38.0/test/test_snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_model.py` & `data-repo-client-2.38.0/test/test_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_patch_request_model.py` & `data-repo-client-2.38.0/test/test_snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_preview_model.py` & `data-repo-client-2.38.0/test/test_snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_asset_model.py` & `data-repo-client-2.38.0/test/test_snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_contents_model.py` & `data-repo-client-2.38.0/test/test_snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_model.py` & `data-repo-client-2.38.0/test/test_snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_model_policies.py` & `data-repo-client-2.38.0/test/test_snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_query_model.py` & `data-repo-client-2.38.0/test/test_snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_row_id_model.py` & `data-repo-client-2.38.0/test/test_snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_request_row_id_table_model.py` & `data-repo-client-2.38.0/test/test_snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_retrieve_include_model.py` & `data-repo-client-2.38.0/test/test_snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_source_model.py` & `data-repo-client-2.38.0/test/test_snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshot_summary_model.py` & `data-repo-client-2.38.0/test/test_snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_snapshots_api.py` & `data-repo-client-2.38.0/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_sql_sort_direction_asc_default.py` & `data-repo-client-2.38.0/test/test_sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_sql_sort_direction_desc_default.py` & `data-repo-client-2.38.0/test/test_sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_storage_resource_model.py` & `data-repo-client-2.38.0/test/test_storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_table_data_type.py` & `data-repo-client-2.38.0/test/test_table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_table_model.py` & `data-repo-client-2.38.0/test/test_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_tag_count.py` & `data-repo-client-2.38.0/test/test_tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_tag_count_result_model.py` & `data-repo-client-2.38.0/test/test_tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_tag_update_request_model.py` & `data-repo-client-2.38.0/test/test_tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_transaction_close_model.py` & `data-repo-client-2.38.0/test/test_transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_transaction_create_model.py` & `data-repo-client-2.38.0/test/test_transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_transaction_model.py` & `data-repo-client-2.38.0/test/test_transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_unauthenticated_api.py` & `data-repo-client-2.38.0/test/test_unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_unlock_resource_request.py` & `data-repo-client-2.38.0/test/test_unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_upgrade_api.py` & `data-repo-client-2.38.0/test/test_upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_upgrade_model.py` & `data-repo-client-2.38.0/test/test_upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_upgrade_response_model.py` & `data-repo-client-2.38.0/test/test_upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_user_status_info.py` & `data-repo-client-2.38.0/test/test_user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.37.0/test/test_workspace_policy_model.py` & `data-repo-client-2.38.0/test/test_workspace_policy_model.py`

 * *Files identical despite different names*

