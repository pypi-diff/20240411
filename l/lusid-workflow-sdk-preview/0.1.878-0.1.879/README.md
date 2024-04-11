# Comparing `tmp/lusid-workflow-sdk-preview-0.1.878.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.878.tar", last modified: Tue Apr  9 16:33:01 2024, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.879.tar", last modified: Wed Apr 10 12:57:57 2024, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.878.tar` & `lusid-workflow-sdk-preview-0.1.879.tar`

### file list

```diff
@@ -1,97 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10301 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     6326 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/event_handlers_api.py
--rw-r--r--   0 root         (0) root         (0)    57864 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    42809 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    62480 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27758 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     5179 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8262 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_definition.py
--rw-r--r--   0 root         (0) root         (0)     6409 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0 root         (0) root         (0)    12100 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_details.py
--rw-r--r--   0 root         (0) root         (0)    10733 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_details_response.py
--rw-r--r--   0 root         (0) root         (0)    10122 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6232 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0 root         (0) root         (0)     5895 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0 root         (0) root         (0)    14189 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_event_handler_request.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     7821 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9176 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)    14474 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/event_handler.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/event_handler_mapping.py
--rw-r--r--   0 root         (0) root         (0)     6798 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/event_matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)     4368 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/fail.py
--rw-r--r--   0 root         (0) root         (0)     4239 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/fail_response.py
--rw-r--r--   0 root         (0) root         (0)     5622 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/field_mapping.py
--rw-r--r--   0 root         (0) root         (0)     6800 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0 root         (0) root         (0)     5878 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5112 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/health_check_response.py
--rw-r--r--   0 root         (0) root         (0)     5984 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0 root         (0) root         (0)     5113 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0 root         (0) root         (0)     9530 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7295 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7575 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0 root         (0) root         (0)     9076 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/parameter.py
--rw-r--r--   0 root         (0) root         (0)     5767 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/parameter_value.py
--rw-r--r--   0 root         (0) root         (0)     4822 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7175 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7211 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/result_field.py
--rw-r--r--   0 root         (0) root         (0)     4985 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)    10386 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0 root         (0) root         (0)    10247 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0 root         (0) root         (0)     4435 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     5179 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0 root         (0) root         (0)     5383 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/scheduler_job.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/scheduler_job_response.py
--rw-r--r--   0 root         (0) root         (0)     4377 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/sleep.py
--rw-r--r--   0 root         (0) root         (0)     4441 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/sleep_response.py
--rw-r--r--   0 root         (0) root         (0)    11504 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/stack.py
--rw-r--r--   0 root         (0) root         (0)    19688 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    14093 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     6387 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5243 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     4944 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_summary.py
--rw-r--r--   0 root         (0) root         (0)    12376 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     6067 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     6451 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0 root         (0) root         (0)     5348 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0 root         (0) root         (0)     4440 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    12546 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6427 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)     8188 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/update_worker_request.py
--rw-r--r--   0 root         (0) root         (0)    11105 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/version_info.py
--rw-r--r--   0 root         (0) root         (0)    11171 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     8585 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7048 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0 root         (0) root         (0)     8967 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0 root         (0) root         (0)    13551 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/utilities/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3804 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 16:33:01.000000 lusid-workflow-sdk-preview-0.1.878/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2024-04-09 16:31:41.000000 lusid-workflow-sdk-preview-0.1.878/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11512 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     5955 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57864 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    42809 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    62480 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27758 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6409 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0 root         (0) root         (0)    12100 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_details.py
+-rw-r--r--   0 root         (0) root         (0)    10733 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0 root         (0) root         (0)    10122 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0 root         (0) root         (0)     5895 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     7821 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/fail.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/fail_response.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/result_field.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10386 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0 root         (0) root         (0)     5383 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/sleep.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0 root         (0) root         (0)    11504 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/stack.py
+-rw-r--r--   0 root         (0) root         (0)    19688 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    14093 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_summary.py
+-rw-r--r--   0 root         (0) root         (0)    12376 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     8188 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)    11105 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/version_info.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     8585 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/utilities/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3575 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 12:57:57.000000 lusid-workflow-sdk-preview-0.1.879/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-04-10 12:57:27.000000 lusid-workflow-sdk-preview-0.1.879/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/README.md` & `lusid-workflow-sdk-preview-0.1.879/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.878
-- Package version: 0.1.878
+- API version: 0.1.879
+- Package version: 0.1.879
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -70,33 +70,32 @@
 )
 configuration.access_token = 'YOUR_ACCESS_TOKEN'
 
 
 # Enter a context with an instance of the API client
 with lusid_workflow.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = lusid_workflow.EventHandlersApi(api_client)
-    create_event_handler_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example Event Handler","description":"Test","status":"Active","eventMatchingPattern":{"eventType":"PortfolioCreated","filter":"body.scope eq 'TestScope'"},"runAsUserId":{"setTo":"ExampleUserId"},"taskDefinitionId":{"scope":"A1","code":"YYY"},"taskDefinitionAsAt":"9999-12-31T23:59:59.9999999+00:00","taskActivity":{"InitialTrigger":"InitialTrigger","Type":"CreateNewTask","CorrelationIds":[],"TaskFields":{}}} # CreateEventHandlerRequest | The data to create an Event Handler
+    api_instance = lusid_workflow.TaskDefinitionsApi(api_client)
+    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","runAsUserId":"user-id","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
 
     try:
-        # [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
-        api_response = api_instance.create_event_handler(create_event_handler_request)
+        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
+        api_response = api_instance.create_task_definition(create_task_definition_request)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling EventHandlersApi->create_event_handler: %s\n" % e)
+        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://www.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*EventHandlersApi* | [**create_event_handler**](docs/EventHandlersApi.md#create_event_handler) | **POST** /api/eventhandlers | [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
 *TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
 *TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
 *TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
 *TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
 *TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
 *TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
 *TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
@@ -118,22 +117,18 @@
  - [ActionDefinition](docs/ActionDefinition.md)
  - [ActionDefinitionResponse](docs/ActionDefinitionResponse.md)
  - [ActionDetails](docs/ActionDetails.md)
  - [ActionDetailsResponse](docs/ActionDetailsResponse.md)
  - [CreateChildTaskConfiguration](docs/CreateChildTaskConfiguration.md)
  - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateChildTasksActionResponse](docs/CreateChildTasksActionResponse.md)
- - [CreateEventHandlerRequest](docs/CreateEventHandlerRequest.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
- - [EventHandler](docs/EventHandler.md)
- - [EventHandlerMapping](docs/EventHandlerMapping.md)
- - [EventMatchingPattern](docs/EventMatchingPattern.md)
  - [Fail](docs/Fail.md)
  - [FailResponse](docs/FailResponse.md)
  - [FieldMapping](docs/FieldMapping.md)
  - [GetWorkerResultResponse](docs/GetWorkerResultResponse.md)
  - [HealthCheck](docs/HealthCheck.md)
  - [HealthCheckResponse](docs/HealthCheckResponse.md)
  - [InitialState](docs/InitialState.md)
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.878"
+__version__ = "0.1.879"
 
 # import apis into sdk package
-from lusid_workflow.api.event_handlers_api import EventHandlersApi
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.configuration import Configuration
@@ -35,22 +34,18 @@
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.action_details import ActionDetails
 from lusid_workflow.models.action_details_response import ActionDetailsResponse
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
-from lusid_workflow.models.create_event_handler_request import CreateEventHandlerRequest
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
-from lusid_workflow.models.event_handler import EventHandler
-from lusid_workflow.models.event_handler_mapping import EventHandlerMapping
-from lusid_workflow.models.event_matching_pattern import EventMatchingPattern
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.health_check_response import HealthCheckResponse
 from lusid_workflow.models.initial_state import InitialState
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/task_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -328,15 +328,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -505,15 +505,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -681,15 +681,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -858,15 +858,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -1042,15 +1042,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -173,15 +173,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Task",
             400: "LusidValidationProblemDetails",
@@ -323,15 +323,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -481,15 +481,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
@@ -657,15 +657,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -833,15 +833,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api/workers_api.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api/workers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -163,15 +163,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -334,15 +334,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -513,15 +513,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -655,15 +655,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetWorkerResultResponse",
             400: "LusidValidationProblemDetails",
@@ -815,15 +815,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfWorker",
             400: "LusidValidationProblemDetails",
@@ -1005,15 +1005,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RunWorkerResponse",
             400: "LusidValidationProblemDetails",
@@ -1190,15 +1190,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.878'
+        header_params['X-LUSID-SDK-Version'] = '0.1.879'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Worker",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.878/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.879/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.878\n"\
-               "SDK Package Version: 0.1.878".\
+               "Version of the API: 0.1.879\n"\
+               "SDK Package Version: 0.1.879".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -18,22 +18,18 @@
 from lusid_workflow.models.action_definition import ActionDefinition
 from lusid_workflow.models.action_definition_response import ActionDefinitionResponse
 from lusid_workflow.models.action_details import ActionDetails
 from lusid_workflow.models.action_details_response import ActionDetailsResponse
 from lusid_workflow.models.create_child_task_configuration import CreateChildTaskConfiguration
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
-from lusid_workflow.models.create_event_handler_request import CreateEventHandlerRequest
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
-from lusid_workflow.models.event_handler import EventHandler
-from lusid_workflow.models.event_handler_mapping import EventHandlerMapping
-from lusid_workflow.models.event_matching_pattern import EventMatchingPattern
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.get_worker_result_response import GetWorkerResultResponse
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.health_check_response import HealthCheckResponse
 from lusid_workflow.models.initial_state import InitialState
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_definition.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_definition_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_definition_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_details.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/action_details_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/action_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_child_task_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_child_tasks_action.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_child_tasks_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_event_handler_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_definition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class CreateEventHandlerRequest(object):
+class TaskDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -36,312 +36,341 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'ResourceId',
+        'version': 'VersionInfo',
         'display_name': 'str',
         'description': 'str',
-        'status': 'str',
-        'event_matching_pattern': 'EventMatchingPattern',
-        'run_as_user_id': 'EventHandlerMapping',
-        'task_definition_id': 'ResourceId',
-        'task_definition_as_at': 'datetime',
-        'task_activity': 'object'
+        'states': 'list[TaskStateDefinition]',
+        'field_schema': 'list[TaskFieldDefinition]',
+        'initial_state': 'InitialState',
+        'triggers': 'list[TransitionTriggerDefinition]',
+        'actions': 'list[ActionDefinitionResponse]',
+        'transitions': 'list[TaskTransitionDefinition]'
     }
 
     attribute_map = {
         'id': 'id',
+        'version': 'version',
         'display_name': 'displayName',
         'description': 'description',
-        'status': 'status',
-        'event_matching_pattern': 'eventMatchingPattern',
-        'run_as_user_id': 'runAsUserId',
-        'task_definition_id': 'taskDefinitionId',
-        'task_definition_as_at': 'taskDefinitionAsAt',
-        'task_activity': 'taskActivity'
+        'states': 'states',
+        'field_schema': 'fieldSchema',
+        'initial_state': 'initialState',
+        'triggers': 'triggers',
+        'actions': 'actions',
+        'transitions': 'transitions'
     }
 
     required_map = {
         'id': 'required',
+        'version': 'optional',
         'display_name': 'required',
         'description': 'optional',
-        'status': 'required',
-        'event_matching_pattern': 'required',
-        'run_as_user_id': 'required',
-        'task_definition_id': 'required',
-        'task_definition_as_at': 'optional',
-        'task_activity': 'required'
+        'states': 'required',
+        'field_schema': 'optional',
+        'initial_state': 'required',
+        'triggers': 'optional',
+        'actions': 'optional',
+        'transitions': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, status=None, event_matching_pattern=None, run_as_user_id=None, task_definition_id=None, task_definition_as_at=None, task_activity=None, local_vars_configuration=None):  # noqa: E501
-        """CreateEventHandlerRequest - a model defined in OpenAPI"
+    def __init__(self, id=None, version=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, actions=None, transitions=None, local_vars_configuration=None):  # noqa: E501
+        """TaskDefinition - a model defined in OpenAPI"
         
         :param id:  (required)
         :type id: lusid_workflow.ResourceId
+        :param version: 
+        :type version: lusid_workflow.VersionInfo
         :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
-        :param status:  The current status of the event handler (required)
-        :type status: str
-        :param event_matching_pattern:  (required)
-        :type event_matching_pattern: lusid_workflow.EventMatchingPattern
-        :param run_as_user_id:  (required)
-        :type run_as_user_id: lusid_workflow.EventHandlerMapping
-        :param task_definition_id:  (required)
-        :type task_definition_id: lusid_workflow.ResourceId
-        :param task_definition_as_at:  AsAt of the required task definition
-        :type task_definition_as_at: datetime
-        :param task_activity:  Defines what the event handler should do after being triggered (required)
-        :type task_activity: object
+        :param states:  The states this Task Definition operates over (required)
+        :type states: list[lusid_workflow.TaskStateDefinition]
+        :param field_schema:  The Fields that this Task Definition operates on
+        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
+        :param initial_state:  (required)
+        :type initial_state: lusid_workflow.InitialState
+        :param triggers:  The Triggers for State transition
+        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
+        :param actions:  The Actions of this Task - executed after a Transition completion
+        :type actions: list[lusid_workflow.ActionDefinitionResponse]
+        :param transitions:  The Transitions between States
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
+        self._version = None
         self._display_name = None
         self._description = None
-        self._status = None
-        self._event_matching_pattern = None
-        self._run_as_user_id = None
-        self._task_definition_id = None
-        self._task_definition_as_at = None
-        self._task_activity = None
+        self._states = None
+        self._field_schema = None
+        self._initial_state = None
+        self._triggers = None
+        self._actions = None
+        self._transitions = None
         self.discriminator = None
 
         self.id = id
+        if version is not None:
+            self.version = version
         self.display_name = display_name
         self.description = description
-        self.status = status
-        self.event_matching_pattern = event_matching_pattern
-        self.run_as_user_id = run_as_user_id
-        self.task_definition_id = task_definition_id
-        self.task_definition_as_at = task_definition_as_at
-        self.task_activity = task_activity
+        self.states = states
+        self.field_schema = field_schema
+        self.initial_state = initial_state
+        self.triggers = triggers
+        self.actions = actions
+        self.transitions = transitions
 
     @property
     def id(self):
-        """Gets the id of this CreateEventHandlerRequest.  # noqa: E501
+        """Gets the id of this TaskDefinition.  # noqa: E501
 
 
-        :return: The id of this CreateEventHandlerRequest.  # noqa: E501
+        :return: The id of this TaskDefinition.  # noqa: E501
         :rtype: lusid_workflow.ResourceId
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this CreateEventHandlerRequest.
+        """Sets the id of this TaskDefinition.
 
 
-        :param id: The id of this CreateEventHandlerRequest.  # noqa: E501
+        :param id: The id of this TaskDefinition.  # noqa: E501
         :type id: lusid_workflow.ResourceId
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
+    def version(self):
+        """Gets the version of this TaskDefinition.  # noqa: E501
+
+
+        :return: The version of this TaskDefinition.  # noqa: E501
+        :rtype: lusid_workflow.VersionInfo
+        """
+        return self._version
+
+    @version.setter
+    def version(self, version):
+        """Sets the version of this TaskDefinition.
+
+
+        :param version: The version of this TaskDefinition.  # noqa: E501
+        :type version: lusid_workflow.VersionInfo
+        """
+
+        self._version = version
+
+    @property
     def display_name(self):
-        """Gets the display_name of this CreateEventHandlerRequest.  # noqa: E501
+        """Gets the display_name of this TaskDefinition.  # noqa: E501
 
         Human readable name  # noqa: E501
 
-        :return: The display_name of this CreateEventHandlerRequest.  # noqa: E501
+        :return: The display_name of this TaskDefinition.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this CreateEventHandlerRequest.
+        """Sets the display_name of this TaskDefinition.
 
         Human readable name  # noqa: E501
 
-        :param display_name: The display_name of this CreateEventHandlerRequest.  # noqa: E501
+        :param display_name: The display_name of this TaskDefinition.  # noqa: E501
         :type display_name: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) < 1):
             raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this CreateEventHandlerRequest.  # noqa: E501
+        """Gets the description of this TaskDefinition.  # noqa: E501
 
         Human readable description  # noqa: E501
 
-        :return: The description of this CreateEventHandlerRequest.  # noqa: E501
+        :return: The description of this TaskDefinition.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateEventHandlerRequest.
+        """Sets the description of this TaskDefinition.
 
         Human readable description  # noqa: E501
 
-        :param description: The description of this CreateEventHandlerRequest.  # noqa: E501
+        :param description: The description of this TaskDefinition.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
-    def status(self):
-        """Gets the status of this CreateEventHandlerRequest.  # noqa: E501
+    def states(self):
+        """Gets the states of this TaskDefinition.  # noqa: E501
 
-        The current status of the event handler  # noqa: E501
+        The states this Task Definition operates over  # noqa: E501
 
-        :return: The status of this CreateEventHandlerRequest.  # noqa: E501
-        :rtype: str
+        :return: The states of this TaskDefinition.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskStateDefinition]
         """
-        return self._status
+        return self._states
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this CreateEventHandlerRequest.
+    @states.setter
+    def states(self, states):
+        """Sets the states of this TaskDefinition.
 
-        The current status of the event handler  # noqa: E501
+        The states this Task Definition operates over  # noqa: E501
 
-        :param status: The status of this CreateEventHandlerRequest.  # noqa: E501
-        :type status: str
+        :param states: The states of this TaskDefinition.  # noqa: E501
+        :type states: list[lusid_workflow.TaskStateDefinition]
         """
-        if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
-            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and states is None:  # noqa: E501
+            raise ValueError("Invalid value for `states`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                status is not None and len(status) < 1):
-            raise ValueError("Invalid value for `status`, length must be greater than or equal to `1`")  # noqa: E501
+                states is not None and len(states) < 1):
+            raise ValueError("Invalid value for `states`, number of items must be greater than or equal to `1`")  # noqa: E501
 
-        self._status = status
+        self._states = states
 
     @property
-    def event_matching_pattern(self):
-        """Gets the event_matching_pattern of this CreateEventHandlerRequest.  # noqa: E501
+    def field_schema(self):
+        """Gets the field_schema of this TaskDefinition.  # noqa: E501
 
+        The Fields that this Task Definition operates on  # noqa: E501
 
-        :return: The event_matching_pattern of this CreateEventHandlerRequest.  # noqa: E501
-        :rtype: lusid_workflow.EventMatchingPattern
+        :return: The field_schema of this TaskDefinition.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskFieldDefinition]
         """
-        return self._event_matching_pattern
+        return self._field_schema
 
-    @event_matching_pattern.setter
-    def event_matching_pattern(self, event_matching_pattern):
-        """Sets the event_matching_pattern of this CreateEventHandlerRequest.
+    @field_schema.setter
+    def field_schema(self, field_schema):
+        """Sets the field_schema of this TaskDefinition.
 
+        The Fields that this Task Definition operates on  # noqa: E501
 
-        :param event_matching_pattern: The event_matching_pattern of this CreateEventHandlerRequest.  # noqa: E501
-        :type event_matching_pattern: lusid_workflow.EventMatchingPattern
+        :param field_schema: The field_schema of this TaskDefinition.  # noqa: E501
+        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         """
-        if self.local_vars_configuration.client_side_validation and event_matching_pattern is None:  # noqa: E501
-            raise ValueError("Invalid value for `event_matching_pattern`, must not be `None`")  # noqa: E501
 
-        self._event_matching_pattern = event_matching_pattern
+        self._field_schema = field_schema
 
     @property
-    def run_as_user_id(self):
-        """Gets the run_as_user_id of this CreateEventHandlerRequest.  # noqa: E501
+    def initial_state(self):
+        """Gets the initial_state of this TaskDefinition.  # noqa: E501
 
 
-        :return: The run_as_user_id of this CreateEventHandlerRequest.  # noqa: E501
-        :rtype: lusid_workflow.EventHandlerMapping
+        :return: The initial_state of this TaskDefinition.  # noqa: E501
+        :rtype: lusid_workflow.InitialState
         """
-        return self._run_as_user_id
+        return self._initial_state
 
-    @run_as_user_id.setter
-    def run_as_user_id(self, run_as_user_id):
-        """Sets the run_as_user_id of this CreateEventHandlerRequest.
+    @initial_state.setter
+    def initial_state(self, initial_state):
+        """Sets the initial_state of this TaskDefinition.
 
 
-        :param run_as_user_id: The run_as_user_id of this CreateEventHandlerRequest.  # noqa: E501
-        :type run_as_user_id: lusid_workflow.EventHandlerMapping
+        :param initial_state: The initial_state of this TaskDefinition.  # noqa: E501
+        :type initial_state: lusid_workflow.InitialState
         """
-        if self.local_vars_configuration.client_side_validation and run_as_user_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `run_as_user_id`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and initial_state is None:  # noqa: E501
+            raise ValueError("Invalid value for `initial_state`, must not be `None`")  # noqa: E501
 
-        self._run_as_user_id = run_as_user_id
+        self._initial_state = initial_state
 
     @property
-    def task_definition_id(self):
-        """Gets the task_definition_id of this CreateEventHandlerRequest.  # noqa: E501
+    def triggers(self):
+        """Gets the triggers of this TaskDefinition.  # noqa: E501
 
+        The Triggers for State transition  # noqa: E501
 
-        :return: The task_definition_id of this CreateEventHandlerRequest.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
+        :return: The triggers of this TaskDefinition.  # noqa: E501
+        :rtype: list[lusid_workflow.TransitionTriggerDefinition]
         """
-        return self._task_definition_id
+        return self._triggers
 
-    @task_definition_id.setter
-    def task_definition_id(self, task_definition_id):
-        """Sets the task_definition_id of this CreateEventHandlerRequest.
+    @triggers.setter
+    def triggers(self, triggers):
+        """Sets the triggers of this TaskDefinition.
 
+        The Triggers for State transition  # noqa: E501
 
-        :param task_definition_id: The task_definition_id of this CreateEventHandlerRequest.  # noqa: E501
-        :type task_definition_id: lusid_workflow.ResourceId
+        :param triggers: The triggers of this TaskDefinition.  # noqa: E501
+        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         """
-        if self.local_vars_configuration.client_side_validation and task_definition_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `task_definition_id`, must not be `None`")  # noqa: E501
 
-        self._task_definition_id = task_definition_id
+        self._triggers = triggers
 
     @property
-    def task_definition_as_at(self):
-        """Gets the task_definition_as_at of this CreateEventHandlerRequest.  # noqa: E501
+    def actions(self):
+        """Gets the actions of this TaskDefinition.  # noqa: E501
 
-        AsAt of the required task definition  # noqa: E501
+        The Actions of this Task - executed after a Transition completion  # noqa: E501
 
-        :return: The task_definition_as_at of this CreateEventHandlerRequest.  # noqa: E501
-        :rtype: datetime
+        :return: The actions of this TaskDefinition.  # noqa: E501
+        :rtype: list[lusid_workflow.ActionDefinitionResponse]
         """
-        return self._task_definition_as_at
+        return self._actions
 
-    @task_definition_as_at.setter
-    def task_definition_as_at(self, task_definition_as_at):
-        """Sets the task_definition_as_at of this CreateEventHandlerRequest.
+    @actions.setter
+    def actions(self, actions):
+        """Sets the actions of this TaskDefinition.
 
-        AsAt of the required task definition  # noqa: E501
+        The Actions of this Task - executed after a Transition completion  # noqa: E501
 
-        :param task_definition_as_at: The task_definition_as_at of this CreateEventHandlerRequest.  # noqa: E501
-        :type task_definition_as_at: datetime
+        :param actions: The actions of this TaskDefinition.  # noqa: E501
+        :type actions: list[lusid_workflow.ActionDefinitionResponse]
         """
 
-        self._task_definition_as_at = task_definition_as_at
+        self._actions = actions
 
     @property
-    def task_activity(self):
-        """Gets the task_activity of this CreateEventHandlerRequest.  # noqa: E501
+    def transitions(self):
+        """Gets the transitions of this TaskDefinition.  # noqa: E501
 
-        Defines what the event handler should do after being triggered  # noqa: E501
+        The Transitions between States  # noqa: E501
 
-        :return: The task_activity of this CreateEventHandlerRequest.  # noqa: E501
-        :rtype: object
+        :return: The transitions of this TaskDefinition.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskTransitionDefinition]
         """
-        return self._task_activity
+        return self._transitions
 
-    @task_activity.setter
-    def task_activity(self, task_activity):
-        """Sets the task_activity of this CreateEventHandlerRequest.
+    @transitions.setter
+    def transitions(self, transitions):
+        """Sets the transitions of this TaskDefinition.
 
-        Defines what the event handler should do after being triggered  # noqa: E501
+        The Transitions between States  # noqa: E501
 
-        :param task_activity: The task_activity of this CreateEventHandlerRequest.  # noqa: E501
-        :type task_activity: object
+        :param transitions: The transitions of this TaskDefinition.  # noqa: E501
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
         """
 
-        self._task_activity = task_activity
+        self._transitions = transitions
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -377,18 +406,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateEventHandlerRequest):
+        if not isinstance(other, TaskDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateEventHandlerRequest):
+        if not isinstance(other, TaskDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/create_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/deleted_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/event_handler.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_transition_definition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class EventHandler(object):
+class TaskTransitionDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,342 +35,234 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'ResourceId',
-        'version': 'VersionInfo',
-        'display_name': 'str',
-        'description': 'str',
-        'status': 'str',
-        'event_matching_pattern': 'EventMatchingPattern',
-        'run_as_user_id': 'EventHandlerMapping',
-        'task_definition_id': 'ResourceId',
-        'task_definition_as_at': 'datetime',
-        'task_activity': 'object'
+        'from_state': 'str',
+        'to_state': 'str',
+        'trigger': 'str',
+        'guard': 'str',
+        'action': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
-        'version': 'version',
-        'display_name': 'displayName',
-        'description': 'description',
-        'status': 'status',
-        'event_matching_pattern': 'eventMatchingPattern',
-        'run_as_user_id': 'runAsUserId',
-        'task_definition_id': 'taskDefinitionId',
-        'task_definition_as_at': 'taskDefinitionAsAt',
-        'task_activity': 'taskActivity'
+        'from_state': 'fromState',
+        'to_state': 'toState',
+        'trigger': 'trigger',
+        'guard': 'guard',
+        'action': 'action'
     }
 
     required_map = {
-        'id': 'required',
-        'version': 'optional',
-        'display_name': 'required',
-        'description': 'optional',
-        'status': 'required',
-        'event_matching_pattern': 'required',
-        'run_as_user_id': 'required',
-        'task_definition_id': 'required',
-        'task_definition_as_at': 'optional',
-        'task_activity': 'required'
+        'from_state': 'required',
+        'to_state': 'required',
+        'trigger': 'required',
+        'guard': 'optional',
+        'action': 'optional'
     }
 
-    def __init__(self, id=None, version=None, display_name=None, description=None, status=None, event_matching_pattern=None, run_as_user_id=None, task_definition_id=None, task_definition_as_at=None, task_activity=None, local_vars_configuration=None):  # noqa: E501
-        """EventHandler - a model defined in OpenAPI"
+    def __init__(self, from_state=None, to_state=None, trigger=None, guard=None, action=None, local_vars_configuration=None):  # noqa: E501
+        """TaskTransitionDefinition - a model defined in OpenAPI"
         
-        :param id:  (required)
-        :type id: lusid_workflow.ResourceId
-        :param version: 
-        :type version: lusid_workflow.VersionInfo
-        :param display_name:  Human readable name (required)
-        :type display_name: str
-        :param description:  Human readable description
-        :type description: str
-        :param status:  The current status of the event handler (required)
-        :type status: str
-        :param event_matching_pattern:  (required)
-        :type event_matching_pattern: lusid_workflow.EventMatchingPattern
-        :param run_as_user_id:  (required)
-        :type run_as_user_id: lusid_workflow.EventHandlerMapping
-        :param task_definition_id:  (required)
-        :type task_definition_id: lusid_workflow.ResourceId
-        :param task_definition_as_at:  AsAt of the required task definition
-        :type task_definition_as_at: datetime
-        :param task_activity:  Defines what the event handler should do after being triggered (required)
-        :type task_activity: object
+        :param from_state:  The State this Transition if coming From (required)
+        :type from_state: str
+        :param to_state:  The State this Transition is going To (required)
+        :type to_state: str
+        :param trigger:  The Trigger for this Transition (required)
+        :type trigger: str
+        :param guard:  The Guard for this Transition, if any
+        :type guard: str
+        :param action:  The Action to invoke on successful Transition
+        :type action: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._version = None
-        self._display_name = None
-        self._description = None
-        self._status = None
-        self._event_matching_pattern = None
-        self._run_as_user_id = None
-        self._task_definition_id = None
-        self._task_definition_as_at = None
-        self._task_activity = None
+        self._from_state = None
+        self._to_state = None
+        self._trigger = None
+        self._guard = None
+        self._action = None
         self.discriminator = None
 
-        self.id = id
-        if version is not None:
-            self.version = version
-        self.display_name = display_name
-        self.description = description
-        self.status = status
-        self.event_matching_pattern = event_matching_pattern
-        self.run_as_user_id = run_as_user_id
-        self.task_definition_id = task_definition_id
-        self.task_definition_as_at = task_definition_as_at
-        self.task_activity = task_activity
+        self.from_state = from_state
+        self.to_state = to_state
+        self.trigger = trigger
+        self.guard = guard
+        self.action = action
 
     @property
-    def id(self):
-        """Gets the id of this EventHandler.  # noqa: E501
+    def from_state(self):
+        """Gets the from_state of this TaskTransitionDefinition.  # noqa: E501
 
+        The State this Transition if coming From  # noqa: E501
 
-        :return: The id of this EventHandler.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this EventHandler.
-
-
-        :param id: The id of this EventHandler.  # noqa: E501
-        :type id: lusid_workflow.ResourceId
-        """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-
-        self._id = id
-
-    @property
-    def version(self):
-        """Gets the version of this EventHandler.  # noqa: E501
-
-
-        :return: The version of this EventHandler.  # noqa: E501
-        :rtype: lusid_workflow.VersionInfo
-        """
-        return self._version
-
-    @version.setter
-    def version(self, version):
-        """Sets the version of this EventHandler.
-
-
-        :param version: The version of this EventHandler.  # noqa: E501
-        :type version: lusid_workflow.VersionInfo
-        """
-
-        self._version = version
-
-    @property
-    def display_name(self):
-        """Gets the display_name of this EventHandler.  # noqa: E501
-
-        Human readable name  # noqa: E501
-
-        :return: The display_name of this EventHandler.  # noqa: E501
+        :return: The from_state of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
-        return self._display_name
+        return self._from_state
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this EventHandler.
+    @from_state.setter
+    def from_state(self, from_state):
+        """Sets the from_state of this TaskTransitionDefinition.
 
-        Human readable name  # noqa: E501
+        The State this Transition if coming From  # noqa: E501
 
-        :param display_name: The display_name of this EventHandler.  # noqa: E501
-        :type display_name: str
+        :param from_state: The from_state of this TaskTransitionDefinition.  # noqa: E501
+        :type from_state: str
         """
-        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and from_state is None:  # noqa: E501
+            raise ValueError("Invalid value for `from_state`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                from_state is not None and len(from_state) > 1024):
+            raise ValueError("Invalid value for `from_state`, length must be less than or equal to `1024`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 1):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
+                from_state is not None and len(from_state) < 1):
+            raise ValueError("Invalid value for `from_state`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                from_state is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', from_state)):  # noqa: E501
+            raise ValueError(r"Invalid value for `from_state`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
-        self._display_name = display_name
+        self._from_state = from_state
 
     @property
-    def description(self):
-        """Gets the description of this EventHandler.  # noqa: E501
+    def to_state(self):
+        """Gets the to_state of this TaskTransitionDefinition.  # noqa: E501
 
-        Human readable description  # noqa: E501
+        The State this Transition is going To  # noqa: E501
 
-        :return: The description of this EventHandler.  # noqa: E501
+        :return: The to_state of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._to_state
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this EventHandler.
+    @to_state.setter
+    def to_state(self, to_state):
+        """Sets the to_state of this TaskTransitionDefinition.
 
-        Human readable description  # noqa: E501
+        The State this Transition is going To  # noqa: E501
 
-        :param description: The description of this EventHandler.  # noqa: E501
-        :type description: str
+        :param to_state: The to_state of this TaskTransitionDefinition.  # noqa: E501
+        :type to_state: str
         """
+        if self.local_vars_configuration.client_side_validation and to_state is None:  # noqa: E501
+            raise ValueError("Invalid value for `to_state`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                to_state is not None and len(to_state) > 1024):
+            raise ValueError("Invalid value for `to_state`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                to_state is not None and len(to_state) < 1):
+            raise ValueError("Invalid value for `to_state`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                to_state is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', to_state)):  # noqa: E501
+            raise ValueError(r"Invalid value for `to_state`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
-        self._description = description
+        self._to_state = to_state
 
     @property
-    def status(self):
-        """Gets the status of this EventHandler.  # noqa: E501
+    def trigger(self):
+        """Gets the trigger of this TaskTransitionDefinition.  # noqa: E501
 
-        The current status of the event handler  # noqa: E501
+        The Trigger for this Transition  # noqa: E501
 
-        :return: The status of this EventHandler.  # noqa: E501
+        :return: The trigger of this TaskTransitionDefinition.  # noqa: E501
         :rtype: str
         """
-        return self._status
+        return self._trigger
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this EventHandler.
+    @trigger.setter
+    def trigger(self, trigger):
+        """Sets the trigger of this TaskTransitionDefinition.
 
-        The current status of the event handler  # noqa: E501
+        The Trigger for this Transition  # noqa: E501
 
-        :param status: The status of this EventHandler.  # noqa: E501
-        :type status: str
+        :param trigger: The trigger of this TaskTransitionDefinition.  # noqa: E501
+        :type trigger: str
         """
-        if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
-            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and trigger is None:  # noqa: E501
+            raise ValueError("Invalid value for `trigger`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                status is not None and len(status) < 1):
-            raise ValueError("Invalid value for `status`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._status = status
-
-    @property
-    def event_matching_pattern(self):
-        """Gets the event_matching_pattern of this EventHandler.  # noqa: E501
-
-
-        :return: The event_matching_pattern of this EventHandler.  # noqa: E501
-        :rtype: lusid_workflow.EventMatchingPattern
-        """
-        return self._event_matching_pattern
-
-    @event_matching_pattern.setter
-    def event_matching_pattern(self, event_matching_pattern):
-        """Sets the event_matching_pattern of this EventHandler.
-
-
-        :param event_matching_pattern: The event_matching_pattern of this EventHandler.  # noqa: E501
-        :type event_matching_pattern: lusid_workflow.EventMatchingPattern
-        """
-        if self.local_vars_configuration.client_side_validation and event_matching_pattern is None:  # noqa: E501
-            raise ValueError("Invalid value for `event_matching_pattern`, must not be `None`")  # noqa: E501
-
-        self._event_matching_pattern = event_matching_pattern
-
-    @property
-    def run_as_user_id(self):
-        """Gets the run_as_user_id of this EventHandler.  # noqa: E501
-
-
-        :return: The run_as_user_id of this EventHandler.  # noqa: E501
-        :rtype: lusid_workflow.EventHandlerMapping
-        """
-        return self._run_as_user_id
-
-    @run_as_user_id.setter
-    def run_as_user_id(self, run_as_user_id):
-        """Sets the run_as_user_id of this EventHandler.
-
-
-        :param run_as_user_id: The run_as_user_id of this EventHandler.  # noqa: E501
-        :type run_as_user_id: lusid_workflow.EventHandlerMapping
-        """
-        if self.local_vars_configuration.client_side_validation and run_as_user_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `run_as_user_id`, must not be `None`")  # noqa: E501
-
-        self._run_as_user_id = run_as_user_id
-
-    @property
-    def task_definition_id(self):
-        """Gets the task_definition_id of this EventHandler.  # noqa: E501
-
-
-        :return: The task_definition_id of this EventHandler.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
-        """
-        return self._task_definition_id
-
-    @task_definition_id.setter
-    def task_definition_id(self, task_definition_id):
-        """Sets the task_definition_id of this EventHandler.
-
-
-        :param task_definition_id: The task_definition_id of this EventHandler.  # noqa: E501
-        :type task_definition_id: lusid_workflow.ResourceId
-        """
-        if self.local_vars_configuration.client_side_validation and task_definition_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `task_definition_id`, must not be `None`")  # noqa: E501
+                trigger is not None and len(trigger) > 1024):
+            raise ValueError("Invalid value for `trigger`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                trigger is not None and len(trigger) < 1):
+            raise ValueError("Invalid value for `trigger`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                trigger is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', trigger)):  # noqa: E501
+            raise ValueError(r"Invalid value for `trigger`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
-        self._task_definition_id = task_definition_id
+        self._trigger = trigger
 
     @property
-    def task_definition_as_at(self):
-        """Gets the task_definition_as_at of this EventHandler.  # noqa: E501
+    def guard(self):
+        """Gets the guard of this TaskTransitionDefinition.  # noqa: E501
 
-        AsAt of the required task definition  # noqa: E501
+        The Guard for this Transition, if any  # noqa: E501
 
-        :return: The task_definition_as_at of this EventHandler.  # noqa: E501
-        :rtype: datetime
+        :return: The guard of this TaskTransitionDefinition.  # noqa: E501
+        :rtype: str
         """
-        return self._task_definition_as_at
+        return self._guard
 
-    @task_definition_as_at.setter
-    def task_definition_as_at(self, task_definition_as_at):
-        """Sets the task_definition_as_at of this EventHandler.
+    @guard.setter
+    def guard(self, guard):
+        """Sets the guard of this TaskTransitionDefinition.
 
-        AsAt of the required task definition  # noqa: E501
+        The Guard for this Transition, if any  # noqa: E501
 
-        :param task_definition_as_at: The task_definition_as_at of this EventHandler.  # noqa: E501
-        :type task_definition_as_at: datetime
+        :param guard: The guard of this TaskTransitionDefinition.  # noqa: E501
+        :type guard: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                guard is not None and len(guard) > 1024):
+            raise ValueError("Invalid value for `guard`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                guard is not None and len(guard) < 1):
+            raise ValueError("Invalid value for `guard`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                guard is not None and not re.search(r'^[\s\S]*$', guard)):  # noqa: E501
+            raise ValueError(r"Invalid value for `guard`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
-        self._task_definition_as_at = task_definition_as_at
+        self._guard = guard
 
     @property
-    def task_activity(self):
-        """Gets the task_activity of this EventHandler.  # noqa: E501
+    def action(self):
+        """Gets the action of this TaskTransitionDefinition.  # noqa: E501
 
-        Defines what the event handler should do after being triggered  # noqa: E501
+        The Action to invoke on successful Transition  # noqa: E501
 
-        :return: The task_activity of this EventHandler.  # noqa: E501
-        :rtype: object
+        :return: The action of this TaskTransitionDefinition.  # noqa: E501
+        :rtype: str
         """
-        return self._task_activity
+        return self._action
 
-    @task_activity.setter
-    def task_activity(self, task_activity):
-        """Sets the task_activity of this EventHandler.
+    @action.setter
+    def action(self, action):
+        """Sets the action of this TaskTransitionDefinition.
 
-        Defines what the event handler should do after being triggered  # noqa: E501
+        The Action to invoke on successful Transition  # noqa: E501
 
-        :param task_activity: The task_activity of this EventHandler.  # noqa: E501
-        :type task_activity: object
+        :param action: The action of this TaskTransitionDefinition.  # noqa: E501
+        :type action: str
         """
+        if (self.local_vars_configuration.client_side_validation and
+                action is not None and len(action) > 1024):
+            raise ValueError("Invalid value for `action`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                action is not None and len(action) < 1):
+            raise ValueError("Invalid value for `action`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                action is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', action)):  # noqa: E501
+            raise ValueError(r"Invalid value for `action`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
-        self._task_activity = task_activity
+        self._action = action
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -406,18 +298,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EventHandler):
+        if not isinstance(other, TaskTransitionDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, EventHandler):
+        if not isinstance(other, TaskTransitionDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/event_handler_mapping.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_instance_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class EventHandlerMapping(object):
+class TaskInstanceField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,93 +35,98 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'map_from': 'str',
-        'set_to': 'str'
+        'name': 'str',
+        'value': 'object'
     }
 
     attribute_map = {
-        'map_from': 'mapFrom',
-        'set_to': 'setTo'
+        'name': 'name',
+        'value': 'value'
     }
 
     required_map = {
-        'map_from': 'optional',
-        'set_to': 'optional'
+        'name': 'required',
+        'value': 'optional'
     }
 
-    def __init__(self, map_from=None, set_to=None, local_vars_configuration=None):  # noqa: E501
-        """EventHandlerMapping - a model defined in OpenAPI"
+    def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
+        """TaskInstanceField - a model defined in OpenAPI"
         
-        :param map_from:  The field to map from
-        :type map_from: str
-        :param set_to:  The (constant) value to set
-        :type set_to: str
+        :param name:  The name of this Field (required)
+        :type name: str
+        :param value:  The value of this Field
+        :type value: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._map_from = None
-        self._set_to = None
+        self._name = None
+        self._value = None
         self.discriminator = None
 
-        self.map_from = map_from
-        self.set_to = set_to
+        self.name = name
+        self.value = value
 
     @property
-    def map_from(self):
-        """Gets the map_from of this EventHandlerMapping.  # noqa: E501
+    def name(self):
+        """Gets the name of this TaskInstanceField.  # noqa: E501
 
-        The field to map from  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :return: The map_from of this EventHandlerMapping.  # noqa: E501
+        :return: The name of this TaskInstanceField.  # noqa: E501
         :rtype: str
         """
-        return self._map_from
+        return self._name
 
-    @map_from.setter
-    def map_from(self, map_from):
-        """Sets the map_from of this EventHandlerMapping.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this TaskInstanceField.
 
-        The field to map from  # noqa: E501
+        The name of this Field  # noqa: E501
 
-        :param map_from: The map_from of this EventHandlerMapping.  # noqa: E501
-        :type map_from: str
+        :param name: The name of this TaskInstanceField.  # noqa: E501
+        :type name: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
-        self._map_from = map_from
+        self._name = name
 
     @property
-    def set_to(self):
-        """Gets the set_to of this EventHandlerMapping.  # noqa: E501
+    def value(self):
+        """Gets the value of this TaskInstanceField.  # noqa: E501
 
-        The (constant) value to set  # noqa: E501
+        The value of this Field  # noqa: E501
 
-        :return: The set_to of this EventHandlerMapping.  # noqa: E501
-        :rtype: str
+        :return: The value of this TaskInstanceField.  # noqa: E501
+        :rtype: object
         """
-        return self._set_to
+        return self._value
 
-    @set_to.setter
-    def set_to(self, set_to):
-        """Sets the set_to of this EventHandlerMapping.
+    @value.setter
+    def value(self, value):
+        """Sets the value of this TaskInstanceField.
 
-        The (constant) value to set  # noqa: E501
+        The value of this Field  # noqa: E501
 
-        :param set_to: The set_to of this EventHandlerMapping.  # noqa: E501
-        :type set_to: str
+        :param value: The value of this TaskInstanceField.  # noqa: E501
+        :type value: object
         """
 
-        self._set_to = set_to
+        self._value = value
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -157,18 +162,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EventHandlerMapping):
+        if not isinstance(other, TaskInstanceField):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, EventHandlerMapping):
+        if not isinstance(other, TaskInstanceField):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/event_matching_pattern.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/luminesce_view.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class EventMatchingPattern(object):
+class LuminesceView(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,104 +35,112 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'event_type': 'str',
-        'filter': 'str'
+        'type': 'str',
+        'name': 'str'
     }
 
     attribute_map = {
-        'event_type': 'eventType',
-        'filter': 'filter'
+        'type': 'type',
+        'name': 'name'
     }
 
     required_map = {
-        'event_type': 'required',
-        'filter': 'optional'
+        'type': 'required',
+        'name': 'required'
     }
 
-    def __init__(self, event_type=None, filter=None, local_vars_configuration=None):  # noqa: E501
-        """EventMatchingPattern - a model defined in OpenAPI"
+    def __init__(self, type=None, name=None, local_vars_configuration=None):  # noqa: E501
+        """LuminesceView - a model defined in OpenAPI"
         
-        :param event_type:  The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint in the Notifications service (required)
-        :type event_type: str
-        :param filter:  A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information.  If not provided, all events will be matched.
-        :type filter: str
+        :param type:  The type of worker (required)
+        :type type: str
+        :param name:  Name of the view in Luminesce (required)
+        :type name: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._event_type = None
-        self._filter = None
+        self._type = None
+        self._name = None
         self.discriminator = None
 
-        self.event_type = event_type
-        self.filter = filter
+        self.type = type
+        self.name = name
 
     @property
-    def event_type(self):
-        """Gets the event_type of this EventMatchingPattern.  # noqa: E501
+    def type(self):
+        """Gets the type of this LuminesceView.  # noqa: E501
 
-        The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint in the Notifications service  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :return: The event_type of this EventMatchingPattern.  # noqa: E501
+        :return: The type of this LuminesceView.  # noqa: E501
         :rtype: str
         """
-        return self._event_type
+        return self._type
 
-    @event_type.setter
-    def event_type(self, event_type):
-        """Sets the event_type of this EventMatchingPattern.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this LuminesceView.
 
-        The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint in the Notifications service  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :param event_type: The event_type of this EventMatchingPattern.  # noqa: E501
-        :type event_type: str
+        :param type: The type of this LuminesceView.  # noqa: E501
+        :type type: str
         """
-        if self.local_vars_configuration.client_side_validation and event_type is None:  # noqa: E501
-            raise ValueError("Invalid value for `event_type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                event_type is not None and len(event_type) > 512):
-            raise ValueError("Invalid value for `event_type`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                event_type is not None and len(event_type) < 0):
-            raise ValueError("Invalid value for `event_type`, length must be greater than or equal to `0`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                event_type is not None and not re.search(r'^[a-zA-Z]*$', event_type)):  # noqa: E501
-            raise ValueError(r"Invalid value for `event_type`, must be a follow pattern or equal to `/^[a-zA-Z]*$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["LuminesceView"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
-        self._event_type = event_type
+        self._type = type
 
     @property
-    def filter(self):
-        """Gets the filter of this EventMatchingPattern.  # noqa: E501
+    def name(self):
+        """Gets the name of this LuminesceView.  # noqa: E501
 
-        A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information.  If not provided, all events will be matched.  # noqa: E501
+        Name of the view in Luminesce  # noqa: E501
 
-        :return: The filter of this EventMatchingPattern.  # noqa: E501
+        :return: The name of this LuminesceView.  # noqa: E501
         :rtype: str
         """
-        return self._filter
+        return self._name
 
-    @filter.setter
-    def filter(self, filter):
-        """Sets the filter of this EventMatchingPattern.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this LuminesceView.
 
-        A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information.  If not provided, all events will be matched.  # noqa: E501
+        Name of the view in Luminesce  # noqa: E501
 
-        :param filter: The filter of this EventMatchingPattern.  # noqa: E501
-        :type filter: str
+        :param name: The name of this LuminesceView.  # noqa: E501
+        :type name: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) > 512):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `512`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'^[\s\S]*$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
-        self._filter = filter
+        self._name = name
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -168,18 +176,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EventMatchingPattern):
+        if not isinstance(other, LuminesceView):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, EventMatchingPattern):
+        if not isinstance(other, LuminesceView):
             return True
 
         return self.to_dict() != other.to_dict()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/fail.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/fail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/fail_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/fail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/field_mapping.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/field_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/get_worker_result_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/get_worker_result_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/health_check.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/health_check_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/health_check_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/initial_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/luminesce_view.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/parameter_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class LuminesceView(object):
+class ParameterValue(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,113 +35,105 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
-        'name': 'str'
+        'name': 'str',
+        'value': 'object'
     }
 
     attribute_map = {
-        'type': 'type',
-        'name': 'name'
+        'name': 'name',
+        'value': 'value'
     }
 
     required_map = {
-        'type': 'required',
-        'name': 'required'
+        'name': 'required',
+        'value': 'optional'
     }
 
-    def __init__(self, type=None, name=None, local_vars_configuration=None):  # noqa: E501
-        """LuminesceView - a model defined in OpenAPI"
+    def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
+        """ParameterValue - a model defined in OpenAPI"
         
-        :param type:  The type of worker (required)
-        :type type: str
-        :param name:  Name of the view in Luminesce (required)
+        :param name:  Name (required)
         :type name: str
+        :param value:  Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)
+        :type value: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
         self._name = None
+        self._value = None
         self.discriminator = None
 
-        self.type = type
         self.name = name
-
-    @property
-    def type(self):
-        """Gets the type of this LuminesceView.  # noqa: E501
-
-        The type of worker  # noqa: E501
-
-        :return: The type of this LuminesceView.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this LuminesceView.
-
-        The type of worker  # noqa: E501
-
-        :param type: The type of this LuminesceView.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["LuminesceView"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                .format(type, allowed_values)
-            )
-
-        self._type = type
+        self.value = value
 
     @property
     def name(self):
-        """Gets the name of this LuminesceView.  # noqa: E501
+        """Gets the name of this ParameterValue.  # noqa: E501
 
-        Name of the view in Luminesce  # noqa: E501
+        Name  # noqa: E501
 
-        :return: The name of this LuminesceView.  # noqa: E501
+        :return: The name of this ParameterValue.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this LuminesceView.
+        """Sets the name of this ParameterValue.
 
-        Name of the view in Luminesce  # noqa: E501
+        Name  # noqa: E501
 
-        :param name: The name of this LuminesceView.  # noqa: E501
+        :param name: The name of this ParameterValue.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 512):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `512`")  # noqa: E501
+                name is not None and len(name) > 1024):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `1024`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 name is not None and len(name) < 1):
             raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                name is not None and not re.search(r'^[\s\S]*$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
+                name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
         self._name = name
 
+    @property
+    def value(self):
+        """Gets the value of this ParameterValue.  # noqa: E501
+
+        Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)  # noqa: E501
+
+        :return: The value of this ParameterValue.  # noqa: E501
+        :rtype: object
+        """
+        return self._value
+
+    @value.setter
+    def value(self, value):
+        """Sets the value of this ParameterValue.
+
+        Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)  # noqa: E501
+
+        :param value: The value of this ParameterValue.  # noqa: E501
+        :type value: object
+        """
+
+        self._value = value
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -176,18 +168,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LuminesceView):
+        if not isinstance(other, ParameterValue):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LuminesceView):
+        if not isinstance(other, ParameterValue):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/luminesce_view_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/luminesce_view_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/parameter.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/parameter_value.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/scheduler_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class ParameterValue(object):
+class SchedulerJob(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,104 +35,101 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'name': 'str',
-        'value': 'object'
+        'type': 'str',
+        'job_id': 'ResourceId'
     }
 
     attribute_map = {
-        'name': 'name',
-        'value': 'value'
+        'type': 'type',
+        'job_id': 'jobId'
     }
 
     required_map = {
-        'name': 'required',
-        'value': 'optional'
+        'type': 'required',
+        'job_id': 'required'
     }
 
-    def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
-        """ParameterValue - a model defined in OpenAPI"
+    def __init__(self, type=None, job_id=None, local_vars_configuration=None):  # noqa: E501
+        """SchedulerJob - a model defined in OpenAPI"
         
-        :param name:  Name (required)
-        :type name: str
-        :param value:  Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)
-        :type value: object
+        :param type:  The type of worker (required)
+        :type type: str
+        :param job_id:  (required)
+        :type job_id: lusid_workflow.ResourceId
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._value = None
+        self._type = None
+        self._job_id = None
         self.discriminator = None
 
-        self.name = name
-        self.value = value
+        self.type = type
+        self.job_id = job_id
 
     @property
-    def name(self):
-        """Gets the name of this ParameterValue.  # noqa: E501
+    def type(self):
+        """Gets the type of this SchedulerJob.  # noqa: E501
 
-        Name  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :return: The name of this ParameterValue.  # noqa: E501
+        :return: The type of this SchedulerJob.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this ParameterValue.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this SchedulerJob.
 
-        Name  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :param name: The name of this ParameterValue.  # noqa: E501
-        :type name: str
+        :param type: The type of this SchedulerJob.  # noqa: E501
+        :type type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 1024):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `1024`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["SchedulerJob"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
-        self._name = name
+        self._type = type
 
     @property
-    def value(self):
-        """Gets the value of this ParameterValue.  # noqa: E501
+    def job_id(self):
+        """Gets the job_id of this SchedulerJob.  # noqa: E501
 
-        Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)  # noqa: E501
 
-        :return: The value of this ParameterValue.  # noqa: E501
-        :rtype: object
+        :return: The job_id of this SchedulerJob.  # noqa: E501
+        :rtype: lusid_workflow.ResourceId
         """
-        return self._value
+        return self._job_id
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this ParameterValue.
+    @job_id.setter
+    def job_id(self, job_id):
+        """Sets the job_id of this SchedulerJob.
 
-        Value which can be a String, Boolean, Decimal or DateTime (ISO 8601)  # noqa: E501
 
-        :param value: The value of this ParameterValue.  # noqa: E501
-        :type value: object
+        :param job_id: The job_id of this SchedulerJob.  # noqa: E501
+        :type job_id: lusid_workflow.ResourceId
         """
+        if self.local_vars_configuration.client_side_validation and job_id is None:  # noqa: E501
+            raise ValueError("Invalid value for `job_id`, must not be `None`")  # noqa: E501
 
-        self._value = value
+        self._job_id = job_id
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -168,18 +165,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ParameterValue):
+        if not isinstance(other, SchedulerJob):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ParameterValue):
+        if not isinstance(other, SchedulerJob):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/result_field.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/result_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/result_matching_pattern.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/result_matching_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_action.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_action_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/run_worker_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/run_worker_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/scheduler_job.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/scheduler_job_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class SchedulerJob(object):
+class SchedulerJobResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -45,89 +45,86 @@
 
     attribute_map = {
         'type': 'type',
         'job_id': 'jobId'
     }
 
     required_map = {
-        'type': 'required',
-        'job_id': 'required'
+        'type': 'optional',
+        'job_id': 'optional'
     }
 
     def __init__(self, type=None, job_id=None, local_vars_configuration=None):  # noqa: E501
-        """SchedulerJob - a model defined in OpenAPI"
+        """SchedulerJobResponse - a model defined in OpenAPI"
         
-        :param type:  The type of worker (required)
+        :param type:  The type of worker
         :type type: str
-        :param job_id:  (required)
+        :param job_id: 
         :type job_id: lusid_workflow.ResourceId
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._job_id = None
         self.discriminator = None
 
         self.type = type
-        self.job_id = job_id
+        if job_id is not None:
+            self.job_id = job_id
 
     @property
     def type(self):
-        """Gets the type of this SchedulerJob.  # noqa: E501
+        """Gets the type of this SchedulerJobResponse.  # noqa: E501
 
         The type of worker  # noqa: E501
 
-        :return: The type of this SchedulerJob.  # noqa: E501
+        :return: The type of this SchedulerJobResponse.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this SchedulerJob.
+        """Sets the type of this SchedulerJobResponse.
 
         The type of worker  # noqa: E501
 
-        :param type: The type of this SchedulerJob.  # noqa: E501
+        :param type: The type of this SchedulerJobResponse.  # noqa: E501
         :type type: str
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["SchedulerJob"]  # noqa: E501
+        allowed_values = [None,"SchedulerJob"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
 
     @property
     def job_id(self):
-        """Gets the job_id of this SchedulerJob.  # noqa: E501
+        """Gets the job_id of this SchedulerJobResponse.  # noqa: E501
 
 
-        :return: The job_id of this SchedulerJob.  # noqa: E501
+        :return: The job_id of this SchedulerJobResponse.  # noqa: E501
         :rtype: lusid_workflow.ResourceId
         """
         return self._job_id
 
     @job_id.setter
     def job_id(self, job_id):
-        """Sets the job_id of this SchedulerJob.
+        """Sets the job_id of this SchedulerJobResponse.
 
 
-        :param job_id: The job_id of this SchedulerJob.  # noqa: E501
+        :param job_id: The job_id of this SchedulerJobResponse.  # noqa: E501
         :type job_id: lusid_workflow.ResourceId
         """
-        if self.local_vars_configuration.client_side_validation and job_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `job_id`, must not be `None`")  # noqa: E501
 
         self._job_id = job_id
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -165,18 +162,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SchedulerJob):
+        if not isinstance(other, SchedulerJobResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SchedulerJob):
+        if not isinstance(other, SchedulerJobResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/scheduler_job_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class SchedulerJobResponse(object):
+class TriggerParentTaskActionResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -36,97 +36,98 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'type': 'str',
-        'job_id': 'ResourceId'
+        'trigger': 'str'
     }
 
     attribute_map = {
         'type': 'type',
-        'job_id': 'jobId'
+        'trigger': 'trigger'
     }
 
     required_map = {
         'type': 'optional',
-        'job_id': 'optional'
+        'trigger': 'optional'
     }
 
-    def __init__(self, type=None, job_id=None, local_vars_configuration=None):  # noqa: E501
-        """SchedulerJobResponse - a model defined in OpenAPI"
+    def __init__(self, type=None, trigger=None, local_vars_configuration=None):  # noqa: E501
+        """TriggerParentTaskActionResponse - a model defined in OpenAPI"
         
-        :param type:  The type of worker
+        :param type:  Type name for this Action
         :type type: str
-        :param job_id: 
-        :type job_id: lusid_workflow.ResourceId
+        :param trigger:  Trigger on parent task to be invoked
+        :type trigger: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
-        self._job_id = None
+        self._trigger = None
         self.discriminator = None
 
         self.type = type
-        if job_id is not None:
-            self.job_id = job_id
+        self.trigger = trigger
 
     @property
     def type(self):
-        """Gets the type of this SchedulerJobResponse.  # noqa: E501
+        """Gets the type of this TriggerParentTaskActionResponse.  # noqa: E501
 
-        The type of worker  # noqa: E501
+        Type name for this Action  # noqa: E501
 
-        :return: The type of this SchedulerJobResponse.  # noqa: E501
+        :return: The type of this TriggerParentTaskActionResponse.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this SchedulerJobResponse.
+        """Sets the type of this TriggerParentTaskActionResponse.
 
-        The type of worker  # noqa: E501
+        Type name for this Action  # noqa: E501
 
-        :param type: The type of this SchedulerJobResponse.  # noqa: E501
+        :param type: The type of this TriggerParentTaskActionResponse.  # noqa: E501
         :type type: str
         """
-        allowed_values = [None,"SchedulerJob"]  # noqa: E501
+        allowed_values = [None,"TriggerParentTask"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
 
     @property
-    def job_id(self):
-        """Gets the job_id of this SchedulerJobResponse.  # noqa: E501
+    def trigger(self):
+        """Gets the trigger of this TriggerParentTaskActionResponse.  # noqa: E501
 
+        Trigger on parent task to be invoked  # noqa: E501
 
-        :return: The job_id of this SchedulerJobResponse.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
+        :return: The trigger of this TriggerParentTaskActionResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._job_id
+        return self._trigger
 
-    @job_id.setter
-    def job_id(self, job_id):
-        """Sets the job_id of this SchedulerJobResponse.
+    @trigger.setter
+    def trigger(self, trigger):
+        """Sets the trigger of this TriggerParentTaskActionResponse.
 
+        Trigger on parent task to be invoked  # noqa: E501
 
-        :param job_id: The job_id of this SchedulerJobResponse.  # noqa: E501
-        :type job_id: lusid_workflow.ResourceId
+        :param trigger: The trigger of this TriggerParentTaskActionResponse.  # noqa: E501
+        :type trigger: str
         """
 
-        self._job_id = job_id
+        self._trigger = trigger
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -162,18 +163,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SchedulerJobResponse):
+        if not isinstance(other, TriggerParentTaskActionResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SchedulerJobResponse):
+        if not isinstance(other, TriggerParentTaskActionResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/sleep.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/sleep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/sleep_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/sleep_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/stack.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/update_task_definition_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TaskDefinition(object):
+class UpdateTaskDefinitionRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,342 +35,283 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'ResourceId',
-        'version': 'VersionInfo',
         'display_name': 'str',
         'description': 'str',
         'states': 'list[TaskStateDefinition]',
         'field_schema': 'list[TaskFieldDefinition]',
         'initial_state': 'InitialState',
         'triggers': 'list[TransitionTriggerDefinition]',
-        'actions': 'list[ActionDefinitionResponse]',
-        'transitions': 'list[TaskTransitionDefinition]'
+        'transitions': 'list[TaskTransitionDefinition]',
+        'actions': 'list[ActionDefinition]'
     }
 
     attribute_map = {
-        'id': 'id',
-        'version': 'version',
         'display_name': 'displayName',
         'description': 'description',
         'states': 'states',
         'field_schema': 'fieldSchema',
         'initial_state': 'initialState',
         'triggers': 'triggers',
-        'actions': 'actions',
-        'transitions': 'transitions'
+        'transitions': 'transitions',
+        'actions': 'actions'
     }
 
     required_map = {
-        'id': 'required',
-        'version': 'optional',
         'display_name': 'required',
         'description': 'optional',
         'states': 'required',
         'field_schema': 'optional',
         'initial_state': 'required',
         'triggers': 'optional',
-        'actions': 'optional',
-        'transitions': 'optional'
+        'transitions': 'optional',
+        'actions': 'optional'
     }
 
-    def __init__(self, id=None, version=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, actions=None, transitions=None, local_vars_configuration=None):  # noqa: E501
-        """TaskDefinition - a model defined in OpenAPI"
+    def __init__(self, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, actions=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateTaskDefinitionRequest - a model defined in OpenAPI"
         
-        :param id:  (required)
-        :type id: lusid_workflow.ResourceId
-        :param version: 
-        :type version: lusid_workflow.VersionInfo
         :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
         :param states:  The states this Task Definition operates over (required)
         :type states: list[lusid_workflow.TaskStateDefinition]
-        :param field_schema:  The Fields that this Task Definition operates on
+        :param field_schema:  Defines the fields associated with this Task
         :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         :param initial_state:  (required)
         :type initial_state: lusid_workflow.InitialState
-        :param triggers:  The Triggers for State transition
+        :param triggers:  Triggers
         :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
-        :param actions:  The Actions of this Task - executed after a Transition completion
-        :type actions: list[lusid_workflow.ActionDefinitionResponse]
-        :param transitions:  The Transitions between States
+        :param transitions:  Transitions
         :type transitions: list[lusid_workflow.TaskTransitionDefinition]
+        :param actions:  Actions
+        :type actions: list[lusid_workflow.ActionDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._version = None
         self._display_name = None
         self._description = None
         self._states = None
         self._field_schema = None
         self._initial_state = None
         self._triggers = None
-        self._actions = None
         self._transitions = None
+        self._actions = None
         self.discriminator = None
 
-        self.id = id
-        if version is not None:
-            self.version = version
         self.display_name = display_name
         self.description = description
         self.states = states
         self.field_schema = field_schema
         self.initial_state = initial_state
         self.triggers = triggers
-        self.actions = actions
         self.transitions = transitions
-
-    @property
-    def id(self):
-        """Gets the id of this TaskDefinition.  # noqa: E501
-
-
-        :return: The id of this TaskDefinition.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this TaskDefinition.
-
-
-        :param id: The id of this TaskDefinition.  # noqa: E501
-        :type id: lusid_workflow.ResourceId
-        """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-
-        self._id = id
-
-    @property
-    def version(self):
-        """Gets the version of this TaskDefinition.  # noqa: E501
-
-
-        :return: The version of this TaskDefinition.  # noqa: E501
-        :rtype: lusid_workflow.VersionInfo
-        """
-        return self._version
-
-    @version.setter
-    def version(self, version):
-        """Sets the version of this TaskDefinition.
-
-
-        :param version: The version of this TaskDefinition.  # noqa: E501
-        :type version: lusid_workflow.VersionInfo
-        """
-
-        self._version = version
+        self.actions = actions
 
     @property
     def display_name(self):
-        """Gets the display_name of this TaskDefinition.  # noqa: E501
+        """Gets the display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
 
         Human readable name  # noqa: E501
 
-        :return: The display_name of this TaskDefinition.  # noqa: E501
+        :return: The display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this TaskDefinition.
+        """Sets the display_name of this UpdateTaskDefinitionRequest.
 
         Human readable name  # noqa: E501
 
-        :param display_name: The display_name of this TaskDefinition.  # noqa: E501
+        :param display_name: The display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type display_name: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) < 1):
             raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this TaskDefinition.  # noqa: E501
+        """Gets the description of this UpdateTaskDefinitionRequest.  # noqa: E501
 
         Human readable description  # noqa: E501
 
-        :return: The description of this TaskDefinition.  # noqa: E501
+        :return: The description of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this TaskDefinition.
+        """Sets the description of this UpdateTaskDefinitionRequest.
 
         Human readable description  # noqa: E501
 
-        :param description: The description of this TaskDefinition.  # noqa: E501
+        :param description: The description of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
     def states(self):
-        """Gets the states of this TaskDefinition.  # noqa: E501
+        """Gets the states of this UpdateTaskDefinitionRequest.  # noqa: E501
 
         The states this Task Definition operates over  # noqa: E501
 
-        :return: The states of this TaskDefinition.  # noqa: E501
+        :return: The states of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TaskStateDefinition]
         """
         return self._states
 
     @states.setter
     def states(self, states):
-        """Sets the states of this TaskDefinition.
+        """Sets the states of this UpdateTaskDefinitionRequest.
 
         The states this Task Definition operates over  # noqa: E501
 
-        :param states: The states of this TaskDefinition.  # noqa: E501
+        :param states: The states of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type states: list[lusid_workflow.TaskStateDefinition]
         """
         if self.local_vars_configuration.client_side_validation and states is None:  # noqa: E501
             raise ValueError("Invalid value for `states`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 states is not None and len(states) < 1):
             raise ValueError("Invalid value for `states`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._states = states
 
     @property
     def field_schema(self):
-        """Gets the field_schema of this TaskDefinition.  # noqa: E501
+        """Gets the field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Fields that this Task Definition operates on  # noqa: E501
+        Defines the fields associated with this Task  # noqa: E501
 
-        :return: The field_schema of this TaskDefinition.  # noqa: E501
+        :return: The field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TaskFieldDefinition]
         """
         return self._field_schema
 
     @field_schema.setter
     def field_schema(self, field_schema):
-        """Sets the field_schema of this TaskDefinition.
+        """Sets the field_schema of this UpdateTaskDefinitionRequest.
 
-        The Fields that this Task Definition operates on  # noqa: E501
+        Defines the fields associated with this Task  # noqa: E501
 
-        :param field_schema: The field_schema of this TaskDefinition.  # noqa: E501
+        :param field_schema: The field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         """
 
         self._field_schema = field_schema
 
     @property
     def initial_state(self):
-        """Gets the initial_state of this TaskDefinition.  # noqa: E501
+        """Gets the initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
 
 
-        :return: The initial_state of this TaskDefinition.  # noqa: E501
+        :return: The initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: lusid_workflow.InitialState
         """
         return self._initial_state
 
     @initial_state.setter
     def initial_state(self, initial_state):
-        """Sets the initial_state of this TaskDefinition.
+        """Sets the initial_state of this UpdateTaskDefinitionRequest.
 
 
-        :param initial_state: The initial_state of this TaskDefinition.  # noqa: E501
+        :param initial_state: The initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type initial_state: lusid_workflow.InitialState
         """
         if self.local_vars_configuration.client_side_validation and initial_state is None:  # noqa: E501
             raise ValueError("Invalid value for `initial_state`, must not be `None`")  # noqa: E501
 
         self._initial_state = initial_state
 
     @property
     def triggers(self):
-        """Gets the triggers of this TaskDefinition.  # noqa: E501
+        """Gets the triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Triggers for State transition  # noqa: E501
+        Triggers  # noqa: E501
 
-        :return: The triggers of this TaskDefinition.  # noqa: E501
+        :return: The triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TransitionTriggerDefinition]
         """
         return self._triggers
 
     @triggers.setter
     def triggers(self, triggers):
-        """Sets the triggers of this TaskDefinition.
+        """Sets the triggers of this UpdateTaskDefinitionRequest.
 
-        The Triggers for State transition  # noqa: E501
+        Triggers  # noqa: E501
 
-        :param triggers: The triggers of this TaskDefinition.  # noqa: E501
+        :param triggers: The triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         """
 
         self._triggers = triggers
 
     @property
-    def actions(self):
-        """Gets the actions of this TaskDefinition.  # noqa: E501
+    def transitions(self):
+        """Gets the transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Actions of this Task - executed after a Transition completion  # noqa: E501
+        Transitions  # noqa: E501
 
-        :return: The actions of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.ActionDefinitionResponse]
+        :return: The transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.TaskTransitionDefinition]
         """
-        return self._actions
+        return self._transitions
 
-    @actions.setter
-    def actions(self, actions):
-        """Sets the actions of this TaskDefinition.
+    @transitions.setter
+    def transitions(self, transitions):
+        """Sets the transitions of this UpdateTaskDefinitionRequest.
 
-        The Actions of this Task - executed after a Transition completion  # noqa: E501
+        Transitions  # noqa: E501
 
-        :param actions: The actions of this TaskDefinition.  # noqa: E501
-        :type actions: list[lusid_workflow.ActionDefinitionResponse]
+        :param transitions: The transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
         """
 
-        self._actions = actions
+        self._transitions = transitions
 
     @property
-    def transitions(self):
-        """Gets the transitions of this TaskDefinition.  # noqa: E501
+    def actions(self):
+        """Gets the actions of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Transitions between States  # noqa: E501
+        Actions  # noqa: E501
 
-        :return: The transitions of this TaskDefinition.  # noqa: E501
-        :rtype: list[lusid_workflow.TaskTransitionDefinition]
+        :return: The actions of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.ActionDefinition]
         """
-        return self._transitions
+        return self._actions
 
-    @transitions.setter
-    def transitions(self, transitions):
-        """Sets the transitions of this TaskDefinition.
+    @actions.setter
+    def actions(self, actions):
+        """Sets the actions of this UpdateTaskDefinitionRequest.
 
-        The Transitions between States  # noqa: E501
+        Actions  # noqa: E501
 
-        :param transitions: The transitions of this TaskDefinition.  # noqa: E501
-        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
+        :param actions: The actions of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :type actions: list[lusid_workflow.ActionDefinition]
         """
 
-        self._transitions = transitions
+        self._actions = actions
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -406,18 +347,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TaskDefinition):
+        if not isinstance(other, UpdateTaskDefinitionRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TaskDefinition):
+        if not isinstance(other, UpdateTaskDefinitionRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_definition_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_instance_field.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_state_definition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TaskInstanceField(object):
+class TaskStateDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,99 +35,75 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'name': 'str',
-        'value': 'object'
+        'name': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'value': 'value'
+        'name': 'name'
     }
 
     required_map = {
-        'name': 'required',
-        'value': 'optional'
+        'name': 'required'
     }
 
-    def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
-        """TaskInstanceField - a model defined in OpenAPI"
+    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
+        """TaskStateDefinition - a model defined in OpenAPI"
         
-        :param name:  The name of this Field (required)
+        :param name:  The Name of this State (required)
         :type name: str
-        :param value:  The value of this Field
-        :type value: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
-        self._value = None
         self.discriminator = None
 
         self.name = name
-        self.value = value
 
     @property
     def name(self):
-        """Gets the name of this TaskInstanceField.  # noqa: E501
+        """Gets the name of this TaskStateDefinition.  # noqa: E501
 
-        The name of this Field  # noqa: E501
+        The Name of this State  # noqa: E501
 
-        :return: The name of this TaskInstanceField.  # noqa: E501
+        :return: The name of this TaskStateDefinition.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this TaskInstanceField.
+        """Sets the name of this TaskStateDefinition.
 
-        The name of this Field  # noqa: E501
+        The Name of this State  # noqa: E501
 
-        :param name: The name of this TaskInstanceField.  # noqa: E501
+        :param name: The name of this TaskStateDefinition.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) > 1024):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
                 name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
             raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
         self._name = name
 
-    @property
-    def value(self):
-        """Gets the value of this TaskInstanceField.  # noqa: E501
-
-        The value of this Field  # noqa: E501
-
-        :return: The value of this TaskInstanceField.  # noqa: E501
-        :rtype: object
-        """
-        return self._value
-
-    @value.setter
-    def value(self, value):
-        """Sets the value of this TaskInstanceField.
-
-        The value of this Field  # noqa: E501
-
-        :param value: The value of this TaskInstanceField.  # noqa: E501
-        :type value: object
-        """
-
-        self._value = value
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -162,18 +138,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TaskInstanceField):
+        if not isinstance(other, TaskStateDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TaskInstanceField):
+        if not isinstance(other, TaskStateDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/task_summary.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/task_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/trigger_parent_task_action.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker_configuration_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TriggerParentTaskActionResponse(object):
+class WorkerConfigurationResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -36,98 +36,159 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'type': 'str',
-        'trigger': 'str'
+        'url': 'str',
+        'name': 'str',
+        'job_id': 'ResourceId'
     }
 
     attribute_map = {
         'type': 'type',
-        'trigger': 'trigger'
+        'url': 'url',
+        'name': 'name',
+        'job_id': 'jobId'
     }
 
     required_map = {
-        'type': 'optional',
-        'trigger': 'optional'
+        'type': 'required',
+        'url': 'optional',
+        'name': 'optional',
+        'job_id': 'optional'
     }
 
-    def __init__(self, type=None, trigger=None, local_vars_configuration=None):  # noqa: E501
-        """TriggerParentTaskActionResponse - a model defined in OpenAPI"
+    def __init__(self, type=None, url=None, name=None, job_id=None, local_vars_configuration=None):  # noqa: E501
+        """WorkerConfigurationResponse - a model defined in OpenAPI"
         
-        :param type:  Type name for this Action
+        :param type:  The type of worker (required)
         :type type: str
-        :param trigger:  Trigger on parent task to be invoked
-        :type trigger: str
+        :param url:  The URL to check, eg: https://www.google.com/
+        :type url: str
+        :param name:  Name of the view in Luminesce
+        :type name: str
+        :param job_id: 
+        :type job_id: lusid_workflow.ResourceId
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
-        self._trigger = None
+        self._url = None
+        self._name = None
+        self._job_id = None
         self.discriminator = None
 
         self.type = type
-        self.trigger = trigger
+        self.url = url
+        self.name = name
+        if job_id is not None:
+            self.job_id = job_id
 
     @property
     def type(self):
-        """Gets the type of this TriggerParentTaskActionResponse.  # noqa: E501
+        """Gets the type of this WorkerConfigurationResponse.  # noqa: E501
 
-        Type name for this Action  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :return: The type of this TriggerParentTaskActionResponse.  # noqa: E501
+        :return: The type of this WorkerConfigurationResponse.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this TriggerParentTaskActionResponse.
+        """Sets the type of this WorkerConfigurationResponse.
 
-        Type name for this Action  # noqa: E501
+        The type of worker  # noqa: E501
 
-        :param type: The type of this TriggerParentTaskActionResponse.  # noqa: E501
+        :param type: The type of this WorkerConfigurationResponse.  # noqa: E501
         :type type: str
         """
-        allowed_values = [None,"TriggerParentTask"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["Sleep"]  # noqa: E501
         if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
             raise ValueError(
                 "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
                 .format(type, allowed_values)
             )
 
         self._type = type
 
     @property
-    def trigger(self):
-        """Gets the trigger of this TriggerParentTaskActionResponse.  # noqa: E501
+    def url(self):
+        """Gets the url of this WorkerConfigurationResponse.  # noqa: E501
 
-        Trigger on parent task to be invoked  # noqa: E501
+        The URL to check, eg: https://www.google.com/  # noqa: E501
 
-        :return: The trigger of this TriggerParentTaskActionResponse.  # noqa: E501
+        :return: The url of this WorkerConfigurationResponse.  # noqa: E501
         :rtype: str
         """
-        return self._trigger
+        return self._url
 
-    @trigger.setter
-    def trigger(self, trigger):
-        """Sets the trigger of this TriggerParentTaskActionResponse.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this WorkerConfigurationResponse.
 
-        Trigger on parent task to be invoked  # noqa: E501
+        The URL to check, eg: https://www.google.com/  # noqa: E501
 
-        :param trigger: The trigger of this TriggerParentTaskActionResponse.  # noqa: E501
-        :type trigger: str
+        :param url: The url of this WorkerConfigurationResponse.  # noqa: E501
+        :type url: str
         """
 
-        self._trigger = trigger
+        self._url = url
+
+    @property
+    def name(self):
+        """Gets the name of this WorkerConfigurationResponse.  # noqa: E501
+
+        Name of the view in Luminesce  # noqa: E501
+
+        :return: The name of this WorkerConfigurationResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this WorkerConfigurationResponse.
+
+        Name of the view in Luminesce  # noqa: E501
+
+        :param name: The name of this WorkerConfigurationResponse.  # noqa: E501
+        :type name: str
+        """
+
+        self._name = name
+
+    @property
+    def job_id(self):
+        """Gets the job_id of this WorkerConfigurationResponse.  # noqa: E501
+
+
+        :return: The job_id of this WorkerConfigurationResponse.  # noqa: E501
+        :rtype: lusid_workflow.ResourceId
+        """
+        return self._job_id
+
+    @job_id.setter
+    def job_id(self, job_id):
+        """Sets the job_id of this WorkerConfigurationResponse.
+
+
+        :param job_id: The job_id of this WorkerConfigurationResponse.  # noqa: E501
+        :type job_id: lusid_workflow.ResourceId
+        """
+
+        self._job_id = job_id
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -163,18 +224,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TriggerParentTaskActionResponse):
+        if not isinstance(other, WorkerConfigurationResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TriggerParentTaskActionResponse):
+        if not isinstance(other, WorkerConfigurationResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/trigger_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/update_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class UpdateTaskDefinitionRequest(object):
+class Worker(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,283 +35,275 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
-        'states': 'list[TaskStateDefinition]',
-        'field_schema': 'list[TaskFieldDefinition]',
-        'initial_state': 'InitialState',
-        'triggers': 'list[TransitionTriggerDefinition]',
-        'transitions': 'list[TaskTransitionDefinition]',
-        'actions': 'list[ActionDefinition]'
+        'worker_configuration': 'WorkerConfigurationResponse',
+        'version': 'VersionInfo',
+        'parameters': 'list[Parameter]',
+        'result_fields': 'list[ResultField]',
+        'links': 'list[Link]'
     }
 
     attribute_map = {
+        'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
-        'states': 'states',
-        'field_schema': 'fieldSchema',
-        'initial_state': 'initialState',
-        'triggers': 'triggers',
-        'transitions': 'transitions',
-        'actions': 'actions'
+        'worker_configuration': 'workerConfiguration',
+        'version': 'version',
+        'parameters': 'parameters',
+        'result_fields': 'resultFields',
+        'links': 'links'
     }
 
     required_map = {
+        'id': 'required',
         'display_name': 'required',
         'description': 'optional',
-        'states': 'required',
-        'field_schema': 'optional',
-        'initial_state': 'required',
-        'triggers': 'optional',
-        'transitions': 'optional',
-        'actions': 'optional'
+        'worker_configuration': 'required',
+        'version': 'optional',
+        'parameters': 'optional',
+        'result_fields': 'optional',
+        'links': 'optional'
     }
 
-    def __init__(self, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, actions=None, local_vars_configuration=None):  # noqa: E501
-        """UpdateTaskDefinitionRequest - a model defined in OpenAPI"
+    def __init__(self, id=None, display_name=None, description=None, worker_configuration=None, version=None, parameters=None, result_fields=None, links=None, local_vars_configuration=None):  # noqa: E501
+        """Worker - a model defined in OpenAPI"
         
+        :param id:  (required)
+        :type id: lusid_workflow.ResourceId
         :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
-        :param states:  The states this Task Definition operates over (required)
-        :type states: list[lusid_workflow.TaskStateDefinition]
-        :param field_schema:  Defines the fields associated with this Task
-        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
-        :param initial_state:  (required)
-        :type initial_state: lusid_workflow.InitialState
-        :param triggers:  Triggers
-        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
-        :param transitions:  Transitions
-        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
-        :param actions:  Actions
-        :type actions: list[lusid_workflow.ActionDefinition]
+        :param worker_configuration:  (required)
+        :type worker_configuration: lusid_workflow.WorkerConfigurationResponse
+        :param version: 
+        :type version: lusid_workflow.VersionInfo
+        :param parameters:  The Parameters this Worker accepts or requires.
+        :type parameters: list[lusid_workflow.Parameter]
+        :param result_fields:  The Fields that the Worker results will come back with.
+        :type result_fields: list[lusid_workflow.ResultField]
+        :param links: 
+        :type links: list[lusid_workflow.Link]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
         self._display_name = None
         self._description = None
-        self._states = None
-        self._field_schema = None
-        self._initial_state = None
-        self._triggers = None
-        self._transitions = None
-        self._actions = None
+        self._worker_configuration = None
+        self._version = None
+        self._parameters = None
+        self._result_fields = None
+        self._links = None
         self.discriminator = None
 
+        self.id = id
         self.display_name = display_name
         self.description = description
-        self.states = states
-        self.field_schema = field_schema
-        self.initial_state = initial_state
-        self.triggers = triggers
-        self.transitions = transitions
-        self.actions = actions
+        self.worker_configuration = worker_configuration
+        if version is not None:
+            self.version = version
+        self.parameters = parameters
+        self.result_fields = result_fields
+        self.links = links
+
+    @property
+    def id(self):
+        """Gets the id of this Worker.  # noqa: E501
+
+
+        :return: The id of this Worker.  # noqa: E501
+        :rtype: lusid_workflow.ResourceId
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Worker.
+
+
+        :param id: The id of this Worker.  # noqa: E501
+        :type id: lusid_workflow.ResourceId
+        """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+
+        self._id = id
 
     @property
     def display_name(self):
-        """Gets the display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
+        """Gets the display_name of this Worker.  # noqa: E501
 
         Human readable name  # noqa: E501
 
-        :return: The display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :return: The display_name of this Worker.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this UpdateTaskDefinitionRequest.
+        """Sets the display_name of this Worker.
 
         Human readable name  # noqa: E501
 
-        :param display_name: The display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :param display_name: The display_name of this Worker.  # noqa: E501
         :type display_name: str
         """
         if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 display_name is not None and len(display_name) < 1):
             raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this UpdateTaskDefinitionRequest.  # noqa: E501
+        """Gets the description of this Worker.  # noqa: E501
 
         Human readable description  # noqa: E501
 
-        :return: The description of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :return: The description of this Worker.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this UpdateTaskDefinitionRequest.
+        """Sets the description of this Worker.
 
         Human readable description  # noqa: E501
 
-        :param description: The description of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :param description: The description of this Worker.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
-    def states(self):
-        """Gets the states of this UpdateTaskDefinitionRequest.  # noqa: E501
-
-        The states this Task Definition operates over  # noqa: E501
-
-        :return: The states of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.TaskStateDefinition]
-        """
-        return self._states
-
-    @states.setter
-    def states(self, states):
-        """Sets the states of this UpdateTaskDefinitionRequest.
-
-        The states this Task Definition operates over  # noqa: E501
-
-        :param states: The states of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :type states: list[lusid_workflow.TaskStateDefinition]
-        """
-        if self.local_vars_configuration.client_side_validation and states is None:  # noqa: E501
-            raise ValueError("Invalid value for `states`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                states is not None and len(states) < 1):
-            raise ValueError("Invalid value for `states`, number of items must be greater than or equal to `1`")  # noqa: E501
-
-        self._states = states
-
-    @property
-    def field_schema(self):
-        """Gets the field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
+    def worker_configuration(self):
+        """Gets the worker_configuration of this Worker.  # noqa: E501
 
-        Defines the fields associated with this Task  # noqa: E501
 
-        :return: The field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.TaskFieldDefinition]
+        :return: The worker_configuration of this Worker.  # noqa: E501
+        :rtype: lusid_workflow.WorkerConfigurationResponse
         """
-        return self._field_schema
+        return self._worker_configuration
 
-    @field_schema.setter
-    def field_schema(self, field_schema):
-        """Sets the field_schema of this UpdateTaskDefinitionRequest.
+    @worker_configuration.setter
+    def worker_configuration(self, worker_configuration):
+        """Sets the worker_configuration of this Worker.
 
-        Defines the fields associated with this Task  # noqa: E501
 
-        :param field_schema: The field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :type field_schema: list[lusid_workflow.TaskFieldDefinition]
+        :param worker_configuration: The worker_configuration of this Worker.  # noqa: E501
+        :type worker_configuration: lusid_workflow.WorkerConfigurationResponse
         """
+        if self.local_vars_configuration.client_side_validation and worker_configuration is None:  # noqa: E501
+            raise ValueError("Invalid value for `worker_configuration`, must not be `None`")  # noqa: E501
 
-        self._field_schema = field_schema
+        self._worker_configuration = worker_configuration
 
     @property
-    def initial_state(self):
-        """Gets the initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
+    def version(self):
+        """Gets the version of this Worker.  # noqa: E501
 
 
-        :return: The initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :rtype: lusid_workflow.InitialState
+        :return: The version of this Worker.  # noqa: E501
+        :rtype: lusid_workflow.VersionInfo
         """
-        return self._initial_state
+        return self._version
 
-    @initial_state.setter
-    def initial_state(self, initial_state):
-        """Sets the initial_state of this UpdateTaskDefinitionRequest.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this Worker.
 
 
-        :param initial_state: The initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :type initial_state: lusid_workflow.InitialState
+        :param version: The version of this Worker.  # noqa: E501
+        :type version: lusid_workflow.VersionInfo
         """
-        if self.local_vars_configuration.client_side_validation and initial_state is None:  # noqa: E501
-            raise ValueError("Invalid value for `initial_state`, must not be `None`")  # noqa: E501
 
-        self._initial_state = initial_state
+        self._version = version
 
     @property
-    def triggers(self):
-        """Gets the triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
+    def parameters(self):
+        """Gets the parameters of this Worker.  # noqa: E501
 
-        Triggers  # noqa: E501
+        The Parameters this Worker accepts or requires.  # noqa: E501
 
-        :return: The triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.TransitionTriggerDefinition]
+        :return: The parameters of this Worker.  # noqa: E501
+        :rtype: list[lusid_workflow.Parameter]
         """
-        return self._triggers
+        return self._parameters
 
-    @triggers.setter
-    def triggers(self, triggers):
-        """Sets the triggers of this UpdateTaskDefinitionRequest.
+    @parameters.setter
+    def parameters(self, parameters):
+        """Sets the parameters of this Worker.
 
-        Triggers  # noqa: E501
+        The Parameters this Worker accepts or requires.  # noqa: E501
 
-        :param triggers: The triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
+        :param parameters: The parameters of this Worker.  # noqa: E501
+        :type parameters: list[lusid_workflow.Parameter]
         """
 
-        self._triggers = triggers
+        self._parameters = parameters
 
     @property
-    def transitions(self):
-        """Gets the transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
+    def result_fields(self):
+        """Gets the result_fields of this Worker.  # noqa: E501
 
-        Transitions  # noqa: E501
+        The Fields that the Worker results will come back with.  # noqa: E501
 
-        :return: The transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.TaskTransitionDefinition]
+        :return: The result_fields of this Worker.  # noqa: E501
+        :rtype: list[lusid_workflow.ResultField]
         """
-        return self._transitions
+        return self._result_fields
 
-    @transitions.setter
-    def transitions(self, transitions):
-        """Sets the transitions of this UpdateTaskDefinitionRequest.
+    @result_fields.setter
+    def result_fields(self, result_fields):
+        """Sets the result_fields of this Worker.
 
-        Transitions  # noqa: E501
+        The Fields that the Worker results will come back with.  # noqa: E501
 
-        :param transitions: The transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :type transitions: list[lusid_workflow.TaskTransitionDefinition]
+        :param result_fields: The result_fields of this Worker.  # noqa: E501
+        :type result_fields: list[lusid_workflow.ResultField]
         """
 
-        self._transitions = transitions
+        self._result_fields = result_fields
 
     @property
-    def actions(self):
-        """Gets the actions of this UpdateTaskDefinitionRequest.  # noqa: E501
+    def links(self):
+        """Gets the links of this Worker.  # noqa: E501
 
-        Actions  # noqa: E501
 
-        :return: The actions of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :rtype: list[lusid_workflow.ActionDefinition]
+        :return: The links of this Worker.  # noqa: E501
+        :rtype: list[lusid_workflow.Link]
         """
-        return self._actions
+        return self._links
 
-    @actions.setter
-    def actions(self, actions):
-        """Sets the actions of this UpdateTaskDefinitionRequest.
+    @links.setter
+    def links(self, links):
+        """Sets the links of this Worker.
 
-        Actions  # noqa: E501
 
-        :param actions: The actions of this UpdateTaskDefinitionRequest.  # noqa: E501
-        :type actions: list[lusid_workflow.ActionDefinition]
+        :param links: The links of this Worker.  # noqa: E501
+        :type links: list[lusid_workflow.Link]
         """
 
-        self._actions = actions
+        self._links = links
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -347,18 +339,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateTaskDefinitionRequest):
+        if not isinstance(other, Worker):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UpdateTaskDefinitionRequest):
+        if not isinstance(other, Worker):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/update_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/update_worker_request.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/update_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/version_info.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/version_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/models/worker_status_triggers.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/models/worker_status_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.878
+    The version of the OpenAPI document: 0.1.879
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow/utilities/config_keys.json` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-workflow-sdk-preview-0.1.878/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.879/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,29 @@
 lusid_workflow/__init__.py
 lusid_workflow/__version__.py
 lusid_workflow/api_client.py
 lusid_workflow/configuration.py
 lusid_workflow/exceptions.py
 lusid_workflow/rest.py
 lusid_workflow/api/__init__.py
-lusid_workflow/api/event_handlers_api.py
 lusid_workflow/api/task_definitions_api.py
 lusid_workflow/api/tasks_api.py
 lusid_workflow/api/workers_api.py
 lusid_workflow/models/__init__.py
 lusid_workflow/models/action_definition.py
 lusid_workflow/models/action_definition_response.py
 lusid_workflow/models/action_details.py
 lusid_workflow/models/action_details_response.py
 lusid_workflow/models/create_child_task_configuration.py
 lusid_workflow/models/create_child_tasks_action.py
 lusid_workflow/models/create_child_tasks_action_response.py
-lusid_workflow/models/create_event_handler_request.py
 lusid_workflow/models/create_task_definition_request.py
 lusid_workflow/models/create_task_request.py
 lusid_workflow/models/create_worker_request.py
 lusid_workflow/models/deleted_entity_response.py
-lusid_workflow/models/event_handler.py
-lusid_workflow/models/event_handler_mapping.py
-lusid_workflow/models/event_matching_pattern.py
 lusid_workflow/models/fail.py
 lusid_workflow/models/fail_response.py
 lusid_workflow/models/field_mapping.py
 lusid_workflow/models/get_worker_result_response.py
 lusid_workflow/models/health_check.py
 lusid_workflow/models/health_check_response.py
 lusid_workflow/models/initial_state.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.878/setup.py` & `lusid-workflow-sdk-preview-0.1.879/setup.py`

 * *Files identical despite different names*

