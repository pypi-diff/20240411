# Comparing `tmp/lusid_workflow_sdk-2.1.1.tar.gz` & `tmp/lusid_workflow_sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_workflow_sdk-2.1.1.tar", max compression
+gzip compressed data, was "lusid_workflow_sdk-2.1.2.tar", max compression
```

## Comparing `lusid_workflow_sdk-2.1.1.tar` & `lusid_workflow_sdk-2.1.2.tar`

### file list

```diff
@@ -1,93 +1,88 @@
--rw-r--r--   0        0        0    13185 2024-04-10 10:42:19.477844 lusid_workflow_sdk-2.1.1/README.md
--rw-r--r--   0        0        0     8289 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/__init__.py
--rw-r--r--   0        0        0      388 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/__init__.py
--rw-r--r--   0        0        0     8588 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/event_handlers_api.py
--rw-r--r--   0        0        0    57597 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0        0        0    44655 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/tasks_api.py
--rw-r--r--   0        0        0    61860 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/api/workers_api.py
--rw-r--r--   0        0        0    30785 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/api_client.py
--rw-r--r--   0        0        0      852 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/api_response.py
--rw-r--r--   0        0        0    14451 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/configuration.py
--rw-r--r--   0        0        0     5339 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/exceptions.py
--rw-r--r--   0        0        0      587 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/__init__.py
--rw-r--r--   0        0        0    30652 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client.py
--rw-r--r--   0        0        0     9862 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8097 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_configuration.py
--rw-r--r--   0        0        0     6796 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12707 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/rest.py
--rw-r--r--   0        0        0    11573 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3886 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     6872 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/__init__.py
--rw-r--r--   0        0        0     3649 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition.py
--rw-r--r--   0        0        0     3233 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0        0        0     6172 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details.py
--rw-r--r--   0        0        0     6643 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details_response.py
--rw-r--r--   0        0        0     5406 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0        0        0     3165 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0        0        0     3766 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0        0        0     5424 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_event_handler_request.py
--rw-r--r--   0        0        0     7468 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0        0        0     4145 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_request.py
--rw-r--r--   0        0        0     3972 2024-04-10 10:42:19.469844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0        0        0     3459 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0        0        0     5704 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_handler.py
--rw-r--r--   0        0        0     2554 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_handler_mapping.py
--rw-r--r--   0        0        0     2951 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_matching_pattern.py
--rw-r--r--   0        0        0     2193 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail.py
--rw-r--r--   0        0        0     2505 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail_response.py
--rw-r--r--   0        0        0     2878 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/field_mapping.py
--rw-r--r--   0        0        0     2607 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0        0        0     2341 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check.py
--rw-r--r--   0        0        0     2814 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check_response.py
--rw-r--r--   0        0        0     2723 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/initial_state.py
--rw-r--r--   0        0        0     2262 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/link.py
--rw-r--r--   0        0        0     2607 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0        0        0     2811 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0        0        0     3857 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4693 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4053 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0        0        0     4174 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0        0        0     4077 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0        0        0     3317 2024-04-10 10:42:19.470844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter.py
--rw-r--r--   0        0        0     2583 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter_value.py
--rw-r--r--   0        0        0     1869 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_id.py
--rw-r--r--   0        0        0     4013 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0        0        0     2793 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_field.py
--rw-r--r--   0        0        0     2293 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0        0        0     5713 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0        0        0     5913 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0        0        0     6227 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0        0        0     2428 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0        0        0     2360 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0        0        0     2541 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job.py
--rw-r--r--   0        0        0     2864 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job_response.py
--rw-r--r--   0        0        0     2116 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep.py
--rw-r--r--   0        0        0     2172 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep_response.py
--rw-r--r--   0        0        0     4397 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/stack.py
--rw-r--r--   0        0        0     8353 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task.py
--rw-r--r--   0        0        0     7864 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition.py
--rw-r--r--   0        0        0     2090 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0        0        0     2483 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0        0        0     2546 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0        0        0     2279 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0        0        0     3415 2024-04-10 10:42:19.471844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_summary.py
--rw-r--r--   0        0        0     4806 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0        0        0     2728 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0        0        0     2716 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0        0        0     2910 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0        0        0     1951 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0        0        0     7130 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0        0        0     3588 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_request.py
--rw-r--r--   0        0        0     3579 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_worker_request.py
--rw-r--r--   0        0        0     5124 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/version_info.py
--rw-r--r--   0        0        0     6137 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker.py
--rw-r--r--   0        0        0     7051 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0        0        0     7753 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0        0        0     4204 2024-04-10 10:42:19.472844 lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0        0        0        0 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/py.typed
--rw-r--r--   0        0        0    10160 2024-04-10 10:42:19.473844 lusid_workflow_sdk-2.1.1/lusid_workflow/rest.py
--rw-r--r--   0        0        0      855 2024-04-10 10:42:19.477844 lusid_workflow_sdk-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    14230 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    14402 2024-04-10 12:59:40.701110 lusid_workflow_sdk-2.1.2/README.md
+-rw-r--r--   0        0        0     7786 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/api/__init__.py
+-rw-r--r--   0        0        0    57597 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0        0        0    44655 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0        0        0    61860 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/api/workers_api.py
+-rw-r--r--   0        0        0    30785 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/api_response.py
+-rw-r--r--   0        0        0    14451 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/configuration.py
+-rw-r--r--   0        0        0     5339 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/exceptions.py
+-rw-r--r--   0        0        0      587 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/__init__.py
+-rw-r--r--   0        0        0    30652 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/api_client.py
+-rw-r--r--   0        0        0     9862 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8097 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6796 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12707 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/rest.py
+-rw-r--r--   0        0        0    11573 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3886 2024-04-10 12:59:40.698110 lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     6460 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/__init__.py
+-rw-r--r--   0        0        0     3649 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_definition.py
+-rw-r--r--   0        0        0     3233 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0        0        0     6172 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_details.py
+-rw-r--r--   0        0        0     6643 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0        0        0     5406 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0        0        0     3165 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0        0        0     3766 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0        0        0     7468 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0        0        0     4145 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0        0        0     3972 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0        0        0     3459 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     2193 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/fail.py
+-rw-r--r--   0        0        0     2505 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/fail_response.py
+-rw-r--r--   0        0        0     2878 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0        0        0     2607 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0        0        0     2341 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/health_check.py
+-rw-r--r--   0        0        0     2814 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0        0        0     2723 2024-04-10 12:59:40.694110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/initial_state.py
+-rw-r--r--   0        0        0     2262 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/link.py
+-rw-r--r--   0        0        0     2607 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0        0        0     2811 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0        0        0     3857 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4053 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0        0        0     4174 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0        0        0     4077 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0        0        0     3317 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/parameter.py
+-rw-r--r--   0        0        0     2583 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0        0        0     1869 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/resource_id.py
+-rw-r--r--   0        0        0     4013 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0        0        0     2793 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/result_field.py
+-rw-r--r--   0        0        0     2293 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0        0        0     5713 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0        0        0     5913 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0        0        0     6227 2024-04-10 12:59:40.695110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0        0        0     2428 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0        0        0     2360 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0        0        0     2541 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0        0        0     2864 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0        0        0     2116 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/sleep.py
+-rw-r--r--   0        0        0     2172 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0        0        0     4397 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/stack.py
+-rw-r--r--   0        0        0     8353 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task.py
+-rw-r--r--   0        0        0     7864 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_definition.py
+-rw-r--r--   0        0        0     2090 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0        0        0     2483 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0        0        0     2546 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0        0        0     2279 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0        0        0     3415 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_summary.py
+-rw-r--r--   0        0        0     4806 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0        0        0     2728 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0        0        0     2716 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0        0        0     2910 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0        0        0     1951 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0        0        0     7130 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0        0        0     3588 2024-04-10 12:59:40.696110 lusid_workflow_sdk-2.1.2/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0        0        0     3579 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0        0        0     5124 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/version_info.py
+-rw-r--r--   0        0        0     6137 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker.py
+-rw-r--r--   0        0        0     7051 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0        0        0     7753 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0        0        0     4204 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/py.typed
+-rw-r--r--   0        0        0    10160 2024-04-10 12:59:40.697111 lusid_workflow_sdk-2.1.2/lusid_workflow/rest.py
+-rw-r--r--   0        0        0      855 2024-04-10 12:59:40.701110 lusid_workflow_sdk-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15447 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.2/PKG-INFO
```

### Comparing `lusid_workflow_sdk-2.1.1/README.md` & `lusid_workflow_sdk-2.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.878
-- Package version: 2.1.1
+- API version: 0.1.879
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -130,15 +130,15 @@
 import lusid_workflow
 from lusid_workflow.exceptions import ApiException
 from pprint import pprint
 
 import os
 from lusid_workflow import (
     ApiClientFactory,
-    EventHandlersApi,
+    TaskDefinitionsApi,
     EnvironmentVariablesConfigurationLoader,
     SecretsFileConfigurationLoader,
     ArgsConfigurationLoader
 )
 
 # Use the lusid_workflow ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
@@ -166,34 +166,33 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = api_client_factory.build(EventHandlersApi)
-    create_event_handler_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example Event Handler","description":"Test","status":"Active","eventMatchingPattern":{"eventType":"PortfolioCreated","filter":"body.scope eq 'TestScope'"},"runAsUserId":{"setTo":"ExampleUserId"},"taskDefinitionId":{"scope":"A1","code":"YYY"},"taskDefinitionAsAt":"9999-12-31T23:59:59.9999999+00:00","taskActivity":{"InitialTrigger":"InitialTrigger","Type":"CreateNewTask","CorrelationIds":[],"TaskFields":{}}} # CreateEventHandlerRequest | The data to create an Event Handler
+    api_instance = api_client_factory.build(TaskDefinitionsApi)
+    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","runAsUserId":"user-id","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
 
     try:
-        # [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
-        api_response = await api_instance.create_event_handler(create_event_handler_request)
-        print("The response of EventHandlersApi->create_event_handler:\n")
+        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
+        api_response = await api_instance.create_task_definition(create_task_definition_request)
+        print("The response of TaskDefinitionsApi->create_task_definition:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling EventHandlersApi->create_event_handler: %s\n" % e)
+        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/workflow*
 
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
@@ -215,22 +214,18 @@
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

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/__init__.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Do not edit the class manually.
 """
 
 
 from __future__ import absolute_import
 
 # import apis into sdk package
-from lusid_workflow.api.event_handlers_api import EventHandlersApi
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.configuration import Configuration
@@ -34,22 +33,18 @@
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
@@ -107,33 +102,28 @@
     EnvironmentVariablesConfigurationLoader,
     ArgsConfigurationLoader,
     SyncApiClient
 )
 
 
 __all__ = [
-    "EventHandlersApi",
     "TaskDefinitionsApi",
     "TasksApi",
     "WorkersApi",
     "ActionDefinition",
     "ActionDefinitionResponse",
     "ActionDetails",
     "ActionDetailsResponse",
     "CreateChildTaskConfiguration",
     "CreateChildTasksAction",
     "CreateChildTasksActionResponse",
-    "CreateEventHandlerRequest",
     "CreateTaskDefinitionRequest",
     "CreateTaskRequest",
     "CreateWorkerRequest",
     "DeletedEntityResponse",
-    "EventHandler",
-    "EventHandlerMapping",
-    "EventMatchingPattern",
     "Fail",
     "FailResponse",
     "FieldMapping",
     "GetWorkerResultResponse",
     "HealthCheck",
     "HealthCheckResponse",
     "InitialState",
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/api/task_definitions_api.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/api/task_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/api/tasks_api.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/api/workers_api.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/api/workers_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/api_client.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/api_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/configuration.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_workflow-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.878\n"\
+               "Version of the API: 0.1.879\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/exceptions.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/__init__.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_client_factory.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/api_configuration.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/configuration_loaders.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/proxy_config.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/refreshing_token.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/rest.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/retry.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/socket_keep_alive.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/extensions/tcp_keep_alive_connector.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/__init__.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,18 @@
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
@@ -86,22 +82,18 @@
     "ActionDefinition",
     "ActionDefinitionResponse",
     "ActionDetails",
     "ActionDetailsResponse",
     "CreateChildTaskConfiguration",
     "CreateChildTasksAction",
     "CreateChildTasksActionResponse",
-    "CreateEventHandlerRequest",
     "CreateTaskDefinitionRequest",
     "CreateTaskRequest",
     "CreateWorkerRequest",
     "DeletedEntityResponse",
-    "EventHandler",
-    "EventHandlerMapping",
-    "EventMatchingPattern",
     "Fail",
     "FailResponse",
     "FieldMapping",
     "GetWorkerResultResponse",
     "HealthCheck",
     "HealthCheckResponse",
     "InitialState",
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_definition_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_definition_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/action_details_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/action_details_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_task_configuration.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_child_tasks_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_event_handler_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,33 +15,40 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic.v1 import BaseModel, Field, StrictStr, constr
-from lusid_workflow.models.event_handler_mapping import EventHandlerMapping
-from lusid_workflow.models.event_matching_pattern import EventMatchingPattern
+from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
+from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.resource_id import ResourceId
+from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
 
-class CreateEventHandlerRequest(BaseModel):
+class ResultantChildTaskConfiguration(BaseModel):
     """
-    Contains information for creating an Event Handler  # noqa: E501
+    Child Task Configuration  # noqa: E501
     """
-    id: ResourceId = Field(...)
-    display_name: constr(strict=True, min_length=1) = Field(..., alias="displayName", description="Human readable name")
-    description: Optional[StrictStr] = Field(None, description="Human readable description")
-    status: constr(strict=True, min_length=1) = Field(..., description="The current status of the event handler")
-    event_matching_pattern: EventMatchingPattern = Field(..., alias="eventMatchingPattern")
-    run_as_user_id: EventHandlerMapping = Field(..., alias="runAsUserId")
+    result_matching_pattern: Optional[ResultMatchingPattern] = Field(None, alias="resultMatchingPattern")
     task_definition_id: ResourceId = Field(..., alias="taskDefinitionId")
-    task_definition_as_at: Optional[datetime] = Field(None, alias="taskDefinitionAsAt", description="AsAt of the required task definition")
-    task_activity: Optional[Any] = Field(..., alias="taskActivity", description="Defines what the event handler should do after being triggered")
-    __properties = ["id", "displayName", "description", "status", "eventMatchingPattern", "runAsUserId", "taskDefinitionId", "taskDefinitionAsAt", "taskActivity"]
+    task_definition_as_at: Optional[datetime] = Field(None, alias="taskDefinitionAsAt", description="TaskDefinition AsAt timestamp")
+    initial_trigger: Optional[constr(strict=True, max_length=1024)] = Field(None, alias="initialTrigger", description="The Initial Trigger for automatic start")
+    child_task_fields: Dict[str, FieldMapping] = Field(..., alias="childTaskFields", description="Field Mappings")
+    map_stacking_key_from: Optional[StrictStr] = Field(None, alias="mapStackingKeyFrom", description="The field to be mapped as the ChildTasks Stacking Key")
+    __properties = ["resultMatchingPattern", "taskDefinitionId", "taskDefinitionAsAt", "initialTrigger", "childTaskFields", "mapStackingKeyFrom"]
+
+    @validator('initial_trigger')
+    def initial_trigger_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if value is None:
+            return value
+
+        if not re.match(r"^[a-zA-Z0-9\-_]+$", value):
+            raise ValueError(r"must validate the regular expression /^[a-zA-Z0-9\-_]+$/")
+        return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -49,67 +56,70 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateEventHandlerRequest:
-        """Create an instance of CreateEventHandlerRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultantChildTaskConfiguration:
+        """Create an instance of ResultantChildTaskConfiguration from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of id
-        if self.id:
-            _dict['id'] = self.id.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of event_matching_pattern
-        if self.event_matching_pattern:
-            _dict['eventMatchingPattern'] = self.event_matching_pattern.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of run_as_user_id
-        if self.run_as_user_id:
-            _dict['runAsUserId'] = self.run_as_user_id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of result_matching_pattern
+        if self.result_matching_pattern:
+            _dict['resultMatchingPattern'] = self.result_matching_pattern.to_dict()
         # override the default output from pydantic by calling `to_dict()` of task_definition_id
         if self.task_definition_id:
             _dict['taskDefinitionId'] = self.task_definition_id.to_dict()
-        # set to None if description (nullable) is None
-        # and __fields_set__ contains the field
-        if self.description is None and "description" in self.__fields_set__:
-            _dict['description'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of each value in child_task_fields (dict)
+        _field_dict = {}
+        if self.child_task_fields:
+            for _key in self.child_task_fields:
+                if self.child_task_fields[_key]:
+                    _field_dict[_key] = self.child_task_fields[_key].to_dict()
+            _dict['childTaskFields'] = _field_dict
         # set to None if task_definition_as_at (nullable) is None
         # and __fields_set__ contains the field
         if self.task_definition_as_at is None and "task_definition_as_at" in self.__fields_set__:
             _dict['taskDefinitionAsAt'] = None
 
-        # set to None if task_activity (nullable) is None
+        # set to None if initial_trigger (nullable) is None
+        # and __fields_set__ contains the field
+        if self.initial_trigger is None and "initial_trigger" in self.__fields_set__:
+            _dict['initialTrigger'] = None
+
+        # set to None if map_stacking_key_from (nullable) is None
         # and __fields_set__ contains the field
-        if self.task_activity is None and "task_activity" in self.__fields_set__:
-            _dict['taskActivity'] = None
+        if self.map_stacking_key_from is None and "map_stacking_key_from" in self.__fields_set__:
+            _dict['mapStackingKeyFrom'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateEventHandlerRequest:
-        """Create an instance of CreateEventHandlerRequest from a dict"""
+    def from_dict(cls, obj: dict) -> ResultantChildTaskConfiguration:
+        """Create an instance of ResultantChildTaskConfiguration from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreateEventHandlerRequest.parse_obj(obj)
+            return ResultantChildTaskConfiguration.parse_obj(obj)
 
-        _obj = CreateEventHandlerRequest.parse_obj({
-            "id": ResourceId.from_dict(obj.get("id")) if obj.get("id") is not None else None,
-            "display_name": obj.get("displayName"),
-            "description": obj.get("description"),
-            "status": obj.get("status"),
-            "event_matching_pattern": EventMatchingPattern.from_dict(obj.get("eventMatchingPattern")) if obj.get("eventMatchingPattern") is not None else None,
-            "run_as_user_id": EventHandlerMapping.from_dict(obj.get("runAsUserId")) if obj.get("runAsUserId") is not None else None,
+        _obj = ResultantChildTaskConfiguration.parse_obj({
+            "result_matching_pattern": ResultMatchingPattern.from_dict(obj.get("resultMatchingPattern")) if obj.get("resultMatchingPattern") is not None else None,
             "task_definition_id": ResourceId.from_dict(obj.get("taskDefinitionId")) if obj.get("taskDefinitionId") is not None else None,
             "task_definition_as_at": obj.get("taskDefinitionAsAt"),
-            "task_activity": obj.get("taskActivity")
+            "initial_trigger": obj.get("initialTrigger"),
+            "child_task_fields": dict(
+                (_k, FieldMapping.from_dict(_v))
+                for _k, _v in obj.get("childTaskFields").items()
+            )
+            if obj.get("childTaskFields") is not None
+            else None,
+            "map_stacking_key_from": obj.get("mapStackingKeyFrom")
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_definition_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_task_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/create_worker_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/create_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/deleted_entity_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/deleted_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/event_handler_mapping.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,23 +15,33 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic.v1 import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr, validator
 
-class EventHandlerMapping(BaseModel):
+class TriggerParentTaskActionResponse(BaseModel):
     """
-    Defines a mapping for event handler properties  # noqa: E501
+    Defines a read-only Trigger Parent Task Action  # noqa: E501
     """
-    map_from: Optional[StrictStr] = Field(None, alias="mapFrom", description="The field to map from")
-    set_to: Optional[StrictStr] = Field(None, alias="setTo", description="The (constant) value to set")
-    __properties = ["mapFrom", "setTo"]
+    type: Optional[StrictStr] = Field(None, description="Type name for this Action")
+    trigger: Optional[StrictStr] = Field(None, description="Trigger on parent task to be invoked")
+    __properties = ["type", "trigger"]
+
+    @validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('TriggerParentTask'):
+            raise ValueError("must be one of enum values ('TriggerParentTask')")
+        return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,43 +49,43 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> EventHandlerMapping:
-        """Create an instance of EventHandlerMapping from a JSON string"""
+    def from_json(cls, json_str: str) -> TriggerParentTaskActionResponse:
+        """Create an instance of TriggerParentTaskActionResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if map_from (nullable) is None
+        # set to None if type (nullable) is None
         # and __fields_set__ contains the field
-        if self.map_from is None and "map_from" in self.__fields_set__:
-            _dict['mapFrom'] = None
+        if self.type is None and "type" in self.__fields_set__:
+            _dict['type'] = None
 
-        # set to None if set_to (nullable) is None
+        # set to None if trigger (nullable) is None
         # and __fields_set__ contains the field
-        if self.set_to is None and "set_to" in self.__fields_set__:
-            _dict['setTo'] = None
+        if self.trigger is None and "trigger" in self.__fields_set__:
+            _dict['trigger'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> EventHandlerMapping:
-        """Create an instance of EventHandlerMapping from a dict"""
+    def from_dict(cls, obj: dict) -> TriggerParentTaskActionResponse:
+        """Create an instance of TriggerParentTaskActionResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return EventHandlerMapping.parse_obj(obj)
+            return TriggerParentTaskActionResponse.parse_obj(obj)
 
-        _obj = EventHandlerMapping.parse_obj({
-            "map_from": obj.get("mapFrom"),
-            "set_to": obj.get("setTo")
+        _obj = TriggerParentTaskActionResponse.parse_obj({
+            "type": obj.get("type"),
+            "trigger": obj.get("trigger")
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/fail.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/fail_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/fail_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/field_mapping.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/field_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/get_worker_result_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/get_worker_result_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/health_check.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/health_check_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/health_check_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/initial_state.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/initial_state.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/link.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/luminesce_view.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/luminesce_view_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/luminesce_view_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_problem_details.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/parameter_value.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/parameter_value.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_id.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/resource_list_of_task.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_field.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/result_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/result_matching_pattern.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/result_matching_pattern.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_action_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,40 +14,41 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Any, Dict, Optional
-from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
+from typing import Any, Dict, List, Optional
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
 from lusid_workflow.models.field_mapping import FieldMapping
 from lusid_workflow.models.resource_id import ResourceId
-from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
+from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
+from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
 
-class ResultantChildTaskConfiguration(BaseModel):
+class RunWorkerActionResponse(BaseModel):
     """
-    Child Task Configuration  # noqa: E501
+    Defines a read-only Run Worker Action  # noqa: E501
     """
-    result_matching_pattern: Optional[ResultMatchingPattern] = Field(None, alias="resultMatchingPattern")
-    task_definition_id: ResourceId = Field(..., alias="taskDefinitionId")
-    task_definition_as_at: Optional[datetime] = Field(None, alias="taskDefinitionAsAt", description="TaskDefinition AsAt timestamp")
-    initial_trigger: Optional[constr(strict=True, max_length=1024)] = Field(None, alias="initialTrigger", description="The Initial Trigger for automatic start")
-    child_task_fields: Dict[str, FieldMapping] = Field(..., alias="childTaskFields", description="Field Mappings")
-    map_stacking_key_from: Optional[StrictStr] = Field(None, alias="mapStackingKeyFrom", description="The field to be mapped as the ChildTasks Stacking Key")
-    __properties = ["resultMatchingPattern", "taskDefinitionId", "taskDefinitionAsAt", "initialTrigger", "childTaskFields", "mapStackingKeyFrom"]
-
-    @validator('initial_trigger')
-    def initial_trigger_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
+    type: Optional[StrictStr] = Field(None, description="Type name for this Action")
+    worker_id: Optional[ResourceId] = Field(None, alias="workerId")
+    worker_as_at: Optional[datetime] = Field(None, alias="workerAsAt", description="Worker AsAt")
+    worker_parameters: Optional[Dict[str, FieldMapping]] = Field(None, alias="workerParameters", description="Parameters for this Worker")
+    worker_status_triggers: Optional[WorkerStatusTriggers] = Field(None, alias="workerStatusTriggers")
+    child_task_configurations: Optional[conlist(ResultantChildTaskConfiguration)] = Field(None, alias="childTaskConfigurations", description="Tasks can be generated from run worker results; this is the configuration")
+    __properties = ["type", "workerId", "workerAsAt", "workerParameters", "workerStatusTriggers", "childTaskConfigurations"]
+
+    @validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
         if value is None:
             return value
 
-        if not re.match(r"^[a-zA-Z0-9\-_]+$", value):
-            raise ValueError(r"must validate the regular expression /^[a-zA-Z0-9\-_]+$/")
+        if value not in ('RunWorker'):
+            raise ValueError("must be one of enum values ('RunWorker')")
         return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -56,70 +57,82 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ResultantChildTaskConfiguration:
-        """Create an instance of ResultantChildTaskConfiguration from a JSON string"""
+    def from_json(cls, json_str: str) -> RunWorkerActionResponse:
+        """Create an instance of RunWorkerActionResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of result_matching_pattern
-        if self.result_matching_pattern:
-            _dict['resultMatchingPattern'] = self.result_matching_pattern.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of task_definition_id
-        if self.task_definition_id:
-            _dict['taskDefinitionId'] = self.task_definition_id.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each value in child_task_fields (dict)
+        # override the default output from pydantic by calling `to_dict()` of worker_id
+        if self.worker_id:
+            _dict['workerId'] = self.worker_id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each value in worker_parameters (dict)
         _field_dict = {}
-        if self.child_task_fields:
-            for _key in self.child_task_fields:
-                if self.child_task_fields[_key]:
-                    _field_dict[_key] = self.child_task_fields[_key].to_dict()
-            _dict['childTaskFields'] = _field_dict
-        # set to None if task_definition_as_at (nullable) is None
+        if self.worker_parameters:
+            for _key in self.worker_parameters:
+                if self.worker_parameters[_key]:
+                    _field_dict[_key] = self.worker_parameters[_key].to_dict()
+            _dict['workerParameters'] = _field_dict
+        # override the default output from pydantic by calling `to_dict()` of worker_status_triggers
+        if self.worker_status_triggers:
+            _dict['workerStatusTriggers'] = self.worker_status_triggers.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in child_task_configurations (list)
+        _items = []
+        if self.child_task_configurations:
+            for _item in self.child_task_configurations:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['childTaskConfigurations'] = _items
+        # set to None if type (nullable) is None
         # and __fields_set__ contains the field
-        if self.task_definition_as_at is None and "task_definition_as_at" in self.__fields_set__:
-            _dict['taskDefinitionAsAt'] = None
+        if self.type is None and "type" in self.__fields_set__:
+            _dict['type'] = None
 
-        # set to None if initial_trigger (nullable) is None
+        # set to None if worker_as_at (nullable) is None
         # and __fields_set__ contains the field
-        if self.initial_trigger is None and "initial_trigger" in self.__fields_set__:
-            _dict['initialTrigger'] = None
+        if self.worker_as_at is None and "worker_as_at" in self.__fields_set__:
+            _dict['workerAsAt'] = None
 
-        # set to None if map_stacking_key_from (nullable) is None
+        # set to None if worker_parameters (nullable) is None
         # and __fields_set__ contains the field
-        if self.map_stacking_key_from is None and "map_stacking_key_from" in self.__fields_set__:
-            _dict['mapStackingKeyFrom'] = None
+        if self.worker_parameters is None and "worker_parameters" in self.__fields_set__:
+            _dict['workerParameters'] = None
+
+        # set to None if child_task_configurations (nullable) is None
+        # and __fields_set__ contains the field
+        if self.child_task_configurations is None and "child_task_configurations" in self.__fields_set__:
+            _dict['childTaskConfigurations'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ResultantChildTaskConfiguration:
-        """Create an instance of ResultantChildTaskConfiguration from a dict"""
+    def from_dict(cls, obj: dict) -> RunWorkerActionResponse:
+        """Create an instance of RunWorkerActionResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ResultantChildTaskConfiguration.parse_obj(obj)
+            return RunWorkerActionResponse.parse_obj(obj)
 
-        _obj = ResultantChildTaskConfiguration.parse_obj({
-            "result_matching_pattern": ResultMatchingPattern.from_dict(obj.get("resultMatchingPattern")) if obj.get("resultMatchingPattern") is not None else None,
-            "task_definition_id": ResourceId.from_dict(obj.get("taskDefinitionId")) if obj.get("taskDefinitionId") is not None else None,
-            "task_definition_as_at": obj.get("taskDefinitionAsAt"),
-            "initial_trigger": obj.get("initialTrigger"),
-            "child_task_fields": dict(
+        _obj = RunWorkerActionResponse.parse_obj({
+            "type": obj.get("type"),
+            "worker_id": ResourceId.from_dict(obj.get("workerId")) if obj.get("workerId") is not None else None,
+            "worker_as_at": obj.get("workerAsAt"),
+            "worker_parameters": dict(
                 (_k, FieldMapping.from_dict(_v))
-                for _k, _v in obj.get("childTaskFields").items()
+                for _k, _v in obj.get("workerParameters").items()
             )
-            if obj.get("childTaskFields") is not None
+            if obj.get("workerParameters") is not None
             else None,
-            "map_stacking_key_from": obj.get("mapStackingKeyFrom")
+            "worker_status_triggers": WorkerStatusTriggers.from_dict(obj.get("workerStatusTriggers")) if obj.get("workerStatusTriggers") is not None else None,
+            "child_task_configurations": [ResultantChildTaskConfiguration.from_dict(_item) for _item in obj.get("childTaskConfigurations")] if obj.get("childTaskConfigurations") is not None else None
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_action_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,43 +13,37 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Any, Dict, List, Optional
-from pydantic.v1 import BaseModel, Field, StrictStr, conlist, validator
-from lusid_workflow.models.field_mapping import FieldMapping
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
+from lusid_workflow.models.link import Link
+from lusid_workflow.models.parameter import Parameter
 from lusid_workflow.models.resource_id import ResourceId
-from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
-from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
+from lusid_workflow.models.result_field import ResultField
+from lusid_workflow.models.version_info import VersionInfo
+from lusid_workflow.models.worker_configuration_response import WorkerConfigurationResponse
 
-class RunWorkerActionResponse(BaseModel):
+class Worker(BaseModel):
     """
-    Defines a read-only Run Worker Action  # noqa: E501
+    Information about the Worker  # noqa: E501
     """
-    type: Optional[StrictStr] = Field(None, description="Type name for this Action")
-    worker_id: Optional[ResourceId] = Field(None, alias="workerId")
-    worker_as_at: Optional[datetime] = Field(None, alias="workerAsAt", description="Worker AsAt")
-    worker_parameters: Optional[Dict[str, FieldMapping]] = Field(None, alias="workerParameters", description="Parameters for this Worker")
-    worker_status_triggers: Optional[WorkerStatusTriggers] = Field(None, alias="workerStatusTriggers")
-    child_task_configurations: Optional[conlist(ResultantChildTaskConfiguration)] = Field(None, alias="childTaskConfigurations", description="Tasks can be generated from run worker results; this is the configuration")
-    __properties = ["type", "workerId", "workerAsAt", "workerParameters", "workerStatusTriggers", "childTaskConfigurations"]
-
-    @validator('type')
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('RunWorker'):
-            raise ValueError("must be one of enum values ('RunWorker')")
-        return value
+    id: ResourceId = Field(...)
+    display_name: constr(strict=True, min_length=1) = Field(..., alias="displayName", description="Human readable name")
+    description: Optional[StrictStr] = Field(None, description="Human readable description")
+    worker_configuration: WorkerConfigurationResponse = Field(..., alias="workerConfiguration")
+    version: Optional[VersionInfo] = None
+    parameters: Optional[conlist(Parameter)] = Field(None, description="The Parameters this Worker accepts or requires.")
+    result_fields: Optional[conlist(ResultField)] = Field(None, alias="resultFields", description="The Fields that the Worker results will come back with.")
+    links: Optional[conlist(Link)] = None
+    __properties = ["id", "displayName", "description", "workerConfiguration", "version", "parameters", "resultFields", "links"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -57,82 +51,89 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> RunWorkerActionResponse:
-        """Create an instance of RunWorkerActionResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Worker:
+        """Create an instance of Worker from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of worker_id
-        if self.worker_id:
-            _dict['workerId'] = self.worker_id.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each value in worker_parameters (dict)
-        _field_dict = {}
-        if self.worker_parameters:
-            for _key in self.worker_parameters:
-                if self.worker_parameters[_key]:
-                    _field_dict[_key] = self.worker_parameters[_key].to_dict()
-            _dict['workerParameters'] = _field_dict
-        # override the default output from pydantic by calling `to_dict()` of worker_status_triggers
-        if self.worker_status_triggers:
-            _dict['workerStatusTriggers'] = self.worker_status_triggers.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in child_task_configurations (list)
+        # override the default output from pydantic by calling `to_dict()` of id
+        if self.id:
+            _dict['id'] = self.id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of worker_configuration
+        if self.worker_configuration:
+            _dict['workerConfiguration'] = self.worker_configuration.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of version
+        if self.version:
+            _dict['version'] = self.version.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in parameters (list)
+        _items = []
+        if self.parameters:
+            for _item in self.parameters:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['parameters'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in result_fields (list)
+        _items = []
+        if self.result_fields:
+            for _item in self.result_fields:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['resultFields'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in links (list)
         _items = []
-        if self.child_task_configurations:
-            for _item in self.child_task_configurations:
+        if self.links:
+            for _item in self.links:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['childTaskConfigurations'] = _items
-        # set to None if type (nullable) is None
+            _dict['links'] = _items
+        # set to None if description (nullable) is None
         # and __fields_set__ contains the field
-        if self.type is None and "type" in self.__fields_set__:
-            _dict['type'] = None
+        if self.description is None and "description" in self.__fields_set__:
+            _dict['description'] = None
 
-        # set to None if worker_as_at (nullable) is None
+        # set to None if parameters (nullable) is None
         # and __fields_set__ contains the field
-        if self.worker_as_at is None and "worker_as_at" in self.__fields_set__:
-            _dict['workerAsAt'] = None
+        if self.parameters is None and "parameters" in self.__fields_set__:
+            _dict['parameters'] = None
 
-        # set to None if worker_parameters (nullable) is None
+        # set to None if result_fields (nullable) is None
         # and __fields_set__ contains the field
-        if self.worker_parameters is None and "worker_parameters" in self.__fields_set__:
-            _dict['workerParameters'] = None
+        if self.result_fields is None and "result_fields" in self.__fields_set__:
+            _dict['resultFields'] = None
 
-        # set to None if child_task_configurations (nullable) is None
+        # set to None if links (nullable) is None
         # and __fields_set__ contains the field
-        if self.child_task_configurations is None and "child_task_configurations" in self.__fields_set__:
-            _dict['childTaskConfigurations'] = None
+        if self.links is None and "links" in self.__fields_set__:
+            _dict['links'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> RunWorkerActionResponse:
-        """Create an instance of RunWorkerActionResponse from a dict"""
+    def from_dict(cls, obj: dict) -> Worker:
+        """Create an instance of Worker from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return RunWorkerActionResponse.parse_obj(obj)
+            return Worker.parse_obj(obj)
 
-        _obj = RunWorkerActionResponse.parse_obj({
-            "type": obj.get("type"),
-            "worker_id": ResourceId.from_dict(obj.get("workerId")) if obj.get("workerId") is not None else None,
-            "worker_as_at": obj.get("workerAsAt"),
-            "worker_parameters": dict(
-                (_k, FieldMapping.from_dict(_v))
-                for _k, _v in obj.get("workerParameters").items()
-            )
-            if obj.get("workerParameters") is not None
-            else None,
-            "worker_status_triggers": WorkerStatusTriggers.from_dict(obj.get("workerStatusTriggers")) if obj.get("workerStatusTriggers") is not None else None,
-            "child_task_configurations": [ResultantChildTaskConfiguration.from_dict(_item) for _item in obj.get("childTaskConfigurations")] if obj.get("childTaskConfigurations") is not None else None
+        _obj = Worker.parse_obj({
+            "id": ResourceId.from_dict(obj.get("id")) if obj.get("id") is not None else None,
+            "display_name": obj.get("displayName"),
+            "description": obj.get("description"),
+            "worker_configuration": WorkerConfigurationResponse.from_dict(obj.get("workerConfiguration")) if obj.get("workerConfiguration") is not None else None,
+            "version": VersionInfo.from_dict(obj.get("version")) if obj.get("version") is not None else None,
+            "parameters": [Parameter.from_dict(_item) for _item in obj.get("parameters")] if obj.get("parameters") is not None else None,
+            "result_fields": [ResultField.from_dict(_item) for _item in obj.get("resultFields")] if obj.get("resultFields") is not None else None,
+            "links": [Link.from_dict(_item) for _item in obj.get("links")] if obj.get("links") is not None else None
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/run_worker_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/run_worker_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/scheduler_job.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/scheduler_job_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/scheduler_job_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/sleep.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/sleep_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/sleep_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/stack.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/stack.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_definition_version.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_definition_version.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_field_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_instance_field.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_instance_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_state_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_state_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_summary.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/task_transition_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/task_transition_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/transition_trigger_definition.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/transition_trigger_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/trigger_schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,34 +14,23 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic.v1 import BaseModel, Field, StrictStr, validator
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field, constr
 
-class TriggerParentTaskActionResponse(BaseModel):
+class TriggerSchema(BaseModel):
     """
-    Defines a read-only Trigger Parent Task Action  # noqa: E501
+    Triggers can operate in response to different stimuli  # noqa: E501
     """
-    type: Optional[StrictStr] = Field(None, description="Type name for this Action")
-    trigger: Optional[StrictStr] = Field(None, description="Trigger on parent task to be invoked")
-    __properties = ["type", "trigger"]
-
-    @validator('type')
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('TriggerParentTask'):
-            raise ValueError("must be one of enum values ('TriggerParentTask')")
-        return value
+    type: constr(strict=True, min_length=1) = Field(..., description="The type of Trigger; available value(s): External")
+    __properties = ["type"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -49,43 +38,32 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TriggerParentTaskActionResponse:
-        """Create an instance of TriggerParentTaskActionResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> TriggerSchema:
+        """Create an instance of TriggerSchema from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if type (nullable) is None
-        # and __fields_set__ contains the field
-        if self.type is None and "type" in self.__fields_set__:
-            _dict['type'] = None
-
-        # set to None if trigger (nullable) is None
-        # and __fields_set__ contains the field
-        if self.trigger is None and "trigger" in self.__fields_set__:
-            _dict['trigger'] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TriggerParentTaskActionResponse:
-        """Create an instance of TriggerParentTaskActionResponse from a dict"""
+    def from_dict(cls, obj: dict) -> TriggerSchema:
+        """Create an instance of TriggerSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return TriggerParentTaskActionResponse.parse_obj(obj)
+            return TriggerSchema.parse_obj(obj)
 
-        _obj = TriggerParentTaskActionResponse.parse_obj({
-            "type": obj.get("type"),
-            "trigger": obj.get("trigger")
+        _obj = TriggerSchema.parse_obj({
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_definition_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/update_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_task_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/update_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/update_worker_request.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/update_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/version_info.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/version_info.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_configuration_response.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker_configuration_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/models/worker_status_triggers.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/models/worker_status_triggers.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/lusid_workflow/rest.py` & `lusid_workflow_sdk-2.1.2/lusid_workflow/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.1/pyproject.toml` & `lusid_workflow_sdk-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-workflow-sdk"
-version = "2.1.1"
+version = "2.1.2"
 description = "FINBOURNE Workflow API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/workflow-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Workflow API", "lusid-workflow-sdk"]
 packages = [
```

### Comparing `lusid_workflow_sdk-2.1.1/PKG-INFO` & `lusid_workflow_sdk-2.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-workflow-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: FINBOURNE Workflow API
 Home-page: https://github.com/finbourne/workflow-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Workflow API,lusid-workflow-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.878
-- Package version: 2.1.1
+- API version: 0.1.879
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -156,15 +156,15 @@
 import lusid_workflow
 from lusid_workflow.exceptions import ApiException
 from pprint import pprint
 
 import os
 from lusid_workflow import (
     ApiClientFactory,
-    EventHandlersApi,
+    TaskDefinitionsApi,
     EnvironmentVariablesConfigurationLoader,
     SecretsFileConfigurationLoader,
     ArgsConfigurationLoader
 )
 
 # Use the lusid_workflow ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
@@ -192,34 +192,33 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = api_client_factory.build(EventHandlersApi)
-    create_event_handler_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example Event Handler","description":"Test","status":"Active","eventMatchingPattern":{"eventType":"PortfolioCreated","filter":"body.scope eq 'TestScope'"},"runAsUserId":{"setTo":"ExampleUserId"},"taskDefinitionId":{"scope":"A1","code":"YYY"},"taskDefinitionAsAt":"9999-12-31T23:59:59.9999999+00:00","taskActivity":{"InitialTrigger":"InitialTrigger","Type":"CreateNewTask","CorrelationIds":[],"TaskFields":{}}} # CreateEventHandlerRequest | The data to create an Event Handler
+    api_instance = api_client_factory.build(TaskDefinitionsApi)
+    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","runAsUserId":"user-id","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{"started":null,"completedWithResults":null,"completedNoResults":null,"failedToStart":null,"failedToComplete":null},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"mapStackingKeyFrom":null,"childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}},"resultMatchingPattern":null,"taskDefinitionAsAt":null,"initialTrigger":"test-trigger"}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
 
     try:
-        # [EXPERIMENTAL] CreateEventHandler: Create a new Event Handler
-        api_response = await api_instance.create_event_handler(create_event_handler_request)
-        print("The response of EventHandlersApi->create_event_handler:\n")
+        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
+        api_response = await api_instance.create_task_definition(create_task_definition_request)
+        print("The response of TaskDefinitionsApi->create_task_definition:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling EventHandlersApi->create_event_handler: %s\n" % e)
+        print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/workflow*
 
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
@@ -241,22 +240,18 @@
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

