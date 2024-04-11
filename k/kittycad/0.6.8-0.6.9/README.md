# Comparing `tmp/kittycad-0.6.8.tar.gz` & `tmp/kittycad-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.6.8.tar", max compression
+gzip compressed data, was "kittycad-0.6.9.tar", max compression
```

## Comparing `kittycad-0.6.8.tar` & `kittycad-0.6.9.tar`

### file list

```diff
@@ -1,405 +1,411 @@
--rw-r--r--   0        0        0     1065 2024-03-04 21:13:23.675802 kittycad-0.6.8/LICENSE
--rw-r--r--   0        0        0      749 2024-03-04 21:13:23.675802 kittycad-0.6.8/README.md
--rw-r--r--   0        0        0       48 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/__init__.py
--rw-r--r--   0        0        0      120 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     2820 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/create_kcl_code_completions.py
--rw-r--r--   0        0        0     4393 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/create_text_to_cad.py
--rw-r--r--   0        0        0     2952 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/create_text_to_cad_model_feedback.py
--rw-r--r--   0        0        0     2582 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/get_ai_prompt.py
--rw-r--r--   0        0        0     2700 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/get_text_to_cad_model_for_user.py
--rw-r--r--   0        0        0     4422 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/list_ai_prompts.py
--rw-r--r--   0        0        0     5029 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/ai/list_text_to_cad_models_for_user.py
--rw-r--r--   0        0        0      199 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3081 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2791 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/api_calls/get_api_call_for_org.py
--rw-r--r--   0        0        0     2780 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3218 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6514 2024-03-04 21:13:26.783867 kittycad-0.6.8/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4215 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     4992 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4796 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4487 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_calls/org_list_api_calls.py
--rw-r--r--   0        0        0     4340 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2958 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2864 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2751 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4273 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2578 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2884 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2329 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0      161 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1349 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3188 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     5121 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4648 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     6286 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     6468 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     5033 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     4975 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0      133 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2803 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3217 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     3354 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/hidden/get_auth_saml.py
--rw-r--r--   0        0        0     2130 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0     2552 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/hidden/post_auth_saml.py
--rw-r--r--   0        0        0      105 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2188 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/create_event.py
--rw-r--r--   0        0        0     2292 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/get_ipinfo.py
--rw-r--r--   0        0        0     2602 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2403 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/get_pricing_subscriptions.py
--rw-r--r--   0        0        0     2184 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     3072 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/internal_get_api_token_for_discord_user.py
--rw-r--r--   0        0        0     2228 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      139 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/modeling/__init__.py
--rw-r--r--   0        0        0     5084 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/modeling/modeling_commands_ws.py
--rw-r--r--   0        0        0      123 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      190 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/__init__.py
--rw-r--r--   0        0        0     2858 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/create_org.py
--rw-r--r--   0        0        0     3616 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/create_org_member.py
--rw-r--r--   0        0        0     2940 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/create_org_saml_idp.py
--rw-r--r--   0        0        0     2579 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/delete_org.py
--rw-r--r--   0        0        0     2581 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/delete_org_member.py
--rw-r--r--   0        0        0     2182 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/delete_org_saml_idp.py
--rw-r--r--   0        0        0     2661 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/get_any_org.py
--rw-r--r--   0        0        0     2452 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/get_org.py
--rw-r--r--   0        0        0     2829 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/get_org_member.py
--rw-r--r--   0        0        0     2625 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/get_org_privacy_settings.py
--rw-r--r--   0        0        0     2546 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/get_org_saml_idp.py
--rw-r--r--   0        0        0     2683 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/get_user_org.py
--rw-r--r--   0        0        0     4459 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/list_org_members.py
--rw-r--r--   0        0        0     4070 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/list_orgs.py
--rw-r--r--   0        0        0     3120 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/update_enterprise_pricing_for_org.py
--rw-r--r--   0        0        0     2736 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/update_org.py
--rw-r--r--   0        0        0     3193 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/update_org_member.py
--rw-r--r--   0        0        0     2889 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/update_org_privacy_settings.py
--rw-r--r--   0        0        0     2938 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/orgs/update_org_saml_idp.py
--rw-r--r--   0        0        0      117 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     3163 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/create_org_subscription.py
--rw-r--r--   0        0        0     2970 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/create_payment_information_for_org.py
--rw-r--r--   0        0        0     2957 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2636 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/create_payment_intent_for_org.py
--rw-r--r--   0        0        0     2611 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     3131 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/create_user_subscription.py
--rw-r--r--   0        0        0     2433 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/delete_payment_information_for_org.py
--rw-r--r--   0        0        0     2422 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2486 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/delete_payment_method_for_org.py
--rw-r--r--   0        0        0     2475 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2704 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_org_subscription.py
--rw-r--r--   0        0        0     2808 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_any_org.py
--rw-r--r--   0        0        0     2811 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_any_user.py
--rw-r--r--   0        0        0     2639 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_org.py
--rw-r--r--   0        0        0     2628 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2675 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_payment_information_for_org.py
--rw-r--r--   0        0        0     2664 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2665 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/get_user_subscription.py
--rw-r--r--   0        0        0     2600 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/list_invoices_for_org.py
--rw-r--r--   0        0        0     2589 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2668 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/list_payment_methods_for_org.py
--rw-r--r--   0        0        0     2657 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     3161 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/update_org_subscription.py
--rw-r--r--   0        0        0     3163 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/update_payment_balance_for_any_org.py
--rw-r--r--   0        0        0     3166 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/update_payment_balance_for_any_user.py
--rw-r--r--   0        0        0     2966 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/update_payment_information_for_org.py
--rw-r--r--   0        0        0     2955 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     3129 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/update_user_subscription.py
--rw-r--r--   0        0        0     2453 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/validate_customer_tax_information_for_org.py
--rw-r--r--   0        0        0     2456 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      430 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/service_accounts/__init__.py
--rw-r--r--   0        0        0     3023 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/service_accounts/create_service_account_for_org.py
--rw-r--r--   0        0        0     2929 2024-03-04 21:13:26.787867 kittycad-0.6.8/kittycad/api/service_accounts/delete_service_account_for_org.py
--rw-r--r--   0        0        0     2844 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/service_accounts/get_service_account_for_org.py
--rw-r--r--   0        0        0     4356 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/service_accounts/list_service_accounts_for_org.py
--rw-r--r--   0        0        0      111 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/store/__init__.py
--rw-r--r--   0        0        0     2869 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/store/create_store_coupon.py
--rw-r--r--   0        0        0      101 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3666 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     3640 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3716 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_current_unit_conversion.py
--rw-r--r--   0        0        0     3690 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3664 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3768 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_frequency_unit_conversion.py
--rw-r--r--   0        0        0     3690 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     3638 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3664 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3742 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3820 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3690 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_torque_unit_conversion.py
--rw-r--r--   0        0        0     3690 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      292 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2560 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2928 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_oauth2_providers_for_user.py
--rw-r--r--   0        0        0     2738 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3032 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3156 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2489 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2586 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_user_privacy_settings.py
--rw-r--r--   0        0        0     2506 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2612 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4084 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4166 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2850 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/update_user_privacy_settings.py
--rw-r--r--   0        0        0     2770 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2466 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/client.py
--rw-r--r--   0        0        0    16248 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/client_test.py
--rw-r--r--   0        0        0   179066 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/examples_test.py
--rw-r--r--   0        0        0    11829 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/__init__.py
--rw-r--r--   0        0        0      721 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/account_provider.py
--rw-r--r--   0        0        0      266 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/add_org_member.py
--rw-r--r--   0        0        0      429 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/address_details.py
--rw-r--r--   0        0        0      312 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/ai_feedback.py
--rw-r--r--   0        0        0      830 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/ai_prompt.py
--rw-r--r--   0        0        0      314 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/ai_prompt_results_page.py
--rw-r--r--   0        0        0      235 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/ai_prompt_type.py
--rw-r--r--   0        0        0      250 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/angle.py
--rw-r--r--   0        0        0      210 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_line_end.py
--rw-r--r--   0        0        0      301 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_line_end_options.py
--rw-r--r--   0        0        0      635 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_options.py
--rw-r--r--   0        0        0      240 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_text_alignment_x.py
--rw-r--r--   0        0        0      238 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_text_alignment_y.py
--rw-r--r--   0        0        0      431 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_text_options.py
--rw-r--r--   0        0        0      316 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/annotation_type.py
--rw-r--r--   0        0        0      256 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     1155 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0      348 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0      237 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_error.py
--rw-r--r--   0        0        0      472 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_token.py
--rw-r--r--   0        0        0      314 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0      248 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0      750 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0     5269 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0      331 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      729 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0      443 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/auth_callback.py
--rw-r--r--   0        0        0      426 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/axis.py
--rw-r--r--   0        0        0      304 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/axis_direction_pair.py
--rw-r--r--   0        0        0     1414 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/base64data.py
--rw-r--r--   0        0        0      372 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/billing_info.py
--rw-r--r--   0        0        0      467 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/block_reason.py
--rw-r--r--   0        0        0      247 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0      274 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/camera_drag_end.py
--rw-r--r--   0        0        0      440 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/camera_drag_interaction_type.py
--rw-r--r--   0        0        0      377 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/camera_drag_move.py
--rw-r--r--   0        0        0      412 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/camera_settings.py
--rw-r--r--   0        0        0      583 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/card_details.py
--rw-r--r--   0        0        0      312 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/center_of_mass.py
--rw-r--r--   0        0        0      462 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/client_metrics.py
--rw-r--r--   0        0        0      415 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/cluster.py
--rw-r--r--   0        0        0      833 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/code_language.py
--rw-r--r--   0        0        0      946 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/code_output.py
--rw-r--r--   0        0        0      207 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/color.py
--rw-r--r--   0        0        0     2143 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/connection.py
--rw-r--r--   0        0        0      472 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/country_code.py
--rw-r--r--   0        0        0      434 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/coupon.py
--rw-r--r--   0        0        0      509 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0      626 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/currency.py
--rw-r--r--   0        0        0      304 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/curve_get_control_points.py
--rw-r--r--   0        0        0      245 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/curve_get_end_points.py
--rw-r--r--   0        0        0      259 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/curve_get_type.py
--rw-r--r--   0        0        0      234 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/curve_type.py
--rw-r--r--   0        0        0      704 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/customer.py
--rw-r--r--   0        0        0      881 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0      296 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/default_camera_get_settings.py
--rw-r--r--   0        0        0      282 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/default_camera_zoom.py
--rw-r--r--   0        0        0      257 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/density.py
--rw-r--r--   0        0        0      268 2024-03-04 21:13:26.791867 kittycad-0.6.8/kittycad/models/der_encoded_key_pair.py
--rw-r--r--   0        0        0      335 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0      247 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0      269 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0      327 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/direction.py
--rw-r--r--   0        0        0      233 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/discount.py
--rw-r--r--   0        0        0      306 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/discount_code.py
--rw-r--r--   0        0        0      713 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/distance_type.py
--rw-r--r--   0        0        0      286 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0      285 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/empty.py
--rw-r--r--   0        0        0      259 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_circular_pattern.py
--rw-r--r--   0        0        0      261 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_get_all_child_uuids.py
--rw-r--r--   0        0        0      222 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_get_child_uuid.py
--rw-r--r--   0        0        0      306 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_get_distance.py
--rw-r--r--   0        0        0      220 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_get_num_children.py
--rw-r--r--   0        0        0      220 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_get_parent_id.py
--rw-r--r--   0        0        0      255 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_linear_pattern.py
--rw-r--r--   0        0        0      367 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/entity_type.py
--rw-r--r--   0        0        0      529 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/environment.py
--rw-r--r--   0        0        0      277 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/error.py
--rw-r--r--   0        0        0     1469 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/error_code.py
--rw-r--r--   0        0        0      276 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/export.py
--rw-r--r--   0        0        0      255 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/export_file.py
--rw-r--r--   0        0        0     1153 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/extended_user.py
--rw-r--r--   0        0        0      330 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0      389 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/extrusion_face_cap_type.py
--rw-r--r--   0        0        0      458 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/extrusion_face_info.py
--rw-r--r--   0        0        0      302 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/face_get_gradient.py
--rw-r--r--   0        0        0      252 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/face_get_position.py
--rw-r--r--   0        0        0      402 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/face_is_planar.py
--rw-r--r--   0        0        0      348 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/failure_web_socket_response.py
--rw-r--r--   0        0        0      322 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/fbx_storage.py
--rw-r--r--   0        0        0      820 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     1045 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0      882 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1387 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1012 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0      879 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_mass.py
--rw-r--r--   0        0        0      770 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0      258 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0      759 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/file_volume.py
--rw-r--r--   0        0        0      363 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/gateway.py
--rw-r--r--   0        0        0      265 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/get_entity_type.py
--rw-r--r--   0        0        0      277 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/get_sketch_mode_plane.py
--rw-r--r--   0        0        0      307 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/global_axis.py
--rw-r--r--   0        0        0      429 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/gltf_presentation.py
--rw-r--r--   0        0        0      660 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/gltf_storage.py
--rw-r--r--   0        0        0      303 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/highlight_set_entity.py
--rw-r--r--   0        0        0      430 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/ice_server.py
--rw-r--r--   0        0        0      805 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/idp_metadata_source.py
--rw-r--r--   0        0        0      329 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/image_format.py
--rw-r--r--   0        0        0      324 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/import_file.py
--rw-r--r--   0        0        0      193 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/import_files.py
--rw-r--r--   0        0        0     1772 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/input_format.py
--rw-r--r--   0        0        0     1387 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/invoice.py
--rw-r--r--   0        0        0      475 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      503 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0      913 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/ip_addr_info.py
--rw-r--r--   0        0        0      487 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/jetstream.py
--rw-r--r--   0        0        0      306 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0      348 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0      525 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0      422 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/kcl_code_completion_params.py
--rw-r--r--   0        0        0      674 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/kcl_code_completion_request.py
--rw-r--r--   0        0        0      247 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/kcl_code_completion_response.py
--rw-r--r--   0        0        0      334 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0      428 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/length_unit.py
--rw-r--r--   0        0        0      239 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/mass.py
--rw-r--r--   0        0        0      303 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0      573 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1793 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/method.py
--rw-r--r--   0        0        0      353 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_app_individual_subscription_tier.py
--rw-r--r--   0        0        0      378 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_app_organization_subscription_tier.py
--rw-r--r--   0        0        0     1095 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_app_subscription_tier.py
--rw-r--r--   0        0        0      476 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_app_subscription_tier_name.py
--rw-r--r--   0        0        0    28168 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_cmd.py
--rw-r--r--   0        0        0      488 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_cmd_id.py
--rw-r--r--   0        0        0      366 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/modeling_cmd_req.py
--rw-r--r--   0        0        0      278 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/mouse_click.py
--rw-r--r--   0        0        0      330 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0    15102 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/ok_modeling_cmd_response.py
--rw-r--r--   0        0        0     3019 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/ok_web_socket_response_data.py
--rw-r--r--   0        0        0      412 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/onboarding.py
--rw-r--r--   0        0        0      781 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/org.py
--rw-r--r--   0        0        0      452 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/org_details.py
--rw-r--r--   0        0        0      735 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/org_member.py
--rw-r--r--   0        0        0      318 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/org_member_results_page.py
--rw-r--r--   0        0        0      293 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/org_results_page.py
--rw-r--r--   0        0        0      458 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/org_role.py
--rw-r--r--   0        0        0      676 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/output_file.py
--rw-r--r--   0        0        0     2164 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/output_format.py
--rw-r--r--   0        0        0      333 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_command.py
--rw-r--r--   0        0        0      332 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_component_constraint_bound.py
--rw-r--r--   0        0        0      380 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_component_constraint_type.py
--rw-r--r--   0        0        0      272 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_get_curve_uuids_for_vertices.py
--rw-r--r--   0        0        0      304 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_get_info.py
--rw-r--r--   0        0        0      253 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_get_vertex_uuids.py
--rw-r--r--   0        0        0     1943 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_segment.py
--rw-r--r--   0        0        0      392 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/path_segment_info.py
--rw-r--r--   0        0        0      196 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0      576 2024-03-04 21:13:26.795867 kittycad-0.6.8/kittycad/models/payment_method.py
--rw-r--r--   0        0        0      333 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0      242 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/perspective_camera_parameters.py
--rw-r--r--   0        0        0      365 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/plan_interval.py
--rw-r--r--   0        0        0      353 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/plane_intersect_and_project.py
--rw-r--r--   0        0        0      607 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/ply_storage.py
--rw-r--r--   0        0        0      241 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/point2d.py
--rw-r--r--   0        0        0      201 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/point3d.py
--rw-r--r--   0        0        0      194 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/pong.py
--rw-r--r--   0        0        0      213 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/privacy_settings.py
--rw-r--r--   0        0        0      326 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/raw_file.py
--rw-r--r--   0        0        0      371 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/rtc_ice_candidate_init.py
--rw-r--r--   0        0        0     1369 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/rtc_sdp_type.py
--rw-r--r--   0        0        0      310 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/rtc_session_description.py
--rw-r--r--   0        0        0      666 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/saml_identity_provider.py
--rw-r--r--   0        0        0      548 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/saml_identity_provider_create.py
--rw-r--r--   0        0        0      398 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/scene_selection_type.py
--rw-r--r--   0        0        0      413 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/scene_tool_type.py
--rw-r--r--   0        0        0      235 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/select_get.py
--rw-r--r--   0        0        0      261 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/select_with_point.py
--rw-r--r--   0        0        0     1374 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/selection.py
--rw-r--r--   0        0        0      587 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/service_account.py
--rw-r--r--   0        0        0      338 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/service_account_results_page.py
--rw-r--r--   0        0        0      373 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/session.py
--rw-r--r--   0        0        0      256 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/solid3d_get_all_edge_faces.py
--rw-r--r--   0        0        0      264 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/solid3d_get_all_opposite_edges.py
--rw-r--r--   0        0        0      391 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/solid3d_get_extrusion_face_info.py
--rw-r--r--   0        0        0      278 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/solid3d_get_next_adjacent_edge.py
--rw-r--r--   0        0        0      225 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/solid3d_get_opposite_edge.py
--rw-r--r--   0        0        0      278 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/solid3d_get_prev_adjacent_edge.py
--rw-r--r--   0        0        0      323 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/stl_storage.py
--rw-r--r--   0        0        0      210 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/store_coupon_params.py
--rw-r--r--   0        0        0      199 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/subscription_tier_feature.py
--rw-r--r--   0        0        0     1024 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/subscription_tier_price.py
--rw-r--r--   0        0        0      750 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/subscription_tier_type.py
--rw-r--r--   0        0        0      583 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/subscription_training_data_behavior.py
--rw-r--r--   0        0        0      380 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/success_web_socket_response.py
--rw-r--r--   0        0        0      469 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/support_tier.py
--rw-r--r--   0        0        0      262 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/surface_area.py
--rw-r--r--   0        0        0      514 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/system.py
--rw-r--r--   0        0        0      251 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/take_snapshot.py
--rw-r--r--   0        0        0      890 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/text_to_cad.py
--rw-r--r--   0        0        0      206 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/text_to_cad_create_body.py
--rw-r--r--   0        0        0      319 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/text_to_cad_results_page.py
--rw-r--r--   0        0        0      377 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_angle.py
--rw-r--r--   0        0        0      750 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0     1013 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_area.py
--rw-r--r--   0        0        0      745 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      623 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_current.py
--rw-r--r--   0        0        0      760 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_current_conversion.py
--rw-r--r--   0        0        0      322 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_density.py
--rw-r--r--   0        0        0      934 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_energy.py
--rw-r--r--   0        0        0      755 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0      916 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_force.py
--rw-r--r--   0        0        0      750 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      997 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_frequency.py
--rw-r--r--   0        0        0      770 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_frequency_conversion.py
--rw-r--r--   0        0        0      708 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_length.py
--rw-r--r--   0        0        0      755 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0      436 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_mass.py
--rw-r--r--   0        0        0      745 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1014 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_power.py
--rw-r--r--   0        0        0      750 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      973 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_pressure.py
--rw-r--r--   0        0        0      765 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      593 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_temperature.py
--rw-r--r--   0        0        0      780 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      415 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_torque.py
--rw-r--r--   0        0        0      755 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_torque_conversion.py
--rw-r--r--   0        0        0     1131 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_volume.py
--rw-r--r--   0        0        0      755 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0      261 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/update_member_to_org_body.py
--rw-r--r--   0        0        0      375 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/update_payment_balance.py
--rw-r--r--   0        0        0      435 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/update_user.py
--rw-r--r--   0        0        0      832 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/user.py
--rw-r--r--   0        0        0      840 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/user_org_info.py
--rw-r--r--   0        0        0      381 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/user_org_role.py
--rw-r--r--   0        0        0      297 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0      437 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/uuid.py
--rw-r--r--   0        0        0      462 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/verification_token_response.py
--rw-r--r--   0        0        0      251 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/volume.py
--rw-r--r--   0        0        0     2167 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/web_socket_request.py
--rw-r--r--   0        0        0      309 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/web_socket_response.py
--rw-r--r--   0        0        0     1164 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/zoo_product_subscription.py
--rw-r--r--   0        0        0      321 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/zoo_product_subscriptions.py
--rw-r--r--   0        0        0      450 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/zoo_product_subscriptions_org_request.py
--rw-r--r--   0        0        0      436 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/zoo_product_subscriptions_user_request.py
--rw-r--r--   0        0        0      440 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/models/zoo_tool.py
--rw-r--r--   0        0        0       26 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/py.typed
--rw-r--r--   0        0        0     1050 2024-03-04 21:13:26.799867 kittycad-0.6.8/kittycad/types.py
--rw-r--r--   0        0        0     2606 2024-03-04 21:13:26.799867 kittycad-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 kittycad-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-05 20:15:38.981479 kittycad-0.6.9/LICENSE
+-rw-r--r--   0        0        0      749 2024-04-05 20:15:38.981479 kittycad-0.6.9/README.md
+-rw-r--r--   0        0        0       48 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      120 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     2820 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/create_kcl_code_completions.py
+-rw-r--r--   0        0        0     4393 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/create_text_to_cad.py
+-rw-r--r--   0        0        0     2952 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/create_text_to_cad_model_feedback.py
+-rw-r--r--   0        0        0     2582 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/get_ai_prompt.py
+-rw-r--r--   0        0        0     2700 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/get_text_to_cad_model_for_user.py
+-rw-r--r--   0        0        0     4422 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/list_ai_prompts.py
+-rw-r--r--   0        0        0     5029 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/ai/list_text_to_cad_models_for_user.py
+-rw-r--r--   0        0        0      199 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3081 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2791 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/get_api_call_for_org.py
+-rw-r--r--   0        0        0     2780 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3218 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6514 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4215 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     4992 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4796 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4487 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/org_list_api_calls.py
+-rw-r--r--   0        0        0     4340 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2864 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2751 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4273 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2578 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2884 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2329 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1349 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3188 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     5121 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4648 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     6286 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     6468 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     5033 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     4975 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0      133 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2803 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3217 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     3354 2024-04-05 20:15:40.857496 kittycad-0.6.9/kittycad/api/hidden/get_auth_saml.py
+-rw-r--r--   0        0        0     2130 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0     2552 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/hidden/post_auth_saml.py
+-rw-r--r--   0        0        0      105 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2430 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/create_event.py
+-rw-r--r--   0        0        0     2292 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/get_ipinfo.py
+-rw-r--r--   0        0        0     2602 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2403 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/get_pricing_subscriptions.py
+-rw-r--r--   0        0        0     2184 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     3072 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/internal_get_api_token_for_discord_user.py
+-rw-r--r--   0        0        0     2228 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      139 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/modeling/__init__.py
+-rw-r--r--   0        0        0     5906 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/modeling/modeling_commands_ws.py
+-rw-r--r--   0        0        0      123 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/__init__.py
+-rw-r--r--   0        0        0     2858 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/create_org.py
+-rw-r--r--   0        0        0     3616 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/create_org_member.py
+-rw-r--r--   0        0        0     2940 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/create_org_saml_idp.py
+-rw-r--r--   0        0        0     2579 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/delete_org.py
+-rw-r--r--   0        0        0     2581 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/delete_org_member.py
+-rw-r--r--   0        0        0     2182 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/delete_org_saml_idp.py
+-rw-r--r--   0        0        0     2661 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/get_any_org.py
+-rw-r--r--   0        0        0     2452 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/get_org.py
+-rw-r--r--   0        0        0     2829 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/get_org_member.py
+-rw-r--r--   0        0        0     2625 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/get_org_privacy_settings.py
+-rw-r--r--   0        0        0     2546 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/get_org_saml_idp.py
+-rw-r--r--   0        0        0     2683 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/get_user_org.py
+-rw-r--r--   0        0        0     4459 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/list_org_members.py
+-rw-r--r--   0        0        0     4070 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/list_orgs.py
+-rw-r--r--   0        0        0     3120 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/update_enterprise_pricing_for_org.py
+-rw-r--r--   0        0        0     2736 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/update_org.py
+-rw-r--r--   0        0        0     3193 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/update_org_member.py
+-rw-r--r--   0        0        0     2889 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/update_org_privacy_settings.py
+-rw-r--r--   0        0        0     2938 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/orgs/update_org_saml_idp.py
+-rw-r--r--   0        0        0      117 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     3163 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/create_org_subscription.py
+-rw-r--r--   0        0        0     2970 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/create_payment_information_for_org.py
+-rw-r--r--   0        0        0     2957 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2636 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/create_payment_intent_for_org.py
+-rw-r--r--   0        0        0     2611 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     3131 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/create_user_subscription.py
+-rw-r--r--   0        0        0     2433 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/delete_payment_information_for_org.py
+-rw-r--r--   0        0        0     2422 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2486 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/delete_payment_method_for_org.py
+-rw-r--r--   0        0        0     2475 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2704 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_org_subscription.py
+-rw-r--r--   0        0        0     2808 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_any_org.py
+-rw-r--r--   0        0        0     2811 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_any_user.py
+-rw-r--r--   0        0        0     2639 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_org.py
+-rw-r--r--   0        0        0     2628 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2675 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_payment_information_for_org.py
+-rw-r--r--   0        0        0     2664 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2665 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/get_user_subscription.py
+-rw-r--r--   0        0        0     2600 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/list_invoices_for_org.py
+-rw-r--r--   0        0        0     2589 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2668 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/list_payment_methods_for_org.py
+-rw-r--r--   0        0        0     2657 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     3161 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/update_org_subscription.py
+-rw-r--r--   0        0        0     3163 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/update_payment_balance_for_any_org.py
+-rw-r--r--   0        0        0     3166 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/update_payment_balance_for_any_user.py
+-rw-r--r--   0        0        0     2966 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/update_payment_information_for_org.py
+-rw-r--r--   0        0        0     2955 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     3129 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/update_user_subscription.py
+-rw-r--r--   0        0        0     2453 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/validate_customer_tax_information_for_org.py
+-rw-r--r--   0        0        0     2456 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      430 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/service_accounts/__init__.py
+-rw-r--r--   0        0        0     3023 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/service_accounts/create_service_account_for_org.py
+-rw-r--r--   0        0        0     2929 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/service_accounts/delete_service_account_for_org.py
+-rw-r--r--   0        0        0     2844 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/service_accounts/get_service_account_for_org.py
+-rw-r--r--   0        0        0     4356 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/service_accounts/list_service_accounts_for_org.py
+-rw-r--r--   0        0        0      111 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/store/__init__.py
+-rw-r--r--   0        0        0     2869 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/store/create_store_coupon.py
+-rw-r--r--   0        0        0      101 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3666 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3640 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3716 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_current_unit_conversion.py
+-rw-r--r--   0        0        0     3690 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3664 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3768 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_frequency_unit_conversion.py
+-rw-r--r--   0        0        0     3690 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     3638 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3664 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3742 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3820 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3690 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_torque_unit_conversion.py
+-rw-r--r--   0        0        0     3690 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      292 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2928 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_oauth2_providers_for_user.py
+-rw-r--r--   0        0        0     2738 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3032 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3156 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2489 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2586 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_user_privacy_settings.py
+-rw-r--r--   0        0        0     2506 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2612 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4084 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4166 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2850 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/update_user_privacy_settings.py
+-rw-r--r--   0        0        0     2770 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2466 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/client.py
+-rw-r--r--   0        0        0    16248 2024-04-05 20:15:40.861496 kittycad-0.6.9/kittycad/client_test.py
+-rw-r--r--   0        0        0   180482 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/examples_test.py
+-rw-r--r--   0        0        0    12106 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0      266 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/add_org_member.py
+-rw-r--r--   0        0        0      429 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/address_details.py
+-rw-r--r--   0        0        0      312 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/ai_feedback.py
+-rw-r--r--   0        0        0      830 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/ai_prompt.py
+-rw-r--r--   0        0        0      314 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/ai_prompt_results_page.py
+-rw-r--r--   0        0        0      235 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/ai_prompt_type.py
+-rw-r--r--   0        0        0      250 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/angle.py
+-rw-r--r--   0        0        0      210 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_line_end.py
+-rw-r--r--   0        0        0      301 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_line_end_options.py
+-rw-r--r--   0        0        0      635 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_options.py
+-rw-r--r--   0        0        0      240 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_text_alignment_x.py
+-rw-r--r--   0        0        0      238 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_text_alignment_y.py
+-rw-r--r--   0        0        0      431 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_text_options.py
+-rw-r--r--   0        0        0      316 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/annotation_type.py
+-rw-r--r--   0        0        0      256 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     1155 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0      348 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0      237 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_error.py
+-rw-r--r--   0        0        0      472 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_token.py
+-rw-r--r--   0        0        0      314 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0      248 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0      750 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0     5269 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0      331 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      729 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0      443 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/auth_callback.py
+-rw-r--r--   0        0        0      426 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/axis.py
+-rw-r--r--   0        0        0      304 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/axis_direction_pair.py
+-rw-r--r--   0        0        0     1414 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/base64data.py
+-rw-r--r--   0        0        0      372 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0      467 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/block_reason.py
+-rw-r--r--   0        0        0      247 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0      274 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/camera_drag_end.py
+-rw-r--r--   0        0        0      440 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/camera_drag_interaction_type.py
+-rw-r--r--   0        0        0      377 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/camera_drag_move.py
+-rw-r--r--   0        0        0      412 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/camera_settings.py
+-rw-r--r--   0        0        0      583 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/card_details.py
+-rw-r--r--   0        0        0      312 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/center_of_mass.py
+-rw-r--r--   0        0        0      462 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/client_metrics.py
+-rw-r--r--   0        0        0      415 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      833 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/code_language.py
+-rw-r--r--   0        0        0      946 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/code_output.py
+-rw-r--r--   0        0        0      207 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/color.py
+-rw-r--r--   0        0        0     2143 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/connection.py
+-rw-r--r--   0        0        0      472 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      434 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/coupon.py
+-rw-r--r--   0        0        0      509 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0      626 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/currency.py
+-rw-r--r--   0        0        0      304 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/curve_get_control_points.py
+-rw-r--r--   0        0        0      245 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/curve_get_end_points.py
+-rw-r--r--   0        0        0      259 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/curve_get_type.py
+-rw-r--r--   0        0        0      234 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/curve_type.py
+-rw-r--r--   0        0        0      704 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/customer.py
+-rw-r--r--   0        0        0      881 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0      206 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/default_camera_focus_on.py
+-rw-r--r--   0        0        0      296 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/default_camera_get_settings.py
+-rw-r--r--   0        0        0      282 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/default_camera_zoom.py
+-rw-r--r--   0        0        0      257 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/density.py
+-rw-r--r--   0        0        0      268 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/der_encoded_key_pair.py
+-rw-r--r--   0        0        0      335 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0      247 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0      269 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0      327 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/direction.py
+-rw-r--r--   0        0        0      233 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/discount.py
+-rw-r--r--   0        0        0      306 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/discount_code.py
+-rw-r--r--   0        0        0      713 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/distance_type.py
+-rw-r--r--   0        0        0      286 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0      285 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/empty.py
+-rw-r--r--   0        0        0      259 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_circular_pattern.py
+-rw-r--r--   0        0        0      261 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_get_all_child_uuids.py
+-rw-r--r--   0        0        0      222 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_get_child_uuid.py
+-rw-r--r--   0        0        0      306 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_get_distance.py
+-rw-r--r--   0        0        0      220 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_get_num_children.py
+-rw-r--r--   0        0        0      220 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_get_parent_id.py
+-rw-r--r--   0        0        0      255 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_linear_pattern.py
+-rw-r--r--   0        0        0      367 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/entity_type.py
+-rw-r--r--   0        0        0      529 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/environment.py
+-rw-r--r--   0        0        0      277 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/error.py
+-rw-r--r--   0        0        0     1469 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/error_code.py
+-rw-r--r--   0        0        0      806 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/event.py
+-rw-r--r--   0        0        0      276 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/export.py
+-rw-r--r--   0        0        0      255 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/export_file.py
+-rw-r--r--   0        0        0     1153 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0      330 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0      389 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/extrusion_face_cap_type.py
+-rw-r--r--   0        0        0      458 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/extrusion_face_info.py
+-rw-r--r--   0        0        0      302 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/face_get_gradient.py
+-rw-r--r--   0        0        0      252 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/face_get_position.py
+-rw-r--r--   0        0        0      402 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/face_is_planar.py
+-rw-r--r--   0        0        0      348 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/failure_web_socket_response.py
+-rw-r--r--   0        0        0      322 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/fbx_storage.py
+-rw-r--r--   0        0        0      820 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     1045 2024-04-05 20:15:40.865496 kittycad-0.6.9/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0      882 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1387 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1012 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0      879 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0      770 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0      258 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0      759 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0      363 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      265 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/get_entity_type.py
+-rw-r--r--   0        0        0      214 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/get_num_objects.py
+-rw-r--r--   0        0        0      277 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/get_sketch_mode_plane.py
+-rw-r--r--   0        0        0      307 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/global_axis.py
+-rw-r--r--   0        0        0      429 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/gltf_presentation.py
+-rw-r--r--   0        0        0      660 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/gltf_storage.py
+-rw-r--r--   0        0        0      303 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/highlight_set_entity.py
+-rw-r--r--   0        0        0      430 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/ice_server.py
+-rw-r--r--   0        0        0      805 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/idp_metadata_source.py
+-rw-r--r--   0        0        0      329 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/image_format.py
+-rw-r--r--   0        0        0      324 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/import_file.py
+-rw-r--r--   0        0        0      193 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/import_files.py
+-rw-r--r--   0        0        0      237 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/imported_geometry.py
+-rw-r--r--   0        0        0     1772 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/input_format.py
+-rw-r--r--   0        0        0     1387 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/invoice.py
+-rw-r--r--   0        0        0      475 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      503 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0      913 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/ip_addr_info.py
+-rw-r--r--   0        0        0      487 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0      306 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0      348 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0      525 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0      422 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/kcl_code_completion_params.py
+-rw-r--r--   0        0        0      674 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/kcl_code_completion_request.py
+-rw-r--r--   0        0        0      247 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/kcl_code_completion_response.py
+-rw-r--r--   0        0        0      334 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0      428 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/length_unit.py
+-rw-r--r--   0        0        0      239 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/mass.py
+-rw-r--r--   0        0        0      303 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0      573 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1793 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/method.py
+-rw-r--r--   0        0        0      425 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_app_event_type.py
+-rw-r--r--   0        0        0      353 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_app_individual_subscription_tier.py
+-rw-r--r--   0        0        0      378 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_app_organization_subscription_tier.py
+-rw-r--r--   0        0        0     1095 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_app_subscription_tier.py
+-rw-r--r--   0        0        0      476 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_app_subscription_tier_name.py
+-rw-r--r--   0        0        0    30412 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_cmd.py
+-rw-r--r--   0        0        0      488 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_cmd_id.py
+-rw-r--r--   0        0        0      366 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/modeling_cmd_req.py
+-rw-r--r--   0        0        0      278 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/mouse_click.py
+-rw-r--r--   0        0        0      330 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0    16112 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/ok_modeling_cmd_response.py
+-rw-r--r--   0        0        0     3019 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/ok_web_socket_response_data.py
+-rw-r--r--   0        0        0      412 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0      781 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/org.py
+-rw-r--r--   0        0        0      452 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/org_details.py
+-rw-r--r--   0        0        0      735 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/org_member.py
+-rw-r--r--   0        0        0      318 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/org_member_results_page.py
+-rw-r--r--   0        0        0      293 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/org_results_page.py
+-rw-r--r--   0        0        0      458 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/org_role.py
+-rw-r--r--   0        0        0      676 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     2164 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/output_format.py
+-rw-r--r--   0        0        0      333 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_command.py
+-rw-r--r--   0        0        0      332 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_component_constraint_bound.py
+-rw-r--r--   0        0        0      380 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_component_constraint_type.py
+-rw-r--r--   0        0        0      272 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_get_curve_uuids_for_vertices.py
+-rw-r--r--   0        0        0      304 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_get_info.py
+-rw-r--r--   0        0        0      253 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_get_vertex_uuids.py
+-rw-r--r--   0        0        0     1943 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_segment.py
+-rw-r--r--   0        0        0      392 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/path_segment_info.py
+-rw-r--r--   0        0        0      196 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0      576 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0      333 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0      242 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/perspective_camera_parameters.py
+-rw-r--r--   0        0        0      365 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/plan_interval.py
+-rw-r--r--   0        0        0      353 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/plane_intersect_and_project.py
+-rw-r--r--   0        0        0      607 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/ply_storage.py
+-rw-r--r--   0        0        0      241 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/point2d.py
+-rw-r--r--   0        0        0      201 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/point3d.py
+-rw-r--r--   0        0        0      194 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/pong.py
+-rw-r--r--   0        0        0      231 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/post_effect_type.py
+-rw-r--r--   0        0        0      213 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/privacy_settings.py
+-rw-r--r--   0        0        0      326 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/raw_file.py
+-rw-r--r--   0        0        0      371 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/rtc_ice_candidate_init.py
+-rw-r--r--   0        0        0     1369 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/rtc_sdp_type.py
+-rw-r--r--   0        0        0      310 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/rtc_session_description.py
+-rw-r--r--   0        0        0      666 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/saml_identity_provider.py
+-rw-r--r--   0        0        0      548 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/saml_identity_provider_create.py
+-rw-r--r--   0        0        0      398 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/scene_selection_type.py
+-rw-r--r--   0        0        0      413 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/scene_tool_type.py
+-rw-r--r--   0        0        0      235 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/select_get.py
+-rw-r--r--   0        0        0      261 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/select_with_point.py
+-rw-r--r--   0        0        0     1374 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/selection.py
+-rw-r--r--   0        0        0      587 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/service_account.py
+-rw-r--r--   0        0        0      338 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/service_account_results_page.py
+-rw-r--r--   0        0        0      321 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/session.py
+-rw-r--r--   0        0        0      256 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/solid3d_get_all_edge_faces.py
+-rw-r--r--   0        0        0      264 2024-04-05 20:15:40.869496 kittycad-0.6.9/kittycad/models/solid3d_get_all_opposite_edges.py
+-rw-r--r--   0        0        0      391 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/solid3d_get_extrusion_face_info.py
+-rw-r--r--   0        0        0      278 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/solid3d_get_next_adjacent_edge.py
+-rw-r--r--   0        0        0      225 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/solid3d_get_opposite_edge.py
+-rw-r--r--   0        0        0      278 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/solid3d_get_prev_adjacent_edge.py
+-rw-r--r--   0        0        0      323 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/stl_storage.py
+-rw-r--r--   0        0        0      210 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/store_coupon_params.py
+-rw-r--r--   0        0        0      199 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/subscription_tier_feature.py
+-rw-r--r--   0        0        0     1024 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/subscription_tier_price.py
+-rw-r--r--   0        0        0      750 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/subscription_tier_type.py
+-rw-r--r--   0        0        0      583 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/subscription_training_data_behavior.py
+-rw-r--r--   0        0        0      380 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/success_web_socket_response.py
+-rw-r--r--   0        0        0      469 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/support_tier.py
+-rw-r--r--   0        0        0      262 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/surface_area.py
+-rw-r--r--   0        0        0      514 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/system.py
+-rw-r--r--   0        0        0      251 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/take_snapshot.py
+-rw-r--r--   0        0        0      890 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/text_to_cad.py
+-rw-r--r--   0        0        0      206 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/text_to_cad_create_body.py
+-rw-r--r--   0        0        0      319 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/text_to_cad_results_page.py
+-rw-r--r--   0        0        0      377 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_angle.py
+-rw-r--r--   0        0        0      750 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0     1013 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_area.py
+-rw-r--r--   0        0        0      745 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      623 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_current.py
+-rw-r--r--   0        0        0      760 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_current_conversion.py
+-rw-r--r--   0        0        0      322 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_density.py
+-rw-r--r--   0        0        0      934 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_energy.py
+-rw-r--r--   0        0        0      755 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0      916 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_force.py
+-rw-r--r--   0        0        0      750 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      997 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_frequency.py
+-rw-r--r--   0        0        0      770 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_frequency_conversion.py
+-rw-r--r--   0        0        0      708 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_length.py
+-rw-r--r--   0        0        0      755 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0      436 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_mass.py
+-rw-r--r--   0        0        0      745 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1014 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_power.py
+-rw-r--r--   0        0        0      750 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      973 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_pressure.py
+-rw-r--r--   0        0        0      765 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      593 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_temperature.py
+-rw-r--r--   0        0        0      780 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      415 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_torque.py
+-rw-r--r--   0        0        0      755 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_torque_conversion.py
+-rw-r--r--   0        0        0     1131 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_volume.py
+-rw-r--r--   0        0        0      755 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0      261 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/update_member_to_org_body.py
+-rw-r--r--   0        0        0      375 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/update_payment_balance.py
+-rw-r--r--   0        0        0      435 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/update_user.py
+-rw-r--r--   0        0        0      832 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/user.py
+-rw-r--r--   0        0        0      840 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/user_org_info.py
+-rw-r--r--   0        0        0      381 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/user_org_role.py
+-rw-r--r--   0        0        0      297 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0      437 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/uuid.py
+-rw-r--r--   0        0        0      462 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/verification_token_response.py
+-rw-r--r--   0        0        0      251 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/volume.py
+-rw-r--r--   0        0        0     2244 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/web_socket_request.py
+-rw-r--r--   0        0        0      309 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/web_socket_response.py
+-rw-r--r--   0        0        0     1164 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/zoo_product_subscription.py
+-rw-r--r--   0        0        0      321 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/zoo_product_subscriptions.py
+-rw-r--r--   0        0        0      450 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/zoo_product_subscriptions_org_request.py
+-rw-r--r--   0        0        0      436 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/zoo_product_subscriptions_user_request.py
+-rw-r--r--   0        0        0      440 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/models/zoo_tool.py
+-rw-r--r--   0        0        0       26 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/py.typed
+-rw-r--r--   0        0        0     1050 2024-04-05 20:15:40.873497 kittycad-0.6.9/kittycad/types.py
+-rw-r--r--   0        0        0     2606 2024-04-05 20:15:40.873497 kittycad-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 kittycad-0.6.9/PKG-INFO
```

### Comparing `kittycad-0.6.8/LICENSE` & `kittycad-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/README.md` & `kittycad-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/create_kcl_code_completions.py` & `kittycad-0.6.9/kittycad/api/ai/create_kcl_code_completions.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/create_text_to_cad.py` & `kittycad-0.6.9/kittycad/api/ai/create_text_to_cad.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/create_text_to_cad_model_feedback.py` & `kittycad-0.6.9/kittycad/api/ai/create_text_to_cad_model_feedback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/get_ai_prompt.py` & `kittycad-0.6.9/kittycad/api/ai/get_ai_prompt.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/get_text_to_cad_model_for_user.py` & `kittycad-0.6.9/kittycad/api/ai/get_text_to_cad_model_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/list_ai_prompts.py` & `kittycad-0.6.9/kittycad/api/ai/list_ai_prompts.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/ai/list_text_to_cad_models_for_user.py` & `kittycad-0.6.9/kittycad/api/ai/list_text_to_cad_models_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.6.9/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/get_api_call_for_org.py` & `kittycad-0.6.9/kittycad/api/api_calls/get_api_call_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.6.9/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.6.9/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.6.9/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.6.9/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.6.9/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.6.9/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/org_list_api_calls.py` & `kittycad-0.6.9/kittycad/api/api_calls/org_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.6.9/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.6.9/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.6.9/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.6.9/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.6.9/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.6.9/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.6.9/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.6.9/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/executor/create_executor_term.py` & `kittycad-0.6.9/kittycad/api/executor/create_executor_term.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/executor/create_file_execution.py` & `kittycad-0.6.9/kittycad/api/executor/create_file_execution.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(*, response: httpx.Response) -> Optional[Union[CodeOutput, Error]]:
-    if response.status_code == 200:
-        response_200 = CodeOutput(**response.json())
-        return response_200
+    if response.status_code == 201:
+        response_201 = CodeOutput(**response.json())
+        return response_201
     if response.status_code == 400:
         response_4XX = Error(**response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error(**response.json())
         return response_5XX
     return Error(**response.json())
```

### Comparing `kittycad-0.6.8/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.6.9/kittycad/api/file/create_file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/file/create_file_conversion.py` & `kittycad-0.6.9/kittycad/api/file/create_file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/file/create_file_density.py` & `kittycad-0.6.9/kittycad/api/file/create_file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/file/create_file_mass.py` & `kittycad-0.6.9/kittycad/api/file/create_file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.6.9/kittycad/api/file/create_file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/file/create_file_volume.py` & `kittycad-0.6.9/kittycad/api/file/create_file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/hidden/auth_email.py` & `kittycad-0.6.9/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.6.9/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/hidden/get_auth_saml.py` & `kittycad-0.6.9/kittycad/api/hidden/get_auth_saml.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/hidden/logout.py` & `kittycad-0.6.9/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/hidden/post_auth_saml.py` & `kittycad-0.6.9/kittycad/api/hidden/post_auth_saml.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/meta/create_event.py` & `kittycad-0.6.9/kittycad/api/orgs/delete_org_saml_idp.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/events".format(
+    url = "{}/org/saml/idp".format(
         client.base_url,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
@@ -50,27 +50,27 @@
     *,
     client: Client,
 ) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.delete(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Error]:
-    """We collect anonymous telemetry data for improving our product."""  # noqa: E501
+    """This endpoint requires authentication by an org admin."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -78,23 +78,23 @@
     client: Client,
 ) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.delete(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Error]:
-    """We collect anonymous telemetry data for improving our product."""  # noqa: E501
+    """This endpoint requires authentication by an org admin."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/meta/get_ipinfo.py` & `kittycad-0.6.9/kittycad/api/meta/get_ipinfo.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/meta/get_metadata.py` & `kittycad-0.6.9/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/meta/get_pricing_subscriptions.py` & `kittycad-0.6.9/kittycad/api/meta/get_pricing_subscriptions.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/meta/get_schema.py` & `kittycad-0.6.9/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/meta/internal_get_api_token_for_discord_user.py` & `kittycad-0.6.9/kittycad/api/meta/internal_get_api_token_for_discord_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/meta/ping.py` & `kittycad-0.6.9/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/modeling/modeling_commands_ws.py` & `kittycad-0.6.9/kittycad/api/modeling/modeling_commands_ws.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 import json
-from typing import Any, Dict, Iterator
+from typing import Any, Dict, Iterator, Optional
 
 import bson
 from websockets.client import WebSocketClientProtocol, connect as ws_connect_async
 from websockets.sync.client import ClientConnection, connect as ws_connect
 
 from ...client import Client
+from ...models.post_effect_type import PostEffectType
 from ...models.web_socket_request import WebSocketRequest
 from ...models.web_socket_response import WebSocketResponse
 
 
 def _get_kwargs(
     fps: int,
+    post_effect: PostEffectType,
     unlocked_framerate: bool,
     video_res_height: int,
     video_res_width: int,
     webrtc: bool,
     *,
     client: Client,
+    pool: Optional[str] = None,
 ) -> Dict[str, Any]:
     url = "{}/ws/modeling/commands".format(client.base_url)  # noqa: E501
 
     if fps is not None:
 
         if "?" in url:
             url = url + "&fps=" + str(fps)
         else:
             url = url + "?fps=" + str(fps)
 
+    if pool is not None:
+
+        if "?" in url:
+            url = url + "&pool=" + str(pool)
+        else:
+            url = url + "?pool=" + str(pool)
+
+    if post_effect is not None:
+
+        if "?" in url:
+            url = url + "&post_effect=" + str(post_effect)
+        else:
+            url = url + "?post_effect=" + str(post_effect)
+
     if unlocked_framerate is not None:
 
         if "?" in url:
             url = url + "&unlocked_framerate=" + str(unlocked_framerate).lower()
         else:
             url = url + "?unlocked_framerate=" + str(unlocked_framerate).lower()
 
@@ -65,48 +82,56 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def sync(
     fps: int,
+    post_effect: PostEffectType,
     unlocked_framerate: bool,
     video_res_height: int,
     video_res_width: int,
     webrtc: bool,
     *,
     client: Client,
+    pool: Optional[str] = None,
 ) -> ClientConnection:
     """Pass those commands to the engine via websocket, and pass responses back to the client. Basically, this is a websocket proxy between the frontend/client and the engine."""  # noqa: E501
 
     kwargs = _get_kwargs(
         fps=fps,
+        pool=pool,
+        post_effect=post_effect,
         unlocked_framerate=unlocked_framerate,
         video_res_height=video_res_height,
         video_res_width=video_res_width,
         webrtc=webrtc,
         client=client,
     )
 
     return ws_connect(kwargs["url"].replace("http", "ws"), additional_headers=kwargs["headers"], close_timeout=120, max_size=None)  # type: ignore
 
 
 async def asyncio(
     fps: int,
+    post_effect: PostEffectType,
     unlocked_framerate: bool,
     video_res_height: int,
     video_res_width: int,
     webrtc: bool,
     *,
     client: Client,
+    pool: Optional[str] = None,
 ) -> WebSocketClientProtocol:
     """Pass those commands to the engine via websocket, and pass responses back to the client. Basically, this is a websocket proxy between the frontend/client and the engine."""  # noqa: E501
 
     kwargs = _get_kwargs(
         fps=fps,
+        pool=pool,
+        post_effect=post_effect,
         unlocked_framerate=unlocked_framerate,
         video_res_height=video_res_height,
         video_res_width=video_res_width,
         webrtc=webrtc,
         client=client,
     )
 
@@ -122,22 +147,26 @@
     """A websocket connection to the API endpoint."""
 
     ws: ClientConnection
 
     def __init__(
         self,
         fps: int,
+        post_effect: PostEffectType,
         unlocked_framerate: bool,
         video_res_height: int,
         video_res_width: int,
         webrtc: bool,
         client: Client,
+        pool: Optional[str] = None,
     ):
         self.ws = sync(
             fps,
+            pool,
+            post_effect,
             unlocked_framerate,
             video_res_height,
             video_res_width,
             webrtc,
             client=client,
         )
```

### Comparing `kittycad-0.6.8/kittycad/api/orgs/create_org.py` & `kittycad-0.6.9/kittycad/api/orgs/create_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/create_org_member.py` & `kittycad-0.6.9/kittycad/api/orgs/create_org_member.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/create_org_saml_idp.py` & `kittycad-0.6.9/kittycad/api/orgs/create_org_saml_idp.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/delete_org.py` & `kittycad-0.6.9/kittycad/api/orgs/delete_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/delete_org_member.py` & `kittycad-0.6.9/kittycad/api/orgs/delete_org_member.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/delete_org_saml_idp.py` & `kittycad-0.6.9/kittycad/api/orgs/get_org_saml_idp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
+from ...models.saml_identity_provider import SamlIdentityProvider
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
@@ -22,79 +23,85 @@
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Error]:
-    return None
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[SamlIdentityProvider, Error]]:
+    if response.status_code == 200:
+        response_200 = SamlIdentityProvider(**response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error(**response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error(**response.json())
         return response_5XX
     return Error(**response.json())
 
 
-def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
+def _build_response(
+    *, response: httpx.Response
+) -> Response[Optional[Union[SamlIdentityProvider, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Optional[Error]]:
+) -> Response[Optional[Union[SamlIdentityProvider, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
-    response = httpx.delete(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Error]:
+) -> Optional[Union[SamlIdentityProvider, Error]]:
     """This endpoint requires authentication by an org admin."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Optional[Error]]:
+) -> Response[Optional[Union[SamlIdentityProvider, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.delete(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Error]:
+) -> Optional[Union[SamlIdentityProvider, Error]]:
     """This endpoint requires authentication by an org admin."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/orgs/get_any_org.py` & `kittycad-0.6.9/kittycad/api/orgs/get_any_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/get_org.py` & `kittycad-0.6.9/kittycad/api/orgs/get_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/get_org_member.py` & `kittycad-0.6.9/kittycad/api/orgs/get_org_member.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/get_org_privacy_settings.py` & `kittycad-0.6.9/kittycad/api/orgs/get_org_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/get_org_saml_idp.py` & `kittycad-0.6.9/kittycad/api/payments/get_org_subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.saml_identity_provider import SamlIdentityProvider
+from ...models.zoo_product_subscriptions import ZooProductSubscriptions
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/org/saml/idp".format(
+    url = "{}/org/payment/subscriptions".format(
         client.base_url,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
@@ -25,42 +25,42 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[SamlIdentityProvider, Error]]:
+) -> Optional[Union[ZooProductSubscriptions, Error]]:
     if response.status_code == 200:
-        response_200 = SamlIdentityProvider(**response.json())
+        response_200 = ZooProductSubscriptions(**response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error(**response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error(**response.json())
         return response_5XX
     return Error(**response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[SamlIdentityProvider, Error]]]:
+) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[SamlIdentityProvider, Error]]]:
+) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
@@ -68,40 +68,40 @@
 
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[Union[SamlIdentityProvider, Error]]:
-    """This endpoint requires authentication by an org admin."""  # noqa: E501
+) -> Optional[Union[ZooProductSubscriptions, Error]]:
+    """This endpoint requires authentication by an org admin. It gets the subscription for the authenticated user's org."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Optional[Union[SamlIdentityProvider, Error]]]:
+) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[Union[SamlIdentityProvider, Error]]:
-    """This endpoint requires authentication by an org admin."""  # noqa: E501
+) -> Optional[Union[ZooProductSubscriptions, Error]]:
+    """This endpoint requires authentication by an org admin. It gets the subscription for the authenticated user's org."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/orgs/get_user_org.py` & `kittycad-0.6.9/kittycad/api/orgs/get_user_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/list_org_members.py` & `kittycad-0.6.9/kittycad/api/orgs/list_org_members.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/list_orgs.py` & `kittycad-0.6.9/kittycad/api/orgs/list_orgs.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/update_enterprise_pricing_for_org.py` & `kittycad-0.6.9/kittycad/api/orgs/update_enterprise_pricing_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/update_org.py` & `kittycad-0.6.9/kittycad/api/orgs/update_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/update_org_member.py` & `kittycad-0.6.9/kittycad/api/orgs/update_org_member.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/update_org_privacy_settings.py` & `kittycad-0.6.9/kittycad/api/orgs/update_org_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/orgs/update_org_saml_idp.py` & `kittycad-0.6.9/kittycad/api/orgs/update_org_saml_idp.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/create_org_subscription.py` & `kittycad-0.6.9/kittycad/api/payments/create_org_subscription.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/create_payment_information_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/create_payment_information_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/create_payment_intent_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/create_payment_intent_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/create_user_subscription.py` & `kittycad-0.6.9/kittycad/api/payments/create_user_subscription.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/delete_payment_information_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/delete_payment_information_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/delete_payment_method_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/delete_payment_method_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_org_subscription.py` & `kittycad-0.6.9/kittycad/api/payments/get_user_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/org/payment/subscriptions".format(
+    url = "{}/user/payment/subscriptions".format(
         client.base_url,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
@@ -69,15 +69,15 @@
     return _build_response(response=response)
 
 
 def sync(
     *,
     client: Client,
 ) -> Optional[Union[ZooProductSubscriptions, Error]]:
-    """This endpoint requires authentication by an org admin. It gets the subscription for the authenticated user's org."""  # noqa: E501
+    """This endpoint requires authentication by any Zoo user. It gets the subscription for the user."""  # noqa: E501
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
@@ -94,14 +94,14 @@
     return _build_response(response=response)
 
 
 async def asyncio(
     *,
     client: Client,
 ) -> Optional[Union[ZooProductSubscriptions, Error]]:
-    """This endpoint requires authentication by an org admin. It gets the subscription for the authenticated user's org."""  # noqa: E501
+    """This endpoint requires authentication by any Zoo user. It gets the subscription for the user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_any_org.py` & `kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_any_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_any_user.py` & `kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_any_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_payment_information_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/get_payment_information_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/get_user_subscription.py` & `kittycad-0.6.9/kittycad/api/payments/update_user_subscription.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...models.zoo_product_subscriptions import ZooProductSubscriptions
+from ...models.zoo_product_subscriptions_user_request import (
+    ZooProductSubscriptionsUserRequest,
+)
 from ...types import Response
 
 
 def _get_kwargs(
+    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/user/payment/subscriptions".format(
         client.base_url,
     )  # noqa: E501
 
@@ -20,14 +24,15 @@
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "content": body.model_dump_json(),
     }
 
 
 def _parse_response(
     *, response: httpx.Response
 ) -> Optional[Union[ZooProductSubscriptions, Error]]:
     if response.status_code == 200:
@@ -50,58 +55,66 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
 ) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
 ) -> Optional[Union[ZooProductSubscriptions, Error]]:
-    """This endpoint requires authentication by any Zoo user. It gets the subscription for the user."""  # noqa: E501
+    """This endpoint requires authentication by any Zoo user. It updates the subscription for the user."""  # noqa: E501
 
     return sync_detailed(
+        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
 ) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
 ) -> Optional[Union[ZooProductSubscriptions, Error]]:
-    """This endpoint requires authentication by any Zoo user. It gets the subscription for the user."""  # noqa: E501
+    """This endpoint requires authentication by any Zoo user. It updates the subscription for the user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/payments/list_invoices_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/list_invoices_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/list_payment_methods_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/list_payment_methods_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/update_org_subscription.py` & `kittycad-0.6.9/kittycad/api/payments/update_org_subscription.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/update_payment_balance_for_any_org.py` & `kittycad-0.6.9/kittycad/api/payments/update_payment_balance_for_any_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/update_payment_balance_for_any_user.py` & `kittycad-0.6.9/kittycad/api/payments/update_payment_balance_for_any_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/update_payment_information_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/update_payment_information_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/update_user_subscription.py` & `kittycad-0.6.9/kittycad/api/users/get_user_onboarding_self.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,120 +1,105 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.zoo_product_subscriptions import ZooProductSubscriptions
-from ...models.zoo_product_subscriptions_user_request import (
-    ZooProductSubscriptionsUserRequest,
-)
+from ...models.onboarding import Onboarding
 from ...types import Response
 
 
 def _get_kwargs(
-    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/payment/subscriptions".format(
+    url = "{}/user/onboarding".format(
         client.base_url,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "content": body.model_dump_json(),
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[ZooProductSubscriptions, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[Onboarding, Error]]:
     if response.status_code == 200:
-        response_200 = ZooProductSubscriptions(**response.json())
+        response_200 = Onboarding(**response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error(**response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error(**response.json())
         return response_5XX
     return Error(**response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
-) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     kwargs = _get_kwargs(
-        body=body,
         client=client,
     )
 
-    response = httpx.put(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
-) -> Optional[Union[ZooProductSubscriptions, Error]]:
-    """This endpoint requires authentication by any Zoo user. It updates the subscription for the user."""  # noqa: E501
+) -> Optional[Union[Onboarding, Error]]:
+    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
 
     return sync_detailed(
-        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
-) -> Response[Optional[Union[ZooProductSubscriptions, Error]]]:
+) -> Response[Optional[Union[Onboarding, Error]]]:
     kwargs = _get_kwargs(
-        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.put(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: ZooProductSubscriptionsUserRequest,
     *,
     client: Client,
-) -> Optional[Union[ZooProductSubscriptions, Error]]:
-    """This endpoint requires authentication by any Zoo user. It updates the subscription for the user."""  # noqa: E501
+) -> Optional[Union[Onboarding, Error]]:
+    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/payments/validate_customer_tax_information_for_org.py` & `kittycad-0.6.9/kittycad/api/payments/validate_customer_tax_information_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.6.9/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/service_accounts/create_service_account_for_org.py` & `kittycad-0.6.9/kittycad/api/service_accounts/create_service_account_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/service_accounts/delete_service_account_for_org.py` & `kittycad-0.6.9/kittycad/api/service_accounts/delete_service_account_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/service_accounts/get_service_account_for_org.py` & `kittycad-0.6.9/kittycad/api/service_accounts/get_service_account_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/service_accounts/list_service_accounts_for_org.py` & `kittycad-0.6.9/kittycad/api/service_accounts/list_service_accounts_for_org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/store/create_store_coupon.py` & `kittycad-0.6.9/kittycad/api/store/create_store_coupon.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_current_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_current_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_frequency_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_frequency_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_torque_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_torque_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.6.9/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/delete_user_self.py` & `kittycad-0.6.9/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_oauth2_providers_for_user.py` & `kittycad-0.6.9/kittycad/api/users/get_oauth2_providers_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_session_for_user.py` & `kittycad-0.6.9/kittycad/api/users/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_user.py` & `kittycad-0.6.9/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_user_extended.py` & `kittycad-0.6.9/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.6.9/kittycad/api/users/update_user_self.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,116 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.onboarding import Onboarding
+from ...models.update_user import UpdateUser
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
+    body: UpdateUser,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/onboarding".format(
+    url = "{}/user".format(
         client.base_url,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "content": body.model_dump_json(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Onboarding, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
     if response.status_code == 200:
-        response_200 = Onboarding(**response.json())
+        response_200 = User(**response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error(**response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error(**response.json())
         return response_5XX
     return Error(**response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[Onboarding, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Optional[Union[Onboarding, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
-    response = httpx.get(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[Onboarding, Error]]:
-    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any Zoo user. It updates information about the authenticated user."""  # noqa: E501
 
     return sync_detailed(
+        body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Optional[Union[Onboarding, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
+        body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.get(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[Onboarding, Error]]:
-    """Checks key part of their api usage to determine their onboarding progress"""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any Zoo user. It updates information about the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
+            body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/api/users/get_user_privacy_settings.py` & `kittycad-0.6.9/kittycad/api/users/get_user_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_user_self.py` & `kittycad-0.6.9/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.6.9/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/list_users.py` & `kittycad-0.6.9/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/list_users_extended.py` & `kittycad-0.6.9/kittycad/api/users/list_users_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/update_user_privacy_settings.py` & `kittycad-0.6.9/kittycad/api/users/update_user_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/api/users/update_user_self.py` & `kittycad-0.6.9/kittycad/api/meta/create_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.update_user import UpdateUser
-from ...models.user import User
+from ...models.event import Event
 from ...types import Response
 
 
 def _get_kwargs(
-    body: UpdateUser,
+    body: Event,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(
+    url = "{}/events".format(
         client.base_url,
     )  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
@@ -26,91 +25,87 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body.model_dump_json(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
-    if response.status_code == 200:
-        response_200 = User(**response.json())
-        return response_200
+def _parse_response(*, response: httpx.Response) -> Optional[Error]:
+    return None
     if response.status_code == 400:
         response_4XX = Error(**response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error(**response.json())
         return response_5XX
     return Error(**response.json())
 
 
-def _build_response(
-    *, response: httpx.Response
-) -> Response[Optional[Union[User, Error]]]:
+def _build_response(*, response: httpx.Response) -> Response[Optional[Error]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: UpdateUser,
+    body: Event,
     *,
     client: Client,
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
-    response = httpx.put(
+    response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: UpdateUser,
+    body: Event,
     *,
     client: Client,
-) -> Optional[Union[User, Error]]:
-    """This endpoint requires authentication by any Zoo user. It updates information about the authenticated user."""  # noqa: E501
+) -> Optional[Error]:
+    """We collect anonymous telemetry data for improving our product."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: UpdateUser,
+    body: Event,
     *,
     client: Client,
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Error]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.put(**kwargs)
+        response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: UpdateUser,
+    body: Event,
     *,
     client: Client,
-) -> Optional[Union[User, Error]]:
-    """This endpoint requires authentication by any Zoo user. It updates information about the authenticated user."""  # noqa: E501
+) -> Optional[Error]:
+    """We collect anonymous telemetry data for improving our product."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.6.8/kittycad/client.py` & `kittycad-0.6.9/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/client_test.py` & `kittycad-0.6.9/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/examples_test.py` & `kittycad-0.6.9/kittycad/examples_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
     Org,
     OrgMember,
     OrgMemberResultsPage,
     OrgResultsPage,
     PaymentIntent,
     PaymentMethod,
     Pong,
-    PrivacySettings,
     SamlIdentityProvider,
     ServiceAccount,
     ServiceAccountResultsPage,
     Session,
     TextToCad,
     TextToCadResultsPage,
     UnitAngleConversion,
@@ -218,27 +217,31 @@
 from kittycad.models.ai_feedback import AiFeedback
 from kittycad.models.api_call_query_group_by import ApiCallQueryGroupBy
 from kittycad.models.api_call_status import ApiCallStatus
 from kittycad.models.billing_info import BillingInfo
 from kittycad.models.code_language import CodeLanguage
 from kittycad.models.created_at_sort_mode import CreatedAtSortMode
 from kittycad.models.email_authentication_form import EmailAuthenticationForm
+from kittycad.models.event import modeling_app_event
 from kittycad.models.file_export_format import FileExportFormat
 from kittycad.models.file_import_format import FileImportFormat
 from kittycad.models.idp_metadata_source import base64_encoded_xml
 from kittycad.models.kcl_code_completion_params import KclCodeCompletionParams
 from kittycad.models.kcl_code_completion_request import KclCodeCompletionRequest
+from kittycad.models.modeling_app_event_type import ModelingAppEventType
 from kittycad.models.modeling_app_individual_subscription_tier import (
     ModelingAppIndividualSubscriptionTier,
 )
 from kittycad.models.modeling_app_organization_subscription_tier import (
     ModelingAppOrganizationSubscriptionTier,
 )
 from kittycad.models.org_details import OrgDetails
 from kittycad.models.plan_interval import PlanInterval
+from kittycad.models.post_effect_type import PostEffectType
+from kittycad.models.privacy_settings import PrivacySettings
 from kittycad.models.rtc_sdp_type import RtcSdpType
 from kittycad.models.rtc_session_description import RtcSessionDescription
 from kittycad.models.saml_identity_provider_create import SamlIdentityProviderCreate
 from kittycad.models.store_coupon_params import StoreCouponParams
 from kittycad.models.subscription_tier_price import per_user
 from kittycad.models.text_to_cad_create_body import TextToCadCreateBody
 from kittycad.models.unit_angle import UnitAngle
@@ -1275,43 +1278,71 @@
 @pytest.mark.skip
 def test_create_event():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Error] = create_event.sync(
         client=client,
+        body=modeling_app_event(
+            created_at="<string>",
+            event_type=ModelingAppEventType.SUCCESSFUL_COMPILE_BEFORE_CLOSE,
+            project_name="<string>",
+            source_id="<uuid>",
+            user_id="<string>",
+        ),
     )
 
     if isinstance(result, Error) or result is None:
         print(result)
         raise Exception("Error in response")
 
     body: Error = result
     print(body)
 
     # OR if you need more info (e.g. status_code)
     response: Response[Optional[Error]] = create_event.sync_detailed(
         client=client,
+        body=modeling_app_event(
+            created_at="<string>",
+            event_type=ModelingAppEventType.SUCCESSFUL_COMPILE_BEFORE_CLOSE,
+            project_name="<string>",
+            source_id="<uuid>",
+            user_id="<string>",
+        ),
     )
 
 
 # OR run async
 @pytest.mark.asyncio
 @pytest.mark.skip
 async def test_create_event_async():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Error] = await create_event.asyncio(
         client=client,
+        body=modeling_app_event(
+            created_at="<string>",
+            event_type=ModelingAppEventType.SUCCESSFUL_COMPILE_BEFORE_CLOSE,
+            project_name="<string>",
+            source_id="<uuid>",
+            user_id="<string>",
+        ),
     )
 
     # OR run async with more info
     response: Response[Optional[Error]] = await create_event.asyncio_detailed(
         client=client,
+        body=modeling_app_event(
+            created_at="<string>",
+            event_type=ModelingAppEventType.SUCCESSFUL_COMPILE_BEFORE_CLOSE,
+            project_name="<string>",
+            source_id="<uuid>",
+            user_id="<string>",
+        ),
     )
 
 
 @pytest.mark.skip
 def test_create_file_center_of_mass():
     # Create our client.
     client = ClientFromEnv()
@@ -6728,18 +6759,20 @@
     # Create our client.
     client = ClientFromEnv()
 
     # Connect to the websocket.
     with modeling_commands_ws.WebSocket(
         client=client,
         fps=10,
+        post_effect=PostEffectType.PHOSPHOR,
         unlocked_framerate=False,
         video_res_height=10,
         video_res_width=10,
         webrtc=False,
+        pool=None,  # Optional[str]
     ) as websocket:
 
         # Send a message.
         websocket.send(
             WebSocketRequest(
                 sdp_offer(
                     offer=RtcSessionDescription(
@@ -6762,18 +6795,20 @@
     # Create our client.
     client = ClientFromEnv()
 
     # Connect to the websocket.
     websocket = await modeling_commands_ws.asyncio(
         client=client,
         fps=10,
+        post_effect=PostEffectType.PHOSPHOR,
         unlocked_framerate=False,
         video_res_height=10,
         video_res_width=10,
         webrtc=False,
+        pool=None,  # Optional[str]
     )
 
     # Send a message.
     await websocket.send("{}")
 
     # Get the messages.
     async for message in websocket:
```

### Comparing `kittycad-0.6.8/kittycad/models/__init__.py` & `kittycad-0.6.9/kittycad/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from .currency import Currency
 from .curve_get_control_points import CurveGetControlPoints
 from .curve_get_end_points import CurveGetEndPoints
 from .curve_get_type import CurveGetType
 from .curve_type import CurveType
 from .customer import Customer
 from .customer_balance import CustomerBalance
+from .default_camera_focus_on import DefaultCameraFocusOn
 from .default_camera_get_settings import DefaultCameraGetSettings
 from .default_camera_zoom import DefaultCameraZoom
 from .density import Density
 from .der_encoded_key_pair import DerEncodedKeyPair
 from .device_access_token_request_form import DeviceAccessTokenRequestForm
 from .device_auth_request_form import DeviceAuthRequestForm
 from .device_auth_verify_params import DeviceAuthVerifyParams
@@ -76,14 +77,15 @@
 from .entity_get_num_children import EntityGetNumChildren
 from .entity_get_parent_id import EntityGetParentId
 from .entity_linear_pattern import EntityLinearPattern
 from .entity_type import EntityType
 from .environment import Environment
 from .error import Error
 from .error_code import ErrorCode
+from .event import Event
 from .export import Export
 from .export_file import ExportFile
 from .extended_user import ExtendedUser
 from .extended_user_results_page import ExtendedUserResultsPage
 from .extrusion_face_cap_type import ExtrusionFaceCapType
 from .extrusion_face_info import ExtrusionFaceInfo
 from .face_get_gradient import FaceGetGradient
@@ -98,24 +100,26 @@
 from .file_import_format import FileImportFormat
 from .file_mass import FileMass
 from .file_surface_area import FileSurfaceArea
 from .file_system_metadata import FileSystemMetadata
 from .file_volume import FileVolume
 from .gateway import Gateway
 from .get_entity_type import GetEntityType
+from .get_num_objects import GetNumObjects
 from .get_sketch_mode_plane import GetSketchModePlane
 from .global_axis import GlobalAxis
 from .gltf_presentation import GltfPresentation
 from .gltf_storage import GltfStorage
 from .highlight_set_entity import HighlightSetEntity
 from .ice_server import IceServer
 from .idp_metadata_source import IdpMetadataSource
 from .image_format import ImageFormat
 from .import_file import ImportFile
 from .import_files import ImportFiles
+from .imported_geometry import ImportedGeometry
 from .input_format import InputFormat
 from .invoice import Invoice
 from .invoice_line_item import InvoiceLineItem
 from .invoice_status import InvoiceStatus
 from .ip_addr_info import IpAddrInfo
 from .jetstream import Jetstream
 from .jetstream_api_stats import JetstreamApiStats
@@ -126,14 +130,15 @@
 from .kcl_code_completion_response import KclCodeCompletionResponse
 from .leaf_node import LeafNode
 from .length_unit import LengthUnit
 from .mass import Mass
 from .meta_cluster_info import MetaClusterInfo
 from .metadata import Metadata
 from .method import Method
+from .modeling_app_event_type import ModelingAppEventType
 from .modeling_app_individual_subscription_tier import (
     ModelingAppIndividualSubscriptionTier,
 )
 from .modeling_app_organization_subscription_tier import (
     ModelingAppOrganizationSubscriptionTier,
 )
 from .modeling_app_subscription_tier import ModelingAppSubscriptionTier
@@ -170,14 +175,15 @@
 from .perspective_camera_parameters import PerspectiveCameraParameters
 from .plan_interval import PlanInterval
 from .plane_intersect_and_project import PlaneIntersectAndProject
 from .ply_storage import PlyStorage
 from .point2d import Point2d
 from .point3d import Point3d
 from .pong import Pong
+from .post_effect_type import PostEffectType
 from .privacy_settings import PrivacySettings
 from .raw_file import RawFile
 from .rtc_ice_candidate_init import RtcIceCandidateInit
 from .rtc_sdp_type import RtcSdpType
 from .rtc_session_description import RtcSessionDescription
 from .saml_identity_provider import SamlIdentityProvider
 from .saml_identity_provider_create import SamlIdentityProviderCreate
```

### Comparing `kittycad-0.6.8/kittycad/models/account_provider.py` & `kittycad-0.6.9/kittycad/models/account_provider.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/ai_prompt.py` & `kittycad-0.6.9/kittycad/models/ai_prompt.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/annotation_options.py` & `kittycad-0.6.9/kittycad/models/annotation_options.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/api_call_query_group_by.py` & `kittycad-0.6.9/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/api_call_status.py` & `kittycad-0.6.9/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/api_call_with_price.py` & `kittycad-0.6.9/kittycad/models/api_call_with_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/async_api_call.py` & `kittycad-0.6.9/kittycad/models/async_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/async_api_call_output.py` & `kittycad-0.6.9/kittycad/models/async_api_call_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/async_api_call_type.py` & `kittycad-0.6.9/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/base64data.py` & `kittycad-0.6.9/kittycad/models/base64data.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/card_details.py` & `kittycad-0.6.9/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/code_language.py` & `kittycad-0.6.9/kittycad/models/code_language.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/code_output.py` & `kittycad-0.6.9/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/connection.py` & `kittycad-0.6.9/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/currency.py` & `kittycad-0.6.9/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/customer.py` & `kittycad-0.6.9/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/customer_balance.py` & `kittycad-0.6.9/kittycad/models/customer_balance.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/distance_type.py` & `kittycad-0.6.9/kittycad/models/distance_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/environment.py` & `kittycad-0.6.9/kittycad/models/environment.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/error_code.py` & `kittycad-0.6.9/kittycad/models/error_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/extended_user.py` & `kittycad-0.6.9/kittycad/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_center_of_mass.py` & `kittycad-0.6.9/kittycad/models/file_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_conversion.py` & `kittycad-0.6.9/kittycad/models/file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_density.py` & `kittycad-0.6.9/kittycad/models/file_density.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_export_format.py` & `kittycad-0.6.9/kittycad/models/file_export_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_import_format.py` & `kittycad-0.6.9/kittycad/models/file_import_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_mass.py` & `kittycad-0.6.9/kittycad/models/file_mass.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_surface_area.py` & `kittycad-0.6.9/kittycad/models/file_surface_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/file_volume.py` & `kittycad-0.6.9/kittycad/models/file_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/gltf_storage.py` & `kittycad-0.6.9/kittycad/models/gltf_storage.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/idp_metadata_source.py` & `kittycad-0.6.9/kittycad/models/idp_metadata_source.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/input_format.py` & `kittycad-0.6.9/kittycad/models/input_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/invoice.py` & `kittycad-0.6.9/kittycad/models/invoice.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/ip_addr_info.py` & `kittycad-0.6.9/kittycad/models/ip_addr_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/jetstream_stats.py` & `kittycad-0.6.9/kittycad/models/jetstream_stats.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/kcl_code_completion_request.py` & `kittycad-0.6.9/kittycad/models/kcl_code_completion_request.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/metadata.py` & `kittycad-0.6.9/kittycad/models/metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/method.py` & `kittycad-0.6.9/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/modeling_app_subscription_tier.py` & `kittycad-0.6.9/kittycad/models/modeling_app_subscription_tier.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/modeling_cmd.py` & `kittycad-0.6.9/kittycad/models/modeling_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Literal, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, RootModel
 from typing_extensions import Annotated
 
+from ..models.angle import Angle
 from ..models.annotation_options import AnnotationOptions
 from ..models.annotation_type import AnnotationType
 from ..models.camera_drag_interaction_type import CameraDragInteractionType
 from ..models.color import Color
 from ..models.distance_type import DistanceType
 from ..models.entity_type import EntityType
 from ..models.image_format import ImageFormat
@@ -59,27 +60,63 @@
 
     type: Literal["extend_path"] = "extend_path"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class extrude(BaseModel):
-    """Command for extruding a solid."""
+    """Command for extruding a solid 2d."""
 
     cap: bool
 
     distance: LengthUnit
 
     target: ModelingCmdId
 
     type: Literal["extrude"] = "extrude"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class revolve(BaseModel):
+    """Command for revolving a solid 2d."""
+
+    angle: Angle
+
+    axis: Point3d
+
+    axis_is_2d: bool
+
+    origin: Point3d
+
+    target: ModelingCmdId
+
+    tolerance: LengthUnit
+
+    type: Literal["revolve"] = "revolve"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
+class revolve_about_edge(BaseModel):
+    """Command for revolving a solid 2d about a brep edge"""
+
+    angle: Angle
+
+    edge_id: str
+
+    target: ModelingCmdId
+
+    tolerance: LengthUnit
+
+    type: Literal["revolve_about_edge"] = "revolve_about_edge"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 class close_path(BaseModel):
     """Closes a path, converting it to a 2D solid."""
 
     path_id: str
 
     type: Literal["close_path"] = "close_path"
 
@@ -217,16 +254,14 @@
 class export(BaseModel):
     """Export the scene to a file."""
 
     entity_ids: List[str]
 
     format: OutputFormat
 
-    source_unit: UnitLength
-
     type: Literal["export"] = "export"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class entity_get_parent_id(BaseModel):
     """What is this entity's parent?"""
@@ -281,15 +316,15 @@
 
     type: Literal["entity_get_distance"] = "entity_get_distance"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class entity_linear_pattern(BaseModel):
-    """Create a linear pattern using this entity (currently only valid for 3D solids)."""
+    """Create a linear pattern using this entity."""
 
     axis: Point3d
 
     entity_id: str
 
     num_repetitions: int
 
@@ -297,15 +332,15 @@
 
     type: Literal["entity_linear_pattern"] = "entity_linear_pattern"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class entity_circular_pattern(BaseModel):
-    """Create a circular pattern using this entity (currently only valid for 3D solids)."""
+    """Create a circular pattern using this entity."""
 
     arc_degrees: float
 
     axis: Point3d
 
     center: Point3d
 
@@ -316,14 +351,32 @@
     rotate_duplicates: bool
 
     type: Literal["entity_circular_pattern"] = "entity_circular_pattern"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class entity_make_helix(BaseModel):
+    """Create a helix using the input cylinder and other specified parameters."""
+
+    cylinder_id: str
+
+    is_clockwise: bool
+
+    length: LengthUnit
+
+    revolutions: float
+
+    start_angle: Angle
+
+    type: Literal["entity_make_helix"] = "entity_make_helix"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 class edit_mode_enter(BaseModel):
     """Enter edit mode"""
 
     target: str
 
     type: Literal["edit_mode_enter"] = "edit_mode_enter"
 
@@ -358,14 +411,22 @@
     entities: List[str]
 
     type: Literal["select_remove"] = "select_remove"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class scene_clear_all(BaseModel):
+    """Removes all of the Objects in the scene"""
+
+    type: Literal["scene_clear_all"] = "scene_clear_all"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 class select_replace(BaseModel):
     """Replaces current selection with these entities (by UUID)."""
 
     entities: List[str]
 
     type: Literal["select_replace"] = "select_replace"
 
@@ -760,14 +821,44 @@
     ortho: bool
 
     type: Literal["enable_sketch_mode"] = "enable_sketch_mode"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class set_background_color(BaseModel):
+    """Set the background color of the scene."""
+
+    color: Color
+
+    type: Literal["set_background_color"] = "set_background_color"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
+class set_current_tool_properties(BaseModel):
+    """Set the properties of the tool lines for the scene."""
+
+    color: Optional[Color] = None
+
+    type: Literal["set_current_tool_properties"] = "set_current_tool_properties"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
+class set_default_system_properties(BaseModel):
+    """Set the default system properties used when a specific property isn't set."""
+
+    color: Optional[Color] = None
+
+    type: Literal["set_default_system_properties"] = "set_default_system_properties"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 class curve_get_type(BaseModel):
     """Get type of the given curve."""
 
     curve_id: str
 
     type: Literal["curve_get_type"] = "curve_get_type"
 
@@ -947,16 +1038,14 @@
 
     material_density: float
 
     material_density_unit: UnitDensity
 
     output_unit: UnitMass
 
-    source_unit: UnitLength
-
     type: Literal["mass"] = "mass"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class density(BaseModel):
     """Get the density of entities in the scene or the default scene."""
@@ -965,58 +1054,50 @@
 
     material_mass: float
 
     material_mass_unit: UnitMass
 
     output_unit: UnitDensity
 
-    source_unit: UnitLength
-
     type: Literal["density"] = "density"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class volume(BaseModel):
     """Get the volume of entities in the scene or the default scene."""
 
     entity_ids: List[str]
 
     output_unit: UnitVolume
 
-    source_unit: UnitLength
-
     type: Literal["volume"] = "volume"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class center_of_mass(BaseModel):
     """Get the center of mass of entities in the scene or the default scene."""
 
     entity_ids: List[str]
 
     output_unit: UnitLength
 
-    source_unit: UnitLength
-
     type: Literal["center_of_mass"] = "center_of_mass"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class surface_area(BaseModel):
     """Get the surface area of entities in the scene or the default scene."""
 
     entity_ids: List[str]
 
     output_unit: UnitArea
 
-    source_unit: UnitLength
-
     type: Literal["surface_area"] = "surface_area"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class default_camera_focus_on(BaseModel):
     """Focus the default camera upon an object in the scene."""
@@ -1098,21 +1179,31 @@
     """Find all IDs of selected entities"""
 
     type: Literal["select_get"] = "select_get"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class get_num_objects(BaseModel):
+    """Get the number of objects in the scene"""
+
+    type: Literal["get_num_objects"] = "get_num_objects"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 ModelingCmd = RootModel[
     Annotated[
         Union[
             start_path,
             move_path_pen,
             extend_path,
             extrude,
+            revolve,
+            revolve_about_edge,
             close_path,
             camera_drag_start,
             camera_drag_move,
             camera_drag_end,
             default_camera_get_settings,
             default_camera_look_at,
             default_camera_perspective_settings,
@@ -1123,18 +1214,20 @@
             entity_get_parent_id,
             entity_get_num_children,
             entity_get_child_uuid,
             entity_get_all_child_uuids,
             entity_get_distance,
             entity_linear_pattern,
             entity_circular_pattern,
+            entity_make_helix,
             edit_mode_enter,
             select_with_point,
             select_add,
             select_remove,
+            scene_clear_all,
             select_replace,
             highlight_set_entity,
             highlight_set_entities,
             new_annotation,
             update_annotation,
             object_visible,
             object_bring_to_front,
@@ -1159,14 +1252,17 @@
             mouse_move,
             mouse_click,
             sketch_mode_enable,
             sketch_mode_disable,
             get_sketch_mode_plane,
             curve_set_constraint,
             enable_sketch_mode,
+            set_background_color,
+            set_current_tool_properties,
+            set_default_system_properties,
             curve_get_type,
             curve_get_control_points,
             take_snapshot,
             make_axes_gizmo,
             path_get_info,
             path_get_curve_uuids_for_vertices,
             path_get_vertex_uuids,
@@ -1189,11 +1285,12 @@
             set_selection_filter,
             default_camera_set_orthographic,
             default_camera_set_perspective,
             solid3d_get_extrusion_face_info,
             edit_mode_exit,
             select_clear,
             select_get,
+            get_num_objects,
         ],
         Field(discriminator="type"),
     ]
 ]
```

### Comparing `kittycad-0.6.8/kittycad/models/ok_modeling_cmd_response.py` & `kittycad-0.6.9/kittycad/models/ok_modeling_cmd_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ..models.camera_drag_end import CameraDragEnd
 from ..models.camera_drag_move import CameraDragMove
 from ..models.center_of_mass import CenterOfMass
 from ..models.curve_get_control_points import CurveGetControlPoints
 from ..models.curve_get_end_points import CurveGetEndPoints
 from ..models.curve_get_type import CurveGetType
+from ..models.default_camera_focus_on import DefaultCameraFocusOn
 from ..models.default_camera_get_settings import DefaultCameraGetSettings
 from ..models.default_camera_zoom import DefaultCameraZoom
 from ..models.density import Density
 from ..models.entity_circular_pattern import EntityCircularPattern
 from ..models.entity_get_all_child_uuids import EntityGetAllChildUuids
 from ..models.entity_get_child_uuid import EntityGetChildUuid
 from ..models.entity_get_distance import EntityGetDistance
@@ -21,17 +22,19 @@
 from ..models.entity_linear_pattern import EntityLinearPattern
 from ..models.export import Export
 from ..models.extrusion_face_info import ExtrusionFaceInfo
 from ..models.face_get_gradient import FaceGetGradient
 from ..models.face_get_position import FaceGetPosition
 from ..models.face_is_planar import FaceIsPlanar
 from ..models.get_entity_type import GetEntityType
+from ..models.get_num_objects import GetNumObjects
 from ..models.get_sketch_mode_plane import GetSketchModePlane
 from ..models.highlight_set_entity import HighlightSetEntity
 from ..models.import_files import ImportFiles
+from ..models.imported_geometry import ImportedGeometry
 from ..models.mass import Mass
 from ..models.mouse_click import MouseClick
 from ..models.path_get_curve_uuids_for_vertices import PathGetCurveUuidsForVertices
 from ..models.path_get_info import PathGetInfo
 from ..models.path_get_vertex_uuids import PathGetVertexUuids
 from ..models.path_segment_info import PathSegmentInfo
 from ..models.plane_intersect_and_project import PlaneIntersectAndProject
@@ -162,14 +165,34 @@
     data: DefaultCameraZoom
 
     type: Literal["default_camera_zoom"] = "default_camera_zoom"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class get_num_objects(BaseModel):
+    """The response to the 'GetNumObjects' endpoint"""
+
+    data: GetNumObjects
+
+    type: Literal["get_num_objects"] = "get_num_objects"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
+class default_camera_focus_on(BaseModel):
+    """The response to the 'DefaultCameraFocusOn' endpoint"""
+
+    data: DefaultCameraFocusOn
+
+    type: Literal["default_camera_focus_on"] = "default_camera_focus_on"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 class select_get(BaseModel):
     """The response to the 'SelectGet' endpoint"""
 
     data: SelectGet
 
     type: Literal["select_get"] = "select_get"
 
@@ -374,14 +397,24 @@
     data: ImportFiles
 
     type: Literal["import_files"] = "import_files"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
+class imported_geometry(BaseModel):
+    """The response to the 'ImportedGeometry' endpoint"""
+
+    data: ImportedGeometry
+
+    type: Literal["imported_geometry"] = "imported_geometry"
+
+    model_config = ConfigDict(protected_namespaces=())
+
+
 class mass(BaseModel):
     """The response to the 'Mass' endpoint"""
 
     data: Mass
 
     type: Literal["mass"] = "mass"
 
@@ -499,14 +532,16 @@
             entity_get_num_children,
             entity_get_parent_id,
             entity_get_all_child_uuids,
             camera_drag_move,
             camera_drag_end,
             default_camera_get_settings,
             default_camera_zoom,
+            get_num_objects,
+            default_camera_focus_on,
             select_get,
             solid3d_get_all_edge_faces,
             solid3d_get_all_opposite_edges,
             solid3d_get_opposite_edge,
             solid3d_get_next_adjacent_edge,
             solid3d_get_prev_adjacent_edge,
             get_entity_type,
@@ -520,14 +555,15 @@
             path_get_vertex_uuids,
             curve_get_end_points,
             face_is_planar,
             face_get_position,
             face_get_gradient,
             plane_intersect_and_project,
             import_files,
+            imported_geometry,
             mass,
             volume,
             density,
             surface_area,
             center_of_mass,
             get_sketch_mode_plane,
             entity_get_distance,
```

### Comparing `kittycad-0.6.8/kittycad/models/ok_web_socket_response_data.py` & `kittycad-0.6.9/kittycad/models/ok_web_socket_response_data.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/org.py` & `kittycad-0.6.9/kittycad/models/org.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/org_member.py` & `kittycad-0.6.9/kittycad/models/org_member.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/output_file.py` & `kittycad-0.6.9/kittycad/models/output_file.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/output_format.py` & `kittycad-0.6.9/kittycad/models/output_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/path_segment.py` & `kittycad-0.6.9/kittycad/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/payment_method.py` & `kittycad-0.6.9/kittycad/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/ply_storage.py` & `kittycad-0.6.9/kittycad/models/ply_storage.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/rtc_sdp_type.py` & `kittycad-0.6.9/kittycad/models/rtc_sdp_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/saml_identity_provider.py` & `kittycad-0.6.9/kittycad/models/saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/saml_identity_provider_create.py` & `kittycad-0.6.9/kittycad/models/saml_identity_provider_create.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/selection.py` & `kittycad-0.6.9/kittycad/models/selection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/service_account.py` & `kittycad-0.6.9/kittycad/models/service_account.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/subscription_tier_price.py` & `kittycad-0.6.9/kittycad/models/subscription_tier_price.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/subscription_tier_type.py` & `kittycad-0.6.9/kittycad/models/subscription_tier_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/subscription_training_data_behavior.py` & `kittycad-0.6.9/kittycad/models/subscription_training_data_behavior.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/system.py` & `kittycad-0.6.9/kittycad/models/system.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/text_to_cad.py` & `kittycad-0.6.9/kittycad/models/text_to_cad.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_angle_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_angle_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_area.py` & `kittycad-0.6.9/kittycad/models/unit_area.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_area_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_area_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_current.py` & `kittycad-0.6.9/kittycad/models/unit_current.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_current_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_current_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_energy.py` & `kittycad-0.6.9/kittycad/models/unit_energy.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_energy_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_energy_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_force.py` & `kittycad-0.6.9/kittycad/models/unit_force.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_force_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_force_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_frequency.py` & `kittycad-0.6.9/kittycad/models/unit_frequency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_frequency_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_frequency_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_length.py` & `kittycad-0.6.9/kittycad/models/unit_length.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_length_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_length_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_mass_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_mass_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_power.py` & `kittycad-0.6.9/kittycad/models/unit_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_power_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_power_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_pressure.py` & `kittycad-0.6.9/kittycad/models/unit_pressure.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_pressure_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_temperature.py` & `kittycad-0.6.9/kittycad/models/unit_temperature.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_temperature_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_torque_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_torque_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_volume.py` & `kittycad-0.6.9/kittycad/models/unit_volume.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/unit_volume_conversion.py` & `kittycad-0.6.9/kittycad/models/unit_volume_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/user.py` & `kittycad-0.6.9/kittycad/models/user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/user_org_info.py` & `kittycad-0.6.9/kittycad/models/user_org_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/models/web_socket_request.py` & `kittycad-0.6.9/kittycad/models/web_socket_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal, Union
+from typing import List, Literal, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, RootModel
 from typing_extensions import Annotated
 
 from ..models.client_metrics import ClientMetrics
 from ..models.modeling_cmd import ModelingCmd
 from ..models.modeling_cmd_id import ModelingCmdId
@@ -42,16 +42,20 @@
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class modeling_cmd_batch_req(BaseModel):
     """A sequence of modeling requests. If any request fails, following requests will not be tried."""
 
+    batch_id: ModelingCmdId
+
     requests: List[ModelingCmdReq]
 
+    responses: Optional[bool] = None
+
     type: Literal["modeling_cmd_batch_req"] = "modeling_cmd_batch_req"
 
     model_config = ConfigDict(protected_namespaces=())
 
 
 class ping(BaseModel):
     """The client-to-server Ping to ensure the WebSocket stays alive."""
```

### Comparing `kittycad-0.6.8/kittycad/models/zoo_product_subscription.py` & `kittycad-0.6.9/kittycad/models/zoo_product_subscription.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/kittycad/types.py` & `kittycad-0.6.9/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.6.8/pyproject.toml` & `kittycad-0.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.6.8"
+version = "0.6.9"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
```

### Comparing `kittycad-0.6.8/PKG-INFO` & `kittycad-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.6.8
+Version: 0.6.9
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

