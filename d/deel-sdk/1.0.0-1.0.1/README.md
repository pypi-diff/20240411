# Comparing `tmp/deel-sdk-1.0.0.tar.gz` & `tmp/deel-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deel-sdk-1.0.0.tar", last modified: Tue Apr  9 11:23:21 2024, max compression
+gzip compressed data, was "deel-sdk-1.0.1.tar", last modified: Thu Apr 11 17:56:01 2024, max compression
```

## Comparing `deel-sdk-1.0.0.tar` & `deel-sdk-1.0.1.tar`

### file list

```diff
@@ -1,461 +1,462 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.358072 deel-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   189193 2024-04-09 11:23:21.358072 deel-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)   188987 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:23:21.358072 deel-sdk-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.282071 deel-sdk-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.282071 deel-sdk-1.0.0/src/deel_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.286072 deel-sdk-1.0.0/src/deel_sdk/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)    24826 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/add_worker_bank_account_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/additional_eor_info_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_created_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustments_categories_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/adjustments_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/admin_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/admin_user_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/admin_user_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/admin_users_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/agreement_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/alternate_email_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/attachment_file_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_added.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_added_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_guide.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_guide_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_to_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_to_add_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_updated_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/bank_account_value_allowed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/basic_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/basic_invoice_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/basic_legal_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/basic_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/basic_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/basic_timesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/benefit_contribution_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/benefit_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/breakdown_costs_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/calculate_final_payment_calculation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/candidate_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/candidate_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/candidate_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/candidate_to_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/candidate_to_patch_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/client_of_basic_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/client_of_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/client_of_contract_legal_entity_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/compensation_details_of_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_container_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_container_payg_milestones.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_container_payg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_details_to_amend.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_document_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_external_id_to_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_invitation_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_invitation_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_signature_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_signature_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_template_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_template_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_termination_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_termination_result_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_amend_details_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_payg_milestones.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_payg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_payg_milestones.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_payg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_terminate.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_to_terminate_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_type_enum_for_estimate.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contract_who_reports_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contracts_sort_by_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/cost_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/country.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/country_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_admin_user_response_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_people_timeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_public_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_public_token_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_timeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_timeoff_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/create_webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/currency_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/deel_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/deel_invoice_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/departments.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/departments_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/download_worker_documents_by_id_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_agreement_download_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_agreement_download_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_contract_signature_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_contract_signature_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_payslips_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_payslips_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_tax_documents_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_tax_documents_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_creation_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_entitlements_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_entitlements_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_policies_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_policies_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/employment_details_of_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_client_timeoff_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_client_timeoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_client_timeoffs_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_benefits.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_benefits_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_created_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_country_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_country_validations_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_entitlement_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_entitlements.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_entitlements_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_holidays_rollover_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_payslip_download_url_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_payslips_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_quote_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_base_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_employee_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_item_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/equity_stakeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/equity_stakeholders_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/estimate_first_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/estimate_first_payment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/file_attachment_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/file_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/file_ref_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/final_payment_calculated.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/final_payment_calculated_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/first_payment_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/generic_result_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/generic_result_created_with_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/generic_result_deleted.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/generic_result_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/get_contract_list_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/get_employee_compliance_documents_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/get_payment_list_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/global_payroll_g2_n_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/global_payroll_g2_n_report_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_created_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_salary_scale_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_salary_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_status_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_update_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_updated_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_update_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_updated_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_information_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_information_update_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_information_updated_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_pto_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_pto_update_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_payroll_event_report_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_payroll_event_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_payslip_download_url_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/gp_payslips_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/health_insurance_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hiring_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hr_document_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_compensation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_contract_full_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_contract_part_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_job_information_title_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_job_information_title_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/hris_team_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/identifier_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/input_to_create_file_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/input_to_create_pgo_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/input_to_patch_contract_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/internal_people.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/internal_people_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invitations_of_basic_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_created_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_review_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_download_link_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_download_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/invoice_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/job_title.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/job_title_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/legal_entity_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/legal_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/letter_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/marital_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/meta_data_of_contract_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_review_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_review_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_reviews_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/milestone_to_create_form_with_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/monthly_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/organization_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/output_to_create_file_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/output_to_create_file_ref_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/page_info_without_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/page_info_without_cursor_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/patch_webhook_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_break_down.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_break_down_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_method_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payment_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payroll_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payslip_download_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/payslips.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pension_eor_contract_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pension_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_by_id_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_client_legal_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_sort_by_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/people_time_off_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pgo_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pgo_task_reviews_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pgo_task_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/premium_result_added.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/premium_result_added_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/premium_to_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/premium_to_add_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/pro_rata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/profile_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/public_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/public_token_created_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/request_custom_verification_letter_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/request_custom_verification_letter_with_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/requester_time_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/response_estimate_first_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/response_estimate_first_payment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/salary_frequency_scale_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/seniority.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/seniority_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/seniority_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/signatures_of_basic_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/signatures_of_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/sort_dir_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/state_of_country.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/task_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/task_created_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/task_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/team.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/team_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/team_of_basic_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/team_of_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoff_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoff_review_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoff_to_review_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoff_to_review_internal_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoff_type_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_attachments_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_approver.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_id_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_list_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_review_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_review_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_reviews_to_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_shared_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_create_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_create_container_with_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_update_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/update_worker_department.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/update_worker_department_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/update_worker_working_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/update_worker_working_location_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/upload_employee_compliance_document_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/upload_employee_compliance_document_file_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/utils/json_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/validation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/validation_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/webhook_event_type_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/webhook_event_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/webhook_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/webhook_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/webhook_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/week_days_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/work_statement_cycle_end_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/work_statement_cycle_scale_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/work_statement_payment_due_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/work_statement_scale_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_bank_account_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_bank_account_to_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_bank_accounts_info_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_document_download_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_documents_by_id_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_legal_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_of_basic_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_of_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_termination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_termination_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_termination_body_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/worker_termination_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/working_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/models/working_locations_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/net/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/headers/access_token_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.350072 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.354072 deel-sdk-1.0.0/src/deel_sdk/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.358072 deel-sdk-1.0.0/src/deel_sdk/services/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/carta.py
--rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/contractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22181 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/eor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19010 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/global_payroll.py
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/invoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/lookups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/milestones.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/off_cycle_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    22375 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/partner_managed.py
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/people.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/time_off.py
--rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/timesheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.358072 deel-sdk-1.0.0/src/deel_sdk/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/utils/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-09 11:23:11.000000 deel-sdk-1.0.0/src/deel_sdk/services/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:23:21.358072 deel-sdk-1.0.0/src/deel_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)   189193 2024-04-09 11:23:21.000000 deel-sdk-1.0.0/src/deel_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-09 11:23:21.000000 deel-sdk-1.0.0/src/deel_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:23:21.000000 deel-sdk-1.0.0/src/deel_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 11:23:21.000000 deel-sdk-1.0.0/src/deel_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 11:23:21.000000 deel-sdk-1.0.0/src/deel_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1057 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)   189900 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)   189694 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)      343 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.293900 deel-sdk-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.293900 deel-sdk-1.0.1/src/deel_sdk/
+-rw-r--r--   0 runner    (1001) runner    (1001)      125 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.293900 deel-sdk-1.0.1/src/deel_sdk/hooks/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      918 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/models/
+-rw-r--r--   0 runner    (1001) runner    (1001)    24919 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      516 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/add_worker_bank_account_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/additional_eor_info_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1314 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1049 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      849 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2583 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1302 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustments_categories_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustments_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      659 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_user_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_user_create_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_users_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/agreement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      753 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/agreement_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      484 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/alternate_email_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      338 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/attachment_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1254 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_added.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      476 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_added_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1639 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_guide.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_guide_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      699 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_to_add_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_value_allowed.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10358 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3817 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6686 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_invoice_adjustment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1092 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      426 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      410 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_team.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6231 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_timesheet.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      712 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/benefit_contribution_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      650 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/benefit_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1246 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/breakdown_costs_quote.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      916 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/calculate_final_payment_calculation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      838 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2215 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_patch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      502 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_patch_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/client_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1456 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract_legal_entity_5.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1661 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3559 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6134 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      418 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      456 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      446 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      436 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      631 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_custom_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5768 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_details_to_amend.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_document_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_external_id_to_patch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_invitation_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_invitation_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      637 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      540 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2449 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      730 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_template.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_template_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      598 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_template_summary.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      784 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      539 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      581 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_amend_details_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1034 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      831 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      591 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      541 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12731 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12848 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9214 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8828 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1047 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_terminate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      497 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_terminate_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1827 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum_for_estimate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_who_reports_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contracts_sort_by_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1068 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contribution.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1020 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/cost_quote.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1368 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/country.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      453 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/country_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_admin_user_response_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1731 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_people_timeoff.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_public_token.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_public_token_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2762 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_timeoff.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_timeoff_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1942 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_webhook_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      417 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/currency.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      460 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/currency_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1206 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      546 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/departments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      473 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/departments_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      549 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/download_worker_documents_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/email.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9643 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      660 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      386 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_contract_signature_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      597 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_contract_signature_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1796 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1078 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      567 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      553 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_creation_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      651 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3302 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6384 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8435 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      619 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2975 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5398 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7421 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employment_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1396 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employment_details_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2006 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoff_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoffs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9335 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13109 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13924 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_country_validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_country_validations_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1468 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      635 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5990 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4905 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlement_list_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      603 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlements.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlements_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1232 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      937 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_holidays_rollover_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      496 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_payslip_download_url_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      466 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6857 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_quote_base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5045 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_base_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      530 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1724 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_employee_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_item_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      676 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholders_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6024 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      582 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/file_attachment_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/file_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      879 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/file_ref_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/first_payment_date.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      852 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created_with_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      643 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_deleted.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      303 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_contract_list_currencies.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1238 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_documents_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_invoice_list_entities.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      301 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_payment_list_currencies.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_payment_list_entities.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5154 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      990 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7859 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      638 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      685 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      617 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_status_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5709 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      491 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      551 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1372 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      932 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1584 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      602 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      579 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2127 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      577 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      523 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      544 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_report_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      845 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_reports.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      494 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payslip_download_url_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5236 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/health_insurance_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      653 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hiring_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      414 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hr_document_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      542 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_compensation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2037 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_full_time.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2244 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_part_time.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3477 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1109 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3797 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_job_information_title_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      521 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_job_information_title_name.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      485 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_team_information.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      241 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/identifier_value.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      882 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/input_to_create_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/input_to_create_pgo_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/input_to_patch_contract_external_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8507 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/internal_people.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/internal_people_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invitations_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2528 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      503 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_attachment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1336 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      798 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1229 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      583 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1553 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      590 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      949 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1640 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1840 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3514 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1131 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      507 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_download_link_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      347 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_download_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      687 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      961 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      545 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/job_title.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      805 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/job_title_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      572 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2378 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/letter_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1056 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/marital_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      728 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/meta_data_of_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2354 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      467 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_properties.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      492 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      800 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_to_create_form_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      427 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/monthly_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2137 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      469 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      804 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      563 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/organization_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      385 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/output_to_create_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      513 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/output_to_create_file_ref_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      423 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/page_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      359 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/page_info_without_cursor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      601 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/page_info_without_cursor_new.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2010 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/patch_webhook_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1828 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6179 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_break_down.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_break_down_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_method.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1794 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_method_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      664 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      854 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_worker.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4715 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payroll_adjustment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      307 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payslip_download_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      645 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payslips.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      913 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pension_eor_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1290 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pension_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10185 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      736 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_client_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      750 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_custom_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_me.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1095 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1801 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_sort_by_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2067 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_time_off_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1471 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1282 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1349 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1105 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2885 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_result_added.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_result_added_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2487 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_to_add_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3499 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pro_rata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1008 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/profile_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/public_token.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/public_token_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_custom_verification_letter_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2920 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_custom_verification_letter_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2999 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/requester_time_off.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1029 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      914 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/salary_frequency_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      835 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/seniority.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      508 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/seniority_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      774 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/seniority_required.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1129 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/sort_dir_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/state_of_country.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1011 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/task_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      440 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/task_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/task_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      571 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1270 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review_internal.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_to_review_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      515 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_to_review_internal_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      361 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_type_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1006 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_attachments_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1300 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_profile.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      648 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6364 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_approver.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      249 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_id_items.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      711 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1520 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      939 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_shared_properties.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      608 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      568 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      397 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_department.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_department_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_working_location.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_working_location_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/upload_employee_compliance_document_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      406 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/upload_employee_compliance_document_file_container.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/models/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2636 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2642 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/utils/json_map.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/validation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/validation_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      625 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_list_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1682 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2910 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      438 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_item_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      472 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_list_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/week_days_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      776 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_end_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      895 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      666 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_payment_due_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      988 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5945 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5328 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_accounts_info_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1317 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_document.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      618 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_document_download_link.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_documents_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      806 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1237 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3079 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1140 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_body_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/working_locations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/working_locations_container.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/environment/
+-rw-r--r--   0 runner    (1001) runner    (1001)       96 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      396 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/headers/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1184 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/headers/access_token_auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      225 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1221 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1704 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2592 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2452 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1835 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/transport/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2704 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1692 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2304 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8604 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      681 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5090 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/src/deel_sdk/services/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8586 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/accounting.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7738 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/adjustments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/candidates.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1641 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/carta.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12960 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/contractors.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22181 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/contracts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7352 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/eor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19010 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/global_payroll.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17310 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/invoices.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5044 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/lookups.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2584 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/managers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8032 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4151 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/off_cycle_payments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/organizations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22375 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/partner_managed.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18569 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/people.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7063 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8293 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/time_off.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14194 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/timesheets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1385 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/token.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/src/deel_sdk/services/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2256 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1603 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8007 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/utils/validator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5237 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/webhooks.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/src/deel_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)   189900 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    21372 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       17 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/top_level.txt
```

### Comparing `deel-sdk-1.0.0/LICENSE` & `deel-sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/PKG-INFO` & `deel-sdk-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: deel-sdk
-Version: 1.0.0
-Summary: Deel REST API
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# DeelSdk Python SDK 1.0.0
+# DeelSdk Python SDK 1.0.1
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.0
+- SDK version: 1.0.1
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
+- [Environments](#environments)
 - [Using Union Types in Function Parameters](#using-union-types-in-function-parameters)
 - [Services](#services)
 
 ## Installation
 
 ```bash
 pip install deel-sdk
@@ -46,14 +37,31 @@
 
 Or at a later stage:
 
 ```py
 sdk.set_access_token("YOUR_ACCESS_TOKEN")
 ```
 
+## Environments
+
+Here is the list of all available environment variables:
+
+```py
+Demo = "https://api-staging.letsdeel.com/rest/v2"
+Production = "https://api.letsdeel.com/rest/v2"
+```
+
+Here is how you set an environment:
+
+```py
+from deel_sdk import Environment
+
+sdk.set_base_url(Environment.Demo.value)
+```
+
 ## Using Union Types in Function Parameters
 
 In Python, a parameter can be annotated with a Union type, indicating it can accept values of multiple types.
 
 ### Passing Instances or Dictionaries
 
 When we have a model such as:
@@ -132,36 +140,42 @@
 - Endpoint: `/invoices`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | issued_from_date | str | ❌ | Retrieve a list of paid invoices for your workforce. |
 | issued_to_date | str | ❌ | Retrieve a list of paid invoices for your workforce. |
+| entities | GetInvoiceListEntities | ❌ | Retrieve a list of paid invoices for your workforce. |
 | limit | float | ❌ | Retrieve a list of paid invoices for your workforce. |
 | offset | float | ❌ | Retrieve a list of paid invoices for your workforce. |
 
 **Return Type**
 
 `InvoiceListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import GetInvoiceListEntities
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
+entities=GetInvoiceListEntities(**[
+    "individual"
+])
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
+    entities=entities,
     limit=10,
-    offset=808037660.53
+    offset=707020693.68
 )
 
 print(result)
 ```
 
 #### **get_deel_invoice_list**
 
@@ -169,14 +183,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/invoices/deel`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Retrieve a list of invoices related to Deel fees. |
 | limit | float | ❌ | Retrieve a list of invoices related to Deel fees. |
 | offset | float | ❌ | Retrieve a list of invoices related to Deel fees. |
 
 **Return Type**
 
 `DeelInvoiceListContainer`
 
@@ -187,16 +202,17 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.accounting.get_deel_invoice_list(
+    contract_id="contract_id",
     limit=10,
-    offset=237799437.03
+    offset=898896522.23
 )
 
 print(result)
 ```
 
 #### **get_billing_invoice_download_link**
 
@@ -238,34 +254,34 @@
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | date_from | str | ❌ | Retrieve a list of payments made to Deel. |
 | date_to | str | ❌ | Retrieve a list of payments made to Deel. |
 | currencies | GetPaymentListCurrencies | ❌ | Retrieve a list of payments made to Deel. |
-| entities | Entities | ❌ | Retrieve a list of payments made to Deel. |
+| entities | GetPaymentListEntities | ❌ | Retrieve a list of payments made to Deel. |
 
 **Return Type**
 
 `PaymentListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetPaymentListCurrencies, Entities
+from deel_sdk.models import GetPaymentListCurrencies, GetPaymentListEntities
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 currencies=GetPaymentListCurrencies(**[
     "GBP"
 ])
-entities=Entities(**[
+entities=GetPaymentListEntities(**[
     "individual"
 ])
 
 result = sdk.accounting.get_payment_list(
     date_from="1999-12-31",
     date_to="1999-12-31",
     currencies=currencies,
@@ -375,16 +391,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdminUserCreateContainer(**{
     "data": {
-        "first_name": "dolore",
-        "last_name": "proi",
+        "first_name": "proident molli",
+        "last_name": "anim ci",
         "email": "email"
     }
 })
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
@@ -445,36 +461,36 @@
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
     "team_information": {
-        "team_id": 9.77,
-        "legal_entity_id": 2.18
+        "team_id": 1.64,
+        "legal_entity_id": 2.97
     },
     "job_information": {
-        "seniority_id": 9.22,
-        "job_title_id": 6.5
+        "seniority_id": 1.14,
+        "job_title_id": 6.17
     },
     "compensation": {
-        "gross_annual_salary": 7.15,
+        "gross_annual_salary": 5.95,
         "currency": "USD"
     },
     "contract": {
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 9.02,
+        "employee_number": 3.49,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 21.67
+        "part_time_percentage": 75.13
     },
     "vacation_info": {
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 171.07
+        "vacation_yearly_policy": 295.88
     }
 })
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
@@ -503,16 +519,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=978653984.34,
-    limit=43.45
+    offset=92741896.72,
+    limit=88.8
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -525,15 +541,15 @@
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | offset | float | ❌ | Retrieve a list of People in your organization. |
 | limit | float | ❌ | Retrieve a list of People in your organization. |
 | search | str | ❌ | Retrieve a list of People in your organization. |
 | sort_by | PeopleSortByEnum | ❌ | Retrieve a list of People in your organization. |
 | sort_order | SortDirEnum | ❌ | Retrieve a list of People in your organization. |
-| hiring_statuses[] | HiringStatusEnum | ❌ | Retrieve a list of People in your organization. |
+| hiring_statuses | HiringStatusEnum | ❌ | Retrieve a list of People in your organization. |
 
 **Return Type**
 
 `PeopleContainer`
 
 **Example Usage Code Snippet**
 
@@ -543,16 +559,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=44334375.53,
-    limit=105.69,
+    offset=311381742.98,
+    limit=139.17,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -1195,38 +1211,38 @@
                 "country": "US"
             }
         },
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
-            "work_visa_required": False,
+            "work_visa_required": True,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 6.17,
+            "probation_period": 2.27,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 5.67
+            "holidays": 4.71
         },
         "job_title": "job_title",
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
-            "salary": 5.95,
+            "salary": 0.96,
             "currency": "currency",
-            "variable_compensation": 3.49,
+            "variable_compensation": 6.36,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
@@ -1293,46 +1309,46 @@
 )
 
 request_body = GpContractToCreateContainer(**{
     "data": {
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "culpa Lorem inc",
-            "work_email": "in do L",
+            "email": "ipsum ad tempor",
+            "work_email": "Lorem ullamco ",
             "nationality": "US",
             "employee_number": "100",
             "address": {
                 "street": "Deel Street 500",
                 "city": "Denver",
                 "state": "CO",
                 "zip": "44000",
                 "country": "US"
             }
         },
         "employment": {
             "type_": "Full-time",
             "start_date": "1999-12-31",
             "holidays": {
-                "allowance": 5.28,
+                "allowance": 1.94,
                 "start_date": "1999-12-31"
             }
         },
         "job_title": "job_title",
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
             "scale": "YEAR",
-            "salary": 8.05,
+            "salary": 2.33,
             "currency": "GBP"
         }
     }
 })
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
@@ -1978,35 +1994,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "name": "adquis culpa reprehenderit sed in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "ametnos",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 3.56,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2064,28 +2080,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "enim irure dolore magna"
+            "name": "nulla"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis nulla oc",
+            "expected_email": "Duis esse ex",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2149,28 +2165,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "et dolore"
+            "name": "mollit"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "sint ",
+            "expected_email": "proid",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2234,35 +2250,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "cillum"
+            "name": "Lorem"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Lorem sint et",
+            "expected_email": "anim sit",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 7.36,
+            "amount": 6.09,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2320,35 +2336,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "name": "adquis culpa reprehenderit sed in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "ametnos",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 3.56,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2372,15 +2388,15 @@
 - HTTP Method: `GET`
 - Endpoint: `/contracts/{contract_id}/preview`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | contract_id | str | ✅ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
-| templateId | str | ❌ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
+| template_id | str | ❌ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
 
 **Return Type**
 
 `str`
 
 **Example Usage Code Snippet**
 
@@ -2432,21 +2448,21 @@
 request_body = ContractToAmendDetailsContainer(**{
     "data": {
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 0.24,
+        "first_payment": 8.79,
         "frequency": "weekly",
-        "cycle_end": 24.94,
+        "cycle_end": 28.13,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 0.92,
-        "pay_before_weekends": True,
+        "payment_due_days": 6.51,
+        "pay_before_weekends": False,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
 })
@@ -2621,20 +2637,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat exe",
+        "amount": "cupidatat cil",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "qu",
+        "file": "nisi nulla",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2700,18 +2716,18 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdjustmentToUpdateContainer(**{
     "data": {
-        "amount": "ut velit in",
+        "amount": "proident",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "incididunt "
+        "file": "enim repr"
     }
 })
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
@@ -2824,16 +2840,16 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/contracts/{contract_id}/adjustments`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Get all adjustments for the specific contract. |
-| from | str | ❌ | Get all adjustments for the specific contract. |
+| contract*id | str | ✅ | Get all adjustments for the specific contract. |
+| from* | str | ❌ | Get all adjustments for the specific contract. |
 | to | str | ❌ | Get all adjustments for the specific contract. |
 
 **Return Type**
 
 `AdjustmentsContainer`
 
 **Example Usage Code Snippet**
@@ -2896,15 +2912,15 @@
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "dolore",
+        "email": "sunt ullamco es",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.add_candidate(request_body=request_body)
@@ -2944,15 +2960,15 @@
     "data": {
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "Excepteur nu",
+        "email": "laboris a",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.patch_candidate(
@@ -3055,15 +3071,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EmployeeContractSignatureToCreateContainer(**{
     "data": {
-        "signature": "aliqua sed comm"
+        "signature": "inci"
     }
 })
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
@@ -3099,15 +3115,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = RequestCustomVerificationLetterContainer(**{
     "data": {
-        "description": "magnaest ea con",
+        "description": "Excepteur Duisi",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
 })
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
@@ -3180,15 +3196,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=1.72
+    document_id=5.13
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3514,15 +3530,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=1.36
+    document_id=3.06
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3549,15 +3565,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.91
+    document_id=5.72
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3888,16 +3904,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractSignatureToCreateContainer(**{
     "data": {
-        "client_signature": "ea exercitat",
-        "contract_template_id": 8.35
+        "client_signature": "proident e",
+        "contract_template_id": 1.32
     }
 })
 
 result = sdk.contracts.sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -3962,16 +3978,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractInvitationToCreateContainer(**{
     "data": {
-        "email": "eiusm",
-        "message": "officia ut"
+        "email": "dolore c",
+        "message": "mini"
     }
 })
 
 result = sdk.contracts.invite_to_sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -4084,18 +4100,18 @@
         "type_": "ongoing_time_based",
         "country_code": "US",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 2500,
             "currency_code": "GBP",
             "scale": "weekly",
-            "cycle_end": 30.28,
+            "cycle_end": 18.59,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
-            "payment_due_days": 11.81,
+            "payment_due_days": 36.88,
             "calculation_type": "CUSTOM_AMOUNT",
             "work_week_start": "Sunday",
             "work_week_end": "Sunday"
         }
     }
 })
 
@@ -4190,15 +4206,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.contracts.get_download_worker_documents_by_id(
     worker_id="worker_id",
-    document_id=8.43
+    document_id=1.09
 )
 
 print(result)
 ```
 
 ### TasksService
 
@@ -4477,15 +4493,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=564786626.18
+    offset=97685509.73
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4530,15 +4546,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=911169937.96
+    offset=90326358.62
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4639,15 +4655,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = TimesheetToUpdateContainer(**{
     "data": {
         "description": "description",
-        "quantity": 3.77
+        "quantity": 9.63
     }
 })
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
@@ -4761,15 +4777,15 @@
 )
 
 request_body = TimesheetReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            6.19
         ]
     }
 })
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
@@ -5007,15 +5023,15 @@
 )
 
 request_body = MilestoneReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.78
+            1.74
         ]
     }
 })
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
@@ -5218,17 +5234,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": True,
+        "with_multiple_dates": False,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
@@ -5268,17 +5284,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": True,
+        "with_multiple_dates": False,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
@@ -5493,15 +5509,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=226515477.25
+    offset=560002501.34
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5553,15 +5569,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=240522187.51
+    offset=729203388.82
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5594,21 +5610,21 @@
 request_body = InvoiceAdjustmentToCreateContainer(**{
     "data": {
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 6.69
+        "payment_cycle_id": 5.08
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
-    recurring=False
+    recurring=True
 )
 
 print(result)
 ```
 
 #### **update_invoice_adjustment_by_id**
 
@@ -5636,16 +5652,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = InvoiceAdjustmentToUpdateContainer(**{
     "data": {
-        "description": "sunt laborum Duis exercitation id",
-        "amount": 9.39
+        "description": "aute veniam in fugiat",
+        "amount": 2.65
     }
 })
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
@@ -5759,15 +5775,15 @@
 )
 
 request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            6.19
         ]
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
@@ -5823,15 +5839,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/legal-entities`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| type | str | ❌ | Retrieve a list of legal entities in your account. |
+| type\_ | str | ❌ | Retrieve a list of legal entities in your account. |
 
 **Return Type**
 
 `LegalEntityListContainer`
 
 **Example Usage Code Snippet**
 
@@ -6266,15 +6282,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| id | str | ✅ | Retrieve a single webhook subscription. |
+| id\_ | str | ✅ | Retrieve a single webhook subscription. |
 
 **Return Type**
 
 `WebhookItemResponse`
 
 **Example Usage Code Snippet**
 
@@ -6297,16 +6313,16 @@
 
 - HTTP Method: `PATCH`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| request_body | PatchWebhookRequest | ✅ | The request body. |
-| id | str | ✅ | Edit a webhook subscription. |
+| request*body | PatchWebhookRequest | ✅ | The request body. |
+| id* | str | ✅ | Edit a webhook subscription. |
 
 **Return Type**
 
 `WebhookItemResponse`
 
 **Example Usage Code Snippet**
 
@@ -6345,15 +6361,15 @@
 
 - HTTP Method: `DELETE`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| id | str | ✅ | Delete a webhook subscription. |
+| id\_ | str | ✅ | Delete a webhook subscription. |
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
 
 sdk = DeelSdk(
```

### Comparing `deel-sdk-1.0.0/README.md` & `deel-sdk-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,31 @@
-# DeelSdk Python SDK 1.0.0
+Metadata-Version: 2.1
+Name: deel-sdk
+Version: 1.0.1
+Summary: Deel REST API
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# DeelSdk Python SDK 1.0.1
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.0
+- SDK version: 1.0.1
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
+- [Environments](#environments)
 - [Using Union Types in Function Parameters](#using-union-types-in-function-parameters)
 - [Services](#services)
 
 ## Installation
 
 ```bash
 pip install deel-sdk
@@ -36,14 +47,31 @@
 
 Or at a later stage:
 
 ```py
 sdk.set_access_token("YOUR_ACCESS_TOKEN")
 ```
 
+## Environments
+
+Here is the list of all available environment variables:
+
+```py
+Demo = "https://api-staging.letsdeel.com/rest/v2"
+Production = "https://api.letsdeel.com/rest/v2"
+```
+
+Here is how you set an environment:
+
+```py
+from deel_sdk import Environment
+
+sdk.set_base_url(Environment.Demo.value)
+```
+
 ## Using Union Types in Function Parameters
 
 In Python, a parameter can be annotated with a Union type, indicating it can accept values of multiple types.
 
 ### Passing Instances or Dictionaries
 
 When we have a model such as:
@@ -122,36 +150,42 @@
 - Endpoint: `/invoices`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | issued_from_date | str | ❌ | Retrieve a list of paid invoices for your workforce. |
 | issued_to_date | str | ❌ | Retrieve a list of paid invoices for your workforce. |
+| entities | GetInvoiceListEntities | ❌ | Retrieve a list of paid invoices for your workforce. |
 | limit | float | ❌ | Retrieve a list of paid invoices for your workforce. |
 | offset | float | ❌ | Retrieve a list of paid invoices for your workforce. |
 
 **Return Type**
 
 `InvoiceListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import GetInvoiceListEntities
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
+entities=GetInvoiceListEntities(**[
+    "individual"
+])
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
+    entities=entities,
     limit=10,
-    offset=808037660.53
+    offset=707020693.68
 )
 
 print(result)
 ```
 
 #### **get_deel_invoice_list**
 
@@ -159,14 +193,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/invoices/deel`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Retrieve a list of invoices related to Deel fees. |
 | limit | float | ❌ | Retrieve a list of invoices related to Deel fees. |
 | offset | float | ❌ | Retrieve a list of invoices related to Deel fees. |
 
 **Return Type**
 
 `DeelInvoiceListContainer`
 
@@ -177,16 +212,17 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.accounting.get_deel_invoice_list(
+    contract_id="contract_id",
     limit=10,
-    offset=237799437.03
+    offset=898896522.23
 )
 
 print(result)
 ```
 
 #### **get_billing_invoice_download_link**
 
@@ -228,34 +264,34 @@
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | date_from | str | ❌ | Retrieve a list of payments made to Deel. |
 | date_to | str | ❌ | Retrieve a list of payments made to Deel. |
 | currencies | GetPaymentListCurrencies | ❌ | Retrieve a list of payments made to Deel. |
-| entities | Entities | ❌ | Retrieve a list of payments made to Deel. |
+| entities | GetPaymentListEntities | ❌ | Retrieve a list of payments made to Deel. |
 
 **Return Type**
 
 `PaymentListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetPaymentListCurrencies, Entities
+from deel_sdk.models import GetPaymentListCurrencies, GetPaymentListEntities
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 currencies=GetPaymentListCurrencies(**[
     "GBP"
 ])
-entities=Entities(**[
+entities=GetPaymentListEntities(**[
     "individual"
 ])
 
 result = sdk.accounting.get_payment_list(
     date_from="1999-12-31",
     date_to="1999-12-31",
     currencies=currencies,
@@ -365,16 +401,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdminUserCreateContainer(**{
     "data": {
-        "first_name": "dolore",
-        "last_name": "proi",
+        "first_name": "proident molli",
+        "last_name": "anim ci",
         "email": "email"
     }
 })
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
@@ -435,36 +471,36 @@
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
     "team_information": {
-        "team_id": 9.77,
-        "legal_entity_id": 2.18
+        "team_id": 1.64,
+        "legal_entity_id": 2.97
     },
     "job_information": {
-        "seniority_id": 9.22,
-        "job_title_id": 6.5
+        "seniority_id": 1.14,
+        "job_title_id": 6.17
     },
     "compensation": {
-        "gross_annual_salary": 7.15,
+        "gross_annual_salary": 5.95,
         "currency": "USD"
     },
     "contract": {
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 9.02,
+        "employee_number": 3.49,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 21.67
+        "part_time_percentage": 75.13
     },
     "vacation_info": {
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 171.07
+        "vacation_yearly_policy": 295.88
     }
 })
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
@@ -493,16 +529,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=978653984.34,
-    limit=43.45
+    offset=92741896.72,
+    limit=88.8
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -515,15 +551,15 @@
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | offset | float | ❌ | Retrieve a list of People in your organization. |
 | limit | float | ❌ | Retrieve a list of People in your organization. |
 | search | str | ❌ | Retrieve a list of People in your organization. |
 | sort_by | PeopleSortByEnum | ❌ | Retrieve a list of People in your organization. |
 | sort_order | SortDirEnum | ❌ | Retrieve a list of People in your organization. |
-| hiring_statuses[] | HiringStatusEnum | ❌ | Retrieve a list of People in your organization. |
+| hiring_statuses | HiringStatusEnum | ❌ | Retrieve a list of People in your organization. |
 
 **Return Type**
 
 `PeopleContainer`
 
 **Example Usage Code Snippet**
 
@@ -533,16 +569,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=44334375.53,
-    limit=105.69,
+    offset=311381742.98,
+    limit=139.17,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -1185,38 +1221,38 @@
                 "country": "US"
             }
         },
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
-            "work_visa_required": False,
+            "work_visa_required": True,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 6.17,
+            "probation_period": 2.27,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 5.67
+            "holidays": 4.71
         },
         "job_title": "job_title",
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
-            "salary": 5.95,
+            "salary": 0.96,
             "currency": "currency",
-            "variable_compensation": 3.49,
+            "variable_compensation": 6.36,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
@@ -1283,46 +1319,46 @@
 )
 
 request_body = GpContractToCreateContainer(**{
     "data": {
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "culpa Lorem inc",
-            "work_email": "in do L",
+            "email": "ipsum ad tempor",
+            "work_email": "Lorem ullamco ",
             "nationality": "US",
             "employee_number": "100",
             "address": {
                 "street": "Deel Street 500",
                 "city": "Denver",
                 "state": "CO",
                 "zip": "44000",
                 "country": "US"
             }
         },
         "employment": {
             "type_": "Full-time",
             "start_date": "1999-12-31",
             "holidays": {
-                "allowance": 5.28,
+                "allowance": 1.94,
                 "start_date": "1999-12-31"
             }
         },
         "job_title": "job_title",
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
             "scale": "YEAR",
-            "salary": 8.05,
+            "salary": 2.33,
             "currency": "GBP"
         }
     }
 })
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
@@ -1968,35 +2004,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "name": "adquis culpa reprehenderit sed in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "ametnos",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 3.56,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2054,28 +2090,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "enim irure dolore magna"
+            "name": "nulla"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis nulla oc",
+            "expected_email": "Duis esse ex",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2139,28 +2175,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "et dolore"
+            "name": "mollit"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "sint ",
+            "expected_email": "proid",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2224,35 +2260,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "cillum"
+            "name": "Lorem"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Lorem sint et",
+            "expected_email": "anim sit",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 7.36,
+            "amount": 6.09,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2310,35 +2346,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "name": "adquis culpa reprehenderit sed in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "ametnos",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 3.56,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2362,15 +2398,15 @@
 - HTTP Method: `GET`
 - Endpoint: `/contracts/{contract_id}/preview`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | contract_id | str | ✅ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
-| templateId | str | ❌ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
+| template_id | str | ❌ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
 
 **Return Type**
 
 `str`
 
 **Example Usage Code Snippet**
 
@@ -2422,21 +2458,21 @@
 request_body = ContractToAmendDetailsContainer(**{
     "data": {
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 0.24,
+        "first_payment": 8.79,
         "frequency": "weekly",
-        "cycle_end": 24.94,
+        "cycle_end": 28.13,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 0.92,
-        "pay_before_weekends": True,
+        "payment_due_days": 6.51,
+        "pay_before_weekends": False,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
 })
@@ -2611,20 +2647,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat exe",
+        "amount": "cupidatat cil",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "qu",
+        "file": "nisi nulla",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2690,18 +2726,18 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdjustmentToUpdateContainer(**{
     "data": {
-        "amount": "ut velit in",
+        "amount": "proident",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "incididunt "
+        "file": "enim repr"
     }
 })
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
@@ -2814,16 +2850,16 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/contracts/{contract_id}/adjustments`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Get all adjustments for the specific contract. |
-| from | str | ❌ | Get all adjustments for the specific contract. |
+| contract*id | str | ✅ | Get all adjustments for the specific contract. |
+| from* | str | ❌ | Get all adjustments for the specific contract. |
 | to | str | ❌ | Get all adjustments for the specific contract. |
 
 **Return Type**
 
 `AdjustmentsContainer`
 
 **Example Usage Code Snippet**
@@ -2886,15 +2922,15 @@
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "dolore",
+        "email": "sunt ullamco es",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.add_candidate(request_body=request_body)
@@ -2934,15 +2970,15 @@
     "data": {
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "Excepteur nu",
+        "email": "laboris a",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.patch_candidate(
@@ -3045,15 +3081,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EmployeeContractSignatureToCreateContainer(**{
     "data": {
-        "signature": "aliqua sed comm"
+        "signature": "inci"
     }
 })
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
@@ -3089,15 +3125,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = RequestCustomVerificationLetterContainer(**{
     "data": {
-        "description": "magnaest ea con",
+        "description": "Excepteur Duisi",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
 })
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
@@ -3170,15 +3206,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=1.72
+    document_id=5.13
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3504,15 +3540,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=1.36
+    document_id=3.06
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3539,15 +3575,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.91
+    document_id=5.72
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3878,16 +3914,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractSignatureToCreateContainer(**{
     "data": {
-        "client_signature": "ea exercitat",
-        "contract_template_id": 8.35
+        "client_signature": "proident e",
+        "contract_template_id": 1.32
     }
 })
 
 result = sdk.contracts.sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -3952,16 +3988,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractInvitationToCreateContainer(**{
     "data": {
-        "email": "eiusm",
-        "message": "officia ut"
+        "email": "dolore c",
+        "message": "mini"
     }
 })
 
 result = sdk.contracts.invite_to_sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -4074,18 +4110,18 @@
         "type_": "ongoing_time_based",
         "country_code": "US",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 2500,
             "currency_code": "GBP",
             "scale": "weekly",
-            "cycle_end": 30.28,
+            "cycle_end": 18.59,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
-            "payment_due_days": 11.81,
+            "payment_due_days": 36.88,
             "calculation_type": "CUSTOM_AMOUNT",
             "work_week_start": "Sunday",
             "work_week_end": "Sunday"
         }
     }
 })
 
@@ -4180,15 +4216,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.contracts.get_download_worker_documents_by_id(
     worker_id="worker_id",
-    document_id=8.43
+    document_id=1.09
 )
 
 print(result)
 ```
 
 ### TasksService
 
@@ -4467,15 +4503,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=564786626.18
+    offset=97685509.73
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4520,15 +4556,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=911169937.96
+    offset=90326358.62
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4629,15 +4665,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = TimesheetToUpdateContainer(**{
     "data": {
         "description": "description",
-        "quantity": 3.77
+        "quantity": 9.63
     }
 })
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
@@ -4751,15 +4787,15 @@
 )
 
 request_body = TimesheetReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            6.19
         ]
     }
 })
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
@@ -4997,15 +5033,15 @@
 )
 
 request_body = MilestoneReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.78
+            1.74
         ]
     }
 })
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
@@ -5208,17 +5244,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": True,
+        "with_multiple_dates": False,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
@@ -5258,17 +5294,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": True,
+        "with_multiple_dates": False,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
@@ -5483,15 +5519,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=226515477.25
+    offset=560002501.34
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5543,15 +5579,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=240522187.51
+    offset=729203388.82
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5584,21 +5620,21 @@
 request_body = InvoiceAdjustmentToCreateContainer(**{
     "data": {
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 6.69
+        "payment_cycle_id": 5.08
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
-    recurring=False
+    recurring=True
 )
 
 print(result)
 ```
 
 #### **update_invoice_adjustment_by_id**
 
@@ -5626,16 +5662,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = InvoiceAdjustmentToUpdateContainer(**{
     "data": {
-        "description": "sunt laborum Duis exercitation id",
-        "amount": 9.39
+        "description": "aute veniam in fugiat",
+        "amount": 2.65
     }
 })
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
@@ -5749,15 +5785,15 @@
 )
 
 request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            6.19
         ]
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
@@ -5813,15 +5849,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/legal-entities`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| type | str | ❌ | Retrieve a list of legal entities in your account. |
+| type\_ | str | ❌ | Retrieve a list of legal entities in your account. |
 
 **Return Type**
 
 `LegalEntityListContainer`
 
 **Example Usage Code Snippet**
 
@@ -6256,15 +6292,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| id | str | ✅ | Retrieve a single webhook subscription. |
+| id\_ | str | ✅ | Retrieve a single webhook subscription. |
 
 **Return Type**
 
 `WebhookItemResponse`
 
 **Example Usage Code Snippet**
 
@@ -6287,16 +6323,16 @@
 
 - HTTP Method: `PATCH`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| request_body | PatchWebhookRequest | ✅ | The request body. |
-| id | str | ✅ | Edit a webhook subscription. |
+| request*body | PatchWebhookRequest | ✅ | The request body. |
+| id* | str | ✅ | Edit a webhook subscription. |
 
 **Return Type**
 
 `WebhookItemResponse`
 
 **Example Usage Code Snippet**
 
@@ -6335,15 +6371,15 @@
 
 - HTTP Method: `DELETE`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| id | str | ✅ | Delete a webhook subscription. |
+| id\_ | str | ✅ | Delete a webhook subscription. |
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
 
 sdk = DeelSdk(
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/hooks/hook.py` & `deel-sdk-1.0.1/src/deel_sdk/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/__init__.py` & `deel-sdk-1.0.1/src/deel_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # This file was generated by liblab | https://liblab.com/
 
 from .invoice_list_container import InvoiceListContainer
+from .get_invoice_list_entities import GetInvoiceListEntities
 from .deel_invoice_list_container import DeelInvoiceListContainer
 from .invoice_download_link_container import InvoiceDownloadLinkContainer
 from .payment_list_container import PaymentListContainer
 from .get_payment_list_currencies import GetPaymentListCurrencies
-from .entities import Entities
+from .get_payment_list_entities import GetPaymentListEntities
 from .payment_break_down_container import PaymentBreakDownContainer
 from .admin_users_container import AdminUsersContainer
 from .admin_user_create_container import AdminUserCreateContainer
 from .create_admin_user_response_container import CreateAdminUserResponseContainer
 from .hris_direct_employee import HrisDirectEmployee
 from .hris_direct_employee_container import HrisDirectEmployeeContainer
 from .internal_people_container import InternalPeopleContainer
@@ -227,23 +228,23 @@
 from .webhook_event_type_list_response import WebhookEventTypeListResponse
 from .create_public_token_container import CreatePublicTokenContainer
 from .public_token_created_container import PublicTokenCreatedContainer
 from .equity_stakeholders_container import EquityStakeholdersContainer
 from .invoice import Invoice
 from .page_info_without_cursor_new import PageInfoWithoutCursorNew
 from .invoice_status_enum import InvoiceStatusEnum
+from .legal_entity_type import LegalEntityType
 from .deel_invoice import DeelInvoice
 from .invoice_download_object import InvoiceDownloadObject
 from .payment_object import PaymentObject
 from .payment import Payment
 from .payment_method import PaymentMethod
 from .payment_status_enum import PaymentStatusEnum
 from .payment_worker import PaymentWorker
 from .payment_method_enum import PaymentMethodEnum
-from .legal_entity_type import LegalEntityType
 from .payment_break_down import PaymentBreakDown
 from .admin_user import AdminUser
 from .admin_user_create_request import AdminUserCreateRequest
 from .hris_direct_employee_details import HrisDirectEmployeeDetails
 from .hris_team_information import HrisTeamInformation
 from .hris_compensation import HrisCompensation
 from .hris_job_information_title_id import HrisJobInformationTitleId
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/add_worker_bank_account_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/add_worker_bank_account_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/address.py` & `deel-sdk-1.0.1/src/deel_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustment_category.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_category.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustment_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_update.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustment_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/adjustments_categories_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/adjustments_categories_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/admin_user.py` & `deel-sdk-1.0.1/src/deel_sdk/models/admin_user.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/admin_user_create_request.py` & `deel-sdk-1.0.1/src/deel_sdk/models/admin_user_create_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/admin_users_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/admin_users_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/agreement.py` & `deel-sdk-1.0.1/src/deel_sdk/models/agreement.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/agreement_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/agreement_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/bank_account_added.py` & `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_added.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/bank_account_guide.py` & `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_guide.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/bank_account_status.py` & `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_status.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/bank_account_updated.py` & `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/bank_account_value_allowed.py` & `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_value_allowed.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/base.py` & `deel-sdk-1.0.1/src/deel_sdk/models/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         """
         if value is None:
             return None
 
         if re.match(r"{}".format(pattern), value):
             return value
         else:
-            raise ValueError(f"Invalid value for {variable_name}: must match {pattern}")
+            raise ValueError(
+                f"Invalid value for {variable_name}: must match {pattern}, received {value}"
+            )
 
     def _enum_matching(
         self, value: Union[str, Enum], enum_values: List[str], variable_name: str
     ):
         """
         Checks if a value (str or enum) matches the required enum values and returns the value if there's a match.
 
@@ -55,15 +57,15 @@
             return None
 
         str_value = value.value if isinstance(value, Enum) else value
         if str_value in enum_values:
             return value
         else:
             raise ValueError(
-                f"Invalid value for {variable_name}: must match one of {enum_values}"
+                f"Invalid value for {variable_name}: must match one of {enum_values}, received {value}"
             )
 
     def _define_object(self, input_data, input_class):
         """
         Check if the input data is an instance of the input class and return the input data if it is.
         Otherwise, return an instance of the input class.
 
@@ -183,14 +185,15 @@
         if input_data is None:
             return None
 
         if isinstance(input_data, (str, float, int, bool)):
             return input_data
 
         for class_constructor in cls.class_list.values():
+            exception_list = []
             try:
                 # Check if the class is a only a TypeHint
                 origin = get_origin(class_constructor)
                 if origin is not None and isinstance(input_data, list):
                     list_instance = cls._get_list_instance(
                         input_data, class_constructor, origin
                     )
@@ -204,20 +207,18 @@
                     return input_data
 
                 # Check if the input_data is a dictionary that can be used to initialize the class
                 elif isinstance(input_data, dict):
                     instance = class_constructor._unmap(input_data)
                     if cls._check_params(input_data, instance):
                         return instance
-            except Exception:
-                pass
+            except Exception as e:
+                exception_list.append({"class": class_constructor, "exception": e})
 
-        raise ValueError(
-            f"Input data must match one of the models: {list(cls.class_list.keys())}"
-        )
+        cls._raise_one_of_error(exception_list)
 
     @classmethod
     def _get_list_instance(cls, input_data, class_constructor, origin):
         """
         Return the list of elements for a given class constructor and origin type.
 
         :param input_data: The input data to check.
@@ -247,7 +248,27 @@
         """
         input_values = {k: v for k, v in raw_input.items() if v is not None}.values()
         instance_map = instance._map()
         instance_values = {
             k: v for k, v in instance_map.items() if v is not None
         }.values()
         return len(input_values) == len(instance_values)
+
+    @classmethod
+    def _raise_one_of_error(cls, exception_list):
+        """
+        Raises a ValueError with the appropriate error message for one of models.
+
+        :param exception_list: List of exceptions that occurred.
+        :type exception_list: list
+        :raises ValueError: If input data does not match any of the models.
+        """
+        if not exception_list:
+            return
+        exception_messages = "\n".join(
+            f"Class: {exception['class']}, Exception: {exception['exception']}"
+            for exception in exception_list
+        )
+        raise ValueError(
+            f"Input data must match one of the models: {list(cls.class_list.keys())}"
+            f"Errors occurred:\n{exception_messages}"
+        )
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/basic_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/basic_invoice_adjustment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/basic_invoice_adjustment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/basic_legal_entity.py` & `deel-sdk-1.0.1/src/deel_sdk/models/basic_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/basic_timesheet.py` & `deel-sdk-1.0.1/src/deel_sdk/models/basic_timesheet.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/benefit_contribution_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/benefit_contribution_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/benefit_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/benefit_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/breakdown_costs_quote.py` & `deel-sdk-1.0.1/src/deel_sdk/models/breakdown_costs_quote.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/calculate_final_payment_calculation_type.py` & `deel-sdk-1.0.1/src/deel_sdk/models/calculate_final_payment_calculation_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/candidate_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/candidate_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/candidate_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/candidate_to_patch.py` & `deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_patch.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/client_of_basic_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/client_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/client_of_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/client_of_contract_legal_entity_5.py` & `deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract_legal_entity_5.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/compensation_details_of_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py` & `deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_custom_field.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_custom_field.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_details_to_amend.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_details_to_amend.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 from .utils.json_map import JsonMap
 from .base import BaseModel
 from .work_statement_scale_enum import WorkStatementScaleEnum
 from .work_statement_cycle_scale_enum import WorkStatementCycleScaleEnum
 from .work_statement_cycle_end_type_enum import WorkStatementCycleEndTypeEnum
 from .work_statement_payment_due_type_enum import WorkStatementPaymentDueTypeEnum
+from .identifier_value import IdentifierValue, IdentifierValueGuard
 
 
 @JsonMap({})
 class ContractDetailsToAmend(BaseModel):
     """You can specify any combination of data points that need changing.
 
     :param amount: amount, defaults to None
@@ -35,18 +36,18 @@
     :type payment_due_type: WorkStatementPaymentDueTypeEnum, optional
     :param payment_due_days: payment_due_days, defaults to None
     :type payment_due_days: float, optional
     :param pay_before_weekends: If the payment due is on a weekend, pay on Friday., defaults to None
     :type pay_before_weekends: bool, optional
     :param job_title_name: You can enter new job title., defaults to None
     :type job_title_name: str, optional
-    :param job_title_id: Unique identifier of this resource., defaults to None
-    :type job_title_id: str, optional
-    :param seniority_id: Unique identifier of this resource., defaults to None
-    :type seniority_id: str, optional
+    :param job_title_id: job_title_id, defaults to None
+    :type job_title_id: IdentifierValue, optional
+    :param seniority_id: seniority_id, defaults to None
+    :type seniority_id: IdentifierValue, optional
     :param special_clause: Text to describe any special clause in contract., defaults to None
     :type special_clause: str, optional
     :param scope_of_work: Text to describe the scope of work of the contract., defaults to None
     :type scope_of_work: str, optional
     """
 
     def __init__(
@@ -60,16 +61,16 @@
         frequency: WorkStatementCycleScaleEnum = None,
         cycle_end: float = None,
         cycle_end_type: WorkStatementCycleEndTypeEnum = None,
         payment_due_type: WorkStatementPaymentDueTypeEnum = None,
         payment_due_days: float = None,
         pay_before_weekends: bool = None,
         job_title_name: str = None,
-        job_title_id: str = None,
-        seniority_id: str = None,
+        job_title_id: IdentifierValue = None,
+        seniority_id: IdentifierValue = None,
         special_clause: str = None,
         scope_of_work: str = None,
     ):
         if amount is not None:
             self.amount = amount
         if currency_code is not None:
             self.currency_code = self._pattern_matching(
@@ -104,14 +105,14 @@
         if payment_due_days is not None:
             self.payment_due_days = payment_due_days
         if pay_before_weekends is not None:
             self.pay_before_weekends = pay_before_weekends
         if job_title_name is not None:
             self.job_title_name = job_title_name
         if job_title_id is not None:
-            self.job_title_id = job_title_id
+            self.job_title_id = IdentifierValueGuard.return_one_of(job_title_id)
         if seniority_id is not None:
-            self.seniority_id = seniority_id
+            self.seniority_id = IdentifierValueGuard.return_one_of(seniority_id)
         if special_clause is not None:
             self.special_clause = special_clause
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_document_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_document_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_invitation_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_invitation_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_signature_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_signature_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_template.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_template.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_template_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_template_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_template_summary.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_template_summary.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_termination_result.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_termination_result_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_amend_details_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_amend_details_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_payg_milestones.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_milestones.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_container_payg_tasks.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_tasks.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_ongoing_time_based.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_ongoing_time_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 from .work_statement_scale_enum import WorkStatementScaleEnum
 
 
 @JsonMap({"id_": "id"})
 class ClientLegalEntity8(BaseModel):
     """Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
 class ClientTeam5(BaseModel):
     """Choose the Deel team for this contract. Use teams endpoint to retrieve a list of teams in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreateOngoingTimeBasedClient(BaseModel):
     """ContractToCreateOngoingTimeBasedClient
 
     :param legal_entity: Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 from .work_statement_scale_enum import WorkStatementScaleEnum
 
 
 @JsonMap({"id_": "id"})
 class ClientLegalEntity4(BaseModel):
     """Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
 class ClientTeam2(BaseModel):
     """Choose the Deel team for this contract. Use teams endpoint to retrieve a list of teams in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreatePayAsYouGoTimeBasedClient(BaseModel):
     """ContractToCreatePayAsYouGoTimeBasedClient
 
     :param legal_entity: Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_payg_milestones.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_milestones.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 
 
 @JsonMap({"id_": "id"})
 class ClientLegalEntity7(BaseModel):
     """Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
 class ClientTeam4(BaseModel):
     """Choose the Deel team for this contract. Use teams endpoint to retrieve a list of teams in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreatePaygMilestonesClient(BaseModel):
     """ContractToCreatePaygMilestonesClient
 
     :param legal_entity: Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_create_payg_tasks.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 from .identifier_value import IdentifierValue, IdentifierValueGuard
 
 
 @JsonMap({"id_": "id"})
 class ClientLegalEntity6(BaseModel):
     """Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
 class ClientTeam3(BaseModel):
     """Choose the Deel team for this contract. Use teams endpoint to retrieve a list of teams in your organization.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     """
 
-    def __init__(self, id_: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({})
 class ContractToCreatePaygTasksClient(BaseModel):
     """ContractToCreatePaygTasksClient
 
     :param legal_entity: Choose the Deel legal entity for this contract. Use legal entity endpoint to retrieve a list of legal entities in your organization.
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_to_terminate.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_terminate.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_type_enum_for_estimate.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum_for_estimate.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contract_who_reports_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contract_who_reports_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contracts_sort_by_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contracts_sort_by_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/contribution.py` & `deel-sdk-1.0.1/src/deel_sdk/models/contribution.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/cost_quote.py` & `deel-sdk-1.0.1/src/deel_sdk/models/cost_quote.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/country.py` & `deel-sdk-1.0.1/src/deel_sdk/models/country.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/create_people_timeoff.py` & `deel-sdk-1.0.1/src/deel_sdk/models/create_people_timeoff.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/create_timeoff.py` & `deel-sdk-1.0.1/src/deel_sdk/models/create_timeoff.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/create_webhook_request.py` & `deel-sdk-1.0.1/src/deel_sdk/models/create_webhook_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/deel_invoice.py` & `deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/deel_invoice_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/departments.py` & `deel-sdk-1.0.1/src/deel_sdk/models/departments.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/download_worker_documents_by_id_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/download_worker_documents_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/email.py` & `deel-sdk-1.0.1/src/deel_sdk/models/email.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_agreement_download_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_agreement_download_object.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_object.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_contract_signature_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_contract_signature_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_payslips_list.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_payslips_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_tax_documents_list.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_tax_documents_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_creation_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_creation_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_entitlements_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_entitlements_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_item_response.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_policies_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employee_timeoffs_policies_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employment_detail.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employment_detail.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/employment_details_of_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/employment_details_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_client_timeoff_requests.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoff_requests.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_client_timeoffs.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoffs.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_benefits.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_benefits_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_created.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_contract_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_country_validations.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_country_validations.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_entitlement_list_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlement_list_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_entitlements.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlements.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_field.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_field.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_holidays_rollover_type.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_holidays_rollover_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_quote_base.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_quote_base.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_base_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_base_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/eor_timeoffs_employee_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_employee_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/equity_stakeholder.py` & `deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholder.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/equity_stakeholders_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholders_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/estimate_first_payment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/estimate_first_payment_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/file_attachment_info.py` & `deel-sdk-1.0.1/src/deel_sdk/models/file_attachment_info.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/file_ref_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/file_ref_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/final_payment_calculated.py` & `deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/final_payment_calculated_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/generic_result_created.py` & `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/generic_result_created_with_id.py` & `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created_with_id.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/generic_result_deleted.py` & `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_deleted.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/generic_result_updated.py` & `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/get_employee_compliance_documents_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_documents_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/global_payroll_g2_n_report.py` & `deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/global_payroll_g2_n_report_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_client.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_client.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_created.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_salary_scale_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_salary_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_status_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_status_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_contract_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_update_data.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_updated.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_address_updated_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_update_data.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_updated.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_compensation_updated_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_information_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_information_update_data.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_information_updated_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_pto_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_employee_pto_update_data.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_payroll_event_report_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_report_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/gp_payroll_event_reports.py` & `deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_reports.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/health_insurance_provider.py` & `deel-sdk-1.0.1/src/deel_sdk/models/health_insurance_provider.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hiring_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hiring_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_contract_full_time.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_full_time.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_contract_part_time.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_part_time.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee_details.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_details.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_direct_employee_response.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/hris_job_information_title_name.py` & `deel-sdk-1.0.1/src/deel_sdk/models/hris_job_information_title_name.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/input_to_create_file_ref.py` & `deel-sdk-1.0.1/src/deel_sdk/models/input_to_create_file_ref.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/input_to_patch_contract_external_id.py` & `deel-sdk-1.0.1/src/deel_sdk/models/input_to_patch_contract_external_id.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/internal_people.py` & `deel-sdk-1.0.1/src/deel_sdk/models/internal_people.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invitations_of_basic_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invitations_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     :type is_overdue: bool
     :param issued_at: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31.
     :type issued_at: str
     :param vat_id: VAT identification number.
     :type vat_id: str
     :param due_date: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31.
     :type due_date: str
-    :param contract_id: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31.
+    :param contract_id: Unique identifier of the contract.
     :type contract_id: str
     """
 
     def __init__(
         self,
         id_: str,
         status: InvoiceStatusEnum,
@@ -70,10 +70,8 @@
         self.issued_at = self._pattern_matching(
             issued_at, "^\d{4}-\d{2}-\d{2}$", "issued_at"
         )
         self.vat_id = vat_id
         self.due_date = self._pattern_matching(
             due_date, "^\d{4}-\d{2}-\d{2}$", "due_date"
         )
-        self.contract_id = self._pattern_matching(
-            contract_id, "^\d{4}-\d{2}-\d{2}$", "contract_id"
-        )
+        self.contract_id = contract_id
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_created.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_created_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_review_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_update.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/invoice_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/invoice_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/job_title.py` & `deel-sdk-1.0.1/src/deel_sdk/models/job_title.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/job_title_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/job_title_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/legal_entity_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/legal_entity_type.py` & `deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/letter_request.py` & `deel-sdk-1.0.1/src/deel_sdk/models/letter_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/marital_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/meta_data_of_contract_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/meta_data_of_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone_properties.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone_properties.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone_review_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone_review_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone_reviews_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone_reviews_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/milestone_to_create_form_with_file.py` & `deel-sdk-1.0.1/src/deel_sdk/models/milestone_to_create_form_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/off_cycle_payment_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/organization_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/organization_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/output_to_create_file_ref_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/output_to_create_file_ref_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/page_info_without_cursor_new.py` & `deel-sdk-1.0.1/src/deel_sdk/models/page_info_without_cursor_new.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/patch_webhook_request.py` & `deel-sdk-1.0.1/src/deel_sdk/models/patch_webhook_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment_break_down.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment_break_down.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment_method.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment_method_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment_method_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment_object.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment_object.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payment_worker.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payment_worker.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payroll_adjustment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payroll_adjustment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/payslips.py` & `deel-sdk-1.0.1/src/deel_sdk/models/payslips.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pension_eor_contract_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pension_eor_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pension_provider.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pension_provider.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_by_id_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_client_legal_entity.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_client_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_custom_field.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_custom_field.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_me.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_me.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_payment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_sort_by_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_sort_by_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/people_time_off_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/people_time_off_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pgo_task.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pgo_task_reviews_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pgo_task_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/premium_result_added.py` & `deel-sdk-1.0.1/src/deel_sdk/models/premium_result_added.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/premium_to_add.py` & `deel-sdk-1.0.1/src/deel_sdk/models/premium_to_add.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/pro_rata.py` & `deel-sdk-1.0.1/src/deel_sdk/models/pro_rata.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/profile_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/profile_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/request_custom_verification_letter_with_file.py` & `deel-sdk-1.0.1/src/deel_sdk/models/request_custom_verification_letter_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/requester_time_off.py` & `deel-sdk-1.0.1/src/deel_sdk/models/requester_time_off.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/response_estimate_first_payment.py` & `deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/response_estimate_first_payment_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/salary_frequency_scale_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/salary_frequency_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/seniority.py` & `deel-sdk-1.0.1/src/deel_sdk/models/seniority.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/seniority_required.py` & `deel-sdk-1.0.1/src/deel_sdk/models/seniority_required.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/signatures_of_basic_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/signatures_of_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/sort_dir_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/sort_dir_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/task_created.py` & `deel-sdk-1.0.1/src/deel_sdk/models/task_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/team.py` & `deel-sdk-1.0.1/src/deel_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/team_of_basic_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/team_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/team_of_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/team_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoff_review.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoff_review_internal.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review_internal.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoff_to_review_internal_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoff_to_review_internal_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_attachments_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_attachments_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_profile.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_profile.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timeoffs_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_approver.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_approver.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_list_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_review_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_review_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_reviews_to_create.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_reviews_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_shared_properties.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_shared_properties.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_status_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_create_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_create_container_with_file.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_update.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/timesheet_to_update_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/update_worker_department_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/update_worker_department_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/update_worker_working_location_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/update_worker_working_location_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/upload_employee_compliance_document_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/upload_employee_compliance_document_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/utils/cast_models.py` & `deel-sdk-1.0.1/src/deel_sdk/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/utils/json_map.py` & `deel-sdk-1.0.1/src/deel_sdk/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/validation_type.py` & `deel-sdk-1.0.1/src/deel_sdk/models/validation_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/validation_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/validation_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/webhook_event_type_list_response.py` & `deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_list_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/webhook_event_type_response.py` & `deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/webhook_item.py` & `deel-sdk-1.0.1/src/deel_sdk/models/webhook_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/week_days_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/week_days_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/work_statement_cycle_end_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_end_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/work_statement_cycle_scale_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/work_statement_payment_due_type_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_payment_due_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/work_statement_scale_enum.py` & `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_bank_account_info.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_info.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_bank_account_to_add.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_to_add.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_bank_accounts_info_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_accounts_info_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_document.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_document.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_document_download_link.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_document_download_link.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_documents_by_id_container.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_documents_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_legal_entity.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_of_basic_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_of_contract.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/models/worker_termination_body.py` & `deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_body.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/headers/access_token_auth.py` & `deel-sdk-1.0.1/src/deel_sdk/net/headers/access_token_auth.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/base_handler.py` & `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/hook_handler.py` & `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/http_handler.py` & `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/request_chain/handlers/retry_handler.py` & `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/request_chain/request_chain.py` & `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/transport/request.py` & `deel-sdk-1.0.1/src/deel_sdk/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/transport/request_error.py` & `deel-sdk-1.0.1/src/deel_sdk/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/transport/response.py` & `deel-sdk-1.0.1/src/deel_sdk/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/transport/serializer.py` & `deel-sdk-1.0.1/src/deel_sdk/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/net/transport/utils.py` & `deel-sdk-1.0.1/src/deel_sdk/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/sdk.py` & `deel-sdk-1.0.1/src/deel_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/accounting.py` & `deel-sdk-1.0.1/src/deel_sdk/services/accounting.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,89 +4,99 @@
 from .utils.base_service import BaseService
 from ..net.transport.serializer import Serializer
 from ..models.utils.cast_models import cast_models
 from ..models.payment_list_container import PaymentListContainer
 from ..models.payment_break_down_container import PaymentBreakDownContainer
 from ..models.invoice_list_container import InvoiceListContainer
 from ..models.invoice_download_link_container import InvoiceDownloadLinkContainer
+from ..models.get_payment_list_entities import GetPaymentListEntities
 from ..models.get_payment_list_currencies import GetPaymentListCurrencies
-from ..models.entities import Entities
+from ..models.get_invoice_list_entities import GetInvoiceListEntities
 from ..models.deel_invoice_list_container import DeelInvoiceListContainer
 
 
 class AccountingService(BaseService):
 
     @cast_models
     def get_invoice_list(
         self,
         issued_from_date: str = None,
         issued_to_date: str = None,
+        entities: GetInvoiceListEntities = None,
         limit: float = None,
         offset: float = None,
     ) -> InvoiceListContainer:
         """Retrieve a list of paid invoices for your workforce.
 
         :param issued_from_date: to get records created after given issue date, defaults to None
         :type issued_from_date: str, optional
         :param issued_to_date: to get records created before given issued date, defaults to None
         :type issued_to_date: str, optional
+        :param entities: Filter by legal entity type; company, or individual, defaults to None
+        :type entities: GetInvoiceListEntities, optional
         :param limit: Return a page of results with given number of records; NOTE technically ALL query parameters are strings or array of strings, defaults to None
         :type limit: float, optional
         :param offset: Return a page of results after given index of row; NOTE technically ALL query parameters are strings or array of strings', defaults to None
         :type offset: float, optional
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: InvoiceListContainer
         """
 
         Validator(str).is_optional().validate(issued_from_date)
         Validator(str).is_optional().validate(issued_to_date)
+        Validator(GetInvoiceListEntities).is_optional().validate(entities)
         Validator(float).is_optional().min(1).max(99).validate(limit)
         Validator(float).is_optional().min(0).max(999999999).validate(offset)
 
         serialized_request = (
             Serializer(f"{self.base_url}/invoices", self.get_default_headers())
             .add_query("issued_from_date", issued_from_date)
             .add_query("issued_to_date", issued_to_date)
+            .add_query("entities", entities)
             .add_query("limit", limit)
             .add_query("offset", offset)
             .serialize()
             .set_method("GET")
         )
 
         response = self.send_request(serialized_request)
 
         return InvoiceListContainer._unmap(response)
 
     @cast_models
     def get_deel_invoice_list(
-        self, limit: float = None, offset: float = None
+        self, contract_id: str, limit: float = None, offset: float = None
     ) -> DeelInvoiceListContainer:
         """Retrieve a list of invoices related to Deel fees.
 
+        :param contract_id: Deel contract id.
+        :type contract_id: str
         :param limit: Return a page of results with given number of records; NOTE technically ALL query parameters are strings or array of strings, defaults to None
         :type limit: float, optional
         :param offset: Return a page of results after given index of row; NOTE technically ALL query parameters are strings or array of strings', defaults to None
         :type offset: float, optional
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: DeelInvoiceListContainer
         """
 
+        Validator(str).validate(contract_id)
         Validator(float).is_optional().min(1).max(99).validate(limit)
         Validator(float).is_optional().min(0).max(999999999).validate(offset)
 
         serialized_request = (
             Serializer(f"{self.base_url}/invoices/deel", self.get_default_headers())
             .add_query("limit", limit)
             .add_query("offset", offset)
+            .add_query("contract_id", contract_id)
             .serialize()
             .set_method("GET")
         )
 
         response = self.send_request(serialized_request)
 
         return DeelInvoiceListContainer._unmap(response)
@@ -124,37 +134,37 @@
 
     @cast_models
     def get_payment_list(
         self,
         date_from: str = None,
         date_to: str = None,
         currencies: GetPaymentListCurrencies = None,
-        entities: Entities = None,
+        entities: GetPaymentListEntities = None,
     ) -> PaymentListContainer:
         """Retrieve a list of payments made to Deel.
 
         :param date_from: Filtered results will include records created on or after the provided date., defaults to None
         :type date_from: str, optional
         :param date_to: Filtered results will include records created before the provided date., defaults to None
         :type date_to: str, optional
         :param currencies: Currency codes of contracts to filter., defaults to None
         :type currencies: GetPaymentListCurrencies, optional
         :param entities: Filter by legal entity type; company, or individual, defaults to None
-        :type entities: Entities, optional
+        :type entities: GetPaymentListEntities, optional
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: PaymentListContainer
         """
 
         Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_from)
         Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_to)
         Validator(GetPaymentListCurrencies).is_optional().validate(currencies)
-        Validator(Entities).is_optional().validate(entities)
+        Validator(GetPaymentListEntities).is_optional().validate(entities)
 
         serialized_request = (
             Serializer(f"{self.base_url}/payments", self.get_default_headers())
             .add_query("date_from", date_from, nullable=True)
             .add_query("date_to", date_to, nullable=True)
             .add_query("currencies", currencies)
             .add_query("entities", entities)
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/adjustments.py` & `deel-sdk-1.0.1/src/deel_sdk/services/adjustments.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/candidates.py` & `deel-sdk-1.0.1/src/deel_sdk/services/candidates.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/carta.py` & `deel-sdk-1.0.1/src/deel_sdk/services/carta.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/contractors.py` & `deel-sdk-1.0.1/src/deel_sdk/services/contractors.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/contracts.py` & `deel-sdk-1.0.1/src/deel_sdk/services/contracts.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/eor.py` & `deel-sdk-1.0.1/src/deel_sdk/services/eor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: EorCountryValidationsContainer
         """
 
-        Validator(str).pattern("^[A-Z]{2}$").validate(country_code)
+        Validator(str).min_length(2).max_length(2).pattern("^[A-Z]{2}$").validate(
+            country_code
+        )
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/eor/validations/{{country_code}}",
                 self.get_default_headers(),
             )
             .add_path("country_code", country_code)
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/global_payroll.py` & `deel-sdk-1.0.1/src/deel_sdk/services/global_payroll.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/invoices.py` & `deel-sdk-1.0.1/src/deel_sdk/services/invoices.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/lookups.py` & `deel-sdk-1.0.1/src/deel_sdk/services/lookups.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/managers.py` & `deel-sdk-1.0.1/src/deel_sdk/services/managers.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/milestones.py` & `deel-sdk-1.0.1/src/deel_sdk/services/milestones.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/off_cycle_payments.py` & `deel-sdk-1.0.1/src/deel_sdk/services/off_cycle_payments.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/organizations.py` & `deel-sdk-1.0.1/src/deel_sdk/services/organizations.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/partner_managed.py` & `deel-sdk-1.0.1/src/deel_sdk/services/partner_managed.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/people.py` & `deel-sdk-1.0.1/src/deel_sdk/services/people.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/tasks.py` & `deel-sdk-1.0.1/src/deel_sdk/services/tasks.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/time_off.py` & `deel-sdk-1.0.1/src/deel_sdk/services/time_off.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/timesheets.py` & `deel-sdk-1.0.1/src/deel_sdk/services/timesheets.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/token.py` & `deel-sdk-1.0.1/src/deel_sdk/services/token.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/utils/base_service.py` & `deel-sdk-1.0.1/src/deel_sdk/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/utils/default_headers.py` & `deel-sdk-1.0.1/src/deel_sdk/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/utils/validator.py` & `deel-sdk-1.0.1/src/deel_sdk/services/utils/validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file was generated by liblab | https://liblab.com/
 
 import re
+import operator
 from typing import Union, Any, Type, Pattern, get_args
 from ...models.base import OneOfBaseModel
 
 
 class Validator:
     """
     A simple validator class for validating the type and pattern of a value.
@@ -23,16 +24,20 @@
 
         :param Type[Any] _type: The expected type for the value. Defaults to None.
         """
         self._type: Type[Any] = _type
         self._is_optional: bool = False
         self._is_array: bool = False
         self._pattern: Pattern[str] = None
+        self._min_length: int = None
+        self._max_length: int = None
         self._min: int = None
+        self._min_exclusive: bool = False
         self._max: int = None
+        self._max_exclusive: bool = False
 
     def is_array(self) -> "Validator":
         """
         Marks the value as an array.
 
         :return: The Validator instance for method chaining.
         :rtype: Validator
@@ -57,34 +62,60 @@
         :param str pattern: The regular expression pattern.
         :return: The Validator instance for method chaining.
         :rtype: Validator
         """
         self._pattern = re.compile(pattern)
         return self
 
-    def min(self, min: int) -> "Validator":
+    def min(self, min: int, exclusive=False) -> "Validator":
         """
         Specifies a minimum value for validating the value.
 
-        :param int min: The minimum value.
+        :param int min: The minimum value to be validated against.
+        :param bool exclusive: (optional) If set to True, the minimum value is not inclusive.
         :return: The Validator instance for method chaining.
         :rtype: Validator
         """
         self._min = min
+        self._min_exclusive = exclusive
         return self
 
-    def max(self, max: int) -> "Validator":
+    def max(self, max: int, exclusive=False) -> "Validator":
         """
         Specifies a maximum value for validating the value.
 
         :param int max: The maximum value.
+        :param bool exclusive: (optional) If set to True, the maximum value is not inclusive.
         :return: The Validator instance for method chaining.
         :rtype: Validator
         """
         self._max = max
+        self._max_exclusive = exclusive
+        return self
+
+    def min_length(self, min_length: int) -> "Validator":
+        """
+        Specifies a minimum length for validating the value.
+
+        :param int min_length: The minimum length to be validated against.
+        :return: The Validator instance for method chaining.
+        :rtype: Validator
+        """
+        self._min_length = min_length
+        return self
+
+    def max_length(self, max_length: int) -> "Validator":
+        """
+        Specifies a maximum length for validating the value.
+
+        :param int max_length: The maximum length.
+        :return: The Validator instance for method chaining.
+        :rtype: Validator
+        """
+        self._max_length = max_length
         return self
 
     def validate(self, value: Any) -> None:
         """
         Validates the provided value based on the specified criteria.
 
         :param Any value: The input that needs to be checked
@@ -148,18 +179,33 @@
     def _validate_rules(self, value: Any) -> None:
         """
         Validate the rules specified for the value.
 
         :param Any value: The input that needs to be validated
         :raises ValueError: If the value does not meet the specified validation criteria.
         """
-        if self._min is not None and value < self._min:
-            raise ValueError(f"Invalid value: {value} is less than {self._min}")
-        if self._max is not None and value > self._max:
-            raise ValueError(f"Invalid value: {value} is greater than {self._max}")
+        min_operator = operator.lt if self._min_exclusive else operator.le
+        max_operator = operator.gt if self._max_exclusive else operator.ge
+
+        if self._min is not None and not min_operator(self._min, value):
+            raise ValueError(
+                f"Invalid value: {value} is {'less than or equal to' if self._min_exclusive else 'less than'} {self._min}"
+            )
+        if self._max is not None and not max_operator(self._max, value):
+            raise ValueError(
+                f"Invalid value: {value} is {'greater than or equal to' if self._max_exclusive else 'greater than'} {self._max}"
+            )
+        if self._min_length is not None and len(value) < self._min_length:
+            raise ValueError(
+                f"Invalid value: the length of {value} is less than {self._min_length}"
+            )
+        if self._max_length is not None and len(value) > self._max_length:
+            raise ValueError(
+                f"Invalid value: the length of {value} is greater than {self._max_length}"
+            )
         if self._pattern and not self._pattern.match(str(value)):
             raise ValueError(
                 f"Invalid value: {value} does not match pattern {self._pattern}"
             )
 
     def _is_one_of_type(self, cls_type):
         """
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk/services/webhooks.py` & `deel-sdk-1.0.1/src/deel_sdk/services/webhooks.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.0/src/deel_sdk.egg-info/PKG-INFO` & `deel-sdk-1.0.1/src/deel_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: deel-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deel REST API
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# DeelSdk Python SDK 1.0.0
+# DeelSdk Python SDK 1.0.1
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.0
+- SDK version: 1.0.1
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
+- [Environments](#environments)
 - [Using Union Types in Function Parameters](#using-union-types-in-function-parameters)
 - [Services](#services)
 
 ## Installation
 
 ```bash
 pip install deel-sdk
@@ -46,14 +47,31 @@
 
 Or at a later stage:
 
 ```py
 sdk.set_access_token("YOUR_ACCESS_TOKEN")
 ```
 
+## Environments
+
+Here is the list of all available environment variables:
+
+```py
+Demo = "https://api-staging.letsdeel.com/rest/v2"
+Production = "https://api.letsdeel.com/rest/v2"
+```
+
+Here is how you set an environment:
+
+```py
+from deel_sdk import Environment
+
+sdk.set_base_url(Environment.Demo.value)
+```
+
 ## Using Union Types in Function Parameters
 
 In Python, a parameter can be annotated with a Union type, indicating it can accept values of multiple types.
 
 ### Passing Instances or Dictionaries
 
 When we have a model such as:
@@ -132,36 +150,42 @@
 - Endpoint: `/invoices`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | issued_from_date | str | ❌ | Retrieve a list of paid invoices for your workforce. |
 | issued_to_date | str | ❌ | Retrieve a list of paid invoices for your workforce. |
+| entities | GetInvoiceListEntities | ❌ | Retrieve a list of paid invoices for your workforce. |
 | limit | float | ❌ | Retrieve a list of paid invoices for your workforce. |
 | offset | float | ❌ | Retrieve a list of paid invoices for your workforce. |
 
 **Return Type**
 
 `InvoiceListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
+from deel_sdk.models import GetInvoiceListEntities
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
+entities=GetInvoiceListEntities(**[
+    "individual"
+])
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
+    entities=entities,
     limit=10,
-    offset=808037660.53
+    offset=707020693.68
 )
 
 print(result)
 ```
 
 #### **get_deel_invoice_list**
 
@@ -169,14 +193,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/invoices/deel`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
+| contract_id | str | ✅ | Retrieve a list of invoices related to Deel fees. |
 | limit | float | ❌ | Retrieve a list of invoices related to Deel fees. |
 | offset | float | ❌ | Retrieve a list of invoices related to Deel fees. |
 
 **Return Type**
 
 `DeelInvoiceListContainer`
 
@@ -187,16 +212,17 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.accounting.get_deel_invoice_list(
+    contract_id="contract_id",
     limit=10,
-    offset=237799437.03
+    offset=898896522.23
 )
 
 print(result)
 ```
 
 #### **get_billing_invoice_download_link**
 
@@ -238,34 +264,34 @@
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | date_from | str | ❌ | Retrieve a list of payments made to Deel. |
 | date_to | str | ❌ | Retrieve a list of payments made to Deel. |
 | currencies | GetPaymentListCurrencies | ❌ | Retrieve a list of payments made to Deel. |
-| entities | Entities | ❌ | Retrieve a list of payments made to Deel. |
+| entities | GetPaymentListEntities | ❌ | Retrieve a list of payments made to Deel. |
 
 **Return Type**
 
 `PaymentListContainer`
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
-from deel_sdk.models import GetPaymentListCurrencies, Entities
+from deel_sdk.models import GetPaymentListCurrencies, GetPaymentListEntities
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 currencies=GetPaymentListCurrencies(**[
     "GBP"
 ])
-entities=Entities(**[
+entities=GetPaymentListEntities(**[
     "individual"
 ])
 
 result = sdk.accounting.get_payment_list(
     date_from="1999-12-31",
     date_to="1999-12-31",
     currencies=currencies,
@@ -375,16 +401,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdminUserCreateContainer(**{
     "data": {
-        "first_name": "dolore",
-        "last_name": "proi",
+        "first_name": "proident molli",
+        "last_name": "anim ci",
         "email": "email"
     }
 })
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
@@ -445,36 +471,36 @@
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
     "team_information": {
-        "team_id": 9.77,
-        "legal_entity_id": 2.18
+        "team_id": 1.64,
+        "legal_entity_id": 2.97
     },
     "job_information": {
-        "seniority_id": 9.22,
-        "job_title_id": 6.5
+        "seniority_id": 1.14,
+        "job_title_id": 6.17
     },
     "compensation": {
-        "gross_annual_salary": 7.15,
+        "gross_annual_salary": 5.95,
         "currency": "USD"
     },
     "contract": {
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 9.02,
+        "employee_number": 3.49,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 21.67
+        "part_time_percentage": 75.13
     },
     "vacation_info": {
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 171.07
+        "vacation_yearly_policy": 295.88
     }
 })
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
@@ -503,16 +529,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=978653984.34,
-    limit=43.45
+    offset=92741896.72,
+    limit=88.8
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -525,15 +551,15 @@
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | offset | float | ❌ | Retrieve a list of People in your organization. |
 | limit | float | ❌ | Retrieve a list of People in your organization. |
 | search | str | ❌ | Retrieve a list of People in your organization. |
 | sort_by | PeopleSortByEnum | ❌ | Retrieve a list of People in your organization. |
 | sort_order | SortDirEnum | ❌ | Retrieve a list of People in your organization. |
-| hiring_statuses[] | HiringStatusEnum | ❌ | Retrieve a list of People in your organization. |
+| hiring_statuses | HiringStatusEnum | ❌ | Retrieve a list of People in your organization. |
 
 **Return Type**
 
 `PeopleContainer`
 
 **Example Usage Code Snippet**
 
@@ -543,16 +569,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=44334375.53,
-    limit=105.69,
+    offset=311381742.98,
+    limit=139.17,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -1195,38 +1221,38 @@
                 "country": "US"
             }
         },
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
-            "work_visa_required": False,
+            "work_visa_required": True,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 6.17,
+            "probation_period": 2.27,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 5.67
+            "holidays": 4.71
         },
         "job_title": "job_title",
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
-            "salary": 5.95,
+            "salary": 0.96,
             "currency": "currency",
-            "variable_compensation": 3.49,
+            "variable_compensation": 6.36,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
@@ -1293,46 +1319,46 @@
 )
 
 request_body = GpContractToCreateContainer(**{
     "data": {
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "culpa Lorem inc",
-            "work_email": "in do L",
+            "email": "ipsum ad tempor",
+            "work_email": "Lorem ullamco ",
             "nationality": "US",
             "employee_number": "100",
             "address": {
                 "street": "Deel Street 500",
                 "city": "Denver",
                 "state": "CO",
                 "zip": "44000",
                 "country": "US"
             }
         },
         "employment": {
             "type_": "Full-time",
             "start_date": "1999-12-31",
             "holidays": {
-                "allowance": 5.28,
+                "allowance": 1.94,
                 "start_date": "1999-12-31"
             }
         },
         "job_title": "job_title",
         "client": {
             "legal_entity": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "compensation_details": {
             "scale": "YEAR",
-            "salary": 8.05,
+            "salary": 2.33,
             "currency": "GBP"
         }
     }
 })
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
@@ -1978,35 +2004,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "name": "adquis culpa reprehenderit sed in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "ametnos",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 3.56,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2064,28 +2090,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "enim irure dolore magna"
+            "name": "nulla"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis nulla oc",
+            "expected_email": "Duis esse ex",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2149,28 +2175,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "et dolore"
+            "name": "mollit"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "sint ",
+            "expected_email": "proid",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2234,35 +2260,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "cillum"
+            "name": "Lorem"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Lorem sint et",
+            "expected_email": "anim sit",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 7.36,
+            "amount": 6.09,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2320,35 +2346,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "sedDuis officia est laborum in"
+            "name": "adquis culpa reprehenderit sed in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": False,
+            "documents_required": True,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "occae",
+            "expected_email": "ametnos",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 2.6,
+            "amount": 3.56,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2372,15 +2398,15 @@
 - HTTP Method: `GET`
 - Endpoint: `/contracts/{contract_id}/preview`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
 | contract_id | str | ✅ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
-| templateId | str | ❌ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
+| template_id | str | ❌ | Retrieve an IC and EOR contract agreement content in HTML. If no template is specified, the default or currently assigned template will be used. This endpoint does not support Global Payroll contract type. |
 
 **Return Type**
 
 `str`
 
 **Example Usage Code Snippet**
 
@@ -2432,21 +2458,21 @@
 request_body = ContractToAmendDetailsContainer(**{
     "data": {
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 0.24,
+        "first_payment": 8.79,
         "frequency": "weekly",
-        "cycle_end": 24.94,
+        "cycle_end": 28.13,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 0.92,
-        "pay_before_weekends": True,
+        "payment_due_days": 6.51,
+        "pay_before_weekends": False,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
 })
@@ -2621,20 +2647,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat exe",
+        "amount": "cupidatat cil",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "qu",
+        "file": "nisi nulla",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2700,18 +2726,18 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdjustmentToUpdateContainer(**{
     "data": {
-        "amount": "ut velit in",
+        "amount": "proident",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "incididunt "
+        "file": "enim repr"
     }
 })
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
@@ -2824,16 +2850,16 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/contracts/{contract_id}/adjustments`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Get all adjustments for the specific contract. |
-| from | str | ❌ | Get all adjustments for the specific contract. |
+| contract*id | str | ✅ | Get all adjustments for the specific contract. |
+| from* | str | ❌ | Get all adjustments for the specific contract. |
 | to | str | ❌ | Get all adjustments for the specific contract. |
 
 **Return Type**
 
 `AdjustmentsContainer`
 
 **Example Usage Code Snippet**
@@ -2896,15 +2922,15 @@
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "dolore",
+        "email": "sunt ullamco es",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.add_candidate(request_body=request_body)
@@ -2944,15 +2970,15 @@
     "data": {
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "Excepteur nu",
+        "email": "laboris a",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.patch_candidate(
@@ -3055,15 +3081,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EmployeeContractSignatureToCreateContainer(**{
     "data": {
-        "signature": "aliqua sed comm"
+        "signature": "inci"
     }
 })
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
@@ -3099,15 +3125,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = RequestCustomVerificationLetterContainer(**{
     "data": {
-        "description": "magnaest ea con",
+        "description": "Excepteur Duisi",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
 })
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
@@ -3180,15 +3206,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=1.72
+    document_id=5.13
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3514,15 +3540,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=1.36
+    document_id=3.06
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3549,15 +3575,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.91
+    document_id=5.72
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3888,16 +3914,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractSignatureToCreateContainer(**{
     "data": {
-        "client_signature": "ea exercitat",
-        "contract_template_id": 8.35
+        "client_signature": "proident e",
+        "contract_template_id": 1.32
     }
 })
 
 result = sdk.contracts.sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -3962,16 +3988,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractInvitationToCreateContainer(**{
     "data": {
-        "email": "eiusm",
-        "message": "officia ut"
+        "email": "dolore c",
+        "message": "mini"
     }
 })
 
 result = sdk.contracts.invite_to_sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -4084,18 +4110,18 @@
         "type_": "ongoing_time_based",
         "country_code": "US",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 2500,
             "currency_code": "GBP",
             "scale": "weekly",
-            "cycle_end": 30.28,
+            "cycle_end": 18.59,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
-            "payment_due_days": 11.81,
+            "payment_due_days": 36.88,
             "calculation_type": "CUSTOM_AMOUNT",
             "work_week_start": "Sunday",
             "work_week_end": "Sunday"
         }
     }
 })
 
@@ -4190,15 +4216,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.contracts.get_download_worker_documents_by_id(
     worker_id="worker_id",
-    document_id=8.43
+    document_id=1.09
 )
 
 print(result)
 ```
 
 ### TasksService
 
@@ -4477,15 +4503,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=564786626.18
+    offset=97685509.73
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4530,15 +4556,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=911169937.96
+    offset=90326358.62
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4639,15 +4665,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = TimesheetToUpdateContainer(**{
     "data": {
         "description": "description",
-        "quantity": 3.77
+        "quantity": 9.63
     }
 })
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
@@ -4761,15 +4787,15 @@
 )
 
 request_body = TimesheetReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            6.19
         ]
     }
 })
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
@@ -5007,15 +5033,15 @@
 )
 
 request_body = MilestoneReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.78
+            1.74
         ]
     }
 })
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
@@ -5218,17 +5244,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": True,
+        "with_multiple_dates": False,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
@@ -5268,17 +5294,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": True,
+        "with_multiple_dates": False,
         "reason": "Holiday",
-        "is_start_date_half_day": True,
+        "is_start_date_half_day": False,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
@@ -5493,15 +5519,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=226515477.25
+    offset=560002501.34
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5553,15 +5579,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=240522187.51
+    offset=729203388.82
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5594,21 +5620,21 @@
 request_body = InvoiceAdjustmentToCreateContainer(**{
     "data": {
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 6.69
+        "payment_cycle_id": 5.08
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
-    recurring=False
+    recurring=True
 )
 
 print(result)
 ```
 
 #### **update_invoice_adjustment_by_id**
 
@@ -5636,16 +5662,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = InvoiceAdjustmentToUpdateContainer(**{
     "data": {
-        "description": "sunt laborum Duis exercitation id",
-        "amount": 9.39
+        "description": "aute veniam in fugiat",
+        "amount": 2.65
     }
 })
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
@@ -5759,15 +5785,15 @@
 )
 
 request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.77
+            6.19
         ]
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
@@ -5823,15 +5849,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/legal-entities`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| type | str | ❌ | Retrieve a list of legal entities in your account. |
+| type\_ | str | ❌ | Retrieve a list of legal entities in your account. |
 
 **Return Type**
 
 `LegalEntityListContainer`
 
 **Example Usage Code Snippet**
 
@@ -6266,15 +6292,15 @@
 
 - HTTP Method: `GET`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| id | str | ✅ | Retrieve a single webhook subscription. |
+| id\_ | str | ✅ | Retrieve a single webhook subscription. |
 
 **Return Type**
 
 `WebhookItemResponse`
 
 **Example Usage Code Snippet**
 
@@ -6297,16 +6323,16 @@
 
 - HTTP Method: `PATCH`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| request_body | PatchWebhookRequest | ✅ | The request body. |
-| id | str | ✅ | Edit a webhook subscription. |
+| request*body | PatchWebhookRequest | ✅ | The request body. |
+| id* | str | ✅ | Edit a webhook subscription. |
 
 **Return Type**
 
 `WebhookItemResponse`
 
 **Example Usage Code Snippet**
 
@@ -6345,15 +6371,15 @@
 
 - HTTP Method: `DELETE`
 - Endpoint: `/webhooks/{id}`
 
 **Parameters**
 | Name | Type| Required | Description |
 | :-------- | :----------| :----------:| :----------|
-| id | str | ✅ | Delete a webhook subscription. |
+| id\_ | str | ✅ | Delete a webhook subscription. |
 
 **Example Usage Code Snippet**
 
 ```py
 from deel_sdk import DeelSdk, Environment
 
 sdk = DeelSdk(
```

### Comparing `deel-sdk-1.0.0/src/deel_sdk.egg-info/SOURCES.txt` & `deel-sdk-1.0.1/src/deel_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 src/deel_sdk/models/employee_timeoffs_item.py
 src/deel_sdk/models/employee_timeoffs_item_response.py
 src/deel_sdk/models/employee_timeoffs_policies_container.py
 src/deel_sdk/models/employee_timeoffs_policies_item.py
 src/deel_sdk/models/employment.py
 src/deel_sdk/models/employment_detail.py
 src/deel_sdk/models/employment_details_of_contract.py
-src/deel_sdk/models/entities.py
 src/deel_sdk/models/eor_client_timeoff_requests.py
 src/deel_sdk/models/eor_client_timeoffs.py
 src/deel_sdk/models/eor_client_timeoffs_container.py
 src/deel_sdk/models/eor_contract_benefits.py
 src/deel_sdk/models/eor_contract_benefits_container.py
 src/deel_sdk/models/eor_contract_created.py
 src/deel_sdk/models/eor_contract_created_container.py
@@ -179,15 +178,17 @@
 src/deel_sdk/models/generic_result_created.py
 src/deel_sdk/models/generic_result_created_with_id.py
 src/deel_sdk/models/generic_result_deleted.py
 src/deel_sdk/models/generic_result_updated.py
 src/deel_sdk/models/get_contract_list_currencies.py
 src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
 src/deel_sdk/models/get_employee_compliance_documents_container.py
+src/deel_sdk/models/get_invoice_list_entities.py
 src/deel_sdk/models/get_payment_list_currencies.py
+src/deel_sdk/models/get_payment_list_entities.py
 src/deel_sdk/models/global_payroll_g2_n_report.py
 src/deel_sdk/models/global_payroll_g2_n_report_container.py
 src/deel_sdk/models/gp_client.py
 src/deel_sdk/models/gp_contract_created.py
 src/deel_sdk/models/gp_contract_created_container.py
 src/deel_sdk/models/gp_contract_salary_scale_enum.py
 src/deel_sdk/models/gp_contract_salary_status_enum.py
```

