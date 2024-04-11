# Comparing `tmp/finbourne_identity_sdk-2.0.9.tar.gz` & `tmp/finbourne_identity_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_identity_sdk-2.0.9.tar", max compression
+gzip compressed data, was "finbourne_identity_sdk-2.1.1.tar", max compression
```

## Comparing `finbourne_identity_sdk-2.0.9.tar` & `finbourne_identity_sdk-2.1.1.tar`

### file list

```diff
@@ -1,73 +1,78 @@
--rw-r--r--   0        0        0    13179 2023-12-15 17:30:01.092972 finbourne_identity_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     4611 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/__init__.py
--rw-r--r--   0        0        0      662 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/__init__.py
--rw-r--r--   0        0        0     7555 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/application_metadata_api.py
--rw-r--r--   0        0        0    36608 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/applications_api.py
--rw-r--r--   0        0        0    44723 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/authentication_api.py
--rw-r--r--   0        0        0    15650 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/identity_provider_api.py
--rw-r--r--   0        0        0    14849 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/me_api.py
--rw-r--r--   0        0        0    21844 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/personal_authentication_tokens_api.py
--rw-r--r--   0        0        0    57676 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/roles_api.py
--rw-r--r--   0        0        0     6894 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/tokens_api.py
--rw-r--r--   0        0        0    95605 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/users_api.py
--rw-r--r--   0        0        0    30571 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api_client.py
--rw-r--r--   0        0        0      852 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api_response.py
--rw-r--r--   0        0        0    14468 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/configuration.py
--rw-r--r--   0        0        0     5347 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/exceptions.py
--rw-r--r--   0        0        0      302 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/__init__.py
--rw-r--r--   0        0        0    30528 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client.py
--rw-r--r--   0        0        0     9684 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8028 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_configuration.py
--rw-r--r--   0        0        0     6884 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/rest.py
--rw-r--r--   0        0        0    11577 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/retry.py
--rw-r--r--   0        0        0     1653 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2023-12-15 17:30:01.090972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3436 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/__init__.py
--rw-r--r--   0        0        0     3920 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_action.py
--rw-r--r--   0        0        0     4863 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2075 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/action_id.py
--rw-r--r--   0        0        0     2433 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/add_scim_response.py
--rw-r--r--   0        0        0     3346 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/api_key.py
--rw-r--r--   0        0        0     5236 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/authentication_information.py
--rw-r--r--   0        0        0     2781 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_api_key.py
--rw-r--r--   0        0        0     4486 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_application_request.py
--rw-r--r--   0        0        0     3115 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_role_request.py
--rw-r--r--   0        0        0     5258 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_user_request.py
--rw-r--r--   0        0        0     3523 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/created_api_key.py
--rw-r--r--   0        0        0     3518 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/current_user_response.py
--rw-r--r--   0        0        0     2773 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/error_detail.py
--rw-r--r--   0        0        0     3189 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/id_selector_definition.py
--rw-r--r--   0        0        0     3114 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2267 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/link.py
--rw-r--r--   0        0        0     4741 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/list_users_response.py
--rw-r--r--   0        0        0     3862 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4698 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2987 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/o_auth_application.py
--rw-r--r--   0        0        0     2209 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy.py
--rw-r--r--   0        0        0     2276 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_age.py
--rw-r--r--   0        0        0     2553 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_complexity.py
--rw-r--r--   0        0        0     3139 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_conditions.py
--rw-r--r--   0        0        0     2058 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_lockout.py
--rw-r--r--   0        0        0     4268 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     1919 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_id.py
--rw-r--r--   0        0        0     2986 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_response.py
--rw-r--r--   0        0        0     1909 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password.py
--rw-r--r--   0        0        0     2767 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password_response.py
--rw-r--r--   0        0        0     1990 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry.py
--rw-r--r--   0        0        0     2385 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry_with_role.py
--rw-r--r--   0        0        0     3920 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_request.py
--rw-r--r--   0        0        0     5254 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_response.py
--rw-r--r--   0        0        0     3183 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_role.py
--rw-r--r--   0        0        0     2678 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_roles_response.py
--rw-r--r--   0        0        0     1930 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/temporary_password.py
--rw-r--r--   0        0        0     2554 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_role_request.py
--rw-r--r--   0        0        0     4749 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_user_request.py
--rw-r--r--   0        0        0     5145 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_response.py
--rw-r--r--   0        0        0     4917 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_summary.py
--rw-r--r--   0        0        0        0 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/py.typed
--rw-r--r--   0        0        0    10041 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/rest.py
--rw-r--r--   0        0        0      898 2023-12-15 17:30:01.092972 finbourne_identity_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    14269 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    16101 2024-04-10 10:42:11.131018 finbourne_identity_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0     7317 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/__init__.py
+-rw-r--r--   0        0        0     7558 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/application_metadata_api.py
+-rw-r--r--   0        0        0    36614 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/applications_api.py
+-rw-r--r--   0        0        0    53741 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/authentication_api.py
+-rw-r--r--   0        0        0    15656 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/identity_provider_api.py
+-rw-r--r--   0        0        0    14855 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/me_api.py
+-rw-r--r--   0        0        0    21850 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/personal_authentication_tokens_api.py
+-rw-r--r--   0        0        0    57682 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/roles_api.py
+-rw-r--r--   0        0        0     6897 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/tokens_api.py
+-rw-r--r--   0        0        0    95611 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api/users_api.py
+-rw-r--r--   0        0        0    30821 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/api_response.py
+-rw-r--r--   0        0        0    14468 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/configuration.py
+-rw-r--r--   0        0        0     5347 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/__init__.py
+-rw-r--r--   0        0        0    30692 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/api_client.py
+-rw-r--r--   0        0        0     9902 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-04-10 10:42:11.128018 finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     5374 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4866 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2078 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/action_id.py
+-rw-r--r--   0        0        0     2436 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/add_scim_response.py
+-rw-r--r--   0        0        0     3349 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/api_key.py
+-rw-r--r--   0        0        0     5239 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/authentication_information.py
+-rw-r--r--   0        0        0     2784 2024-04-10 10:42:11.123018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_api_key.py
+-rw-r--r--   0        0        0     4489 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_application_request.py
+-rw-r--r--   0        0        0     3118 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_role_request.py
+-rw-r--r--   0        0        0     5261 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_user_request.py
+-rw-r--r--   0        0        0     3526 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/created_api_key.py
+-rw-r--r--   0        0        0     3521 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/current_user_response.py
+-rw-r--r--   0        0        0     2776 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/error_detail.py
+-rw-r--r--   0        0        0     3192 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3117 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2270 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/link.py
+-rw-r--r--   0        0        0     4744 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/list_users_response.py
+-rw-r--r--   0        0        0     3865 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4701 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2990 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/o_auth_application.py
+-rw-r--r--   0        0        0     2302 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response.py
+-rw-r--r--   0        0        0     2311 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_age.py
+-rw-r--r--   0        0        0     2577 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_complexity.py
+-rw-r--r--   0        0        0     3282 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_conditions.py
+-rw-r--r--   0        0        0     2104 2024-04-10 10:42:11.124018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_lockout.py
+-rw-r--r--   0        0        0     4271 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     1922 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/role_id.py
+-rw-r--r--   0        0        0     3430 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/role_response.py
+-rw-r--r--   0        0        0     1912 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/set_password.py
+-rw-r--r--   0        0        0     2770 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/set_password_response.py
+-rw-r--r--   0        0        0     1993 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_expiry.py
+-rw-r--r--   0        0        0     2388 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_expiry_with_role.py
+-rw-r--r--   0        0        0     3923 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_request.py
+-rw-r--r--   0        0        0     5257 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_response.py
+-rw-r--r--   0        0        0     3186 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_role.py
+-rw-r--r--   0        0        0     2681 2024-04-10 10:42:11.125018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_roles_response.py
+-rw-r--r--   0        0        0     1933 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/temporary_password.py
+-rw-r--r--   0        0        0     2363 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_password_policy_request.py
+-rw-r--r--   0        0        0     2437 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_password_policy_request_age.py
+-rw-r--r--   0        0        0     2638 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_password_policy_request_complexity.py
+-rw-r--r--   0        0        0     3380 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_password_policy_request_conditions.py
+-rw-r--r--   0        0        0     2188 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_password_policy_request_lockout.py
+-rw-r--r--   0        0        0     2557 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_role_request.py
+-rw-r--r--   0        0        0     4752 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_user_request.py
+-rw-r--r--   0        0        0     5148 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/user_response.py
+-rw-r--r--   0        0        0     4920 2024-04-10 10:42:11.126018 finbourne_identity_sdk-2.1.1/finbourne_identity/models/user_summary.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/py.typed
+-rw-r--r--   0        0        0    10172 2024-04-10 10:42:11.127018 finbourne_identity_sdk-2.1.1/finbourne_identity/rest.py
+-rw-r--r--   0        0        0      897 2024-04-10 10:42:11.131018 finbourne_identity_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17190 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.1.1/PKG-INFO
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/application_metadata_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from finbourne_identity.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 from finbourne_identity.api_client import ApiClient
 from finbourne_identity.api_response import ApiResponse
 from finbourne_identity.exceptions import (  # noqa: F401
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/applications_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/applications_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool, constr, validator
+from pydantic.v1 import Field, StrictBool, constr, validator
 
 from typing import List, Optional
 
 from finbourne_identity.models.create_application_request import CreateApplicationRequest
 from finbourne_identity.models.o_auth_application import OAuthApplication
 
 from finbourne_identity.api_client import ApiClient
@@ -661,15 +661,15 @@
 
     @overload
     def rotate_application_secrets(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the application")], async_req: Optional[bool]=True, **kwargs) -> OAuthApplication:  # noqa: E501
         ...
 
     @validate_arguments
     def rotate_application_secrets(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the application")], async_req: Optional[bool]=None, **kwargs) -> Union[OAuthApplication, Awaitable[OAuthApplication]]:  # noqa: E501
-        """[EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets  # noqa: E501
+        """[EARLY ACCESS] RotateApplicationSecrets: Rotate Application Secrets  # noqa: E501
 
         Rotate the secrets for the specified application  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.rotate_application_secrets(id, async_req=True)
         >>> result = thread.get()
@@ -693,15 +693,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.rotate_application_secrets_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
     def rotate_application_secrets_with_http_info(self, id : Annotated[constr(strict=True, max_length=64, min_length=1), Field(..., description="The unique identifier for the application")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets  # noqa: E501
+        """[EARLY ACCESS] RotateApplicationSecrets: Rotate Application Secrets  # noqa: E501
 
         Rotate the secrets for the specified application  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.rotate_application_secrets_with_http_info(id, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/authentication_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/authentication_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, constr, validator
+from pydantic.v1 import Field, constr, validator
 
 from typing import List, Optional
 
 from finbourne_identity.models.authentication_information import AuthenticationInformation
-from finbourne_identity.models.password_policy import PasswordPolicy
+from finbourne_identity.models.password_policy_response import PasswordPolicyResponse
 from finbourne_identity.models.support_access_request import SupportAccessRequest
 from finbourne_identity.models.support_access_response import SupportAccessResponse
 from finbourne_identity.models.support_roles_response import SupportRolesResponse
+from finbourne_identity.models.update_password_policy_request import UpdatePasswordPolicyRequest
 
 from finbourne_identity.api_client import ApiClient
 from finbourne_identity.api_response import ApiResponse
 from finbourne_identity.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -191,24 +192,24 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @overload
-    async def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], **kwargs) -> PasswordPolicy:  # noqa: E501
+    async def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], **kwargs) -> PasswordPolicyResponse:  # noqa: E501
         ...
 
     @overload
-    def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], async_req: Optional[bool]=True, **kwargs) -> PasswordPolicy:  # noqa: E501
+    def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], async_req: Optional[bool]=True, **kwargs) -> PasswordPolicyResponse:  # noqa: E501
         ...
 
     @validate_arguments
-    def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], async_req: Optional[bool]=None, **kwargs) -> Union[PasswordPolicy, Awaitable[PasswordPolicy]]:  # noqa: E501
-        """[EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type  # noqa: E501
+    def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], async_req: Optional[bool]=None, **kwargs) -> Union[PasswordPolicyResponse, Awaitable[PasswordPolicyResponse]]:  # noqa: E501
+        """[EXPERIMENTAL] GetPasswordPolicy: Gets password policy for a user type  # noqa: E501
 
         Get the password policy for a given user type  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_password_policy(user_type, async_req=True)
         >>> result = thread.get()
@@ -220,27 +221,27 @@
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PasswordPolicy
+        :rtype: PasswordPolicyResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the get_password_policy_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_password_policy_with_http_info(user_type, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_password_policy_with_http_info(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type  # noqa: E501
+        """[EXPERIMENTAL] GetPasswordPolicy: Gets password policy for a user type  # noqa: E501
 
         Get the password policy for a given user type  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_password_policy_with_http_info(user_type, async_req=True)
         >>> result = thread.get()
@@ -265,15 +266,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PasswordPolicy, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PasswordPolicyResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'user_type'
         ]
@@ -320,15 +321,15 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['oauth2']  # noqa: E501
 
         _response_types_map = {
-            '200': "PasswordPolicy",
+            '200': "PasswordPolicyResponse",
             '400': "LusidValidationProblemDetails",
         }
 
         return self.api_client.call_api(
             '/api/authentication/password-policy/{userType}', 'GET',
             _path_params,
             _query_params,
@@ -940,14 +941,180 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @overload
+    async def update_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], update_password_policy_request : Annotated[Optional[UpdatePasswordPolicyRequest], Field(description="The password policy for the given user type")] = None, **kwargs) -> PasswordPolicyResponse:  # noqa: E501
+        ...
+
+    @overload
+    def update_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], update_password_policy_request : Annotated[Optional[UpdatePasswordPolicyRequest], Field(description="The password policy for the given user type")] = None, async_req: Optional[bool]=True, **kwargs) -> PasswordPolicyResponse:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def update_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], update_password_policy_request : Annotated[Optional[UpdatePasswordPolicyRequest], Field(description="The password policy for the given user type")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PasswordPolicyResponse, Awaitable[PasswordPolicyResponse]]:  # noqa: E501
+        """[EXPERIMENTAL] UpdatePasswordPolicy: Updates password policy for a user type  # noqa: E501
+
+        Update the password policy for a given user type  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_password_policy(user_type, update_password_policy_request, async_req=True)
+        >>> result = thread.get()
+
+        :param user_type: The type of user (should only be personal or service) (required)
+        :type user_type: str
+        :param update_password_policy_request: The password policy for the given user type
+        :type update_password_policy_request: UpdatePasswordPolicyRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: PasswordPolicyResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the update_password_policy_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        if async_req is not None:
+            kwargs['async_req'] = async_req
+        return self.update_password_policy_with_http_info(user_type, update_password_policy_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def update_password_policy_with_http_info(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], update_password_policy_request : Annotated[Optional[UpdatePasswordPolicyRequest], Field(description="The password policy for the given user type")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+        """[EXPERIMENTAL] UpdatePasswordPolicy: Updates password policy for a user type  # noqa: E501
+
+        Update the password policy for a given user type  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_password_policy_with_http_info(user_type, update_password_policy_request, async_req=True)
+        >>> result = thread.get()
+
+        :param user_type: The type of user (should only be personal or service) (required)
+        :type user_type: str
+        :param update_password_policy_request: The password policy for the given user type
+        :type update_password_policy_request: UpdatePasswordPolicyRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(PasswordPolicyResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_type',
+            'update_password_policy_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_password_policy" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_type']:
+            _path_params['userType'] = _params['user_type']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['update_password_policy_request'] is not None:
+            _body_params = _params['update_password_policy_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['oauth2']  # noqa: E501
+
+        _response_types_map = {
+            '200': "PasswordPolicyResponse",
+            '400': "LusidValidationProblemDetails",
+        }
+
+        return self.api_client.call_api(
+            '/api/authentication/password-policy/{userType}', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/identity_provider_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/identity_provider_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field, StrictStr
+from pydantic.v1 import Field, StrictStr
 
 from typing import Optional
 
 from finbourne_identity.models.add_scim_response import AddScimResponse
 
 from finbourne_identity.api_client import ApiClient
 from finbourne_identity.api_response import ApiResponse
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/me_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/me_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field
+from pydantic.v1 import Field
 
 from finbourne_identity.models.current_user_response import CurrentUserResponse
 from finbourne_identity.models.set_password import SetPassword
 from finbourne_identity.models.set_password_response import SetPasswordResponse
 
 from finbourne_identity.api_client import ApiClient
 from finbourne_identity.api_response import ApiResponse
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/personal_authentication_tokens_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/personal_authentication_tokens_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, constr, validator
+from pydantic.v1 import Field, constr, validator
 
 from typing import List
 
 from finbourne_identity.models.api_key import ApiKey
 from finbourne_identity.models.create_api_key import CreateApiKey
 from finbourne_identity.models.created_api_key import CreatedApiKey
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/roles_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/roles_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, constr, validator
+from pydantic.v1 import Field, constr, validator
 
 from typing import List, Optional
 
 from finbourne_identity.models.create_role_request import CreateRoleRequest
 from finbourne_identity.models.role_response import RoleResponse
 from finbourne_identity.models.update_role_request import UpdateRoleRequest
 from finbourne_identity.models.user_response import UserResponse
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/tokens_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/tokens_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 
 from finbourne_identity.api_client import ApiClient
 from finbourne_identity.api_response import ApiResponse
 from finbourne_identity.exceptions import (  # noqa: F401
     ApiTypeError,
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api/users_api.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 """
 
 
 import re  # noqa: F401
 import io
 import warnings
 
-from pydantic import validate_arguments, ValidationError
+from pydantic.v1 import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
-from pydantic import Field, StrictBool, StrictStr, conlist, constr, validator
+from pydantic.v1 import Field, StrictBool, StrictStr, conlist, constr, validator
 
 from typing import List, Optional
 
 from finbourne_identity.models.create_user_request import CreateUserRequest
 from finbourne_identity.models.list_users_response import ListUsersResponse
 from finbourne_identity.models.temporary_password import TemporaryPassword
 from finbourne_identity.models.update_user_request import UpdateUserRequest
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api_client.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
+            # if returning http_data_only then we need to deserialise response.
+            _preload_content = True if _return_http_data_only else _preload_content
             # perform request and return response
             response_data = await self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
@@ -256,16 +258,16 @@
               return_data = None
 
         if _return_http_data_only:
             return return_data
         else:
             return ApiResponse(status_code = response_data.status,
                            data = return_data,
-                           headers = response_data.getheaders(),
-                           raw_data = response_data.data)
+                           headers = response_data.getheaders() if _preload_content else response_data.headers,
+                           raw_data = response_data.data if _preload_content else response_data)
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/api_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/configuration.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_identity-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.2725\n"\
+               "Version of the API: 0.0.2850\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/exceptions.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,16 @@
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
             url_query = self.parameters_to_url_query(query_params,
                                                      collection_formats)
             url += "?" + url_query
 
         try:
+            # if returning http_data_only then we need to deserialise response.
+            _preload_content = True if _return_http_data_only else _preload_content
             # perform request and return response
             response_data = self.request(
                 method, url,
                 query_params=query_params,
                 headers=header_params,
                 post_params=post_params, body=body,
                 _preload_content=_preload_content,
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client_factory.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/api_client_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,38 +180,43 @@
         An aiohttp.ClientSession, pass this to re-use 
         connections across different ApiFactories,
         by default None
         trace_configs: Optional[List[TraceConfig]], optional
         A list of aiohttp TraceConfigs, used to set up request tracing.
         by default None
         """
+        is_owner = True
         api_config = get_api_configuration(config_loaders=config_loaders)
         api_client_config = api_config.build_api_client_config(
             tcp_keep_alive=tcp_keep_alive,
             socket_options=socket_options,
             id_provider_response_handler=id_provider_response_handler
         )
         self.__api_client = ApiClient(
             configuration=api_client_config,
         )
         rc = self.__api_client.rest_client
         try:
             if client_session is not None:
                 connector = client_session.connector
+                is_owner = False
                 # by default take explicitly passed trace_config param
                 # otherwise copy from session.
                 trace_configs = trace_configs or client_session.trace_configs
             else:
                 connector = rc.pool_manager.connector
             if tcp_keep_alive:
                 connector = TcpKeepAliveConnector(connector=connector, socket_options=socket_options)
+            # dereference connector so existing session closes correctly
+            rc.pool_manager._connector = None
             rc.pool_manager = ClientSession(
                 connector=connector,
                 trust_env=True,
-                trace_configs=trace_configs
+                trace_configs=trace_configs,
+                connector_owner=is_owner
             )
         except AttributeError:
             logger.exception("client_session must be an aiohttp.ClientSession"
                              " object with an initialised TCP Connector")
         rest_client_wrapper = RetryingRestWrapperAsync
         wrapped_rest_client = rest_client_wrapper(rc)
         self.__api_client.rest_client = wrapped_rest_client
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_configuration.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/api_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import logging
 from typing import Optional, Union, Tuple, Any, Callable
 from finbourne_identity.configuration import Configuration
 from finbourne_identity.extensions.refreshing_token import RefreshingToken
 from finbourne_identity.extensions.socket_keep_alive import keep_alive_socket_options
+from finbourne_identity.extensions.proxy_config import ProxyConfig
 from requests import Response
 logger = logging.getLogger(__name__)
 
 
 class ApiConfiguration:
     def __init__(
         self,
@@ -15,15 +16,15 @@
         api_url=None,
         username=None,
         password=None,
         client_id=None,
         client_secret=None,
         app_name=None,
         certificate_filename=None,
-        proxy_config=None,
+        proxy_config:Optional[ProxyConfig]=None,
         access_token=None,
     ):
         """
         The configuration required to access LUSID, read more at https://support.finbourne.com/getting-started-with-apis-sdks
 
         :param str token_url: The token URL of the identity provider
         :param str api_url: The API URL for the LUSID client
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/configuration_loaders.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/configuration_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,15 @@
             if value is not None
         }
         config.update(loaded_config)
     proxy_address = config.pop("proxy_address", None)
     proxy_username = config.pop("proxy_username", None)
     proxy_password = config.pop("proxy_password", None)
     # If the proxy address is missing ensure that no proxy is used in the ApiConfiguration
-    if all(
-        (item is not None for item in (proxy_address, proxy_password, proxy_username))
-    ):
+    if proxy_address is not None:
         config["proxy_config"] = ProxyConfig(
             address=proxy_address, username=proxy_username, password=proxy_password
         )
     else:
         config["proxy_config"] = None
     # Create and return the ApiConfiguration
     return ApiConfiguration(**config)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/proxy_config.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/proxy_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib3 import make_headers
-from typing import Any
+from typing import Dict
 
 
 class ProxyConfig:
     """
     This class is used to hold the proxy configuration details
     """
 
@@ -52,18 +52,21 @@
             index = self.address.index("://")
 
             proxy_url = f"{self.address[0:index + 3]}{self.username}:{self.password}@{self.address[index + 3:]}"
 
         return {"http": proxy_url, "https": proxy_url}
 
     @property
-    def headers(self) -> Any:
+    def headers(self) -> Dict[str, str]:
         """Return Proxy auth headers
 
         Returns
         -------
         Any
             Proxy auth headers
         """
-        return make_headers(
-            proxy_basic_auth=f"{self.__username}:{self.__password}"
-        )
+        if self.__username is not None and self.__password is not None:
+            return make_headers(
+                proxy_basic_auth=f"{self.__username}:{self.__password}"
+            )
+        else:
+            return {}
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/refreshing_token.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/rest.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/retry.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/socket_keep_alive.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/tcp_keep_alive_connector.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_action.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr
+from pydantic.v1 import BaseModel, Field, conlist, constr
 from finbourne_identity.models.action_id import ActionId
 from finbourne_identity.models.id_selector_definition import IdSelectorDefinition
 from finbourne_identity.models.link import Link
 
 class AccessControlledAction(BaseModel):
     """
     AccessControlledAction
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_resource.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_identity.models.access_controlled_action import AccessControlledAction
 from finbourne_identity.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_identity.models.link import Link
 
 class AccessControlledResource(BaseModel):
     """
     AccessControlledResource
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/action_id.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/action_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class ActionId(BaseModel):
     """
     ActionId
     """
     scope: constr(strict=True, max_length=100, min_length=3) = Field(...)
     activity: constr(strict=True, max_length=25, min_length=3) = Field(...)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/add_scim_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/add_scim_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class AddScimResponse(BaseModel):
     """
     AddScimResponse
     """
     base_url: Optional[StrictStr] = Field(None, alias="baseUrl")
     api_token: Optional[StrictStr] = Field(None, alias="apiToken")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/api_key.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/api_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class ApiKey(BaseModel):
     """
     The metadata of an API key  # noqa: E501
     """
     id: constr(strict=True, max_length=64, min_length=1) = Field(..., description="The unique Id of the API key")
     display_name: constr(strict=True, max_length=512, min_length=1) = Field(..., alias="displayName", description="The display name of the API key")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/authentication_information.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/authentication_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_identity.models.link import Link
 from finbourne_identity.models.support_access_expiry import SupportAccessExpiry
 from finbourne_identity.models.support_access_expiry_with_role import SupportAccessExpiryWithRole
 
 class AuthenticationInformation(BaseModel):
     """
     AuthenticationInformation
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_api_key.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class CreateApiKey(BaseModel):
     """
     Create an API key  # noqa: E501
     """
     display_name: constr(strict=True, max_length=512, min_length=1) = Field(..., alias="displayName", description="The display name for the API key")
     deactivation_date: Optional[datetime] = Field(None, alias="deactivationDate", description="The optional date at which the key should deactivate")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_application_request.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_application_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 
 class CreateApplicationRequest(BaseModel):
     """
     A request to create an application for authenticating the source of token requests  # noqa: E501
     """
     display_name: constr(strict=True, max_length=50, min_length=1) = Field(..., alias="displayName", description="The Display Name of the application")
     client_id: constr(strict=True, max_length=50, min_length=6) = Field(..., alias="clientId", description="The OpenID Connect ClientId of the application")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_role_request.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_role_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class CreateRoleRequest(BaseModel):
     """
     Specifies the information required to create a new role.  # noqa: E501
     """
     name: constr(strict=True, max_length=512, min_length=1) = Field(..., description="The role name, which must be unique within the system.")
     description: Optional[constr(strict=True, max_length=1024, min_length=0)] = Field(None, description="The description for this role")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_user_request.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/create_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, conlist, constr, validator
 from finbourne_identity.models.role_id import RoleId
 
 class CreateUserRequest(BaseModel):
     """
     Details necessary for creating a new user  # noqa: E501
     """
     first_name: constr(strict=True, max_length=50, min_length=1) = Field(..., alias="firstName", description="The first name of the user")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/created_api_key.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/created_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class CreatedApiKey(BaseModel):
     """
     A newly created API key  # noqa: E501
     """
     key: constr(strict=True, min_length=1) = Field(..., description="The API Key value")
     id: constr(strict=True, max_length=64, min_length=1) = Field(..., description="The unique Id of the API key")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/current_user_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/current_user_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_identity.models.link import Link
 
 class CurrentUserResponse(BaseModel):
     """
     CurrentUserResponse
     """
     id: constr(strict=True, min_length=1) = Field(..., description="The user's system supplied unique identifier")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/error_detail.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/error_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class ErrorDetail(BaseModel):
     """
     Provides details about an entity error that occured  # noqa: E501
     """
     id: Optional[StrictStr] = Field(None, description="Id of the entity this error relates to")
     type: Optional[StrictStr] = Field(None, description="Error type")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/id_selector_definition.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from finbourne_identity.models.action_id import ActionId
 
 class IdSelectorDefinition(BaseModel):
     """
     IdSelectorDefinition
     """
     identifier: Dict[str, StrictStr] = Field(...)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/identifier_part_schema.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt, conlist, constr
 from finbourne_identity.models.link import Link
 
 class IdentifierPartSchema(BaseModel):
     """
     IdentifierPartSchema
     """
     index: StrictInt = Field(...)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/link.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class Link(BaseModel):
     """
     Link
     """
     relation: StrictStr = Field(...)
     href: StrictStr = Field(...)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/list_users_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/list_users_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from finbourne_identity.models.error_detail import ErrorDetail
 from finbourne_identity.models.link import Link
 from finbourne_identity.models.user_summary import UserSummary
 
 class ListUsersResponse(BaseModel):
     """
     Users directory query response  # noqa: E501
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_problem_details.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/lusid_problem_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr
 
 class LusidProblemDetails(BaseModel):
     """
     LusidProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_validation_problem_details.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictInt, StrictStr, conlist, constr
 
 class LusidValidationProblemDetails(BaseModel):
     """
     LusidValidationProblemDetails
     """
     name: constr(strict=True, min_length=1) = Field(...)
     error_details: Optional[conlist(Dict[str, StrictStr])] = Field(None, alias="errorDetails")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/o_auth_application.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/o_auth_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, constr, validator
 
 class OAuthApplication(BaseModel):
     """
     OAuthApplication
     """
     id: constr(strict=True, min_length=1) = Field(...)
     type: constr(strict=True, min_length=1) = Field(...)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel
-from finbourne_identity.models.password_policy_conditions import PasswordPolicyConditions
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field
+from finbourne_identity.models.password_policy_response_conditions import PasswordPolicyResponseConditions
 
-class PasswordPolicy(BaseModel):
+class PasswordPolicyResponse(BaseModel):
     """
-    PasswordPolicy
+    PasswordPolicyResponse
     """
-    conditions: Optional[PasswordPolicyConditions] = None
+    conditions: PasswordPolicyResponseConditions = Field(...)
     __properties = ["conditions"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -39,35 +39,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PasswordPolicy:
-        """Create an instance of PasswordPolicy from a JSON string"""
+    def from_json(cls, json_str: str) -> PasswordPolicyResponse:
+        """Create an instance of PasswordPolicyResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of conditions
         if self.conditions:
             _dict['conditions'] = self.conditions.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PasswordPolicy:
-        """Create an instance of PasswordPolicy from a dict"""
+    def from_dict(cls, obj: dict) -> PasswordPolicyResponse:
+        """Create an instance of PasswordPolicyResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PasswordPolicy.parse_obj(obj)
+            return PasswordPolicyResponse.parse_obj(obj)
 
-        _obj = PasswordPolicy.parse_obj({
-            "conditions": PasswordPolicyConditions.from_dict(obj.get("conditions")) if obj.get("conditions") is not None else None
+        _obj = PasswordPolicyResponse.parse_obj({
+            "conditions": PasswordPolicyResponseConditions.from_dict(obj.get("conditions")) if obj.get("conditions") is not None else None
         })
         return _obj
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_age.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_age.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field, StrictInt
 
-class PasswordPolicyAge(BaseModel):
+class PasswordPolicyResponseAge(BaseModel):
     """
-    PasswordPolicyAge
+    PasswordPolicyResponseAge
     """
-    max_age_days: Optional[StrictInt] = Field(None, alias="maxAgeDays", description="The maximum age (in days) a password can be before expiring and needing to be changed")
-    history_count: Optional[StrictInt] = Field(None, alias="historyCount", description="The number of unique passwords that need to be used before a previous password is permitted again")
+    max_age_days: StrictInt = Field(..., alias="maxAgeDays", description="The maximum age (in days) a password can be before expiring and needing to be changed")
+    history_count: StrictInt = Field(..., alias="historyCount", description="The number of unique passwords that need to be used before a previous password is permitted again")
     __properties = ["maxAgeDays", "historyCount"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -39,33 +39,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PasswordPolicyAge:
-        """Create an instance of PasswordPolicyAge from a JSON string"""
+    def from_json(cls, json_str: str) -> PasswordPolicyResponseAge:
+        """Create an instance of PasswordPolicyResponseAge from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PasswordPolicyAge:
-        """Create an instance of PasswordPolicyAge from a dict"""
+    def from_dict(cls, obj: dict) -> PasswordPolicyResponseAge:
+        """Create an instance of PasswordPolicyResponseAge from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PasswordPolicyAge.parse_obj(obj)
+            return PasswordPolicyResponseAge.parse_obj(obj)
 
-        _obj = PasswordPolicyAge.parse_obj({
+        _obj = PasswordPolicyResponseAge.parse_obj({
             "max_age_days": obj.get("maxAgeDays"),
             "history_count": obj.get("historyCount")
         })
         return _obj
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_complexity.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_complexity.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictInt
 
-class PasswordPolicyComplexity(BaseModel):
+class PasswordPolicyResponseComplexity(BaseModel):
     """
-    PasswordPolicyComplexity
+    PasswordPolicyResponseComplexity
     """
-    min_length: Optional[StrictInt] = Field(None, alias="minLength", description="The minimum length for a password")
-    exclude_first_name: Optional[StrictBool] = Field(None, alias="excludeFirstName", description="Rule determining whether a user's first name should be permitted in their password")
-    exclude_last_name: Optional[StrictBool] = Field(None, alias="excludeLastName", description="Rule determining whether a user's last name should be permitted in their password")
+    min_length: StrictInt = Field(..., alias="minLength", description="The minimum length for a password")
+    exclude_first_name: StrictBool = Field(..., alias="excludeFirstName", description="Rule determining whether a user's first name should be permitted in their password")
+    exclude_last_name: StrictBool = Field(..., alias="excludeLastName", description="Rule determining whether a user's last name should be permitted in their password")
     __properties = ["minLength", "excludeFirstName", "excludeLastName"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -40,34 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PasswordPolicyComplexity:
-        """Create an instance of PasswordPolicyComplexity from a JSON string"""
+    def from_json(cls, json_str: str) -> PasswordPolicyResponseComplexity:
+        """Create an instance of PasswordPolicyResponseComplexity from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PasswordPolicyComplexity:
-        """Create an instance of PasswordPolicyComplexity from a dict"""
+    def from_dict(cls, obj: dict) -> PasswordPolicyResponseComplexity:
+        """Create an instance of PasswordPolicyResponseComplexity from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PasswordPolicyComplexity.parse_obj(obj)
+            return PasswordPolicyResponseComplexity.parse_obj(obj)
 
-        _obj = PasswordPolicyComplexity.parse_obj({
+        _obj = PasswordPolicyResponseComplexity.parse_obj({
             "min_length": obj.get("minLength"),
             "exclude_first_name": obj.get("excludeFirstName"),
             "exclude_last_name": obj.get("excludeLastName")
         })
         return _obj
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_conditions.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_conditions.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel
-from finbourne_identity.models.password_policy_age import PasswordPolicyAge
-from finbourne_identity.models.password_policy_complexity import PasswordPolicyComplexity
-from finbourne_identity.models.password_policy_lockout import PasswordPolicyLockout
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field
+from finbourne_identity.models.password_policy_response_age import PasswordPolicyResponseAge
+from finbourne_identity.models.password_policy_response_complexity import PasswordPolicyResponseComplexity
+from finbourne_identity.models.password_policy_response_lockout import PasswordPolicyResponseLockout
 
-class PasswordPolicyConditions(BaseModel):
+class PasswordPolicyResponseConditions(BaseModel):
     """
     Password policy conditions for a password policy  # noqa: E501
     """
-    complexity: Optional[PasswordPolicyComplexity] = None
-    age: Optional[PasswordPolicyAge] = None
-    lockout: Optional[PasswordPolicyLockout] = None
+    complexity: PasswordPolicyResponseComplexity = Field(...)
+    age: PasswordPolicyResponseAge = Field(...)
+    lockout: PasswordPolicyResponseLockout = Field(...)
     __properties = ["complexity", "age", "lockout"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -43,16 +43,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PasswordPolicyConditions:
-        """Create an instance of PasswordPolicyConditions from a JSON string"""
+    def from_json(cls, json_str: str) -> PasswordPolicyResponseConditions:
+        """Create an instance of PasswordPolicyResponseConditions from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -65,21 +65,21 @@
             _dict['age'] = self.age.to_dict()
         # override the default output from pydantic by calling `to_dict()` of lockout
         if self.lockout:
             _dict['lockout'] = self.lockout.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PasswordPolicyConditions:
-        """Create an instance of PasswordPolicyConditions from a dict"""
+    def from_dict(cls, obj: dict) -> PasswordPolicyResponseConditions:
+        """Create an instance of PasswordPolicyResponseConditions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PasswordPolicyConditions.parse_obj(obj)
+            return PasswordPolicyResponseConditions.parse_obj(obj)
 
-        _obj = PasswordPolicyConditions.parse_obj({
-            "complexity": PasswordPolicyComplexity.from_dict(obj.get("complexity")) if obj.get("complexity") is not None else None,
-            "age": PasswordPolicyAge.from_dict(obj.get("age")) if obj.get("age") is not None else None,
-            "lockout": PasswordPolicyLockout.from_dict(obj.get("lockout")) if obj.get("lockout") is not None else None
+        _obj = PasswordPolicyResponseConditions.parse_obj({
+            "complexity": PasswordPolicyResponseComplexity.from_dict(obj.get("complexity")) if obj.get("complexity") is not None else None,
+            "age": PasswordPolicyResponseAge.from_dict(obj.get("age")) if obj.get("age") is not None else None,
+            "lockout": PasswordPolicyResponseLockout.from_dict(obj.get("lockout")) if obj.get("lockout") is not None else None
         })
         return _obj
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_lockout.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/password_policy_response_lockout.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictInt
+from typing import Any, Dict
+from pydantic.v1 import BaseModel, Field, StrictInt
 
-class PasswordPolicyLockout(BaseModel):
+class PasswordPolicyResponseLockout(BaseModel):
     """
-    PasswordPolicyLockout
+    PasswordPolicyResponseLockout
     """
-    max_attempts: Optional[StrictInt] = Field(None, alias="maxAttempts", description="The maximum number of unsuccessful attempts before the user is locked out of their account")
+    max_attempts: StrictInt = Field(..., alias="maxAttempts", description="The maximum number of unsuccessful attempts before the user is locked out of their account")
     __properties = ["maxAttempts"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -38,32 +38,32 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PasswordPolicyLockout:
-        """Create an instance of PasswordPolicyLockout from a JSON string"""
+    def from_json(cls, json_str: str) -> PasswordPolicyResponseLockout:
+        """Create an instance of PasswordPolicyResponseLockout from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PasswordPolicyLockout:
-        """Create an instance of PasswordPolicyLockout from a dict"""
+    def from_dict(cls, obj: dict) -> PasswordPolicyResponseLockout:
+        """Create an instance of PasswordPolicyResponseLockout from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PasswordPolicyLockout.parse_obj(obj)
+            return PasswordPolicyResponseLockout.parse_obj(obj)
 
-        _obj = PasswordPolicyLockout.parse_obj({
+        _obj = PasswordPolicyResponseLockout.parse_obj({
             "max_attempts": obj.get("maxAttempts")
         })
         return _obj
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/resource_list_of_access_controlled_resource.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from finbourne_identity.models.access_controlled_resource import AccessControlledResource
 from finbourne_identity.models.link import Link
 
 class ResourceListOfAccessControlledResource(BaseModel):
     """
     ResourceListOfAccessControlledResource
     """
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_id.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/role_id.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class RoleId(BaseModel):
     """
     RoleId
     """
     scope: constr(strict=True, max_length=100, min_length=3) = Field(...)
     code: constr(strict=True, max_length=100, min_length=3) = Field(...)
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/role_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr, constr
+from pydantic.v1 import BaseModel, Field, StrictStr, constr
 from finbourne_identity.models.role_id import RoleId
 
 class RoleResponse(BaseModel):
     """
     RoleResponse
     """
     id: constr(strict=True, min_length=1) = Field(..., description="The role's system supplied unique identifier")
     role_id: RoleId = Field(..., alias="roleId")
     source: constr(strict=True, min_length=1) = Field(..., description="The source of the role")
     name: constr(strict=True, min_length=1) = Field(..., description="The role name, which must be unique within the system.")
     description: Optional[StrictStr] = Field(None, description="The description for this role")
-    __properties = ["id", "roleId", "source", "name", "description"]
+    saml_name: Optional[StrictStr] = Field(None, alias="samlName", description="The name to use on the SAML request if assigning this role via SAML Just in Time (JIT)")
+    __properties = ["id", "roleId", "source", "name", "description", "samlName"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -61,14 +62,19 @@
         if self.role_id:
             _dict['roleId'] = self.role_id.to_dict()
         # set to None if description (nullable) is None
         # and __fields_set__ contains the field
         if self.description is None and "description" in self.__fields_set__:
             _dict['description'] = None
 
+        # set to None if saml_name (nullable) is None
+        # and __fields_set__ contains the field
+        if self.saml_name is None and "saml_name" in self.__fields_set__:
+            _dict['samlName'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> RoleResponse:
         """Create an instance of RoleResponse from a dict"""
         if obj is None:
             return None
@@ -77,10 +83,11 @@
             return RoleResponse.parse_obj(obj)
 
         _obj = RoleResponse.parse_obj({
             "id": obj.get("id"),
             "role_id": RoleId.from_dict(obj.get("roleId")) if obj.get("roleId") is not None else None,
             "source": obj.get("source"),
             "name": obj.get("name"),
-            "description": obj.get("description")
+            "description": obj.get("description"),
+            "saml_name": obj.get("samlName")
         })
         return _obj
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/set_password.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class SetPassword(BaseModel):
     """
     Set password request  # noqa: E501
     """
     value: constr(strict=True, max_length=50, min_length=12) = Field(..., description="The value of the new password")
     __properties = ["value"]
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/set_password_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_identity.models.link import Link
 
 class SetPasswordResponse(BaseModel):
     """
     The result of setting a password  # noqa: E501
     """
     updated_at: datetime = Field(..., alias="updatedAt", description="The date and time at which the password was successfully updated")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_expiry.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict
-from pydantic import BaseModel, Field
+from pydantic.v1 import BaseModel, Field
 
 class SupportAccessExpiry(BaseModel):
     """
     Time at which the support access expires  # noqa: E501
     """
     expiry: datetime = Field(..., description="DateTimeOffset at which the access will be revoked")
     __properties = ["expiry"]
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry_with_role.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_expiry_with_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class SupportAccessExpiryWithRole(BaseModel):
     """
     Time at which the support access granted for a role expires  # noqa: E501
     """
     expiry: datetime = Field(..., description="DateTimeOffset at which the access will be revoked")
     permitted_role: constr(strict=True, min_length=1) = Field(..., alias="permittedRole", description="Unique identifier for permitted role.   Use GET /identity/api/authentication/support-roles to lookup role label/code from identifier.")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_request.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr, validator
 
 class SupportAccessRequest(BaseModel):
     """
     A Request to grant support access to your account  # noqa: E501
     """
     duration: constr(strict=True, max_length=30, min_length=2) = Field(..., description="The duration for which access is requested (in any ISO-8601 format)")
     description: Optional[constr(strict=True, max_length=1024, min_length=0)] = Field(None, description="The description of why the support access has been granted (i.e. support ticket numbers)")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_access_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, constr, validator
 
 class SupportAccessResponse(BaseModel):
     """
     Timestamped successful response to grant access to your account  # noqa: E501
     """
     id: constr(strict=True, min_length=1) = Field(..., description="ID of the support access request")
     duration: constr(strict=True, max_length=50, min_length=3) = Field(..., description="The duration for which access is requested (in any ISO-8601 format)")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_role.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic.v1 import BaseModel, Field, StrictStr
 
 class SupportRole(BaseModel):
     """
     SupportRole
     """
     label: Optional[StrictStr] = None
     description: Optional[StrictStr] = None
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_roles_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/support_roles_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist
+from pydantic.v1 import BaseModel, Field, conlist
 from finbourne_identity.models.support_role import SupportRole
 
 class SupportRolesResponse(BaseModel):
     """
     SupportRolesResponse
     """
     support_roles: Optional[conlist(SupportRole)] = Field(None, alias="supportRoles")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/temporary_password.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/temporary_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict
-from pydantic import BaseModel, Field, constr
+from pydantic.v1 import BaseModel, Field, constr
 
 class TemporaryPassword(BaseModel):
     """
     TemporaryPassword
     """
     password: constr(strict=True, min_length=1) = Field(..., description="The user's temporary password")
     __properties = ["password"]
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_role_request.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_role_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
-from pydantic import BaseModel, Field, constr, validator
+from pydantic.v1 import BaseModel, Field, constr, validator
 
 class UpdateRoleRequest(BaseModel):
     """
     UpdateRoleRequest
     """
     description: Optional[constr(strict=True, max_length=1024, min_length=0)] = Field(None, description="The description for this role")
     __properties = ["description"]
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_user_request.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/update_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, conlist, constr, validator
+from pydantic.v1 import BaseModel, Field, conlist, constr, validator
 from finbourne_identity.models.role_id import RoleId
 
 class UpdateUserRequest(BaseModel):
     """
     UpdateUserRequest
     """
     first_name: constr(strict=True, max_length=50, min_length=1) = Field(..., alias="firstName")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_response.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/user_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, constr
+from pydantic.v1 import BaseModel, Field, StrictBool, StrictStr, conlist, constr
 from finbourne_identity.models.link import Link
 from finbourne_identity.models.role_response import RoleResponse
 
 class UserResponse(BaseModel):
     """
     UserResponse
     """
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_summary.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/models/user_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic.v1 import BaseModel, Field, StrictStr, conlist
 from finbourne_identity.models.link import Link
 
 class UserSummary(BaseModel):
     """
     Lightweight view of an user details  # noqa: E501
     """
     id: Optional[StrictStr] = Field(None, description="The user id")
```

### Comparing `finbourne_identity_sdk-2.0.9/finbourne_identity/rest.py` & `finbourne_identity_sdk-2.1.1/finbourne_identity/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,18 @@
         # url already contains the URL query string
         # so reset query_params to empty dict
         query_params = {}
         timeout = _request_timeout or 5 * 60
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/json'
-
+        
+        for content in headers:
+            headers[content] = str(headers[content])
+            
         args = {
             "method": method,
             "url": url,
             "timeout": timeout,
             "headers": headers
         }
 
@@ -155,15 +158,15 @@
                     else:
                         data.add_field(k, v)
                 args["data"] = data
 
             # Pass a `bytes` parameter directly in the body to support
             # other content types than Json when `body` argument is provided
             # in serialized form
-            elif isinstance(body, bytes):
+            elif isinstance(body, str) or isinstance(body, bytes):
                 args["data"] = body
             else:
                 # Cannot generate the request from given parameters
                 msg = """Cannot prepare a request message for provided
                          arguments. Please check that your arguments match
                          declared content type."""
                 raise ApiException(status=0, reason=msg)
```

### Comparing `finbourne_identity_sdk-2.0.9/pyproject.toml` & `finbourne_identity_sdk-2.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-identity-sdk"
-version = "2.0.9"
+version = "2.1.1"
 description = "FINBOURNE Identity Service API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-identity-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Identity Service API", "finbourne-identity-sdk"]
 packages = [
@@ -15,15 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 urllib3 = "^1.25.3"
 python-dateutil = "^2.8.2"
 requests = "^2"
 aiohttp = "^3.8.4"
-pydantic = "^1.10.5"
+pydantic = "^2.6.3"
 aenum = "^3.1.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0"
 flake8 = "^4.0.0"
 black = "^23.9.1"
```

### Comparing `finbourne_identity_sdk-2.0.9/PKG-INFO` & `finbourne_identity_sdk-2.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-identity-sdk
-Version: 2.0.9
+Version: 2.1.1
 Summary: FINBOURNE Identity Service API
 Home-page: https://github.com/finbourne/finbourne-identity-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Identity Service API,finbourne-identity-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
 Project-URL: Repository, https://github.com/finbourne/finbourne-identity-sdk-python
 Description-Content-Type: text/markdown
 
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2725
-- Package version: 2.0.9
+- API version: 0.0.2850
+- Package version: 2.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -69,29 +69,105 @@
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
+You'll need to provide some configuration to connect to the finbourne_identity application.
+These can be provided using a secrets file or environment variables.
+
+### Environment variables
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set for the following environment variables:
+
+``` 
+FBN_TOKEN_URL,
+FBN_FINBOURNE_IDENTITY_API_URL,
+FBN_USERNAME,
+FBN_PASSWORD,
+FBN_CLIENT_ID,
+FBN_CLIENT_SECRET
+```
+
+To use a long lived Personal Access Token, you must provide the following environment variables:
+``` 
+FBN_FINBOURNE_IDENTITY_API_URL,
+FBN_ACCESS_TOKEN
+```
+
+You can send your requests to finbourne_identity via a proxy, by setting `FBN_PROXY_ADDRESS`. 
+If your proxy has basic auth enabled, you must akso supply `FBN_PROXY_USERNAME` and `FBN_PROXY_PASSWORD`
+
+### Secrets file
+
+In order to use [short lived access tokens](https://support.lusid.com/knowledgebase/article/KA-01654/en-us) you will need to have appropriate values set in a `secrets.json` file in the same folder as your script.
+
+``` 
+{
+    "api":
+    {
+        "tokenUrl":"<your-token-url>",
+        "finbourne_identityUrl":"<FINBOURNE-application-url>",
+        "username":"<your-username>",
+        "password":"<your-password>",
+        "clientId":"<your-client-id>",
+        "clientSecret":"<your-client-secret>",
+    }
+}
+```
+
+To use a long lived Personal Access Token, you must provide a `secrets.json` with the following variables:
+``` 
+{
+    "api":
+    {
+        "finbourne_identityUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    }
+}
+```
+
+You can send your requests to finbourne_identity via a proxy, by adding a proxy section to your `secrets.json`. 
+If your proxy has basic auth enabled, you must also supply a `username` and `password` in this section.
+
+``` 
+{
+    "api":
+    {
+        "finbourne_identityUrl":"<FINBOURNE-application-url>",
+        "accessToken":"<your-access-token>"
+    },
+    "proxy":
+    {
+        "address":"<your-proxy-address>",
+        "username":"<your-proxy-username>",
+        "password":"<your-proxy-password>"
+    }
+}
+```
+
+### Using the SDK
+
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
 import finbourne_identity
-from finbourne_identity.rest import ApiException
+from finbourne_identity.exceptions import ApiException
 from pprint import pprint
 
+import os
 from finbourne_identity import (
-	  ApiClientFactory,
-	  ApplicationMetadataApi,
-	  EnvironmentVariablesConfigurationLoader,
-	  SecretsFileConfigurationLoader,
-	  ArgsConfigurationLoader
+    ApiClientFactory,
+    ApplicationMetadataApi,
+    EnvironmentVariablesConfigurationLoader,
+    SecretsFileConfigurationLoader,
+    ArgsConfigurationLoader
 )
 
 # Use the finbourne_identity ApiClientFactory to build Api instances with a configured api client
 # By default this will read config from environment variables
 # Then from a secrets.json file found in the current working directory
 api_client_factory = ApiClientFactory()
 
@@ -116,15 +192,15 @@
 # in accordance with the API server security policy.
 
 
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
-    api_instance = finbourne_identity.ApplicationMetadataApi(api_client)
+    api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
         # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
@@ -139,21 +215,22 @@
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
 *ApplicationsApi* | [**create_application**](docs/ApplicationsApi.md#create_application) | **POST** /api/applications | [EARLY ACCESS] CreateApplication: Create Application
 *ApplicationsApi* | [**delete_application**](docs/ApplicationsApi.md#delete_application) | **DELETE** /api/applications/{id} | [EARLY ACCESS] DeleteApplication: Delete Application
 *ApplicationsApi* | [**get_application**](docs/ApplicationsApi.md#get_application) | **GET** /api/applications/{id} | [EARLY ACCESS] GetApplication: Get Application
 *ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /api/applications | [EARLY ACCESS] ListApplications: List Applications
-*ApplicationsApi* | [**rotate_application_secrets**](docs/ApplicationsApi.md#rotate_application_secrets) | **POST** /api/applications/{id}/lifecycle/$newsecret | [EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets
+*ApplicationsApi* | [**rotate_application_secrets**](docs/ApplicationsApi.md#rotate_application_secrets) | **POST** /api/applications/{id}/lifecycle/$newsecret | [EARLY ACCESS] RotateApplicationSecrets: Rotate Application Secrets
 *AuthenticationApi* | [**get_authentication_information**](docs/AuthenticationApi.md#get_authentication_information) | **GET** /api/authentication/information | GetAuthenticationInformation: Gets AuthenticationInformation
-*AuthenticationApi* | [**get_password_policy**](docs/AuthenticationApi.md#get_password_policy) | **GET** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type
+*AuthenticationApi* | [**get_password_policy**](docs/AuthenticationApi.md#get_password_policy) | **GET** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] GetPasswordPolicy: Gets password policy for a user type
 *AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | [EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
 *AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | [EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
 *AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | [EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account
 *AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | [EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
+*AuthenticationApi* | [**update_password_policy**](docs/AuthenticationApi.md#update_password_policy) | **PUT** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] UpdatePasswordPolicy: Updates password policy for a user type
 *IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | [EARLY ACCESS] AddScim: Add SCIM
 *IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | [EARLY ACCESS] RemoveScim: Remove SCIM
 *MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | [EARLY ACCESS] GetUserInfo: Get User Info
 *MeApi* | [**set_password**](docs/MeApi.md#set_password) | **PUT** /api/me/password | SetPassword: Set password of current user
 *PersonalAuthenticationTokensApi* | [**create_api_key**](docs/PersonalAuthenticationTokensApi.md#create_api_key) | **POST** /api/keys | [EARLY ACCESS] CreateApiKey: Create a Personal Access Token
 *PersonalAuthenticationTokensApi* | [**delete_api_key**](docs/PersonalAuthenticationTokensApi.md#delete_api_key) | **DELETE** /api/keys/{id} | [EARLY ACCESS] DeleteApiKey: Invalidate a Personal Access Token
 *PersonalAuthenticationTokensApi* | [**list_own_api_keys**](docs/PersonalAuthenticationTokensApi.md#list_own_api_keys) | **GET** /api/keys | [EARLY ACCESS] ListOwnApiKeys: Gets the meta data for all of the user&#39;s existing Personal Access Tokens.
@@ -199,31 +276,36 @@
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [ListUsersResponse](docs/ListUsersResponse.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [OAuthApplication](docs/OAuthApplication.md)
- - [PasswordPolicy](docs/PasswordPolicy.md)
- - [PasswordPolicyAge](docs/PasswordPolicyAge.md)
- - [PasswordPolicyComplexity](docs/PasswordPolicyComplexity.md)
- - [PasswordPolicyConditions](docs/PasswordPolicyConditions.md)
- - [PasswordPolicyLockout](docs/PasswordPolicyLockout.md)
+ - [PasswordPolicyResponse](docs/PasswordPolicyResponse.md)
+ - [PasswordPolicyResponseAge](docs/PasswordPolicyResponseAge.md)
+ - [PasswordPolicyResponseComplexity](docs/PasswordPolicyResponseComplexity.md)
+ - [PasswordPolicyResponseConditions](docs/PasswordPolicyResponseConditions.md)
+ - [PasswordPolicyResponseLockout](docs/PasswordPolicyResponseLockout.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [RoleId](docs/RoleId.md)
  - [RoleResponse](docs/RoleResponse.md)
  - [SetPassword](docs/SetPassword.md)
  - [SetPasswordResponse](docs/SetPasswordResponse.md)
  - [SupportAccessExpiry](docs/SupportAccessExpiry.md)
  - [SupportAccessExpiryWithRole](docs/SupportAccessExpiryWithRole.md)
  - [SupportAccessRequest](docs/SupportAccessRequest.md)
  - [SupportAccessResponse](docs/SupportAccessResponse.md)
  - [SupportRole](docs/SupportRole.md)
  - [SupportRolesResponse](docs/SupportRolesResponse.md)
  - [TemporaryPassword](docs/TemporaryPassword.md)
+ - [UpdatePasswordPolicyRequest](docs/UpdatePasswordPolicyRequest.md)
+ - [UpdatePasswordPolicyRequestAge](docs/UpdatePasswordPolicyRequestAge.md)
+ - [UpdatePasswordPolicyRequestComplexity](docs/UpdatePasswordPolicyRequestComplexity.md)
+ - [UpdatePasswordPolicyRequestConditions](docs/UpdatePasswordPolicyRequestConditions.md)
+ - [UpdatePasswordPolicyRequestLockout](docs/UpdatePasswordPolicyRequestLockout.md)
  - [UpdateRoleRequest](docs/UpdateRoleRequest.md)
  - [UpdateUserRequest](docs/UpdateUserRequest.md)
  - [UserResponse](docs/UserResponse.md)
  - [UserSummary](docs/UserSummary.md)
 
 
 <a id="documentation-for-authorization"></a>
```

