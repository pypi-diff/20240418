# Comparing `tmp/deel-sdk-1.0.1.tar.gz` & `tmp/deel_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deel-sdk-1.0.1.tar", last modified: Thu Apr 11 17:56:01 2024, max compression
+gzip compressed data, was "deel_sdk-1.0.2.tar", last modified: Thu Apr 18 09:08:17 2024, max compression
```

## Comparing `deel-sdk-1.0.1.tar` & `deel_sdk-1.0.2.tar`

### file list

```diff
@@ -1,462 +1,462 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/
--rw-r--r--   0 runner    (1001) runner    (1001)     1057 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)   189900 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)   189694 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)      343 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.293900 deel-sdk-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.293900 deel-sdk-1.0.1/src/deel_sdk/
--rw-r--r--   0 runner    (1001) runner    (1001)      125 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.293900 deel-sdk-1.0.1/src/deel_sdk/hooks/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/hooks/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      918 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/models/
--rw-r--r--   0 runner    (1001) runner    (1001)    24919 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      516 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/add_worker_bank_account_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/additional_eor_info_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1314 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/address.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1049 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      849 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2583 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1302 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update.py
--rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustments_categories_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/adjustments_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      659 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_user_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_user_create_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/admin_users_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/agreement.py
--rw-r--r--   0 runner    (1001) runner    (1001)      753 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/agreement_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      484 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/alternate_email_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      338 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/attachment_file_ref.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1254 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_added.py
--rw-r--r--   0 runner    (1001) runner    (1001)      476 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_added_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1639 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_guide.py
--rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_guide_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      699 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_to_add.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_to_add_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/bank_account_value_allowed.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10358 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3817 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6686 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_invoice_adjustment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1092 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_legal_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)      426 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      410 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_team.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6231 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/basic_timesheet.py
--rw-r--r--   0 runner    (1001) runner    (1001)      712 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/benefit_contribution_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      650 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/benefit_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1246 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/breakdown_costs_quote.py
--rw-r--r--   0 runner    (1001) runner    (1001)      916 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/calculate_final_payment_calculation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)      838 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2215 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_patch.py
--rw-r--r--   0 runner    (1001) runner    (1001)      502 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_patch_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/client_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1456 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract_legal_entity_5.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1661 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3559 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6134 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      418 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      456 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      446 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_payg_milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)      436 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_container_payg_tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)      631 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_custom_field.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5768 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_details_to_amend.py
--rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_document_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_external_id_to_patch.py
--rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_invitation_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_invitation_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      637 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      540 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2449 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      730 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_template.py
--rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_template_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      598 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_template_summary.py
--rw-r--r--   0 runner    (1001) runner    (1001)      784 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)      539 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      581 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_amend_details_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1034 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      831 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      591 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)      541 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12731 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_ongoing_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12848 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9214 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8828 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1047 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_terminate.py
--rw-r--r--   0 runner    (1001) runner    (1001)      497 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_to_terminate_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1827 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum_for_estimate.py
--rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contract_who_reports_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contracts_sort_by_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1068 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/contribution.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1020 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/cost_quote.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1368 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/country.py
--rw-r--r--   0 runner    (1001) runner    (1001)      453 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/country_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_admin_user_response_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1731 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_people_timeoff.py
--rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_public_token.py
--rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_public_token_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2762 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_timeoff.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_timeoff_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1942 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/create_webhook_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)      417 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/currency.py
--rw-r--r--   0 runner    (1001) runner    (1001)      460 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/currency_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1206 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice.py
--rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      546 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/departments.py
--rw-r--r--   0 runner    (1001) runner    (1001)      473 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/departments_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      549 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/download_worker_documents_by_id_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/email.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9643 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee.py
--rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      660 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      386 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_contract_signature_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      597 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_contract_signature_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1796 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1078 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)      567 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      553 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_creation_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      651 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3302 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6384 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8435 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      619 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2975 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5398 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7421 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employment_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1396 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/employment_details_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2006 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoff_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoffs.py
--rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoffs_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9335 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13109 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13924 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_country_validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_country_validations_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1468 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)      635 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5990 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4905 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlement_list_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      603 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlements.py
--rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlements_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1232 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_field.py
--rw-r--r--   0 runner    (1001) runner    (1001)      937 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_holidays_rollover_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)      496 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_payslip_download_url_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      466 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_payslips_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6857 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_quote_base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5045 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_base_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      530 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1724 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_employee_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_item_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      676 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholders_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6024 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      582 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/file_attachment_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/file_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      879 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/file_ref_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/first_payment_date.py
--rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      852 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created_with_id.py
--rw-r--r--   0 runner    (1001) runner    (1001)      643 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_deleted.py
--rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/generic_result_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      303 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_contract_list_currencies.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1238 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_documents_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_invoice_list_entities.py
--rw-r--r--   0 runner    (1001) runner    (1001)      301 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_payment_list_currencies.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/get_payment_list_entities.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5154 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report.py
--rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      990 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7859 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      638 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      685 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      617 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_status_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5709 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      491 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      551 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1372 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      932 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1584 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated.py
--rw-r--r--   0 runner    (1001) runner    (1001)      602 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      579 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2127 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)      577 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_updated_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      523 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_update_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)      544 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_report_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      845 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_reports.py
--rw-r--r--   0 runner    (1001) runner    (1001)      494 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payslip_download_url_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/gp_payslips_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5236 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/health_insurance_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)      653 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hiring_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      414 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hr_document_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      542 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_compensation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2037 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_full_time.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2244 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_part_time.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3477 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1109 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3797 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_job_information_title_id.py
--rw-r--r--   0 runner    (1001) runner    (1001)      521 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_job_information_title_name.py
--rw-r--r--   0 runner    (1001) runner    (1001)      485 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/hris_team_information.py
--rw-r--r--   0 runner    (1001) runner    (1001)      241 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/identifier_value.py
--rw-r--r--   0 runner    (1001) runner    (1001)      882 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/input_to_create_file_ref.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/input_to_create_pgo_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/input_to_patch_contract_external_id.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8507 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/internal_people.py
--rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/internal_people_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invitations_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2528 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice.py
--rw-r--r--   0 runner    (1001) runner    (1001)      503 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_attachment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1336 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      798 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1229 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      583 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1553 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      590 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      949 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1640 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1840 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3514 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1131 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      507 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_download_link_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      347 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_download_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      687 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      961 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/invoice_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      545 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/job_title.py
--rw-r--r--   0 runner    (1001) runner    (1001)      805 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/job_title_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      572 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2378 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/letter_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1056 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/marital_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      728 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/meta_data_of_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2354 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone.py
--rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      467 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_properties.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      492 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      800 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/milestone_to_create_form_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)      427 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/monthly_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2137 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      469 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      804 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      563 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/organization_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      385 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/output_to_create_file_ref.py
--rw-r--r--   0 runner    (1001) runner    (1001)      513 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/output_to_create_file_ref_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      423 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/page_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      359 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/page_info_without_cursor.py
--rw-r--r--   0 runner    (1001) runner    (1001)      601 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/page_info_without_cursor_new.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2010 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/patch_webhook_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1828 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6179 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_break_down.py
--rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_break_down_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_method.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1794 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_method_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      664 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_object.py
--rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      854 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payment_worker.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4715 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payroll_adjustment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      307 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payslip_download_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)      645 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/payslips.py
--rw-r--r--   0 runner    (1001) runner    (1001)      913 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pension_eor_contract_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1290 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pension_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10185 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_by_id_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      736 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_client_legal_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)      750 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_custom_field.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_me.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1095 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1801 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_sort_by_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2067 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/people_time_off_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1471 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1282 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1349 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1105 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2885 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_result_added.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_result_added_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2487 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_to_add.py
--rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/premium_to_add_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3499 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/pro_rata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1008 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/profile_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/public_token.py
--rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/public_token_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_custom_verification_letter_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2920 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/request_custom_verification_letter_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2999 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/requester_time_off.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1029 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      914 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/salary_frequency_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      835 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/seniority.py
--rw-r--r--   0 runner    (1001) runner    (1001)      508 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/seniority_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      774 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/seniority_required.py
--rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1129 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/sort_dir_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/state_of_country.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1011 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/task_created.py
--rw-r--r--   0 runner    (1001) runner    (1001)      440 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/task_created_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/task_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team.py
--rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      571 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/team_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1270 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review_internal.py
--rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_to_review_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      515 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_to_review_internal_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      361 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoff_type_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1006 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_attachments_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1300 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_profile.py
--rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      648 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6364 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet.py
--rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_approver.py
--rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      249 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_id_items.py
--rw-r--r--   0 runner    (1001) runner    (1001)      711 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_list_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1520 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create.py
--rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      939 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_shared_properties.py
--rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_status_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      608 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container_with_file.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update.py
--rw-r--r--   0 runner    (1001) runner    (1001)      568 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      397 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_department.py
--rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_department_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_working_location.py
--rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/update_worker_working_location_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/upload_employee_compliance_document_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      406 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/upload_employee_compliance_document_file_container.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/models/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)     2636 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2642 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/utils/json_map.py
--rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/validation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/validation_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      625 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_list_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1682 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2910 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_item.py
--rw-r--r--   0 runner    (1001) runner    (1001)      438 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_item_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      472 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/webhook_list_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/week_days_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      776 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_end_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      895 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      666 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_payment_due_type_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)      988 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/work_statement_scale_enum.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5945 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5328 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_to_add.py
--rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_accounts_info_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1317 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_document.py
--rw-r--r--   0 runner    (1001) runner    (1001)      618 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_document_download_link.py
--rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_documents_by_id_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      806 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_legal_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1237 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_of_basic_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3079 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_of_contract.py
--rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1140 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_body_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_container.py
--rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/working_locations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/models/working_locations_container.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/environment/
--rw-r--r--   0 runner    (1001) runner    (1001)       96 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      396 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/headers/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1184 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/headers/access_token_auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)      225 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1221 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1704 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2592 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2452 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1835 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.337900 deel-sdk-1.0.1/src/deel_sdk/net/transport/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2704 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1692 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2304 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8604 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) runner    (1001)      681 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/net/transport/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5090 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/src/deel_sdk/services/
--rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8586 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/accounting.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7738 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/adjustments.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/candidates.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1641 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/carta.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12960 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/contractors.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22181 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/contracts.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7352 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/eor.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19010 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/global_payroll.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17310 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/invoices.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5044 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/lookups.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2584 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/managers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8032 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/milestones.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4151 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/off_cycle_payments.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/organizations.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22375 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/partner_managed.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18569 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/people.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7063 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/tasks.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8293 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/time_off.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14194 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/timesheets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1385 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/token.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/src/deel_sdk/services/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)     2256 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1603 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8007 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/utils/validator.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5237 2024-04-11 17:55:46.000000 deel-sdk-1.0.1/src/deel_sdk/services/webhooks.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-11 17:56:01.341901 deel-sdk-1.0.1/src/deel_sdk.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)   189900 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    21372 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       17 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-11 17:56:01.000000 deel-sdk-1.0.1/src/deel_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.208049 deel_sdk-1.0.2/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1057 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)   188973 2024-04-18 09:08:17.208049 deel_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)   188767 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)      343 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-18 09:08:17.208049 deel_sdk-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.088049 deel_sdk-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.092049 deel_sdk-1.0.2/src/deel_sdk/
+-rw-r--r--   0 runner    (1001) runner    (1001)      125 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.096048 deel_sdk-1.0.2/src/deel_sdk/hooks/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      918 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.192049 deel_sdk-1.0.2/src/deel_sdk/models/
+-rw-r--r--   0 runner    (1001) runner    (1001)    24919 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      516 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/add_worker_bank_account_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/additional_eor_info_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1314 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1049 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      849 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2484 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1302 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      517 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustments_categories_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/adjustments_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      659 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_user_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_user_create_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/admin_users_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2400 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/agreement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      753 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/agreement_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      484 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/alternate_email_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      338 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/attachment_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1254 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_added.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      476 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_added_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1639 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_guide.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_guide_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      699 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_to_add_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      696 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/bank_account_value_allowed.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10358 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3817 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6686 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_invoice_adjustment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1092 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      426 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      410 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_team.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6231 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/basic_timesheet.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      712 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/benefit_contribution_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      650 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/benefit_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1246 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/breakdown_costs_quote.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      916 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/calculate_final_payment_calculation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      838 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2215 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2372 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_patch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      502 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_patch_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/client_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1456 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract_legal_entity_5.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1661 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3460 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6134 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      418 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      456 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      446 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      436 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_container_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      631 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_custom_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5768 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_details_to_amend.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_document_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      424 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_external_id_to_patch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_invitation_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      547 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_invitation_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      637 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      540 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2449 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      730 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_template.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_template_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      598 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_template_summary.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      661 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      539 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      581 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_amend_details_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1034 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      831 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      591 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      541 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12535 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_ongoing_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12652 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9026 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8731 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_terminate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      497 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_to_terminate_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1827 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum_for_estimate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contract_who_reports_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contracts_sort_by_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1068 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/contribution.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1020 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/cost_quote.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1368 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/country.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      453 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/country_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_admin_user_response_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1731 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_people_timeoff.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      431 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_public_token.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_public_token_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2762 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_timeoff.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_timeoff_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1942 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/create_webhook_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      417 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/currency.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      460 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/currency_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1206 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      546 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/departments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      473 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/departments_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      549 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/download_worker_documents_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/email.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9643 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      570 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      660 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      386 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_contract_signature_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      597 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_contract_signature_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1796 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1078 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      567 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      553 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_creation_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      651 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3302 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6384 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8435 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      619 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2975 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5398 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7421 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employment_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1396 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/employment_details_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2006 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoff_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoffs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9155 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13172 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      498 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13924 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_country_validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_country_validations_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1468 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      635 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5990 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4905 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlement_list_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      603 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlements.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      504 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlements_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1232 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      937 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_holidays_rollover_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      496 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_payslip_download_url_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      466 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_quote_base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5045 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_base_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      530 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1724 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_employee_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_item_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      676 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholders_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6024 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      582 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/file_attachment_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/file_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      879 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/file_ref_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      437 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/first_payment_date.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      852 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created_with_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      643 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_deleted.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      628 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/generic_result_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      303 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_contract_list_currencies.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1238 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_documents_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_invoice_list_entities.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      301 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_payment_list_currencies.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/get_payment_list_entities.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5154 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      990 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7507 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      483 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      638 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      685 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      617 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_status_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5709 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      491 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      551 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      716 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1372 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      932 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1584 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      602 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      579 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2033 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      577 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_updated_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      523 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_update_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      544 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_report_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      845 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_reports.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      494 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payslip_download_url_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/gp_payslips_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5236 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/health_insurance_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      653 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hiring_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      414 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hr_document_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      542 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      505 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_compensation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1948 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_full_time.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2155 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_part_time.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3477 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1109 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3797 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_job_information_title_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      521 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_job_information_title_name.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      485 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/hris_team_information.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      241 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/identifier_value.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      882 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/input_to_create_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/input_to_create_pgo_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/input_to_patch_contract_external_id.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8507 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/internal_people.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/internal_people_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      673 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invitations_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2311 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      503 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_attachment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1336 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      798 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1229 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      583 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1553 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      590 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      949 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1640 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1840 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3514 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1131 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      507 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_download_link_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      347 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_download_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      687 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      961 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/invoice_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      545 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/job_title.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      805 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/job_title_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      576 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      572 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2378 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/letter_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1056 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/marital_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      728 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/meta_data_of_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2541 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      467 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_properties.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1354 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      492 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      800 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/milestone_to_create_form_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      427 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/monthly_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2261 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      469 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      804 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      563 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/organization_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      385 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/output_to_create_file_ref.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      513 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/output_to_create_file_ref_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      423 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/page_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      359 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/page_info_without_cursor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      601 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/page_info_without_cursor_new.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2010 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/patch_webhook_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1828 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6179 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_break_down.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      510 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_break_down_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      450 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      589 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_method.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1794 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_method_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      664 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_object.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      854 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payment_worker.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4715 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payroll_adjustment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      307 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payslip_download_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      645 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/payslips.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      913 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pension_eor_contract_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1290 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pension_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10185 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      736 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_client_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      750 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      624 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_custom_field.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_me.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1095 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1801 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_sort_by_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2067 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/people_time_off_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1567 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1282 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1537 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1105 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2885 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_result_added.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_result_added_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2487 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/premium_to_add_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3499 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/pro_rata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1008 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/profile_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/public_token.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      454 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/public_token_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      586 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      556 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      490 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_custom_verification_letter_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2920 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/request_custom_verification_letter_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2999 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/requester_time_off.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1029 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      914 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/salary_frequency_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      835 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/seniority.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      508 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/seniority_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      774 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/seniority_required.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1129 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      514 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/sort_dir_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      465 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/state_of_country.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1132 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/task_created.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      440 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/task_created_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      448 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/task_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      552 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      571 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      561 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/team_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      620 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1270 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review_internal.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      458 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_to_review_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      515 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_to_review_internal_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      361 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoff_type_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1006 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_attachments_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1300 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_profile.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      648 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6364 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      529 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_approver.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      425 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      249 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_id_items.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      711 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_list_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1196 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1520 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      533 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      939 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_shared_properties.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_status_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      608 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1125 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container_with_file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      568 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      538 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      518 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      606 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      554 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      911 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/upload_employee_compliance_document_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      406 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/upload_employee_compliance_document_file_container.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.192049 deel_sdk-1.0.2/src/deel_sdk/models/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2636 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2642 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/utils/json_map.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/validation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      662 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/validation_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      625 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_list_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1682 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2910 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_item.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      438 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_item_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      472 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/webhook_list_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      951 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/week_days_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      776 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_end_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      895 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      666 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_payment_due_type_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      988 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/work_statement_scale_enum.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5945 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5328 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_to_add.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      548 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_accounts_info_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1317 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_document.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      618 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_document_download_link.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      526 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_documents_by_id_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      806 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_legal_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1237 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_of_basic_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3079 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_of_contract.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1140 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      511 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_body_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      482 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_container.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      555 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/working_locations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      509 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/models/working_locations_container.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.192049 deel_sdk-1.0.2/src/deel_sdk/net/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/environment/
+-rw-r--r--   0 runner    (1001) runner    (1001)       96 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      396 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/headers/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1184 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/headers/access_token_auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      225 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.196049 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1221 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1704 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2578 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2442 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1835 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.200049 deel_sdk-1.0.2/src/deel_sdk/net/transport/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2704 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1652 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2308 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8604 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      681 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5111 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.204048 deel_sdk-1.0.2/src/deel_sdk/services/
+-rw-r--r--   0 runner    (1001) runner    (1001)       58 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/accounting.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7738 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/adjustments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/candidates.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1641 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/carta.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12960 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/contractors.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22150 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/contracts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7352 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/eor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18979 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/global_payroll.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17186 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/invoices.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5044 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/lookups.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2584 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/managers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8032 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/milestones.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4151 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/off_cycle_payments.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/organizations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22375 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/partner_managed.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18569 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/people.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7063 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/tasks.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8293 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/time_off.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14070 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/timesheets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1385 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/token.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.204048 deel_sdk-1.0.2/src/deel_sdk/services/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2256 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1603 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8007 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/utils/validator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5237 2024-04-18 09:07:47.000000 deel_sdk-1.0.2/src/deel_sdk/services/webhooks.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-18 09:08:17.204048 deel_sdk-1.0.2/src/deel_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)   188973 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    21372 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       17 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-18 09:08:17.000000 deel_sdk-1.0.2/src/deel_sdk.egg-info/top_level.txt
```

### Comparing `deel-sdk-1.0.1/LICENSE` & `deel_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/PKG-INFO` & `deel_sdk-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: deel-sdk
-Version: 1.0.1
-Summary: Deel REST API
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# DeelSdk Python SDK 1.0.1
+# DeelSdk Python SDK 1.0.2
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.1
+- SDK version: 1.0.2
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
@@ -177,15 +167,15 @@
 ])
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
     entities=entities,
     limit=10,
-    offset=707020693.68
+    offset=808037660.53
 )
 
 print(result)
 ```
 
 #### **get_deel_invoice_list**
 
@@ -214,15 +204,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.accounting.get_deel_invoice_list(
     contract_id="contract_id",
     limit=10,
-    offset=898896522.23
+    offset=237799437.03
 )
 
 print(result)
 ```
 
 #### **get_billing_invoice_download_link**
 
@@ -401,16 +391,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdminUserCreateContainer(**{
     "data": {
-        "first_name": "proident molli",
-        "last_name": "anim ci",
+        "first_name": "dolore",
+        "last_name": "proi",
         "email": "email"
     }
 })
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
@@ -471,36 +461,36 @@
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
     "team_information": {
-        "team_id": 1.64,
-        "legal_entity_id": 2.97
+        "team_id": 9.77,
+        "legal_entity_id": 2.18
     },
     "job_information": {
-        "seniority_id": 1.14,
-        "job_title_id": 6.17
+        "seniority_id": 9.22,
+        "job_title_id": 6.5
     },
     "compensation": {
-        "gross_annual_salary": 5.95,
+        "gross_annual_salary": 7.15,
         "currency": "USD"
     },
     "contract": {
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 3.49,
+        "employee_number": 9.02,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 75.13
+        "part_time_percentage": 21.67
     },
     "vacation_info": {
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 295.88
+        "vacation_yearly_policy": 171.07
     }
 })
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
@@ -529,16 +519,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=92741896.72,
-    limit=88.8
+    offset=978653984.34,
+    limit=43.45
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -569,16 +559,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=311381742.98,
-    limit=139.17,
+    offset=44334375.53,
+    limit=105.69,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -1221,38 +1211,38 @@
                 "country": "US"
             }
         },
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
-            "work_visa_required": True,
+            "work_visa_required": False,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 2.27,
+            "probation_period": 6.17,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 4.71
+            "holidays": 5.67
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
-            "salary": 0.96,
+            "salary": 5.95,
             "currency": "currency",
-            "variable_compensation": 6.36,
+            "variable_compensation": 3.49,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
@@ -1319,46 +1309,46 @@
 )
 
 request_body = GpContractToCreateContainer(**{
     "data": {
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "ipsum ad tempor",
-            "work_email": "Lorem ullamco ",
+            "email": "culpa Lorem inc",
+            "work_email": "in do L",
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
-                "allowance": 1.94,
+                "allowance": 5.28,
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
-            "salary": 2.33,
+            "salary": 8.05,
             "currency": "GBP"
         }
     }
 })
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
@@ -2004,35 +1994,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "adquis culpa reprehenderit sed in"
+            "name": "sedDuis officia est laborum in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "ametnos",
+            "expected_email": "occae",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 3.56,
+            "amount": 2.6,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2090,28 +2080,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "nulla"
+            "name": "enim irure dolore magna"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis esse ex",
+            "expected_email": "Duis nulla oc",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2175,28 +2165,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "mollit"
+            "name": "et dolore"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "proid",
+            "expected_email": "sint ",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2260,35 +2250,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "Lorem"
+            "name": "cillum"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "anim sit",
+            "expected_email": "Lorem sint et",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 6.09,
+            "amount": 7.36,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2346,35 +2336,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "adquis culpa reprehenderit sed in"
+            "name": "sedDuis officia est laborum in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "ametnos",
+            "expected_email": "occae",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 3.56,
+            "amount": 2.6,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2458,21 +2448,21 @@
 request_body = ContractToAmendDetailsContainer(**{
     "data": {
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 8.79,
+        "first_payment": 0.24,
         "frequency": "weekly",
-        "cycle_end": 28.13,
+        "cycle_end": 24.94,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 6.51,
-        "pay_before_weekends": False,
+        "payment_due_days": 0.92,
+        "pay_before_weekends": True,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
 })
@@ -2647,20 +2637,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat cil",
+        "amount": "cupidatat exe",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "nisi nulla",
+        "file": "qu",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2726,18 +2716,18 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdjustmentToUpdateContainer(**{
     "data": {
-        "amount": "proident",
+        "amount": "ut velit in",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "enim repr"
+        "file": "incididunt "
     }
 })
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
@@ -2922,15 +2912,15 @@
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "sunt ullamco es",
+        "email": "dolore",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.add_candidate(request_body=request_body)
@@ -2970,15 +2960,15 @@
     "data": {
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "laboris a",
+        "email": "Excepteur nu",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.patch_candidate(
@@ -3081,15 +3071,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EmployeeContractSignatureToCreateContainer(**{
     "data": {
-        "signature": "inci"
+        "signature": "aliqua sed comm"
     }
 })
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
@@ -3125,15 +3115,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = RequestCustomVerificationLetterContainer(**{
     "data": {
-        "description": "Excepteur Duisi",
+        "description": "magnaest ea con",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
 })
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
@@ -3206,15 +3196,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=5.13
+    document_id=1.72
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3540,15 +3530,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=3.06
+    document_id=1.36
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3575,15 +3565,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.72
+    document_id=5.91
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3625,15 +3615,14 @@
 | [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
 | [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
 | [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
 | [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
 | [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
 | [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
 | [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
-| [archive_contract](#archive_contract)                                       | Archive a terminated, cancelled or completed contract.                                                                                                                                                               |
 | [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
 | [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
 | [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
 | [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
 | [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
 | [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
 | [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
@@ -3914,58 +3903,27 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractSignatureToCreateContainer(**{
     "data": {
-        "client_signature": "proident e",
-        "contract_template_id": 1.32
+        "client_signature": "ea exercitat",
+        "contract_template_id": 8.35
     }
 })
 
 result = sdk.contracts.sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
 ```
 
-#### **archive_contract**
-
-Archive a terminated, cancelled or completed contract.
-
-- HTTP Method: `PATCH`
-- Endpoint: `/contracts/{contract_id}/archive`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Archive a terminated, cancelled or completed contract. |
-
-**Return Type**
-
-`GenericResultUpdated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.archive_contract(contract_id="contract_id")
-
-print(result)
-```
-
 #### **invite_to_sign_contract**
 
 Invite a worker to sign the contract. Worker will be notified via email.
 
 - HTTP Method: `POST`
 - Endpoint: `/contracts/{contract_id}/invitations`
 
@@ -3988,16 +3946,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractInvitationToCreateContainer(**{
     "data": {
-        "email": "dolore c",
-        "message": "mini"
+        "email": "eiusm",
+        "message": "officia ut"
     }
 })
 
 result = sdk.contracts.invite_to_sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -4110,18 +4068,18 @@
         "type_": "ongoing_time_based",
         "country_code": "US",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 2500,
             "currency_code": "GBP",
             "scale": "weekly",
-            "cycle_end": 18.59,
+            "cycle_end": 30.28,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
-            "payment_due_days": 36.88,
+            "payment_due_days": 11.81,
             "calculation_type": "CUSTOM_AMOUNT",
             "work_week_start": "Sunday",
             "work_week_end": "Sunday"
         }
     }
 })
 
@@ -4216,15 +4174,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.contracts.get_download_worker_documents_by_id(
     worker_id="worker_id",
-    document_id=1.09
+    document_id=8.43
 )
 
 print(result)
 ```
 
 ### TasksService
 
@@ -4503,15 +4461,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=97685509.73
+    offset=564786626.18
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4556,15 +4514,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=90326358.62
+    offset=911169937.96
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4665,15 +4623,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = TimesheetToUpdateContainer(**{
     "data": {
         "description": "description",
-        "quantity": 9.63
+        "quantity": 3.77
     }
 })
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
@@ -4787,15 +4745,15 @@
 )
 
 request_body = TimesheetReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.19
+            1.77
         ]
     }
 })
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
@@ -5033,15 +4991,15 @@
 )
 
 request_body = MilestoneReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.74
+            6.78
         ]
     }
 })
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
@@ -5244,17 +5202,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": False,
+        "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": False,
+        "is_start_date_half_day": True,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
@@ -5294,17 +5252,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": False,
+        "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": False,
+        "is_start_date_half_day": True,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
@@ -5519,15 +5477,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=560002501.34
+    offset=226515477.25
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5579,15 +5537,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=729203388.82
+    offset=240522187.51
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5620,21 +5578,21 @@
 request_body = InvoiceAdjustmentToCreateContainer(**{
     "data": {
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 5.08
+        "payment_cycle_id": 6.69
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
-    recurring=True
+    recurring=False
 )
 
 print(result)
 ```
 
 #### **update_invoice_adjustment_by_id**
 
@@ -5662,16 +5620,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = InvoiceAdjustmentToUpdateContainer(**{
     "data": {
-        "description": "aute veniam in fugiat",
-        "amount": 2.65
+        "description": "sunt laborum Duis exercitation id",
+        "amount": 9.39
     }
 })
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
@@ -5785,15 +5743,15 @@
 )
 
 request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.19
+            1.77
         ]
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
```

### Comparing `deel-sdk-1.0.1/README.md` & `deel_sdk-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# DeelSdk Python SDK 1.0.1
+Metadata-Version: 2.1
+Name: deel-sdk
+Version: 1.0.2
+Summary: Deel REST API
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# DeelSdk Python SDK 1.0.2
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.1
+- SDK version: 1.0.2
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
@@ -167,15 +177,15 @@
 ])
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
     entities=entities,
     limit=10,
-    offset=707020693.68
+    offset=808037660.53
 )
 
 print(result)
 ```
 
 #### **get_deel_invoice_list**
 
@@ -204,15 +214,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.accounting.get_deel_invoice_list(
     contract_id="contract_id",
     limit=10,
-    offset=898896522.23
+    offset=237799437.03
 )
 
 print(result)
 ```
 
 #### **get_billing_invoice_download_link**
 
@@ -391,16 +401,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdminUserCreateContainer(**{
     "data": {
-        "first_name": "proident molli",
-        "last_name": "anim ci",
+        "first_name": "dolore",
+        "last_name": "proi",
         "email": "email"
     }
 })
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
@@ -461,36 +471,36 @@
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
     "team_information": {
-        "team_id": 1.64,
-        "legal_entity_id": 2.97
+        "team_id": 9.77,
+        "legal_entity_id": 2.18
     },
     "job_information": {
-        "seniority_id": 1.14,
-        "job_title_id": 6.17
+        "seniority_id": 9.22,
+        "job_title_id": 6.5
     },
     "compensation": {
-        "gross_annual_salary": 5.95,
+        "gross_annual_salary": 7.15,
         "currency": "USD"
     },
     "contract": {
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 3.49,
+        "employee_number": 9.02,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 75.13
+        "part_time_percentage": 21.67
     },
     "vacation_info": {
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 295.88
+        "vacation_yearly_policy": 171.07
     }
 })
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
@@ -519,16 +529,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=92741896.72,
-    limit=88.8
+    offset=978653984.34,
+    limit=43.45
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -559,16 +569,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=311381742.98,
-    limit=139.17,
+    offset=44334375.53,
+    limit=105.69,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -1211,38 +1221,38 @@
                 "country": "US"
             }
         },
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
-            "work_visa_required": True,
+            "work_visa_required": False,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 2.27,
+            "probation_period": 6.17,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 4.71
+            "holidays": 5.67
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
-            "salary": 0.96,
+            "salary": 5.95,
             "currency": "currency",
-            "variable_compensation": 6.36,
+            "variable_compensation": 3.49,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
@@ -1309,46 +1319,46 @@
 )
 
 request_body = GpContractToCreateContainer(**{
     "data": {
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "ipsum ad tempor",
-            "work_email": "Lorem ullamco ",
+            "email": "culpa Lorem inc",
+            "work_email": "in do L",
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
-                "allowance": 1.94,
+                "allowance": 5.28,
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
-            "salary": 2.33,
+            "salary": 8.05,
             "currency": "GBP"
         }
     }
 })
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
@@ -1994,35 +2004,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "adquis culpa reprehenderit sed in"
+            "name": "sedDuis officia est laborum in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "ametnos",
+            "expected_email": "occae",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 3.56,
+            "amount": 2.6,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2080,28 +2090,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "nulla"
+            "name": "enim irure dolore magna"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis esse ex",
+            "expected_email": "Duis nulla oc",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2165,28 +2175,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "mollit"
+            "name": "et dolore"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "proid",
+            "expected_email": "sint ",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2250,35 +2260,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "Lorem"
+            "name": "cillum"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "anim sit",
+            "expected_email": "Lorem sint et",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 6.09,
+            "amount": 7.36,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2336,35 +2346,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "adquis culpa reprehenderit sed in"
+            "name": "sedDuis officia est laborum in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "ametnos",
+            "expected_email": "occae",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 3.56,
+            "amount": 2.6,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2448,21 +2458,21 @@
 request_body = ContractToAmendDetailsContainer(**{
     "data": {
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 8.79,
+        "first_payment": 0.24,
         "frequency": "weekly",
-        "cycle_end": 28.13,
+        "cycle_end": 24.94,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 6.51,
-        "pay_before_weekends": False,
+        "payment_due_days": 0.92,
+        "pay_before_weekends": True,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
 })
@@ -2637,20 +2647,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat cil",
+        "amount": "cupidatat exe",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "nisi nulla",
+        "file": "qu",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2716,18 +2726,18 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdjustmentToUpdateContainer(**{
     "data": {
-        "amount": "proident",
+        "amount": "ut velit in",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "enim repr"
+        "file": "incididunt "
     }
 })
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
@@ -2912,15 +2922,15 @@
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "sunt ullamco es",
+        "email": "dolore",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.add_candidate(request_body=request_body)
@@ -2960,15 +2970,15 @@
     "data": {
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "laboris a",
+        "email": "Excepteur nu",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.patch_candidate(
@@ -3071,15 +3081,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EmployeeContractSignatureToCreateContainer(**{
     "data": {
-        "signature": "inci"
+        "signature": "aliqua sed comm"
     }
 })
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
@@ -3115,15 +3125,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = RequestCustomVerificationLetterContainer(**{
     "data": {
-        "description": "Excepteur Duisi",
+        "description": "magnaest ea con",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
 })
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
@@ -3196,15 +3206,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=5.13
+    document_id=1.72
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3530,15 +3540,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=3.06
+    document_id=1.36
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3565,15 +3575,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.72
+    document_id=5.91
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3615,15 +3625,14 @@
 | [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
 | [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
 | [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
 | [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
 | [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
 | [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
 | [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
-| [archive_contract](#archive_contract)                                       | Archive a terminated, cancelled or completed contract.                                                                                                                                                               |
 | [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
 | [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
 | [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
 | [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
 | [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
 | [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
 | [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
@@ -3904,58 +3913,27 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractSignatureToCreateContainer(**{
     "data": {
-        "client_signature": "proident e",
-        "contract_template_id": 1.32
+        "client_signature": "ea exercitat",
+        "contract_template_id": 8.35
     }
 })
 
 result = sdk.contracts.sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
 ```
 
-#### **archive_contract**
-
-Archive a terminated, cancelled or completed contract.
-
-- HTTP Method: `PATCH`
-- Endpoint: `/contracts/{contract_id}/archive`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Archive a terminated, cancelled or completed contract. |
-
-**Return Type**
-
-`GenericResultUpdated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.archive_contract(contract_id="contract_id")
-
-print(result)
-```
-
 #### **invite_to_sign_contract**
 
 Invite a worker to sign the contract. Worker will be notified via email.
 
 - HTTP Method: `POST`
 - Endpoint: `/contracts/{contract_id}/invitations`
 
@@ -3978,16 +3956,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractInvitationToCreateContainer(**{
     "data": {
-        "email": "dolore c",
-        "message": "mini"
+        "email": "eiusm",
+        "message": "officia ut"
     }
 })
 
 result = sdk.contracts.invite_to_sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -4100,18 +4078,18 @@
         "type_": "ongoing_time_based",
         "country_code": "US",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 2500,
             "currency_code": "GBP",
             "scale": "weekly",
-            "cycle_end": 18.59,
+            "cycle_end": 30.28,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
-            "payment_due_days": 36.88,
+            "payment_due_days": 11.81,
             "calculation_type": "CUSTOM_AMOUNT",
             "work_week_start": "Sunday",
             "work_week_end": "Sunday"
         }
     }
 })
 
@@ -4206,15 +4184,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.contracts.get_download_worker_documents_by_id(
     worker_id="worker_id",
-    document_id=1.09
+    document_id=8.43
 )
 
 print(result)
 ```
 
 ### TasksService
 
@@ -4493,15 +4471,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=97685509.73
+    offset=564786626.18
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4546,15 +4524,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=90326358.62
+    offset=911169937.96
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4655,15 +4633,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = TimesheetToUpdateContainer(**{
     "data": {
         "description": "description",
-        "quantity": 9.63
+        "quantity": 3.77
     }
 })
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
@@ -4777,15 +4755,15 @@
 )
 
 request_body = TimesheetReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.19
+            1.77
         ]
     }
 })
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
@@ -5023,15 +5001,15 @@
 )
 
 request_body = MilestoneReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.74
+            6.78
         ]
     }
 })
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
@@ -5234,17 +5212,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": False,
+        "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": False,
+        "is_start_date_half_day": True,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
@@ -5284,17 +5262,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": False,
+        "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": False,
+        "is_start_date_half_day": True,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
@@ -5509,15 +5487,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=560002501.34
+    offset=226515477.25
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5569,15 +5547,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=729203388.82
+    offset=240522187.51
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5610,21 +5588,21 @@
 request_body = InvoiceAdjustmentToCreateContainer(**{
     "data": {
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 5.08
+        "payment_cycle_id": 6.69
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
-    recurring=True
+    recurring=False
 )
 
 print(result)
 ```
 
 #### **update_invoice_adjustment_by_id**
 
@@ -5652,16 +5630,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = InvoiceAdjustmentToUpdateContainer(**{
     "data": {
-        "description": "aute veniam in fugiat",
-        "amount": 2.65
+        "description": "sunt laborum Duis exercitation id",
+        "amount": 9.39
     }
 })
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
@@ -5775,15 +5753,15 @@
 )
 
 request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.19
+            1.77
         ]
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/hooks/hook.py` & `deel_sdk-1.0.2/src/deel_sdk/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/__init__.py` & `deel_sdk-1.0.2/src/deel_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/add_worker_bank_account_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/add_worker_bank_account_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/address.py` & `deel_sdk-1.0.2/src/deel_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_category.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_category.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,17 +54,15 @@
         date_of_adjustment: str = None,
         cycle_reference: str = None,
         move_next_cycle: bool = None,
     ):
         self.contract_id = contract_id
         self.amount = AdjustmentToCreateAmountGuard.return_one_of(amount)
         if date_of_adjustment is not None:
-            self.date_of_adjustment = self._pattern_matching(
-                date_of_adjustment, "^\d{4}-\d{2}-\d{2}$", "date_of_adjustment"
-            )
+            self.date_of_adjustment = date_of_adjustment
         self.title = title
         self.description = description
         if cycle_reference is not None:
             self.cycle_reference = cycle_reference
         self.file = file
         self.adjustment_category_id = adjustment_category_id
         if move_next_cycle is not None:
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustment_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustment_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/adjustments_categories_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/adjustments_categories_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/admin_user.py` & `deel_sdk-1.0.2/src/deel_sdk/models/admin_user.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/admin_user_create_request.py` & `deel_sdk-1.0.2/src/deel_sdk/models/admin_user_create_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/admin_users_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/admin_users_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/agreement.py` & `deel_sdk-1.0.2/src/deel_sdk/models/agreement.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,38 +51,38 @@
         self.name = name
 
 
 @JsonMap({"id_": "id"})
 class Agreement(BaseModel):
     """Agreement
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param agreement_title: agreement_title
     :type agreement_title: str
     :param agreement_type: agreement_type
     :type agreement_type: str
     :param msa: msa
     :type msa: Msa
     :param client_legal_entity: client_legal_entity
     :type client_legal_entity: AgreementClientLegalEntity
     :param provider_legal_entity: provider_legal_entity
     :type provider_legal_entity: ProviderLegalEntity
     """
 
     def __init__(
         self,
-        id_: str,
+        id_: IdentifierValue,
         agreement_title: str,
         agreement_type: str,
         msa: Msa,
         client_legal_entity: AgreementClientLegalEntity,
         provider_legal_entity: ProviderLegalEntity,
     ):
-        self.id_ = id_
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.agreement_title = agreement_title
         self.agreement_type = agreement_type
         self.msa = self._define_object(msa, Msa)
         self.client_legal_entity = self._define_object(
             client_legal_entity, AgreementClientLegalEntity
         )
         self.provider_legal_entity = self._define_object(
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/agreement_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/agreement_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_added.py` & `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_added.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_guide.py` & `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_guide.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_status.py` & `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_status.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_updated.py` & `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/bank_account_value_allowed.py` & `deel_sdk-1.0.2/src/deel_sdk/models/bank_account_value_allowed.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/base.py` & `deel_sdk-1.0.2/src/deel_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/basic_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/basic_invoice_adjustment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/basic_invoice_adjustment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/basic_legal_entity.py` & `deel_sdk-1.0.2/src/deel_sdk/models/basic_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/basic_timesheet.py` & `deel_sdk-1.0.2/src/deel_sdk/models/basic_timesheet.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/benefit_contribution_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/benefit_contribution_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/benefit_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/benefit_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/breakdown_costs_quote.py` & `deel_sdk-1.0.2/src/deel_sdk/models/breakdown_costs_quote.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/calculate_final_payment_calculation_type.py` & `deel_sdk-1.0.2/src/deel_sdk/models/calculate_final_payment_calculation_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/candidate_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/candidate_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/candidate_to_patch.py` & `deel_sdk-1.0.2/src/deel_sdk/models/candidate_to_patch.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/client_of_basic_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/client_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/client_of_contract_legal_entity_5.py` & `deel_sdk-1.0.2/src/deel_sdk/models/client_of_contract_legal_entity_5.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py` & `deel_sdk-1.0.2/src/deel_sdk/models/compensation_details_of_contract_to_create_shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,12 @@
         self.payment_due_type = self._enum_matching(
             payment_due_type, WorkStatementPaymentDueTypeEnum.list(), "payment_due_type"
         )
         self.payment_due_days = payment_due_days
         if pay_before_weekends is not None:
             self.pay_before_weekends = pay_before_weekends
         if first_payment_date is not None:
-            self.first_payment_date = self._pattern_matching(
-                first_payment_date, "^\d{4}-\d{2}-\d{2}$", "first_payment_date"
-            )
+            self.first_payment_date = first_payment_date
         if first_payment is not None:
             self.first_payment = first_payment
         if notice_period is not None:
             self.notice_period = notice_period
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_custom_field.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_custom_field.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_details_to_amend.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_details_to_amend.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_document_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_document_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_invitation_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_invitation_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_signature_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_signature_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_template.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_template.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_template_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_template_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_template_summary.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_template_summary.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 
 @JsonMap({"id_": "id"})
 class ContractTerminationResult(BaseModel):
     """ContractTerminationResult
 
     :param id_: Deel Contract ID., defaults to None
     :type id_: str, optional
-    :param completion_date: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31., defaults to None
+    :param completion_date: Long date-time format following ISO-8601, defaults to None
     :type completion_date: str, optional
     """
 
     def __init__(self, id_: str = None, completion_date: str = None):
         if id_ is not None:
             self.id_ = id_
         if completion_date is not None:
-            self.completion_date = self._pattern_matching(
-                completion_date, "^\d{4}-\d{2}-\d{2}$", "completion_date"
-            )
+            self.completion_date = completion_date
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_termination_result_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_termination_result_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_amend_details_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_amend_details_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_ongoing_time_based.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_pay_as_you_go_time_based.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_milestones.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_milestones.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_container_payg_tasks.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_container_payg_tasks.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_ongoing_time_based.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_ongoing_time_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,17 +183,15 @@
         self.payment_due_type = self._enum_matching(
             payment_due_type, WorkStatementPaymentDueTypeEnum.list(), "payment_due_type"
         )
         self.payment_due_days = payment_due_days
         if pay_before_weekends is not None:
             self.pay_before_weekends = pay_before_weekends
         if first_payment_date is not None:
-            self.first_payment_date = self._pattern_matching(
-                first_payment_date, "^\d{4}-\d{2}-\d{2}$", "first_payment_date"
-            )
+            self.first_payment_date = first_payment_date
         if first_payment is not None:
             self.first_payment = first_payment
         if notice_period is not None:
             self.notice_period = notice_period
         self.scale = self._enum_matching(scale, WorkStatementScaleEnum.list(), "scale")
 
 
@@ -265,17 +263,15 @@
         if state_code is not None:
             self.state_code = state_code
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
         if special_clause is not None:
             self.special_clause = special_clause
         if termination_date is not None:
-            self.termination_date = self._pattern_matching(
-                termination_date, "^\d{4}-\d{2}-\d{2}$", "termination_date"
-            )
+            self.termination_date = termination_date
         self.client = self._define_object(
             client, ContractToCreateOngoingTimeBasedClient
         )
         self.job_title = self._define_object(
             job_title, ContractToCreateOngoingTimeBasedJobTitle
         )
         if seniority is not None:
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_pay_as_you_go_time_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,17 +183,15 @@
         self.payment_due_type = self._enum_matching(
             payment_due_type, WorkStatementPaymentDueTypeEnum.list(), "payment_due_type"
         )
         self.payment_due_days = payment_due_days
         if pay_before_weekends is not None:
             self.pay_before_weekends = pay_before_weekends
         if first_payment_date is not None:
-            self.first_payment_date = self._pattern_matching(
-                first_payment_date, "^\d{4}-\d{2}-\d{2}$", "first_payment_date"
-            )
+            self.first_payment_date = first_payment_date
         if first_payment is not None:
             self.first_payment = first_payment
         if notice_period is not None:
             self.notice_period = notice_period
         self.scale = self._enum_matching(scale, WorkStatementScaleEnum.list(), "scale")
 
 
@@ -265,17 +263,15 @@
         if state_code is not None:
             self.state_code = state_code
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
         if special_clause is not None:
             self.special_clause = special_clause
         if termination_date is not None:
-            self.termination_date = self._pattern_matching(
-                termination_date, "^\d{4}-\d{2}-\d{2}$", "termination_date"
-            )
+            self.termination_date = termination_date
         self.client = self._define_object(
             client, ContractToCreatePayAsYouGoTimeBasedClient
         )
         self.job_title = self._define_object(
             job_title, ContractToCreatePayAsYouGoTimeBasedJobTitle
         )
         if seniority is not None:
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_milestones.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_milestones.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,17 +191,15 @@
         if state_code is not None:
             self.state_code = state_code
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
         if special_clause is not None:
             self.special_clause = special_clause
         if termination_date is not None:
-            self.termination_date = self._pattern_matching(
-                termination_date, "^\d{4}-\d{2}-\d{2}$", "termination_date"
-            )
+            self.termination_date = termination_date
         self.client = self._define_object(client, ContractToCreatePaygMilestonesClient)
         self.job_title = self._define_object(
             job_title, ContractToCreatePaygMilestonesJobTitle
         )
         if seniority is not None:
             self.seniority = self._define_object(
                 seniority, ContractToCreatePaygMilestonesSeniority
@@ -219,13 +217,11 @@
             self.worker = self._define_object(
                 worker, ContractToCreatePaygMilestonesWorker
             )
         self.type_ = self._enum_matching(
             type_, ContractToCreatePaygMilestonesType.list(), "type_"
         )
         if start_date is not None:
-            self.start_date = self._pattern_matching(
-                start_date, "^\d{4}-\d{2}-\d{2}$", "start_date"
-            )
+            self.start_date = start_date
         self.compensation_details = self._define_object(
             compensation_details, CompensationDetailsOfContractToCreateShared
         )
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_create_payg_tasks.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_create_payg_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,17 +188,15 @@
         if state_code is not None:
             self.state_code = state_code
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
         if special_clause is not None:
             self.special_clause = special_clause
         if termination_date is not None:
-            self.termination_date = self._pattern_matching(
-                termination_date, "^\d{4}-\d{2}-\d{2}$", "termination_date"
-            )
+            self.termination_date = termination_date
         self.client = self._define_object(client, ContractToCreatePaygTasksClient)
         self.job_title = self._define_object(
             job_title, ContractToCreatePaygTasksJobTitle
         )
         if seniority is not None:
             self.seniority = self._define_object(
                 seniority, ContractToCreatePaygTasksSeniority
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_to_terminate.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_to_terminate.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,12 @@
     def __init__(
         self,
         completion_date: str = None,
         terminate_now: bool = None,
         message: str = None,
     ):
         if completion_date is not None:
-            self.completion_date = self._pattern_matching(
-                completion_date, "^\d{4}-\d{2}-\d{2}$", "completion_date"
-            )
+            self.completion_date = completion_date
         if terminate_now is not None:
             self.terminate_now = terminate_now
         if message is not None:
             self.message = message
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_type_enum_for_estimate.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_type_enum_for_estimate.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contract_who_reports_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contract_who_reports_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contracts_sort_by_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contracts_sort_by_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/contribution.py` & `deel_sdk-1.0.2/src/deel_sdk/models/contribution.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/cost_quote.py` & `deel_sdk-1.0.2/src/deel_sdk/models/cost_quote.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/country.py` & `deel_sdk-1.0.2/src/deel_sdk/models/country.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/create_people_timeoff.py` & `deel_sdk-1.0.2/src/deel_sdk/models/create_people_timeoff.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/create_timeoff.py` & `deel_sdk-1.0.2/src/deel_sdk/models/create_timeoff.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/create_webhook_request.py` & `deel_sdk-1.0.2/src/deel_sdk/models/create_webhook_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice.py` & `deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/deel_invoice_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/deel_invoice_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/departments.py` & `deel_sdk-1.0.2/src/deel_sdk/models/departments.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/download_worker_documents_by_id_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/download_worker_documents_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/email.py` & `deel_sdk-1.0.2/src/deel_sdk/models/email.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_agreement_download_object.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_agreement_download_object.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_contract_signature_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_contract_signature_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_payslips_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_payslips_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_tax_documents_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_tax_documents_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_creation_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_creation_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_entitlements_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_entitlements_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_item_response.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_item_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employee_timeoffs_policies_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employee_timeoffs_policies_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employment_detail.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employment_detail.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/employment_details_of_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/employment_details_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoff_requests.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoff_requests.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_client_timeoffs.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_client_timeoffs.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_benefits_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_benefits_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_created.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_created.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,21 +43,17 @@
         time_off_type: str = None,
         probation_period: float = None,
         calculated_holidays: str = None,
     ):
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
         if start_date is not None:
-            self.start_date = self._pattern_matching(
-                start_date, "^\d{4}-\d{2}-\d{2}$", "start_date"
-            )
+            self.start_date = start_date
         if end_date is not None:
-            self.end_date = self._pattern_matching(
-                end_date, "^\d{4}-\d{2}-\d{2}$", "end_date"
-            )
+            self.end_date = end_date
         if country is not None:
             self.country = country
         if state is not None:
             self.state = state
         if work_visa_required is not None:
             self.work_visa_required = work_visa_required
         if time_off_type is not None:
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_contract_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_contract_to_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from enum import Enum
 from .utils.json_map import JsonMap
 from .base import BaseModel
 from .pension_eor_contract_to_create import PensionEorContractToCreate
+from .identifier_value import IdentifierValue, IdentifierValueGuard
 
 
 @JsonMap({})
 class EmployeeAddress1(BaseModel):
     """EmployeeAddress1
 
     :param street: Street and number., defaults to None
@@ -161,17 +162,15 @@
         if state is not None:
             self.state = state
         if type_ is not None:
             self.type_ = self._enum_matching(type_, EmploymentType.list(), "type_")
         self.work_visa_required = work_visa_required
         self.start_date = start_date
         if end_date is not None:
-            self.end_date = self._pattern_matching(
-                end_date, "^\d{4}-\d{2}-\d{2}$", "end_date"
-            )
+            self.end_date = end_date
         if probation_period is not None:
             self.probation_period = probation_period
         if scope_of_work is not None:
             self.scope_of_work = scope_of_work
         if time_off_type is not None:
             self.time_off_type = self._enum_matching(
                 time_off_type, TimeOffType.list(), "time_off_type"
@@ -180,46 +179,46 @@
             self.holidays = holidays
 
 
 @JsonMap({"id_": "id"})
 class EorContractToCreateSeniority(BaseModel):
     """EorContractToCreateSeniority
 
-    :param id_: Unique identifier of this resource., defaults to None
-    :type id_: str, optional
+    :param id_: id_, defaults to None
+    :type id_: IdentifierValue, optional
     """
 
-    def __init__(self, id_: str = None):
+    def __init__(self, id_: IdentifierValue = None):
         if id_ is not None:
-            self.id_ = id_
+            self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
 class ClientLegalEntity1(BaseModel):
     """ClientLegalEntity1
 
-    :param id_: Unique identifier of this resource., defaults to None
-    :type id_: str, optional
+    :param id_: id_, defaults to None
+    :type id_: IdentifierValue, optional
     """
 
-    def __init__(self, id_: str = None):
+    def __init__(self, id_: IdentifierValue = None):
         if id_ is not None:
-            self.id_ = id_
+            self.id_ = IdentifierValueGuard.return_one_of(id_)
 
 
 @JsonMap({"id_": "id"})
 class ClientTeam1(BaseModel):
     """ClientTeam1
 
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
 class EorContractToCreateClient(BaseModel):
     """EorContractToCreateClient
 
     :param legal_entity: legal_entity, defaults to None
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_country_validations.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_country_validations.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_request_body_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_employee_cost_calculation_response_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlement_list_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlement_list_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_entitlements.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_entitlements.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_field.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_field.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_holidays_rollover_type.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_holidays_rollover_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_quote_base.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_quote_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     :type gross_salary_total: float, optional
     :param gross_salary_total_usd: Total gross salary in USD, defaults to None
     :type gross_salary_total_usd: float, optional
     :param cba_total: Total CBA in local currency, defaults to None
     :type cba_total: float, optional
     :param cba_total_usd: Total CBA in USD, defaults to None
     :type cba_total_usd: float, optional
-    :param created_at: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31., defaults to None
+    :param created_at: Long date-time format following ISO-8601, defaults to None
     :type created_at: str, optional
-    :param updated_at: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31., defaults to None
+    :param updated_at: Long date-time format following ISO-8601, defaults to None
     :type updated_at: str, optional
     """
 
     def __init__(
         self,
         annual_salary: float = None,
         currency: str = None,
@@ -125,14 +125,10 @@
         if gross_salary_total_usd is not None:
             self.gross_salary_total_usd = gross_salary_total_usd
         if cba_total is not None:
             self.cba_total = cba_total
         if cba_total_usd is not None:
             self.cba_total_usd = cba_total_usd
         if created_at is not None:
-            self.created_at = self._pattern_matching(
-                created_at, "^\d{4}-\d{2}-\d{2}$", "created_at"
-            )
+            self.created_at = created_at
         if updated_at is not None:
-            self.updated_at = self._pattern_matching(
-                updated_at, "^\d{4}-\d{2}-\d{2}$", "updated_at"
-            )
+            self.updated_at = updated_at
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_base_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_base_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/eor_timeoffs_employee_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/eor_timeoffs_employee_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholder.py` & `deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholder.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/equity_stakeholders_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/equity_stakeholders_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/estimate_first_payment_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/estimate_first_payment_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/file_attachment_info.py` & `deel_sdk-1.0.2/src/deel_sdk/models/file_attachment_info.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/file_ref_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/file_ref_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated.py` & `deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/final_payment_calculated_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/final_payment_calculated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created.py` & `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_created_with_id.py` & `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_created_with_id.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_deleted.py` & `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_deleted.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/generic_result_updated.py` & `deel_sdk-1.0.2/src/deel_sdk/models/generic_result_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_document_template_download_link_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/get_employee_compliance_documents_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/get_employee_compliance_documents_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report.py` & `deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/global_payroll_g2_n_report_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/global_payroll_g2_n_report_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_client.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_client.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_created.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_created.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,34 +9,32 @@
 
 @JsonMap({})
 class EmploymentHolidays2(BaseModel):
     """EmploymentHolidays2
 
     :param allowance: Number of holidays., defaults to None
     :type allowance: float, optional
-    :param start_date: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31., defaults to None
+    :param start_date: Long date-time format following ISO-8601, defaults to None
     :type start_date: str, optional
     """
 
     def __init__(self, allowance: float = None, start_date: str = None):
         if allowance is not None:
             self.allowance = allowance
         if start_date is not None:
-            self.start_date = self._pattern_matching(
-                start_date, "^\d{4}-\d{2}-\d{2}$", "start_date"
-            )
+            self.start_date = start_date
 
 
 @JsonMap({"type_": "type"})
 class GpContractCreatedEmployment(BaseModel):
     """GpContractCreatedEmployment
 
-    :param start_date: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31., defaults to None
+    :param start_date: Long date-time format following ISO-8601, defaults to None
     :type start_date: str, optional
-    :param end_date: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31., defaults to None
+    :param end_date: Long date-time format following ISO-8601, defaults to None
     :type end_date: str, optional
     :param country: Country of employment., defaults to None
     :type country: str, optional
     :param state: State code of the state/province where this person will be employed., defaults to None
     :type state: str, optional
     :param type_: Is it a full-time contract or a part-time contract?, defaults to None
     :type type_: str, optional
@@ -53,21 +51,17 @@
         country: str = None,
         state: str = None,
         type_: str = None,
         work_visa_required: bool = None,
         holidays: EmploymentHolidays2 = None,
     ):
         if start_date is not None:
-            self.start_date = self._pattern_matching(
-                start_date, "^\d{4}-\d{2}-\d{2}$", "start_date"
-            )
+            self.start_date = start_date
         if end_date is not None:
-            self.end_date = self._pattern_matching(
-                end_date, "^\d{4}-\d{2}-\d{2}$", "end_date"
-            )
+            self.end_date = end_date
         if country is not None:
             self.country = country
         if state is not None:
             self.state = state
         if type_ is not None:
             self.type_ = type_
         if work_visa_required is not None:
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_scale_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_salary_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_salary_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_status_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_status_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_contract_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_update_data.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_address_updated_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_address_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_update_data.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_compensation_updated_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_compensation_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_update_data.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_update_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         if first_name is not None:
             self.first_name = first_name
         if middle_name is not None:
             self.middle_name = middle_name
         if last_name is not None:
             self.last_name = last_name
         if date_of_birth is not None:
-            self.date_of_birth = self._pattern_matching(
-                date_of_birth, "^\d{4}-\d{2}-\d{2}$", "date_of_birth"
-            )
+            self.date_of_birth = date_of_birth
         if gender is not None:
             self.gender = gender
         if marital_status is not None:
             self.marital_status = self._enum_matching(
                 marital_status, MaritalStatusEnum.list(), "marital_status"
             )
         if employee_number is not None:
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_information_updated_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_information_updated_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_employee_pto_update_data.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_employee_pto_update_data.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_report_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_report_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/gp_payroll_event_reports.py` & `deel_sdk-1.0.2/src/deel_sdk/models/gp_payroll_event_reports.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/health_insurance_provider.py` & `deel_sdk-1.0.2/src/deel_sdk/models/health_insurance_provider.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hiring_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hiring_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hr_verification_letters_and_documents_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_full_time.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_full_time.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,15 +53,13 @@
         end_date: str = None,
     ):
         self.contract_oid = contract_oid
         self.start_date = start_date
         if employee_number is not None:
             self.employee_number = employee_number
         if end_date is not None:
-            self.end_date = self._pattern_matching(
-                end_date, "^\d{4}-\d{2}-\d{2}$", "end_date"
-            )
+            self.end_date = end_date
         self.employment_type = self._enum_matching(
             employment_type,
             HrisContractFullTimeEmploymentType.list(),
             "employment_type",
         )
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_contract_part_time.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_contract_part_time.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,16 +56,14 @@
         end_date: str = None,
     ):
         self.contract_oid = contract_oid
         self.start_date = start_date
         if employee_number is not None:
             self.employee_number = employee_number
         if end_date is not None:
-            self.end_date = self._pattern_matching(
-                end_date, "^\d{4}-\d{2}-\d{2}$", "end_date"
-            )
+            self.end_date = end_date
         self.employment_type = self._enum_matching(
             employment_type,
             HrisContractPartTimeEmploymentType.list(),
             "employment_type",
         )
         self.part_time_percentage = part_time_percentage
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_details.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_details.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_direct_employee_response.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_direct_employee_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/hris_job_information_title_name.py` & `deel_sdk-1.0.2/src/deel_sdk/models/hris_job_information_title_name.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/input_to_create_file_ref.py` & `deel_sdk-1.0.2/src/deel_sdk/models/input_to_create_file_ref.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/input_to_patch_contract_external_id.py` & `deel_sdk-1.0.2/src/deel_sdk/models/input_to_patch_contract_external_id.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/internal_people.py` & `deel_sdk-1.0.2/src/deel_sdk/models/internal_people.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invitations_of_basic_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invitations_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     :type paid_at: str
     :param vat_total: Amount of VAT.
     :type vat_total: str
     :param vat_percentage: VAT percentage.
     :type vat_percentage: str
     :param is_overdue: Indicates if the invoice is overdue.
     :type is_overdue: bool
-    :param issued_at: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31.
+    :param issued_at: Long date-time format following ISO-8601
     :type issued_at: str
     :param vat_id: VAT identification number.
     :type vat_id: str
-    :param due_date: Short date in format ISO-8601 (YYYY-MM-DD). For example 2022-12-31.
+    :param due_date: Long date-time format following ISO-8601
     :type due_date: str
     :param contract_id: Unique identifier of the contract.
     :type contract_id: str
     """
 
     def __init__(
         self,
@@ -63,15 +63,11 @@
         self.created_at = created_at
         self.total = total
         self.label = label
         self.paid_at = paid_at
         self.vat_total = vat_total
         self.vat_percentage = vat_percentage
         self.is_overdue = is_overdue
-        self.issued_at = self._pattern_matching(
-            issued_at, "^\d{4}-\d{2}-\d{2}$", "issued_at"
-        )
+        self.issued_at = issued_at
         self.vat_id = vat_id
-        self.due_date = self._pattern_matching(
-            due_date, "^\d{4}-\d{2}-\d{2}$", "due_date"
-        )
+        self.due_date = due_date
         self.contract_id = contract_id
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_created_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_created_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_create_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_adjustment_type_to_create_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/invoice_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/invoice_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/job_title.py` & `deel_sdk-1.0.2/src/deel_sdk/models/job_title.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/job_title_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/job_title_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/legal_entity_type.py` & `deel_sdk-1.0.2/src/deel_sdk/models/legal_entity_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/letter_request.py` & `deel_sdk-1.0.2/src/deel_sdk/models/letter_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/marital_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/meta_data_of_contract_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/meta_data_of_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # This file was generated by liblab | https://liblab.com/
 
+from __future__ import annotations
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .identifier_value import IdentifierValue, IdentifierValueGuard
 
 
 @JsonMap({"id_": "id"})
 class MilestoneReviewedBy(BaseModel):
     """Reviewer's information.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param full_name: Reviewer's full name.
     :type full_name: str
     """
 
-    def __init__(self, id_: str, full_name: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue, full_name: str):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.full_name = full_name
 
 
 @JsonMap({"id_": "id"})
 class MilestoneReportedBy(BaseModel):
     """Milestone creator.
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param full_name: Reporter's full name.
     :type full_name: str
     """
 
-    def __init__(self, id_: str, full_name: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue, full_name: str):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.full_name = full_name
 
 
 @JsonMap({"id_": "id"})
 class Milestone(BaseModel):
     """Milestone
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param amount: Amount to be paid for the milestone.
     :type amount: str
     :param approval_requested: Indicates if the contractor has requested the approval for the milestone.
     :type approval_requested: bool
     :param reviewed_by: Reviewer's information.
     :type reviewed_by: MilestoneReviewedBy
     :param reported_by: Milestone creator.
@@ -56,25 +58,25 @@
     :type status: str
     :param created_at: Long date-time format following ISO-8601
     :type created_at: str
     """
 
     def __init__(
         self,
-        id_: str,
+        id_: IdentifierValue,
         amount: str,
         approval_requested: bool,
         reviewed_by: MilestoneReviewedBy,
         reported_by: MilestoneReportedBy,
         title: str,
         description: str,
         status: str,
         created_at: str,
     ):
-        self.id_ = id_
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.amount = amount
         self.approval_requested = approval_requested
         self.reviewed_by = self._define_object(reviewed_by, MilestoneReviewedBy)
         self.reported_by = self._define_object(reported_by, MilestoneReportedBy)
         self.title = title
         self.description = description
         self.status = status
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone_properties.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone_properties.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone_review_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone_reviews_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/milestone_to_create_form_with_file.py` & `deel_sdk-1.0.2/src/deel_sdk/models/milestone_to_create_form_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .identifier_value import IdentifierValue, IdentifierValueGuard
 from .invoice_adjustment_status_enum import InvoiceAdjustmentStatusEnum
 
 
 @JsonMap({"id_": "id"})
 class OffCyclePaymentReportedBy(BaseModel):
     """OffCyclePaymentReportedBy
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param full_name: Full name of the creator.
     :type full_name: str
     """
 
-    def __init__(self, id_: str, full_name: str):
-        self.id_ = id_
+    def __init__(self, id_: IdentifierValue, full_name: str):
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.full_name = full_name
 
 
 @JsonMap({"id_": "id"})
 class OffCyclePayment(BaseModel):
     """OffCyclePayment
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param status: status of invoice adjustment
     :type status: InvoiceAdjustmentStatusEnum
     :param description: Description of the off-cycle payment entry.
     :type description: str
     :param date_submitted: Long date-time format following ISO-8601
     :type date_submitted: str
     :param currency_code: currency_code
@@ -41,24 +42,24 @@
     :type created_at: str
     :param reported_by: reported_by
     :type reported_by: OffCyclePaymentReportedBy
     """
 
     def __init__(
         self,
-        id_: str,
+        id_: IdentifierValue,
         status: InvoiceAdjustmentStatusEnum,
         description: str,
         date_submitted: str,
         currency_code: str,
         amount: str,
         created_at: str,
         reported_by: OffCyclePaymentReportedBy,
     ):
-        self.id_ = id_
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.status = self._enum_matching(
             status, InvoiceAdjustmentStatusEnum.list(), "status"
         )
         self.description = description
         self.date_submitted = date_submitted
         self.currency_code = self._pattern_matching(
             currency_code, "^[A-Z]{3}$", "currency_code"
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/off_cycle_payment_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/off_cycle_payment_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/organization_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/organization_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/output_to_create_file_ref_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/output_to_create_file_ref_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/page_info_without_cursor_new.py` & `deel_sdk-1.0.2/src/deel_sdk/models/page_info_without_cursor_new.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/patch_webhook_request.py` & `deel_sdk-1.0.2/src/deel_sdk/models/patch_webhook_request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment_break_down.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment_break_down.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment_method.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment_method_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment_method_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment_object.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment_object.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payment_worker.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payment_worker.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payroll_adjustment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payroll_adjustment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/payslips.py` & `deel_sdk-1.0.2/src/deel_sdk/models/payslips.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pension_eor_contract_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pension_eor_contract_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pension_provider.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pension_provider.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_by_id_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_client_legal_entity.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_client_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_custom_field.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_custom_field.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_me.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_me.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_payment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_sort_by_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_sort_by_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/people_time_off_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/people_time_off_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file was generated by liblab | https://liblab.com/
 
 from __future__ import annotations
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .identifier_value import IdentifierValue, IdentifierValueGuard
 from .timesheet_status_enum import TimesheetStatusEnum
 from .file_attachment_info import FileAttachmentInfo
 
 
 @JsonMap({"id_": "id"})
 class PgoTask(BaseModel):
     """PgoTask
 
-    :param id_: Unique identifier of this resource.
-    :type id_: str
+    :param id_: id_
+    :type id_: IdentifierValue
     :param amount: Fixed rate for this task.
     :type amount: str
     :param date_submitted: Short date in format ISO-8601 (YYYY-MM-DD). For example: 2022-12-31.
     :type date_submitted: str
     :param description: Task description.
     :type description: str
     :param status: Status of this entry.
     :type status: TimesheetStatusEnum
     :param attachment: This object is used for linking file attachments to your records., defaults to None
     :type attachment: FileAttachmentInfo, optional
     """
 
     def __init__(
         self,
-        id_: str,
+        id_: IdentifierValue,
         amount: str,
         date_submitted: str,
         description: str,
         status: TimesheetStatusEnum,
         attachment: FileAttachmentInfo = None,
     ):
-        self.id_ = id_
+        self.id_ = IdentifierValueGuard.return_one_of(id_)
         self.amount = amount
         self.date_submitted = date_submitted
         self.description = description
         self.status = self._enum_matching(status, TimesheetStatusEnum.list(), "status")
         if attachment is not None:
             self.attachment = self._define_object(attachment, FileAttachmentInfo)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_by_id_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_reviews_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_reviews_to_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file was generated by liblab | https://liblab.com/
 
+from __future__ import annotations
 from enum import Enum
 from typing import List
 from .utils.json_map import JsonMap
 from .base import BaseModel
+from .identifier_value import IdentifierValue, IdentifierValueGuard
 
 
 class PgoTaskReviewsToCreateStatus(Enum):
     """An enumeration representing different categories.
 
     :cvar APPROVED: "approved"
     :vartype APPROVED: str
@@ -34,19 +36,22 @@
     """PgoTaskReviewsToCreate
 
     :param status: Review status.
     :type status: PgoTaskReviewsToCreateStatus
     :param reason: Additional comments with the reivew., defaults to None
     :type reason: str, optional
     :param ids: ids
-    :type ids: List[str]
+    :type ids: List[IdentifierValue]
     """
 
     def __init__(
-        self, status: PgoTaskReviewsToCreateStatus, ids: List[str], reason: str = None
+        self,
+        status: PgoTaskReviewsToCreateStatus,
+        ids: List[IdentifierValue],
+        reason: str = None,
     ):
         self.status = self._enum_matching(
             status, PgoTaskReviewsToCreateStatus.list(), "status"
         )
         if reason is not None:
             self.reason = reason
-        self.ids = ids
+        self.ids = self._define_list(ids, IdentifierValue)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pgo_task_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pgo_task_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/premium_result_added.py` & `deel_sdk-1.0.2/src/deel_sdk/models/premium_result_added.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/premium_to_add.py` & `deel_sdk-1.0.2/src/deel_sdk/models/premium_to_add.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/pro_rata.py` & `deel_sdk-1.0.2/src/deel_sdk/models/pro_rata.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/profile_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/profile_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_by_id_reviews_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/request_body_to_create_pgo_task_reviews_reviews_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/request_custom_verification_letter_with_file.py` & `deel_sdk-1.0.2/src/deel_sdk/models/request_custom_verification_letter_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/requester_time_off.py` & `deel_sdk-1.0.2/src/deel_sdk/models/requester_time_off.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment.py` & `deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/response_estimate_first_payment_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/response_estimate_first_payment_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/salary_frequency_scale_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/salary_frequency_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/seniority.py` & `deel_sdk-1.0.2/src/deel_sdk/models/seniority.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/seniority_required.py` & `deel_sdk-1.0.2/src/deel_sdk/models/seniority_required.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_basic_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/signatures_of_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/signatures_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/sort_dir_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/sort_dir_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/team.py` & `deel_sdk-1.0.2/src/deel_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/team_of_basic_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/team_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/team_of_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/team_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoff_review_internal.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoff_review_internal.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoff_to_review_internal_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoff_to_review_internal_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_attachments_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_attachments_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_profile.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_profile.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timeoffs_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timeoffs_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_approver.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_approver.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_list_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_list_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_review_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_review_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_reviews_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_reviews_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_shared_properties.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_shared_properties.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_status_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_status_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_create_container_with_file.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_create_container_with_file.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/timesheet_to_update_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/timesheet_to_update_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/update_worker_department_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/update_worker_department_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/update_worker_working_location_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/update_worker_working_location_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/upload_employee_compliance_document_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/upload_employee_compliance_document_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/utils/cast_models.py` & `deel_sdk-1.0.2/src/deel_sdk/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/utils/json_map.py` & `deel_sdk-1.0.2/src/deel_sdk/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/validation_type.py` & `deel_sdk-1.0.2/src/deel_sdk/models/validation_type.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/validation_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/validation_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_list_response.py` & `deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_list_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/webhook_event_type_response.py` & `deel_sdk-1.0.2/src/deel_sdk/models/webhook_event_type_response.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/webhook_item.py` & `deel_sdk-1.0.2/src/deel_sdk/models/webhook_item.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/week_days_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/week_days_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_end_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_end_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_cycle_scale_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_cycle_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_payment_due_type_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_payment_due_type_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/work_statement_scale_enum.py` & `deel_sdk-1.0.2/src/deel_sdk/models/work_statement_scale_enum.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_info.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_info.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_account_to_add.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_account_to_add.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_bank_accounts_info_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_bank_accounts_info_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_document.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_document.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_document_download_link.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_document_download_link.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_documents_by_id_container.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_documents_by_id_container.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_legal_entity.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_legal_entity.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_of_basic_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_of_basic_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_of_contract.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_of_contract.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/models/worker_termination_body.py` & `deel_sdk-1.0.2/src/deel_sdk/models/worker_termination_body.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/headers/access_token_auth.py` & `deel_sdk-1.0.2/src/deel_sdk/net/headers/access_token_auth.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/base_handler.py` & `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/hook_handler.py` & `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/http_handler.py` & `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/http_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,18 +43,18 @@
                 request.url,
                 headers=request.headers,
                 timeout=self._timeout_in_seconds,
                 **request_args,
             )
             response = Response(result)
 
-            if result.status_code >= 400:
+            if response.status >= 400:
                 return None, RequestError(
-                    message=f"{result.status_code} error in request to: {request.url}",
-                    status_code=result.status_code,
+                    message=f"{response.status} error in request to: {request.url}",
+                    status=response.status,
                     response=response,
                 )
 
             return response, None
         except Timeout:
             return None, RequestError("Request timed out")
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/handlers/retry_handler.py` & `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/handlers/retry_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,8 +60,8 @@
         :param Optional[Response] response: The response from the previous handler.
         :param Optional[RequestError] error: The error from the previous handler.
         :return: True if the request should be retried, False otherwise.
         :rtype: bool
         """
         if not error:
             return False
-        return error.status_code == 408 or error.status_code >= 500
+        return error.status == 408 or error.status >= 500
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/request_chain/request_chain.py` & `deel_sdk-1.0.2/src/deel_sdk/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/transport/request.py` & `deel_sdk-1.0.2/src/deel_sdk/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/transport/request_error.py` & `deel_sdk-1.0.2/src/deel_sdk/net/transport/request_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 
 
 class RequestError(IOError):
     """
     Class representing a Request Error.
 
     :ivar bool is_http_error: Indicates if the error is an HTTP error.
-    :ivar int status_code: The status code of the HTTP error.
+    :ivar int status: The status code of the HTTP error.
     :ivar Optional[Response] response: The response associated with the error.
     """
 
     def __init__(
         self,
         message: str,
-        status_code: Optional[int] = None,
+        status: Optional[int] = None,
         response: Optional[Response] = None,
         stack: Optional["RequestError"] = None,
     ):
         """
         Initialize a new instance of RequestError.
 
         :param str message: The error message.
-        :param Optional[int] status_code: The status code of the HTTP error.
+        :param Optional[int] status: The status code of the HTTP error.
         :param Optional[Response] response: The response associated with the error.
         """
         super().__init__(message)
         self.response = response
         self.stack = stack
 
-        if status_code is not None:
-            self.status_code = status_code
+        if status is not None:
+            self.status = status
             self.is_http_error = True
         else:
-            self.status_code = -1
+            self.status = -1
             self.is_http_error = False
 
     def __str__(self):
         """
         Get the string representation of the error.
 
         :return: The string representation of the error.
         :rtype: str
         """
         error_stack = []
         current_error = self
         while current_error is not None:
             error_stack.append(
-                f"Error: {super().__str__()}, Status Code: {current_error.status_code}"
+                f"Error: {super().__str__()}, Status Code: {current_error.status}"
             )
             current_error = current_error.stack
         return "\n".join(error_stack)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/transport/response.py` & `deel_sdk-1.0.2/src/deel_sdk/net/transport/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 from urllib.parse import parse_qs
 
 
 class Response:
     """
     A simple HTTP response wrapper class using the requests library.
 
-    :ivar int status_code: The status code of the HTTP response.
+    :ivar int status: The status code of the HTTP response.
     :ivar dict headers: The headers of the HTTP response.
     :ivar str body: The body of the HTTP response.
     """
 
     def __init__(self, response: RequestsResponse):
         """
         Initializes a Response object.
 
         :param RequestsResponse response: The requests.Response object.
         """
-        self.status_code = response.status_code
+        self.status = response.status_code
         self.headers = response.headers
         self.body = self._get_response_body(response)
 
     def __str__(self) -> str:
         """
         Return a string representation of the Response object.
 
         :return: A string representation of the Response object.
         :rtype: str
         """
-        return f"Response(status_code={self.status_code}, headers={self.headers}, body={self.body})"
+        return (
+            f"Response(status={self.status}, headers={self.headers}, body={self.body})"
+        )
 
     def _get_response_body(self, response: RequestsResponse) -> str:
         """
         Extracts the response body from a given HTTP response.
 
         This method attempts to parse the response body based on its content type.
         If the content type is JSON, it tries to parse the body as JSON.
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/transport/serializer.py` & `deel_sdk-1.0.2/src/deel_sdk/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/net/transport/utils.py` & `deel_sdk-1.0.2/src/deel_sdk/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/sdk.py` & `deel_sdk-1.0.2/src/deel_sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from .services.webhooks import WebhooksService
 from .services.token import TokenService
 from .services.carta import CartaService
 from .net.environment import Environment
 
 
 class DeelSdk:
-    def __init__(self, access_token: str, base_url: str = Environment.DEFAULT.value):
+    def __init__(
+        self, access_token: str = None, base_url: str = Environment.DEFAULT.value
+    ):
         """
         Initializes DeelSdk the SDK class.
         """
         self.accounting = AccountingService(base_url=base_url)
         self.managers = ManagersService(base_url=base_url)
         self.people = PeopleService(base_url=base_url)
         self.eor = EorService(base_url=base_url)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/accounting.py` & `deel_sdk-1.0.2/src/deel_sdk/services/accounting.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
         ...
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: PaymentListContainer
         """
 
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_from)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_to)
+        Validator(str).is_optional().validate(date_from)
+        Validator(str).is_optional().validate(date_to)
         Validator(GetPaymentListCurrencies).is_optional().validate(currencies)
         Validator(GetPaymentListEntities).is_optional().validate(entities)
 
         serialized_request = (
             Serializer(f"{self.base_url}/payments", self.get_default_headers())
             .add_query("date_from", date_from, nullable=True)
             .add_query("date_to", date_to, nullable=True)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/adjustments.py` & `deel_sdk-1.0.2/src/deel_sdk/services/adjustments.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/candidates.py` & `deel_sdk-1.0.2/src/deel_sdk/services/candidates.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/carta.py` & `deel_sdk-1.0.2/src/deel_sdk/services/carta.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/contractors.py` & `deel_sdk-1.0.2/src/deel_sdk/services/contractors.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/contracts.py` & `deel_sdk-1.0.2/src/deel_sdk/services/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: FinalPaymentCalculatedContainer
         """
 
         Validator(str).validate(contract_id)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(end_date)
+        Validator(str).is_optional().validate(end_date)
         Validator(CalculateFinalPaymentCalculationType).is_optional().validate(
             calculation_type
         )
         Validator(str).is_optional().validate(workweek_start)
         Validator(str).is_optional().validate(workweek_end)
 
         serialized_request = (
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/eor.py` & `deel_sdk-1.0.2/src/deel_sdk/services/eor.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/global_payroll.py` & `deel_sdk-1.0.2/src/deel_sdk/services/global_payroll.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         :raises RequestError: Raised when a request fails, with optional HTTP status code and details.
         ...
         :return: Successful operation.
         :rtype: GpPayrollEventReportContainer
         """
 
         Validator(str).validate(legal_entity_id)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(start_date)
+        Validator(str).is_optional().validate(start_date)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/gp/legal-entities/{{legal_entity_id}}/reports",
                 self.get_default_headers(),
             )
             .add_path("legal_entity_id", legal_entity_id)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/invoices.py` & `deel_sdk-1.0.2/src/deel_sdk/services/invoices.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         Validator(ContractTypeEnum).is_array().is_optional().validate(contract_types)
         Validator(InvoiceAdjustmentTypeEnum).is_array().is_optional().validate(types)
         Validator(InvoiceAdjustmentStatusEnum).is_array().is_optional().validate(
             statuses
         )
         Validator(str).is_optional().validate(invoice_id)
         Validator(str).is_optional().validate(reporter_id)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_from)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_to)
+        Validator(str).is_optional().validate(date_from)
+        Validator(str).is_optional().validate(date_to)
         Validator(float).is_optional().min(1).max(99).validate(limit)
         Validator(float).is_optional().min(0).max(999999999).validate(offset)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/contracts/{{contract_id}}/invoice-adjustments",
                 self.get_default_headers(),
@@ -160,16 +160,16 @@
         Validator(ContractTypeEnum).is_array().is_optional().validate(contract_types)
         Validator(InvoiceAdjustmentTypeEnum).is_array().is_optional().validate(types)
         Validator(InvoiceAdjustmentStatusEnum).is_array().is_optional().validate(
             statuses
         )
         Validator(str).is_optional().validate(invoice_id)
         Validator(str).is_optional().validate(reporter_id)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_from)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_to)
+        Validator(str).is_optional().validate(date_from)
+        Validator(str).is_optional().validate(date_to)
         Validator(float).is_optional().min(1).max(99).validate(limit)
         Validator(float).is_optional().min(0).max(999999999).validate(offset)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/invoice-adjustments", self.get_default_headers()
             )
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/lookups.py` & `deel_sdk-1.0.2/src/deel_sdk/services/lookups.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/managers.py` & `deel_sdk-1.0.2/src/deel_sdk/services/managers.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/milestones.py` & `deel_sdk-1.0.2/src/deel_sdk/services/milestones.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/off_cycle_payments.py` & `deel_sdk-1.0.2/src/deel_sdk/services/off_cycle_payments.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/organizations.py` & `deel_sdk-1.0.2/src/deel_sdk/services/organizations.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/partner_managed.py` & `deel_sdk-1.0.2/src/deel_sdk/services/partner_managed.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/people.py` & `deel_sdk-1.0.2/src/deel_sdk/services/people.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/tasks.py` & `deel_sdk-1.0.2/src/deel_sdk/services/tasks.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/time_off.py` & `deel_sdk-1.0.2/src/deel_sdk/services/time_off.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/timesheets.py` & `deel_sdk-1.0.2/src/deel_sdk/services/timesheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
         :rtype: TimesheetListContainer
         """
 
         Validator(str).validate(contract_id)
         Validator(ContractTypeEnum).is_array().is_optional().validate(contract_types)
         Validator(TimesheetStatusEnum).is_array().is_optional().validate(statuses)
         Validator(str).is_optional().validate(reporter_id)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_from)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_to)
+        Validator(str).is_optional().validate(date_from)
+        Validator(str).is_optional().validate(date_to)
         Validator(float).is_optional().min(1).max(99).validate(limit)
         Validator(float).is_optional().min(0).max(999999999).validate(offset)
 
         serialized_request = (
             Serializer(
                 f"{self.base_url}/contracts/{{contract_id}}/timesheets",
                 self.get_default_headers(),
@@ -131,16 +131,16 @@
         :rtype: TimesheetListContainer
         """
 
         Validator(str).is_optional().validate(contract_id)
         Validator(ContractTypeEnum).is_array().is_optional().validate(contract_types)
         Validator(TimesheetStatusEnum).is_array().is_optional().validate(statuses)
         Validator(str).is_optional().validate(reporter_id)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_from)
-        Validator(str).is_optional().pattern("^\d{4}-\d{2}-\d{2}$").validate(date_to)
+        Validator(str).is_optional().validate(date_from)
+        Validator(str).is_optional().validate(date_to)
         Validator(float).is_optional().min(1).max(99).validate(limit)
         Validator(float).is_optional().min(0).max(999999999).validate(offset)
 
         serialized_request = (
             Serializer(f"{self.base_url}/timesheets", self.get_default_headers())
             .add_query("contract_id", contract_id)
             .add_query("contract_types", contract_types)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/token.py` & `deel_sdk-1.0.2/src/deel_sdk/services/token.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/utils/base_service.py` & `deel_sdk-1.0.2/src/deel_sdk/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/utils/default_headers.py` & `deel_sdk-1.0.2/src/deel_sdk/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/utils/validator.py` & `deel_sdk-1.0.2/src/deel_sdk/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk/services/webhooks.py` & `deel_sdk-1.0.2/src/deel_sdk/services/webhooks.py`

 * *Files identical despite different names*

### Comparing `deel-sdk-1.0.1/src/deel_sdk.egg-info/PKG-INFO` & `deel_sdk-1.0.2/src/deel_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: deel-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Deel REST API
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# DeelSdk Python SDK 1.0.1
+# DeelSdk Python SDK 1.0.2
 
 A Python SDK for DeelSdk.
 
 - API version: 1.25.0
-- SDK version: 1.0.1
+- SDK version: 1.0.2
 
 Deel REST API
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Authentication](#authentication)
@@ -177,15 +177,15 @@
 ])
 
 result = sdk.accounting.get_invoice_list(
     issued_from_date="issued_from_date",
     issued_to_date="issued_to_date",
     entities=entities,
     limit=10,
-    offset=707020693.68
+    offset=808037660.53
 )
 
 print(result)
 ```
 
 #### **get_deel_invoice_list**
 
@@ -214,15 +214,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.accounting.get_deel_invoice_list(
     contract_id="contract_id",
     limit=10,
-    offset=898896522.23
+    offset=237799437.03
 )
 
 print(result)
 ```
 
 #### **get_billing_invoice_download_link**
 
@@ -401,16 +401,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdminUserCreateContainer(**{
     "data": {
-        "first_name": "proident molli",
-        "last_name": "anim ci",
+        "first_name": "dolore",
+        "last_name": "proi",
         "email": "email"
     }
 })
 
 result = sdk.managers.create_manager(request_body=request_body)
 
 print(result)
@@ -471,36 +471,36 @@
         "email": "john.doe@domain.com",
         "work_email": "john.doe@domain.com",
         "nationality": "CA",
         "country": "BR",
         "state": "AC"
     },
     "team_information": {
-        "team_id": 1.64,
-        "legal_entity_id": 2.97
+        "team_id": 9.77,
+        "legal_entity_id": 2.18
     },
     "job_information": {
-        "seniority_id": 1.14,
-        "job_title_id": 6.17
+        "seniority_id": 9.22,
+        "job_title_id": 6.5
     },
     "compensation": {
-        "gross_annual_salary": 5.95,
+        "gross_annual_salary": 7.15,
         "currency": "USD"
     },
     "contract": {
         "contract_oid": "pdcMQe0cXCCXWTkqkdytw",
         "start_date": "1999-12-31",
-        "employee_number": 3.49,
+        "employee_number": 9.02,
         "end_date": "1999-12-31",
         "employment_type": "PART_TIME",
-        "part_time_percentage": 75.13
+        "part_time_percentage": 21.67
     },
     "vacation_info": {
         "vacation_accrual_start_date": "vacation_accrual_start_date",
-        "vacation_yearly_policy": 295.88
+        "vacation_yearly_policy": 171.07
     }
 })
 
 result = sdk.people.create_direct_employee(request_body=request_body)
 
 print(result)
 ```
@@ -529,16 +529,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_internal_people_list(
-    offset=92741896.72,
-    limit=88.8
+    offset=978653984.34,
+    limit=43.45
 )
 
 print(result)
 ```
 
 #### **get_people_list**
 
@@ -569,16 +569,16 @@
 
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.people.get_people_list(
-    offset=311381742.98,
-    limit=139.17,
+    offset=44334375.53,
+    limit=105.69,
     search="search",
     sort_by="id",
     sort_order="asc",
     hiring_statuses="active"
 )
 
 print(result)
@@ -1221,38 +1221,38 @@
                 "country": "US"
             }
         },
         "employment": {
             "country": "US",
             "state": "state",
             "type_": "Full-time",
-            "work_visa_required": True,
+            "work_visa_required": False,
             "start_date": "1999-12-31",
             "end_date": "1999-12-31",
-            "probation_period": 2.27,
+            "probation_period": 6.17,
             "scope_of_work": "scope_of_work",
             "time_off_type": "STANDARD",
-            "holidays": 4.71
+            "holidays": 5.67
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
-            "salary": 0.96,
+            "salary": 5.95,
             "currency": "currency",
-            "variable_compensation": 6.36,
+            "variable_compensation": 3.49,
             "variable_compensation_type": "PERCENTAGE"
         },
         "quote_additional_fields": {
             "gender": "gender",
             "worker_type": "Skilled",
             "dob": "dob"
         },
@@ -1319,46 +1319,46 @@
 )
 
 request_body = GpContractToCreateContainer(**{
     "data": {
         "employee": {
             "first_name": "Jane",
             "last_name": "Doe",
-            "email": "ipsum ad tempor",
-            "work_email": "Lorem ullamco ",
+            "email": "culpa Lorem inc",
+            "work_email": "in do L",
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
-                "allowance": 1.94,
+                "allowance": 5.28,
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
-            "salary": 2.33,
+            "salary": 8.05,
             "currency": "GBP"
         }
     }
 })
 
 result = sdk.global_payroll.create_gp_contract(request_body=request_body)
 
@@ -2004,35 +2004,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "adquis culpa reprehenderit sed in"
+            "name": "sedDuis officia est laborum in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "ametnos",
+            "expected_email": "occae",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 3.56,
+            "amount": 2.6,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2090,28 +2090,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "nulla"
+            "name": "enim irure dolore magna"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "Duis esse ex",
+            "expected_email": "Duis nulla oc",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_tasks",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2175,28 +2175,28 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "mollit"
+            "name": "et dolore"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "proid",
+            "expected_email": "sint ",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "payg_milestones",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 100,
@@ -2260,35 +2260,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "Lorem"
+            "name": "cillum"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "anim sit",
+            "expected_email": "Lorem sint et",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "ongoing_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 6.09,
+            "amount": 7.36,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2346,35 +2346,35 @@
             },
             "team": {
                 "id_": "00000000-0000-0000-0000-000000000000"
             }
         },
         "job_title": {
             "id_": "00000000-0000-0000-0000-000000000000",
-            "name": "adquis culpa reprehenderit sed in"
+            "name": "sedDuis officia est laborum in"
         },
         "seniority": {
             "id_": "00000000-0000-0000-0000-000000000000"
         },
         "notice_period": 15,
         "who_reports": "both",
         "meta": {
-            "documents_required": True,
+            "documents_required": False,
             "is_main_income": False
         },
         "external_id": "external_id",
         "worker": {
-            "expected_email": "ametnos",
+            "expected_email": "occae",
             "first_name": "John",
             "last_name": "Doe"
         },
         "type_": "pay_as_you_go_time_based",
         "start_date": "1999-12-31",
         "compensation_details": {
-            "amount": 3.56,
+            "amount": 2.6,
             "currency_code": "GBP",
             "frequency": "weekly",
             "cycle_end": 15,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
             "payment_due_days": 7,
             "pay_before_weekends": True,
@@ -2458,21 +2458,21 @@
 request_body = ContractToAmendDetailsContainer(**{
     "data": {
         "amount": 100,
         "currency_code": "GBP",
         "scale": "hourly",
         "effective_date": "1999-12-31",
         "first_payment_date": "1999-12-31",
-        "first_payment": 8.79,
+        "first_payment": 0.24,
         "frequency": "weekly",
-        "cycle_end": 28.13,
+        "cycle_end": 24.94,
         "cycle_end_type": "DAY_OF_WEEK",
         "payment_due_type": "REGULAR",
-        "payment_due_days": 6.51,
-        "pay_before_weekends": False,
+        "payment_due_days": 0.92,
+        "pay_before_weekends": True,
         "job_title_name": "3D Designer",
         "job_title_id": "00000000-0000-0000-0000-000000000000",
         "seniority_id": "00000000-0000-0000-0000-000000000000",
         "special_clause": "special_clause",
         "scope_of_work": "scope_of_work"
     }
 })
@@ -2647,20 +2647,20 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = {
     "data": {
         "contract_id": "m3jk2j",
-        "amount": "cupidatat cil",
+        "amount": "cupidatat exe",
         "date_of_adjustment": "1999-12-31",
         "title": "Your title here",
         "description": "Your description here",
         "cycle_reference": "my_cycle_reference",
-        "file": "nisi nulla",
+        "file": "qu",
         "adjustment_category_id": "c9cf4c2c0165f48f494415390c3b49",
         "move_next_cycle": True,
         "vendor": "Vendor",
         "country": "US"
     }
 }
 
@@ -2726,18 +2726,18 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = AdjustmentToUpdateContainer(**{
     "data": {
-        "amount": "proident",
+        "amount": "ut velit in",
         "title": "Your title here",
         "description": "Your description here",
-        "file": "enim repr"
+        "file": "incididunt "
     }
 })
 
 result = sdk.adjustments.update_adjustment(
     request_body=request_body,
     adjustment_id="adjustment_id"
 )
@@ -2922,15 +2922,15 @@
         "id_": "id",
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "link": "link",
         "job_title": "3D Designer",
-        "email": "sunt ullamco es",
+        "email": "dolore",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.add_candidate(request_body=request_body)
@@ -2970,15 +2970,15 @@
     "data": {
         "first_name": "John",
         "last_name": "Doe",
         "status": "offer-accepted",
         "start_date": "1999-12-31",
         "job_title": "3D Designer",
         "link": "link",
-        "email": "laboris a",
+        "email": "Excepteur nu",
         "nationality": "US",
         "country": "US",
         "state": "AL"
     }
 })
 
 result = sdk.candidates.patch_candidate(
@@ -3081,15 +3081,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = EmployeeContractSignatureToCreateContainer(**{
     "data": {
-        "signature": "inci"
+        "signature": "aliqua sed comm"
     }
 })
 
 result = sdk.partner_managed.sign_employee_contract(
     request_body=request_body,
     employee_id="employee_id",
     contract_id="contract_id"
@@ -3125,15 +3125,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = RequestCustomVerificationLetterContainer(**{
     "data": {
-        "description": "Excepteur Duisi",
+        "description": "magnaest ea con",
         "include_qr_code": True,
         "type_": "VISA_APPLICATION_FOR_PERSONAL_TRIP"
     }
 })
 
 result = sdk.partner_managed.request_custom_verification_letter(
     request_body=request_body,
@@ -3206,15 +3206,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.download_hr_verification_letters_and_documents(
     employee_id="employee_id",
     contract_id="contract_id",
-    document_id=5.13
+    document_id=1.72
 )
 
 print(result)
 ```
 
 #### **get_offer_letter_preview**
 
@@ -3540,15 +3540,15 @@
 request_body = {
     "file": "file"
 }
 
 result = sdk.partner_managed.upload_employee_compliance_document(
     request_body=request_body,
     employee_id="employee_id",
-    document_id=3.06
+    document_id=1.36
 )
 
 print(result)
 ```
 
 #### **get_employee_compliance_document_template**
 
@@ -3575,15 +3575,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.partner_managed.get_employee_compliance_document_template(
     employee_id="employee_id",
-    document_id=5.72
+    document_id=5.91
 )
 
 print(result)
 ```
 
 #### **get_employee_tax_documents**
 
@@ -3625,15 +3625,14 @@
 | [get_contract_list](#get_contract_list)                                     | Retrieve a list of contracts.                                                                                                                                                                                        |
 | [get_contract_by_id](#get_contract_by_id)                                   | Retrieve a single contract.                                                                                                                                                                                          |
 | [attach_external_id](#attach_external_id)                                   | Add an external Id to a Deel contract. You can use this to add a Deel contract's refernece Id in your platform. External Id can be passed as a query parameter in List contract endpoint to find this conract later. |
 | [add_contract_document](#add_contract_document)                             | Attach a file to contract document.                                                                                                                                                                                  |
 | [edit_contract_document](#edit_contract_document)                           | Overwrite the file currently attached to contract document.                                                                                                                                                          |
 | [get_alternate_emails_by_contract_id](#get_alternate_emails_by_contract_id) | Returns an array of alternate email objects                                                                                                                                                                          |
 | [sign_contract](#sign_contract)                                             | Sign a contract as a client.                                                                                                                                                                                         |
-| [archive_contract](#archive_contract)                                       | Archive a terminated, cancelled or completed contract.                                                                                                                                                               |
 | [invite_to_sign_contract](#invite_to_sign_contract)                         | Invite a worker to sign the contract. Worker will be notified via email.                                                                                                                                             |
 | [uninvite_to_sign_contract](#uninvite_to_sign_contract)                     | Remove invite in order to re-invite a worker to sign the contract.                                                                                                                                                   |
 | [calculate_final_payment](#calculate_final_payment)                         | Calculate the final payment due to the contractor when ending the contract.                                                                                                                                          |
 | [post_contract_estimate](#post_contract_estimate)                           | First payment is calculated from the number of working/calendar days between their start date and the start of the payment cycle.                                                                                    |
 | [get_contract_templates](#get_contract_templates)                           | Retrieve a list of contract templates in your organization.                                                                                                                                                          |
 | [get_worker_documents_by_id](#get_worker_documents_by_id)                   | Retrieve a list of documents of a worker.                                                                                                                                                                            |
 | [get_download_worker_documents_by_id](#get_download_worker_documents_by_id) | Get the download link of worker document.                                                                                                                                                                            |
@@ -3914,58 +3913,27 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractSignatureToCreateContainer(**{
     "data": {
-        "client_signature": "proident e",
-        "contract_template_id": 1.32
+        "client_signature": "ea exercitat",
+        "contract_template_id": 8.35
     }
 })
 
 result = sdk.contracts.sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
 
 print(result)
 ```
 
-#### **archive_contract**
-
-Archive a terminated, cancelled or completed contract.
-
-- HTTP Method: `PATCH`
-- Endpoint: `/contracts/{contract_id}/archive`
-
-**Parameters**
-| Name | Type| Required | Description |
-| :-------- | :----------| :----------:| :----------|
-| contract_id | str | ✅ | Archive a terminated, cancelled or completed contract. |
-
-**Return Type**
-
-`GenericResultUpdated`
-
-**Example Usage Code Snippet**
-
-```py
-from deel_sdk import DeelSdk, Environment
-
-sdk = DeelSdk(
-    access_token="YOUR_ACCESS_TOKEN",
-    base_url=Environment.DEFAULT.value
-)
-
-result = sdk.contracts.archive_contract(contract_id="contract_id")
-
-print(result)
-```
-
 #### **invite_to_sign_contract**
 
 Invite a worker to sign the contract. Worker will be notified via email.
 
 - HTTP Method: `POST`
 - Endpoint: `/contracts/{contract_id}/invitations`
 
@@ -3988,16 +3956,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = ContractInvitationToCreateContainer(**{
     "data": {
-        "email": "dolore c",
-        "message": "mini"
+        "email": "eiusm",
+        "message": "officia ut"
     }
 })
 
 result = sdk.contracts.invite_to_sign_contract(
     request_body=request_body,
     contract_id="contract_id"
 )
@@ -4110,18 +4078,18 @@
         "type_": "ongoing_time_based",
         "country_code": "US",
         "start_date": "1999-12-31",
         "compensation_details": {
             "amount": 2500,
             "currency_code": "GBP",
             "scale": "weekly",
-            "cycle_end": 18.59,
+            "cycle_end": 30.28,
             "cycle_end_type": "DAY_OF_WEEK",
             "payment_due_type": "REGULAR",
-            "payment_due_days": 36.88,
+            "payment_due_days": 11.81,
             "calculation_type": "CUSTOM_AMOUNT",
             "work_week_start": "Sunday",
             "work_week_end": "Sunday"
         }
     }
 })
 
@@ -4216,15 +4184,15 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 result = sdk.contracts.get_download_worker_documents_by_id(
     worker_id="worker_id",
-    document_id=1.09
+    document_id=8.43
 )
 
 print(result)
 ```
 
 ### TasksService
 
@@ -4503,15 +4471,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=97685509.73
+    offset=564786626.18
 )
 
 print(result)
 ```
 
 #### **get_timesheets**
 
@@ -4556,15 +4524,15 @@
     contract_id="contract_id",
     contract_types=contract_types,
     statuses=statuses,
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=99,
-    offset=90326358.62
+    offset=911169937.96
 )
 
 print(result)
 ```
 
 #### **create_timesheet**
 
@@ -4665,15 +4633,15 @@
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = TimesheetToUpdateContainer(**{
     "data": {
         "description": "description",
-        "quantity": 9.63
+        "quantity": 3.77
     }
 })
 
 result = sdk.timesheets.update_timesheet_by_id(
     request_body=request_body,
     timesheet_id="timesheet_id"
 )
@@ -4787,15 +4755,15 @@
 )
 
 request_body = TimesheetReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.19
+            1.77
         ]
     }
 })
 
 result = sdk.timesheets.create_timesheet_reviews(request_body=request_body)
 
 print(result)
@@ -5033,15 +5001,15 @@
 )
 
 request_body = MilestoneReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            1.74
+            6.78
         ]
     }
 })
 
 result = sdk.milestones.create_milestone_reviews(
     request_body=request_body,
     contract_id="contract_id"
@@ -5244,17 +5212,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": False,
+        "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": False,
+        "is_start_date_half_day": True,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.create_eor_time_offs(
     request_body=request_body,
@@ -5294,17 +5262,17 @@
 )
 
 request_body = CreateTimeoffContainer(**{
     "data": {
         "type_": "VACATION",
         "start_date": "2022-09-03T00:00:00.000Z",
         "end_date": "2022-09-05T00:00:00.000Z",
-        "with_multiple_dates": False,
+        "with_multiple_dates": True,
         "reason": "Holiday",
-        "is_start_date_half_day": False,
+        "is_start_date_half_day": True,
         "is_end_date_half_day": False,
         "other_timeoff_name": "Birthday"
     }
 })
 
 result = sdk.time_off.edit_eor_time_offs(
     request_body=request_body,
@@ -5519,15 +5487,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=560002501.34
+    offset=226515477.25
 )
 
 print(result)
 ```
 
 #### **get_invoice_adjustments**
 
@@ -5579,15 +5547,15 @@
     types=types,
     statuses=statuses,
     invoice_id="invoice_id",
     reporter_id="reporter_id",
     date_from="1999-12-31",
     date_to="1999-12-31",
     limit=10,
-    offset=729203388.82
+    offset=240522187.51
 )
 
 print(result)
 ```
 
 #### **create_invoice_adjustment**
 
@@ -5620,21 +5588,21 @@
 request_body = InvoiceAdjustmentToCreateContainer(**{
     "data": {
         "contract_id": "contract_id",
         "date_submitted": "1999-12-31",
         "type_": "bonus",
         "amount": 2500,
         "description": "Bonus for being awesome.",
-        "payment_cycle_id": 5.08
+        "payment_cycle_id": 6.69
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment(
     request_body=request_body,
-    recurring=True
+    recurring=False
 )
 
 print(result)
 ```
 
 #### **update_invoice_adjustment_by_id**
 
@@ -5662,16 +5630,16 @@
 sdk = DeelSdk(
     access_token="YOUR_ACCESS_TOKEN",
     base_url=Environment.DEFAULT.value
 )
 
 request_body = InvoiceAdjustmentToUpdateContainer(**{
     "data": {
-        "description": "aute veniam in fugiat",
-        "amount": 2.65
+        "description": "sunt laborum Duis exercitation id",
+        "amount": 9.39
     }
 })
 
 result = sdk.invoices.update_invoice_adjustment_by_id(
     request_body=request_body,
     invoice_adjustment_id="invoice_adjustment_id"
 )
@@ -5785,15 +5753,15 @@
 )
 
 request_body = InvoiceAdjustmentReviewsToCreateContainer(**{
     "data": {
         "status": "approved",
         "reason": "reason",
         "ids": [
-            6.19
+            1.77
         ]
     }
 })
 
 result = sdk.invoices.create_invoice_adjustment_reviews(request_body=request_body)
 
 print(result)
```

### Comparing `deel-sdk-1.0.1/src/deel_sdk.egg-info/SOURCES.txt` & `deel_sdk-1.0.2/src/deel_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

