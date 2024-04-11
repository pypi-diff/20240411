# Comparing `tmp/forestadmin_agent_toolkit-1.6.6.tar.gz` & `tmp/forestadmin_agent_toolkit-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.6.6.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.6.7.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.6.6.tar` & `forestadmin_agent_toolkit-1.6.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/README.md
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     9526 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0     2477 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/forest_logger.py
--rw-r--r--   0        0        0     4152 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2305 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     9544 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
--rw-r--r--   0        0        0     2780 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1912 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    17490 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    22065 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     4348 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    11052 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5509 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0    12193 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0      935 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      427 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     4696 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
--rw-r--r--   0        0        0      176 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     9001 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/permission_service.py
--rw-r--r--   0        0        0     3261 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
--rw-r--r--   0        0        0      406 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/permissions_types.py
--rw-r--r--   0        0        0     5276 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
--rw-r--r--   0        0        0     3200 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
--rw-r--r--   0        0        0     1010 2024-04-03 13:40:31.129917 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0    10346 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3663 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     4557 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1252 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context_variable_injector.py
--rw-r--r--   0        0        0      655 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
--rw-r--r--   0        0        0     1230 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context_variables.py
--rw-r--r--   0        0        0     1661 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3019 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
--rw-r--r--   0        0        0     6276 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4229 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2298 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     5069 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0    13958 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
--rw-r--r--   0        0        0     2461 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     8562 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     9931 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     7303 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1774 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0     1889 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
--rw-r--r--   0        0        0      513 2024-04-03 13:40:31.133918 forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1776 2024-04-03 13:40:50.062177 forestadmin_agent_toolkit-1.6.6/pyproject.toml
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     9526 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     2477 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0     4152 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2305 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     9544 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1055 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
+-rw-r--r--   0        0        0     2780 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1912 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    17490 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    22065 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     4348 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    13068 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5509 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0    12193 2024-04-11 12:53:03.750892 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0      935 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     4696 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
+-rw-r--r--   0        0        0      176 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     9001 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/permission_service.py
+-rw-r--r--   0        0        0     3261 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
+-rw-r--r--   0        0        0      406 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/permissions_types.py
+-rw-r--r--   0        0        0     5276 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
+-rw-r--r--   0        0        0     3200 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
+-rw-r--r--   0        0        0     1010 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0    10346 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3663 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     4557 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1252 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context_variable_injector.py
+-rw-r--r--   0        0        0      655 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
+-rw-r--r--   0        0        0     1230 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context_variables.py
+-rw-r--r--   0        0        0     1661 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3019 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
+-rw-r--r--   0        0        0     6276 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4229 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2298 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     5069 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0    13958 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
+-rw-r--r--   0        0        0     2461 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     8562 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     9931 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     7303 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1774 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0     1889 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
+-rw-r--r--   0        0        0      513 2024-04-11 12:53:03.754891 forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1776 2024-04-11 12:53:22.602932 forestadmin_agent_toolkit-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.6.7/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/forest_logger.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/forest_logger.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import sys
-from ast import literal_eval
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 if sys.version_info >= (3, 9):
     import zoneinfo
 else:
     from backports import zoneinfo
 
 from forestadmin.agent_toolkit.exceptions import AgentToolkitException
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestRelationCollection
 from forestadmin.agent_toolkit.utils.context import Request
+from forestadmin.agent_toolkit.utils.id import unpack_id
 from forestadmin.datasource_toolkit.collections import Collection, CollectionException
 from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
-from forestadmin.datasource_toolkit.interfaces.fields import PrimitiveType, is_column
+from forestadmin.datasource_toolkit.interfaces.fields import Column, ColumnAlias, Operator, PrimitiveType, is_column
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import (
     ConditionTreeFactory,
     ConditionTreeFactoryException,
 )
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter, FilterComponent
@@ -33,19 +33,37 @@
     ConditionTreeValidatorException,
 )
 from forestadmin.datasource_toolkit.validations.projection import ProjectionValidator
 
 DEFAULT_ITEMS_PER_PAGE = 15
 DEFAULT_PAGE_TO_SKIP = 1
 
+STRING_TO_BOOLEAN = {
+    "true": True,
+    "yes": True,
+    "1": True,
+    "false": False,
+    "no": False,
+    "0": False,
+}
+
 
 class FilterException(AgentToolkitException):
     pass
 
 
+def _get_collection(
+    request: Union[RequestCollection, RequestRelationCollection]
+) -> Union[CollectionCustomizer, Collection]:
+    collection = request.collection
+    if isinstance(request, RequestRelationCollection):
+        collection = request.foreign_collection
+    return collection
+
+
 def _all_records_subset_query(request: Request) -> Dict[str, Any]:
     try:
         return request.body.get("data", {}).get("attributes", {}).get("all_records_subset_query", {})  # type: ignore
     except AttributeError:
         # data may be a list
         return {}
 
@@ -59,44 +77,36 @@
     if not res and request.query:
         res = request.query.get(key)
         if res:
             res = str(res)
     return res
 
 
-def parse_selection_ids(request: Request) -> Tuple[List[CompositeIdAlias], bool]:
+def parse_selection_ids(request: RequestCollection) -> Tuple[List[CompositeIdAlias], bool]:
     if request.body:
         try:
             attributes: Dict[str, Any] = request.body.get("data", {}).get("attributes", {})  # type: ignore
         except AttributeError:
             attributes = {}
         exclude_ids = bool(attributes.get("all_records", False))  # type: ignore
+
         if exclude_ids is True:
-            ids = [[id] for id in attributes.get("all_records_ids_excluded", [])]
+            ids = [unpack_id(request.collection.schema, pk) for pk in attributes.get("all_records_ids_excluded", [])]
         else:
             if "ids" in attributes:
-                ids = [[id] for id in attributes["ids"]]
+                ids = [unpack_id(request.collection.schema, pk) for pk in attributes["ids"]]
             elif isinstance(request.body.get("data"), list):
-                ids = [[r["id"]] for r in request.body["data"]]
+                ids = [unpack_id(request.collection.schema, pk["id"]) for pk in request.body["data"]]
             else:
                 ids = []
         return ids, exclude_ids
 
     raise Exception()
 
 
-def _get_collection(
-    request: Union[RequestCollection, RequestRelationCollection]
-) -> Union[CollectionCustomizer, Collection]:
-    collection = request.collection
-    if isinstance(request, RequestRelationCollection):
-        collection = request.foreign_collection
-    return collection
-
-
 def parse_sort(request: Union[RequestCollection, RequestRelationCollection]):
     sort_string: Optional[str] = _subset_or_query(request, "sort")
     if not sort_string:
         return SortFactory.by_primary_keys(_get_collection(request))
 
     sort_field = sort_string.replace(".", ":")
     is_descending = sort_string[0] == "-"
@@ -178,58 +188,111 @@
             filters = request.body["filter"]
 
     if not filters:
         return None
 
     json_filters = json.loads(filters) if isinstance(filters, str) else filters
     try:
-        if isinstance(request, RequestRelationCollection):
-            collection = request.foreign_collection
-        else:
-            collection = request.collection
-
-        json_filters = _parse_value(json_filters, collection)
+        collection = _get_collection(request)
+        json_filters = sanitize_json_filter(json_filters, collection)
 
         condition_tree = ConditionTreeFactory.from_plain_object(json_filters)
     except ConditionTreeFactoryException as e:
         raise FilterException(str(e))
 
     try:
         ConditionTreeValidator.validate(condition_tree, _get_collection(request))
     except ConditionTreeValidatorException as e:
         raise FilterException(str(e))
 
     return condition_tree
 
 
-def _parse_value(jsoned_filters, collection):
+def sanitize_json_filter(jsoned_filters, collection):
     if "conditions" in jsoned_filters:
         for condition in jsoned_filters["conditions"]:
-            condition = _parse_value(condition, collection)
+            condition = sanitize_json_filter(condition, condition)
         return jsoned_filters
 
-    schema = CollectionUtils.get_field_schema(collection, jsoned_filters["field"])
+    jsoned_filters["value"] = _parse_value(collection, jsoned_filters)
+    return jsoned_filters
 
-    new_value = jsoned_filters["value"]
-    if jsoned_filters["operator"] == "in" and isinstance(jsoned_filters["value"], str):
-        values = [val.strip() for val in jsoned_filters["value"].split(",")]
 
-        if schema["column_type"] == PrimitiveType.NUMBER:
-            new_value = [literal_eval(str(value)) for value in values]
-        else:
-            new_value = values
+def _parse_value(collection: Collection, leaf: Dict[str, Any]):
+    schema = cast(Column, CollectionUtils.get_field_schema(collection, leaf["field"]))
+    expected_type = _get_expected_type_for_condition(Operator(leaf["operator"]), schema)
+
+    return _cast_to_type(leaf["value"], expected_type)
+
+
+def _cast_to_type(value: Any, expected_type: ColumnAlias) -> Any:
+    if value is None:
+        return value
+    expected_type_to_cast: Dict[PrimitiveType, Callable[[Any], Any]] = {
+        PrimitiveType.NUMBER: _parse_str_as_number,
+        PrimitiveType.STRING: lambda value: f"{value}",
+        PrimitiveType.DATE: lambda value: f"{value}",
+        PrimitiveType.DATE_ONLY: lambda value: f"{value}",
+        PrimitiveType.BOOLEAN: lambda value: (
+            STRING_TO_BOOLEAN[value.lower()] if isinstance(value, str) else not not value
+        ),
+    }
+
+    return_value = value
+    if isinstance(expected_type, list) and isinstance(value, str):
+        return_value = [v.strip() for v in value.split(",")]
+
+        return_value = [
+            _cast_to_type(item, expected_type[0])
+            for item in return_value
+            if not (expected_type[0] == PrimitiveType.NUMBER and not _is_str_a_number(item))
+        ]
+    elif expected_type in expected_type_to_cast.keys():
+        method = expected_type_to_cast[expected_type]  # type:ignore
+        return_value = method(value)
+    return return_value
+
+
+def _parse_str_as_number(value: Union[str, int, float]) -> Union[int, float]:
+    if isinstance(value, int) or isinstance(value, float):
+        return value
+    try:
+        return int(value)
+    except Exception:
+        return float(value)
 
-    elif schema["column_type"] == PrimitiveType.NUMBER:
-        new_value = literal_eval(str(jsoned_filters["value"]))
 
-    elif schema["column_type"] == PrimitiveType.BOOLEAN:
-        new_value = jsoned_filters["value"]
+def _is_str_a_number(value: Union[str, int, float]) -> bool:
+    try:
+        _parse_str_as_number(value)
+        return True
+    except Exception:
+        return False
+
+
+def _get_expected_type_for_condition(
+    operator: Operator,
+    field_schema: Column,
+) -> PrimitiveType:
+    operators_expecting_number = [
+        Operator.SHORTER_THAN,
+        Operator.LONGER_THAN,
+        Operator.AFTER_X_HOURS_AGO,
+        Operator.BEFORE_X_HOURS_AGO,
+        Operator.PREVIOUS_X_DAYS,
+        Operator.PREVIOUS_X_DAYS_TO_DATE,
+    ]
 
-    jsoned_filters["value"] = new_value
-    return jsoned_filters
+    if operator in operators_expecting_number:
+        return PrimitiveType.NUMBER
+
+    if operator == Operator.IN:
+        return [cast(PrimitiveType, field_schema["column_type"])]  # type:ignore
+
+    return cast(PrimitiveType, field_schema["column_type"])
 
 
 def parse_projection(request: Union[RequestCollection, RequestRelationCollection]) -> Projection:
     collection = _get_collection(request)
     schema = collection.schema
     if not request.query or not request.query.get(f"fields[{collection.name}]"):
         return ProjectionFactory.all(collection)
```

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/ip_white_list_resource.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/ip_white_list_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/permission_service.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/permission_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/permissions_functions.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/permissions_functions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context_variable_injector.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context_variable_injector.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context_variable_instantiator.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context_variable_instantiator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/context_variables.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/context_variables.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/ip_whitelist_util.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/ip_whitelist_util.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.6.7/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.6.6/pyproject.toml` & `forestadmin_agent_toolkit-1.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
 description = "agent toolkit for forestadmin python agent"
-version = "1.6.6"
+version = "1.6.7"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
@@ -19,15 +19,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 aiohttp = "~=3.9"
 oic = "~=1.4"
 pyjwt = "^2"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
 sseclient-py = "^1.5"
-forestadmin-datasource-toolkit = "1.6.6"
+forestadmin-datasource-toolkit = "1.6.7"
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.4.0"
 python = ">=3.8"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~0.2.1"
 python = "<3.9"
```

### Comparing `forestadmin_agent_toolkit-1.6.6/PKG-INFO` & `forestadmin_agent_toolkit-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.6.6
+Version: 1.6.7
 Summary: agent toolkit for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (==1.6.6)
+Requires-Dist: forestadmin-datasource-toolkit (==1.6.7)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: sseclient-py (>=1.5,<2.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
```

