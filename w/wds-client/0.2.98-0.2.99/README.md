# Comparing `tmp/wds-client-0.2.98.tar.gz` & `tmp/wds-client-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds-client-0.2.98.tar", last modified: Thu Aug 31 18:43:13 2023, max compression
+gzip compressed data, was "wds-client-0.2.99.tar", last modified: Tue Sep 19 15:29:25 2023, max compression
```

## Comparing `wds-client-0.2.98.tar` & `wds-client-0.2.99.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 18:43:13.492611 wds-client-0.2.98/
--rw-r--r--   0 runner    (1001) docker     (999)      357 2023-08-31 18:43:13.492611 wds-client-0.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     7564 2023-08-31 18:41:38.000000 wds-client-0.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-31 18:43:13.492611 wds-client-0.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1111 2023-08-31 18:41:38.000000 wds-client-0.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 18:43:13.484611 wds-client-0.2.98/test/
--rw-r--r--   0 runner    (1001) docker     (999)     1301 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_app.py
--rw-r--r--   0 runner    (1001) docker     (999)     1536 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     1824 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_backup_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     1553 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (999)     1459 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_backup_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     1508 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     3022 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (999)     2791 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     1487 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     1481 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (999)     1782 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_clone_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     1511 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (999)     1423 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_clone_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     1180 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     1395 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (999)     1362 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_component.py
--rw-r--r--   0 runner    (1001) docker     (999)     2430 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_components.py
--rw-r--r--   0 runner    (1001) docker     (999)     1496 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_db_component.py
--rw-r--r--   0 runner    (1001) docker     (999)     1657 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (999)     1586 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (999)     1681 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (999)     1610 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (999)     1650 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     1368 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     1462 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (999)     1419 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (999)     1166 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     1563 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3624 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     2624 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     2745 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     2074 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     1899 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     1485 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (999)     1175 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     1358 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_search_operator.py
--rw-r--r--   0 runner    (1001) docker     (999)     1472 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     1415 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (999)      878 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     1667 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (999)     2237 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     1533 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     2096 2023-08-31 18:41:38.000000 wds-client-0.2.98/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 18:43:13.484611 wds-client-0.2.98/wds_client/
--rw-r--r--   0 runner    (1001) docker     (999)     3336 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 18:43:13.484611 wds-client-0.2.98/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (999)      423 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    17088 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     9761 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (999)    17329 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (999)    61562 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (999)    19354 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     6994 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (999)    26210 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (999)    12787 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (999)     3781 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 18:43:13.492611 wds-client-0.2.98/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (999)     2591 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3917 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/app.py
--rw-r--r--   0 runner    (1001) docker     (999)     6287 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     8187 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/backup_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3337 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (999)     5046 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     4859 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     4707 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (999)     5522 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     4459 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     5563 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (999)     8152 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/clone_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3326 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (999)     4463 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/clone_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     3728 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (999)     3889 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/component.py
--rw-r--r--   0 runner    (1001) docker     (999)     5218 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/components.py
--rw-r--r--   0 runner    (1001) docker     (999)     3991 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/db_component.py
--rw-r--r--   0 runner    (1001) docker     (999)     4168 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/db_validationcomponent.py
--rw-r--r--   0 runner    (1001) docker     (999)     4336 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/db_validationcomponent_details.py
--rw-r--r--   0 runner    (1001) docker     (999)     4063 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/disk_space_component.py
--rw-r--r--   0 runner    (1001) docker     (999)     5414 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/disk_space_component_details.py
--rw-r--r--   0 runner    (1001) docker     (999)     6947 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     3806 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (999)     3560 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (999)     7381 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/job.py
--rw-r--r--   0 runner    (1001) docker     (999)     5723 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     3882 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     5458 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     6722 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     4315 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/request_body_search.py
--rw-r--r--   0 runner    (1001) docker     (999)     2798 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/search_operator.py
--rw-r--r--   0 runner    (1001) docker     (999)     6218 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (999)     2824 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (999)     6496 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/stack_trace_element.py
--rw-r--r--   0 runner    (1001) docker     (999)     4030 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     4507 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (999)     4436 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (999)    12309 2023-08-31 18:41:38.000000 wds-client-0.2.98/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 18:43:13.484611 wds-client-0.2.98/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      357 2023-08-31 18:43:13.000000 wds-client-0.2.98/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3178 2023-08-31 18:43:13.000000 wds-client-0.2.98/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 18:43:13.000000 wds-client-0.2.98/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       48 2023-08-31 18:43:13.000000 wds-client-0.2.98/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-31 18:43:13.000000 wds-client-0.2.98/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.746235 wds-client-0.2.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-19 15:29:25.746235 wds-client-0.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-09-19 15:27:23.000000 wds-client-0.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-19 15:29:25.750235 wds-client-0.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-09-19 15:27:23.000000 wds-client-0.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.738235 wds-client-0.2.99/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_db_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-09-19 15:27:23.000000 wds-client-0.2.99/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.742235 wds-client-0.2.99/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.742235 wds-client-0.2.99/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61562 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26210 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12787 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.746235 wds-client-0.2.99/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/db_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/db_validationcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/db_validationcomponent_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/disk_space_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/disk_space_component_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/request_body_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/search_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/stack_trace_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2023-09-19 15:27:23.000000 wds-client-0.2.99/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:29:25.742235 wds-client-0.2.99/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-19 15:29:25.000000 wds-client-0.2.99/wds_client.egg-info/top_level.txt
```

### Comparing `wds-client-0.2.98/README.md` & `wds-client-0.2.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.2.98
+- Package version: 0.2.99
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `wds-client-0.2.98/setup.py` & `wds-client-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.2.98"
+VERSION = "0.2.99"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds-client-0.2.98/test/test_app.py` & `wds-client-0.2.99/test/test_app.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_attribute_schema.py` & `wds-client-0.2.99/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_backup_job.py` & `wds-client-0.2.99/test/test_backup_job.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_backup_job_all_of.py` & `wds-client-0.2.99/test/test_backup_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_backup_response.py` & `wds-client-0.2.99/test/test_backup_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_backup_restore_request.py` & `wds-client-0.2.99/test/test_backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_batch_operation.py` & `wds-client-0.2.99/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_batch_record_request.py` & `wds-client-0.2.99/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_batch_response.py` & `wds-client-0.2.99/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_build.py` & `wds-client-0.2.99/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_clone_job.py` & `wds-client-0.2.99/test/test_clone_job.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_clone_job_all_of.py` & `wds-client-0.2.99/test/test_clone_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_clone_response.py` & `wds-client-0.2.99/test/test_clone_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_cloning_api.py` & `wds-client-0.2.99/test/test_cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_commit.py` & `wds-client-0.2.99/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_component.py` & `wds-client-0.2.99/test/test_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_components.py` & `wds-client-0.2.99/test/test_components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_db_component.py` & `wds-client-0.2.99/test/test_db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_db_validationcomponent.py` & `wds-client-0.2.99/test/test_db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_db_validationcomponent_details.py` & `wds-client-0.2.99/test/test_db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_disk_space_component.py` & `wds-client-0.2.99/test/test_disk_space_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_disk_space_component_details.py` & `wds-client-0.2.99/test/test_disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_error_response.py` & `wds-client-0.2.99/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_general_wds_information_api.py` & `wds-client-0.2.99/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_git.py` & `wds-client-0.2.99/test/test_git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_inline_object.py` & `wds-client-0.2.99/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_instances_api.py` & `wds-client-0.2.99/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_job.py` & `wds-client-0.2.99/test/test_job.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_record_query_response.py` & `wds-client-0.2.99/test/test_record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_record_request.py` & `wds-client-0.2.99/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_record_response.py` & `wds-client-0.2.99/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_record_type_schema.py` & `wds-client-0.2.99/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_records_api.py` & `wds-client-0.2.99/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_request_body_search.py` & `wds-client-0.2.99/test/test_request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_schema_api.py` & `wds-client-0.2.99/test/test_schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_search_operator.py` & `wds-client-0.2.99/test/test_search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_search_request.py` & `wds-client-0.2.99/test/test_search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_search_sort_direction.py` & `wds-client-0.2.99/test/test_search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_snapshots_api.py` & `wds-client-0.2.99/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_stack_trace_element.py` & `wds-client-0.2.99/test/test_stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_status_response.py` & `wds-client-0.2.99/test/test_status_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_tsv_upload_response.py` & `wds-client-0.2.99/test/test_tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/test/test_version_response.py` & `wds-client-0.2.99/test/test_version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/__init__.py` & `wds-client-0.2.99/wds_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.2.98"
+__version__ = "0.2.99"
 
 # import apis into sdk package
 from wds_client.api.cloning_api import CloningApi
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.instances_api import InstancesApi
 from wds_client.api.records_api import RecordsApi
 from wds_client.api.schema_api import SchemaApi
```

### Comparing `wds-client-0.2.98/wds_client/api/cloning_api.py` & `wds-client-0.2.99/wds_client/api/cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/api/general_wds_information_api.py` & `wds-client-0.2.99/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/api/instances_api.py` & `wds-client-0.2.99/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/api/records_api.py` & `wds-client-0.2.99/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/api/schema_api.py` & `wds-client-0.2.99/wds_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/api/snapshots_api.py` & `wds-client-0.2.99/wds_client/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/api_client.py` & `wds-client-0.2.99/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'wds-client/0.2.98/python'
+        self.user_agent = 'wds-client/0.2.99/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds-client-0.2.98/wds_client/configuration.py` & `wds-client-0.2.99/wds_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.2.98".\
+               "SDK Package Version: 0.2.99".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds-client-0.2.98/wds_client/exceptions.py` & `wds-client-0.2.99/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/__init__.py` & `wds-client-0.2.99/wds_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/app.py` & `wds-client-0.2.99/wds_client/models/app.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/attribute_schema.py` & `wds-client-0.2.99/wds_client/models/attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/backup_job.py` & `wds-client-0.2.99/wds_client/models/backup_job.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/backup_job_all_of.py` & `wds-client-0.2.99/wds_client/models/backup_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/backup_response.py` & `wds-client-0.2.99/wds_client/models/backup_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/backup_restore_request.py` & `wds-client-0.2.99/wds_client/models/backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/batch_operation.py` & `wds-client-0.2.99/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/batch_record_request.py` & `wds-client-0.2.99/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/batch_response.py` & `wds-client-0.2.99/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/build.py` & `wds-client-0.2.99/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/clone_job.py` & `wds-client-0.2.99/wds_client/models/clone_job.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/clone_job_all_of.py` & `wds-client-0.2.99/wds_client/models/clone_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/clone_response.py` & `wds-client-0.2.99/wds_client/models/clone_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/commit.py` & `wds-client-0.2.99/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/component.py` & `wds-client-0.2.99/wds_client/models/component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/components.py` & `wds-client-0.2.99/wds_client/models/components.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/db_component.py` & `wds-client-0.2.99/wds_client/models/db_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/db_validationcomponent.py` & `wds-client-0.2.99/wds_client/models/db_validationcomponent.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/db_validationcomponent_details.py` & `wds-client-0.2.99/wds_client/models/db_validationcomponent_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/disk_space_component.py` & `wds-client-0.2.99/wds_client/models/disk_space_component.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/disk_space_component_details.py` & `wds-client-0.2.99/wds_client/models/disk_space_component_details.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/error_response.py` & `wds-client-0.2.99/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/git.py` & `wds-client-0.2.99/wds_client/models/git.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/inline_object.py` & `wds-client-0.2.99/wds_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/job.py` & `wds-client-0.2.99/wds_client/models/job.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/record_query_response.py` & `wds-client-0.2.99/wds_client/models/record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/record_request.py` & `wds-client-0.2.99/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/record_response.py` & `wds-client-0.2.99/wds_client/models/record_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/record_type_schema.py` & `wds-client-0.2.99/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/request_body_search.py` & `wds-client-0.2.99/wds_client/models/request_body_search.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/search_operator.py` & `wds-client-0.2.99/wds_client/models/search_operator.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/search_request.py` & `wds-client-0.2.99/wds_client/models/search_request.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/search_sort_direction.py` & `wds-client-0.2.99/wds_client/models/search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/stack_trace_element.py` & `wds-client-0.2.99/wds_client/models/stack_trace_element.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/status_response.py` & `wds-client-0.2.99/wds_client/models/status_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/tsv_upload_response.py` & `wds-client-0.2.99/wds_client/models/tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/models/version_response.py` & `wds-client-0.2.99/wds_client/models/version_response.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client/rest.py` & `wds-client-0.2.99/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds-client-0.2.98/wds_client.egg-info/SOURCES.txt` & `wds-client-0.2.99/wds_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

