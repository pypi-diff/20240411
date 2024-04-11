# Comparing `tmp/finbourne_access_sdk-2.1.3.tar.gz` & `tmp/finbourne_access_sdk-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_access_sdk-2.1.3.tar", max compression
+gzip compressed data, was "finbourne_access_sdk-2.1.4.tar", max compression
```

## Comparing `finbourne_access_sdk-2.1.3.tar` & `finbourne_access_sdk-2.1.4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    17778 2024-04-10 11:19:18.364232 finbourne_access_sdk-2.1.3/README.md
--rw-r--r--   0        0        0    10462 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/__init__.py
--rw-r--r--   0        0        0      498 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/api/__init__.py
--rw-r--r--   0        0        0     7551 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/api/application_metadata_api.py
--rw-r--r--   0        0        0   160687 2024-04-10 11:19:18.352232 finbourne_access_sdk-2.1.3/finbourne_access/api/policies_api.py
--rw-r--r--   0        0        0    55454 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/api/policy_templates_api.py
--rw-r--r--   0        0        0    68286 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/api/roles_api.py
--rw-r--r--   0        0        0    76101 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/api/user_roles_api.py
--rw-r--r--   0        0        0    30808 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/api_client.py
--rw-r--r--   0        0        0      852 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/api_response.py
--rw-r--r--   0        0        0    14461 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/configuration.py
--rw-r--r--   0        0        0     5348 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/exceptions.py
--rw-r--r--   0        0        0      593 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/__init__.py
--rw-r--r--   0        0        0    30677 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/api_client.py
--rw-r--r--   0        0        0     9882 2024-04-10 11:19:18.354232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8107 2024-04-10 11:19:18.354232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/api_configuration.py
--rw-r--r--   0        0        0     6804 2024-04-10 11:19:18.354232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12709 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/rest.py
--rw-r--r--   0        0        0    11575 2024-04-10 11:19:18.354232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3888 2024-04-10 11:19:18.355232 finbourne_access_sdk-2.1.3/finbourne_access/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     8919 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/__init__.py
--rw-r--r--   0        0        0     3918 2024-04-10 11:19:18.340232 finbourne_access_sdk-2.1.3/finbourne_access/models/access_controlled_action.py
--rw-r--r--   0        0        0     4861 2024-04-10 11:19:18.340232 finbourne_access_sdk-2.1.3/finbourne_access/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2079 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/action_id.py
--rw-r--r--   0        0        0     2705 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/add_policy_collection_to_role_request.py
--rw-r--r--   0        0        0     2461 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/add_policy_to_role_request.py
--rw-r--r--   0        0        0     3823 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/add_to_policy_collection_request.py
--rw-r--r--   0        0        0     2563 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/as_at_predicate_contract.py
--rw-r--r--   0        0        0     2488 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/as_at_range_for_spec.py
--rw-r--r--   0        0        0     2466 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/as_at_relative.py
--rw-r--r--   0        0        0     6888 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/attached_policy_definition_response.py
--rw-r--r--   0        0        0     1096 2024-04-10 11:19:18.341233 finbourne_access_sdk-2.1.3/finbourne_access/models/date_quality.py
--rw-r--r--   0        0        0      781 2024-04-10 11:19:18.342233 finbourne_access_sdk-2.1.3/finbourne_access/models/date_unit.py
--rw-r--r--   0        0        0     1971 2024-04-10 11:19:18.342233 finbourne_access_sdk-2.1.3/finbourne_access/models/effective_date_has_quality.py
--rw-r--r--   0        0        0     2538 2024-04-10 11:19:18.342233 finbourne_access_sdk-2.1.3/finbourne_access/models/effective_date_relative.py
--rw-r--r--   0        0        0     2148 2024-04-10 11:19:18.342233 finbourne_access_sdk-2.1.3/finbourne_access/models/effective_range.py
--rw-r--r--   0        0        0     2387 2024-04-10 11:19:18.342233 finbourne_access_sdk-2.1.3/finbourne_access/models/entitlement_metadata.py
--rw-r--r--   0        0        0     2625 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/evaluation_request.py
--rw-r--r--   0        0        0     2473 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/evaluation_response.py
--rw-r--r--   0        0        0      766 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/evaluation_result.py
--rw-r--r--   0        0        0     4459 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/for_spec.py
--rw-r--r--   0        0        0     3649 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/generate_policy_from_template_request.py
--rw-r--r--   0        0        0     3731 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/generated_policy_components.py
--rw-r--r--   0        0        0      654 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/grant.py
--rw-r--r--   0        0        0     2867 2024-04-10 11:19:18.343232 finbourne_access_sdk-2.1.3/finbourne_access/models/how_spec.py
--rw-r--r--   0        0        0     3191 2024-04-10 11:19:18.344232 finbourne_access_sdk-2.1.3/finbourne_access/models/id_selector_definition.py
--rw-r--r--   0        0        0     3116 2024-04-10 11:19:18.344232 finbourne_access_sdk-2.1.3/finbourne_access/models/identifier_part_schema.py
--rw-r--r--   0        0        0     4383 2024-04-10 11:19:18.344232 finbourne_access_sdk-2.1.3/finbourne_access/models/if_expression.py
--rw-r--r--   0        0        0     2435 2024-04-10 11:19:18.345233 finbourne_access_sdk-2.1.3/finbourne_access/models/if_feature_chain_expression.py
--rw-r--r--   0        0        0     3651 2024-04-10 11:19:18.345233 finbourne_access_sdk-2.1.3/finbourne_access/models/if_identity_claim_expression.py
--rw-r--r--   0        0        0     2325 2024-04-10 11:19:18.345233 finbourne_access_sdk-2.1.3/finbourne_access/models/if_identity_scope_expression.py
--rw-r--r--   0        0        0     2496 2024-04-10 11:19:18.346233 finbourne_access_sdk-2.1.3/finbourne_access/models/if_request_header_expression.py
--rw-r--r--   0        0        0     2419 2024-04-10 11:19:18.346233 finbourne_access_sdk-2.1.3/finbourne_access/models/key_value_pair_of_string_to_string.py
--rw-r--r--   0        0        0     2271 2024-04-10 11:19:18.346233 finbourne_access_sdk-2.1.3/finbourne_access/models/link.py
--rw-r--r--   0        0        0     3866 2024-04-10 11:19:18.346233 finbourne_access_sdk-2.1.3/finbourne_access/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4702 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3115 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/match_all_selector_definition.py
--rw-r--r--   0        0        0     2448 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/metadata_expression.py
--rw-r--r--   0        0        0     3747 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/metadata_selector_definition.py
--rw-r--r--   0        0        0     2048 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/non_transitive_supervisor_role_resource.py
--rw-r--r--   0        0        0      847 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/operator.py
--rw-r--r--   0        0        0      995 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/point_in_time_specification.py
--rw-r--r--   0        0        0     6049 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_creation_request.py
--rw-r--r--   0        0        0     2945 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_id.py
--rw-r--r--   0        0        0     5205 2024-04-10 11:19:18.347232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_response.py
--rw-r--r--   0        0        0     5467 2024-04-10 11:19:18.348232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_update_request.py
--rw-r--r--   0        0        0     6884 2024-04-10 11:19:18.348232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_creation_request.py
--rw-r--r--   0        0        0     2865 2024-04-10 11:19:18.348232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_id.py
--rw-r--r--   0        0        0     3546 2024-04-10 11:19:18.348232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_id_role_resource.py
--rw-r--r--   0        0        0     7551 2024-04-10 11:19:18.348232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_response.py
--rw-r--r--   0        0        0     4492 2024-04-10 11:19:18.348232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_selector_definition.py
--rw-r--r--   0        0        0     3686 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_template_creation_request.py
--rw-r--r--   0        0        0     5276 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_template_response.py
--rw-r--r--   0        0        0     3153 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_template_update_request.py
--rw-r--r--   0        0        0     2647 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_templated_selector.py
--rw-r--r--   0        0        0      697 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_type.py
--rw-r--r--   0        0        0     6364 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/policy_update_request.py
--rw-r--r--   0        0        0      829 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/relative_to_date_time.py
--rw-r--r--   0        0        0     3866 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/remove_from_policy_collection_request.py
--rw-r--r--   0        0        0     4251 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/request_details.py
--rw-r--r--   0        0        0     3119 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/requested_action_key.py
--rw-r--r--   0        0        0     3222 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/resource_details.py
--rw-r--r--   0        0        0     4268 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4268 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_policy_collection_response.py
--rw-r--r--   0        0        0     4147 2024-04-10 11:19:18.349232 finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_policy_response.py
--rw-r--r--   0        0        0     4244 2024-04-10 11:19:18.350232 finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_policy_template_response.py
--rw-r--r--   0        0        0     4172 2024-04-10 11:19:18.350232 finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_user_role_response.py
--rw-r--r--   0        0        0     3486 2024-04-10 11:19:18.350232 finbourne_access_sdk-2.1.3/finbourne_access/models/role_creation_request.py
--rw-r--r--   0        0        0     2849 2024-04-10 11:19:18.350232 finbourne_access_sdk-2.1.3/finbourne_access/models/role_id.py
--rw-r--r--   0        0        0     3211 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/role_resource_request.py
--rw-r--r--   0        0        0     4782 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/role_response.py
--rw-r--r--   0        0        0     3024 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/role_update_request.py
--rw-r--r--   0        0        0     4283 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/selector_definition.py
--rw-r--r--   0        0        0     3123 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/template_metadata.py
--rw-r--r--   0        0        0     3415 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/template_selection.py
--rw-r--r--   0        0        0     1071 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/text_operator.py
--rw-r--r--   0        0        0     2816 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/user_role_creation_request.py
--rw-r--r--   0        0        0     3274 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/user_role_response.py
--rw-r--r--   0        0        0     2262 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/user_role_update_request.py
--rw-r--r--   0        0        0     2147 2024-04-10 11:19:18.351232 finbourne_access_sdk-2.1.3/finbourne_access/models/when_spec.py
--rw-r--r--   0        0        0        0 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/py.typed
--rw-r--r--   0        0        0    10171 2024-04-10 11:19:18.353232 finbourne_access_sdk-2.1.3/finbourne_access/rest.py
--rw-r--r--   0        0        0      889 2024-04-10 11:19:18.364232 finbourne_access_sdk-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    18861 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    17778 2024-04-11 10:45:52.003212 finbourne_access_sdk-2.1.4/README.md
+-rw-r--r--   0        0        0    10462 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api/__init__.py
+-rw-r--r--   0        0        0     7551 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api/application_metadata_api.py
+-rw-r--r--   0        0        0   160687 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api/policies_api.py
+-rw-r--r--   0        0        0    55454 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api/policy_templates_api.py
+-rw-r--r--   0        0        0    68286 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api/roles_api.py
+-rw-r--r--   0        0        0    76101 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api/user_roles_api.py
+-rw-r--r--   0        0        0    30808 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/api_response.py
+-rw-r--r--   0        0        0    14461 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/configuration.py
+-rw-r--r--   0        0        0     5348 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/exceptions.py
+-rw-r--r--   0        0        0      593 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/__init__.py
+-rw-r--r--   0        0        0    30677 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/api_client.py
+-rw-r--r--   0        0        0     9882 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8107 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6804 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12709 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/rest.py
+-rw-r--r--   0        0        0    11575 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3888 2024-04-11 10:45:51.998212 finbourne_access_sdk-2.1.4/finbourne_access/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     8919 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/__init__.py
+-rw-r--r--   0        0        0     3918 2024-04-11 10:45:51.992212 finbourne_access_sdk-2.1.4/finbourne_access/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4861 2024-04-11 10:45:51.992212 finbourne_access_sdk-2.1.4/finbourne_access/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2079 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/action_id.py
+-rw-r--r--   0        0        0     2705 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/add_policy_collection_to_role_request.py
+-rw-r--r--   0        0        0     2461 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/add_policy_to_role_request.py
+-rw-r--r--   0        0        0     3823 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/add_to_policy_collection_request.py
+-rw-r--r--   0        0        0     2563 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/as_at_predicate_contract.py
+-rw-r--r--   0        0        0     2488 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/as_at_range_for_spec.py
+-rw-r--r--   0        0        0     2466 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/as_at_relative.py
+-rw-r--r--   0        0        0     6888 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/attached_policy_definition_response.py
+-rw-r--r--   0        0        0     1096 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/date_quality.py
+-rw-r--r--   0        0        0      781 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/date_unit.py
+-rw-r--r--   0        0        0     1971 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/effective_date_has_quality.py
+-rw-r--r--   0        0        0     2538 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/effective_date_relative.py
+-rw-r--r--   0        0        0     2148 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/effective_range.py
+-rw-r--r--   0        0        0     2387 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/entitlement_metadata.py
+-rw-r--r--   0        0        0     2625 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/evaluation_request.py
+-rw-r--r--   0        0        0     2473 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/evaluation_response.py
+-rw-r--r--   0        0        0      766 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/evaluation_result.py
+-rw-r--r--   0        0        0     4459 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/for_spec.py
+-rw-r--r--   0        0        0     3649 2024-04-11 10:45:51.993213 finbourne_access_sdk-2.1.4/finbourne_access/models/generate_policy_from_template_request.py
+-rw-r--r--   0        0        0     3731 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/generated_policy_components.py
+-rw-r--r--   0        0        0      654 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/grant.py
+-rw-r--r--   0        0        0     2867 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/how_spec.py
+-rw-r--r--   0        0        0     3191 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3116 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     4383 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/if_expression.py
+-rw-r--r--   0        0        0     2435 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/if_feature_chain_expression.py
+-rw-r--r--   0        0        0     3651 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/if_identity_claim_expression.py
+-rw-r--r--   0        0        0     2325 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/if_identity_scope_expression.py
+-rw-r--r--   0        0        0     2496 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/if_request_header_expression.py
+-rw-r--r--   0        0        0     2419 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/key_value_pair_of_string_to_string.py
+-rw-r--r--   0        0        0     2271 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/link.py
+-rw-r--r--   0        0        0     3866 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4702 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3115 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/match_all_selector_definition.py
+-rw-r--r--   0        0        0     2448 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/metadata_expression.py
+-rw-r--r--   0        0        0     3747 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/metadata_selector_definition.py
+-rw-r--r--   0        0        0     2048 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/non_transitive_supervisor_role_resource.py
+-rw-r--r--   0        0        0      847 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/operator.py
+-rw-r--r--   0        0        0      995 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/point_in_time_specification.py
+-rw-r--r--   0        0        0     6049 2024-04-11 10:45:51.994212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_creation_request.py
+-rw-r--r--   0        0        0     2945 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_id.py
+-rw-r--r--   0        0        0     5205 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_response.py
+-rw-r--r--   0        0        0     5467 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_update_request.py
+-rw-r--r--   0        0        0     6884 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_creation_request.py
+-rw-r--r--   0        0        0     2865 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_id.py
+-rw-r--r--   0        0        0     3546 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_id_role_resource.py
+-rw-r--r--   0        0        0     7551 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_response.py
+-rw-r--r--   0        0        0     4492 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_selector_definition.py
+-rw-r--r--   0        0        0     3686 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_template_creation_request.py
+-rw-r--r--   0        0        0     5276 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_template_response.py
+-rw-r--r--   0        0        0     3153 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_template_update_request.py
+-rw-r--r--   0        0        0     2647 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_templated_selector.py
+-rw-r--r--   0        0        0      697 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_type.py
+-rw-r--r--   0        0        0     6364 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/policy_update_request.py
+-rw-r--r--   0        0        0      829 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/relative_to_date_time.py
+-rw-r--r--   0        0        0     3866 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/remove_from_policy_collection_request.py
+-rw-r--r--   0        0        0     4251 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/request_details.py
+-rw-r--r--   0        0        0     3119 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/requested_action_key.py
+-rw-r--r--   0        0        0     3222 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/resource_details.py
+-rw-r--r--   0        0        0     4268 2024-04-11 10:45:51.995212 finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4268 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_policy_collection_response.py
+-rw-r--r--   0        0        0     4147 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_policy_response.py
+-rw-r--r--   0        0        0     4244 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_policy_template_response.py
+-rw-r--r--   0        0        0     4172 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_user_role_response.py
+-rw-r--r--   0        0        0     3486 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/role_creation_request.py
+-rw-r--r--   0        0        0     2849 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/role_id.py
+-rw-r--r--   0        0        0     3211 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/role_resource_request.py
+-rw-r--r--   0        0        0     4782 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/role_response.py
+-rw-r--r--   0        0        0     3024 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/role_update_request.py
+-rw-r--r--   0        0        0     4283 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/selector_definition.py
+-rw-r--r--   0        0        0     3123 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/template_metadata.py
+-rw-r--r--   0        0        0     3415 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/template_selection.py
+-rw-r--r--   0        0        0     1071 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/text_operator.py
+-rw-r--r--   0        0        0     2816 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/user_role_creation_request.py
+-rw-r--r--   0        0        0     3274 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/user_role_response.py
+-rw-r--r--   0        0        0     2262 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/user_role_update_request.py
+-rw-r--r--   0        0        0     2147 2024-04-11 10:45:51.996212 finbourne_access_sdk-2.1.4/finbourne_access/models/when_spec.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/py.typed
+-rw-r--r--   0        0        0    10171 2024-04-11 10:45:51.997213 finbourne_access_sdk-2.1.4/finbourne_access/rest.py
+-rw-r--r--   0        0        0      889 2024-04-11 10:45:52.003212 finbourne_access_sdk-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    18861 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.1.4/PKG-INFO
```

### Comparing `finbourne_access_sdk-2.1.3/README.md` & `finbourne_access_sdk-2.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3768
-- Package version: 2.1.3
+- API version: 0.0.3769
+- Package version: 2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/__init__.py` & `finbourne_access_sdk-2.1.4/finbourne_access/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api/application_metadata_api.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api/policies_api.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api/policy_templates_api.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api/policy_templates_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api/roles_api.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api/user_roles_api.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api/user_roles_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api_client.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/api_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/configuration.py` & `finbourne_access_sdk-2.1.4/finbourne_access/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_access-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.3768\n"\
+               "Version of the API: 0.0.3769\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/exceptions.py` & `finbourne_access_sdk-2.1.4/finbourne_access/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/__init__.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/api_client.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/api_client_factory.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/api_configuration.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/configuration_loaders.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/proxy_config.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/refreshing_token.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/rest.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/retry.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/socket_keep_alive.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/extensions/tcp_keep_alive_connector.py` & `finbourne_access_sdk-2.1.4/finbourne_access/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/__init__.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/access_controlled_action.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/access_controlled_resource.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/action_id.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/add_policy_collection_to_role_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/add_policy_collection_to_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/add_policy_to_role_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/add_policy_to_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/add_to_policy_collection_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/add_to_policy_collection_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/as_at_predicate_contract.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/as_at_predicate_contract.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/as_at_range_for_spec.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/as_at_range_for_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/as_at_relative.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/as_at_relative.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/attached_policy_definition_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/attached_policy_definition_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/date_quality.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/date_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/date_unit.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/date_unit.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/effective_date_has_quality.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/effective_date_has_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/effective_date_relative.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/effective_date_relative.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/effective_range.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/effective_range.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/entitlement_metadata.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/entitlement_metadata.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/evaluation_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/evaluation_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/evaluation_result.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/for_spec.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/for_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/generate_policy_from_template_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/generate_policy_from_template_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/generated_policy_components.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/generated_policy_components.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/grant.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/grant.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/how_spec.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/how_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/id_selector_definition.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/identifier_part_schema.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/if_expression.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/if_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/if_feature_chain_expression.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/if_feature_chain_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/if_identity_claim_expression.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/if_identity_claim_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/if_identity_scope_expression.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/if_identity_scope_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/if_request_header_expression.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/if_request_header_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/key_value_pair_of_string_to_string.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/key_value_pair_of_string_to_string.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/link.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/lusid_problem_details.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/lusid_validation_problem_details.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/match_all_selector_definition.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/match_all_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/metadata_expression.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/metadata_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/metadata_selector_definition.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/metadata_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/non_transitive_supervisor_role_resource.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/non_transitive_supervisor_role_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/operator.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/point_in_time_specification.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/point_in_time_specification.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_creation_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_id.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_collection_update_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_collection_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_creation_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_id.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_id_role_resource.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_id_role_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_selector_definition.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_template_creation_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_template_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_template_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_template_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_template_update_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_template_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_templated_selector.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_templated_selector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_type.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_type.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/policy_update_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/policy_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/relative_to_date_time.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/relative_to_date_time.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/remove_from_policy_collection_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/remove_from_policy_collection_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/request_details.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/request_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/requested_action_key.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/requested_action_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/resource_details.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/resource_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_access_controlled_resource.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_policy_collection_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_policy_collection_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_policy_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_policy_template_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_policy_template_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/resource_list_of_user_role_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/resource_list_of_user_role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/role_creation_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/role_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/role_id.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/role_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/role_resource_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/role_resource_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/role_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/role_update_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/role_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/selector_definition.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/template_metadata.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/template_metadata.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/template_selection.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/template_selection.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/text_operator.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/text_operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/user_role_creation_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/user_role_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/user_role_response.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/user_role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/user_role_update_request.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/user_role_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/models/when_spec.py` & `finbourne_access_sdk-2.1.4/finbourne_access/models/when_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/finbourne_access/rest.py` & `finbourne_access_sdk-2.1.4/finbourne_access/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.3/pyproject.toml` & `finbourne_access_sdk-2.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-access-sdk"
-version = "2.1.3"
+version = "2.1.4"
 description = "FINBOURNE Access Management API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-access-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Access Management API", "finbourne-access-sdk"]
 packages = [
```

### Comparing `finbourne_access_sdk-2.1.3/PKG-INFO` & `finbourne_access_sdk-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-access-sdk
-Version: 2.1.3
+Version: 2.1.4
 Summary: FINBOURNE Access Management API
 Home-page: https://github.com/finbourne/finbourne-access-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Access Management API,finbourne-access-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3768
-- Package version: 2.1.3
+- API version: 0.0.3769
+- Package version: 2.1.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

