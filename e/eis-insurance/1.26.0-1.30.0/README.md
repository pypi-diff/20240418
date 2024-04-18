# Comparing `tmp/eis-insurance-1.26.0.tar.gz` & `tmp/eis-insurance-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis-insurance-1.26.0.tar", last modified: Wed Mar 20 18:01:58 2024, max compression
+gzip compressed data, was "eis-insurance-1.30.0.tar", last modified: Thu Apr 18 15:36:21 2024, max compression
```

## Comparing `eis-insurance-1.26.0.tar` & `eis-insurance-1.30.0.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.109562 eis-insurance-1.26.0/
--rw-r--r--   0 ricard     (501) staff       (20)      337 2024-03-20 18:01:58.109676 eis-insurance-1.26.0/PKG-INFO
--rw-r--r--   0 ricard     (501) staff       (20)    23000 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/README.md
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.010005 eis-insurance-1.26.0/eis/
--rw-r--r--   0 ricard     (501) staff       (20)        0 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/__init__.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.012462 eis-insurance-1.26.0/eis/insurance/
--rw-r--r--   0 ricard     (501) staff       (20)      735 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/__init__.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.017866 eis-insurance-1.26.0/eis/insurance/api/
--rw-r--r--   0 ricard     (501) staff       (20)      228 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)     5447 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/default_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     7612 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/api/insured_object_types_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    24283 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/api/insured_objects_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    23408 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/api/lead_statuses_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    55099 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/api/leads_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    30117 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/named_ranges_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    64194 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/policies_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    36321 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/premium_formulas_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    37917 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/product_factors_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    36937 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/product_fields_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    13361 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/product_versions_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    36733 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api/products_api.py
--rw-r--r--   0 ricard     (501) staff       (20)    41662 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/api_client.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.018230 eis-insurance-1.26.0/eis/insurance/apis/
--rw-r--r--   0 ricard     (501) staff       (20)     1207 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/apis/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    16484 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/configuration.py
--rw-r--r--   0 ricard     (501) staff       (20)     5074 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/exceptions.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.068392 eis-insurance-1.26.0/eis/insurance/model/
--rw-r--r--   0 ricard     (501) staff       (20)      347 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/model/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    11485 2024-03-20 18:00:00.000000 eis-insurance-1.26.0/eis/insurance/model/activate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11862 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/activate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12128 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/calculate_custom_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12924 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/calculate_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12318 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/calculate_product_fields_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12421 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/clone_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    18487 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11866 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_bank_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12564 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_custom_application_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13015 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_dummy_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14361 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12009 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11606 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_lead_async_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14927 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    21946 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11842 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11759 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_lead_status_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11947 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13809 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/eis/insurance/model/create_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11949 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12316 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_named_request_s3_data_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11927 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_payment_method_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14081 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11864 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15444 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12053 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    18650 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12403 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14404 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11896 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/create_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12383 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/csv_product_factor_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11462 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/delete_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11703 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/delete_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11700 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/empty_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12000 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11938 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11940 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11718 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_policy_data_by_date_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11847 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11657 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12328 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12874 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_factor_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12439 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_factor_value_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11950 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_factor_value_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12517 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_factors_for_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11871 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_factors_for_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11651 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12050 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12954 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11865 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12033 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12018 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/get_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12323 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/grouped_product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12395 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/grouped_product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11940 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/grouped_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    17245 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/grpc_patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    22171 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/grpc_update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12223 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/inline_response200.py
--rw-r--r--   0 ricard     (501) staff       (20)    12223 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/inline_response503.py
--rw-r--r--   0 ricard     (501) staff       (20)    15814 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/insured_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13038 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/insured_object_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    16768 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/invoice_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12653 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/invoice_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/lead_bank_account_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    19631 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/lead_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12384 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/lead_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12158 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_insured_object_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12131 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_insured_objects_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12100 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_lead_statuses_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12674 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_leads_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11874 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_named_ranges_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12703 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_policies_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12265 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_premium_formulas_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12149 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12283 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_product_field_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12121 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_product_fields_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12074 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_products_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12582 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/list_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14789 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/named_range_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    16739 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11811 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/patch_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13591 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/patch_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11851 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/patch_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    17937 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/policy_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13748 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/policy_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12867 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    13319 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/policy_premium_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13714 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/policy_premium_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13763 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/policy_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15539 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/premium_formula_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12952 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/premium_override_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11971 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/premium_override_request_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11905 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/premium_override_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    15269 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/product_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14144 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14246 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/eis/insurance/model/product_factor_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13780 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12756 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/product_factor_value_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    18945 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12863 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/product_field_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13423 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/product_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11637 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/sepa_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    14945 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/shared_create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    18643 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/shared_invoice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12997 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/shared_lead_policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    18963 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/shared_product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12660 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/shared_update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    15824 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/shared_update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12263 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/store_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11884 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/store_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11484 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/suspend_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11859 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/suspend_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11904 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11490 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/terminate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11863 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/terminate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    13994 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/timeslice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14723 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    21581 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11842 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12280 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11949 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    14318 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11854 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    15444 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12029 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    19144 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12403 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12771 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11874 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    12417 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12027 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/update_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    11528 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/uploaded_document_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    12342 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/validate_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)    11860 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/eis/insurance/model/withdraw_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)    82491 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/model_utils.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.068720 eis-insurance-1.26.0/eis/insurance/models/
--rw-r--r--   0 ricard     (501) staff       (20)    12263 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/models/__init__.py
--rw-r--r--   0 ricard     (501) staff       (20)    14277 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/eis/insurance/rest.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.069883 eis-insurance-1.26.0/eis_insurance.egg-info/
--rw-r--r--   0 ricard     (501) staff       (20)      337 2024-03-20 18:01:57.000000 eis-insurance-1.26.0/eis_insurance.egg-info/PKG-INFO
--rw-r--r--   0 ricard     (501) staff       (20)    14232 2024-03-20 18:01:57.000000 eis-insurance-1.26.0/eis_insurance.egg-info/SOURCES.txt
--rw-r--r--   0 ricard     (501) staff       (20)        1 2024-03-20 18:01:57.000000 eis-insurance-1.26.0/eis_insurance.egg-info/dependency_links.txt
--rw-r--r--   0 ricard     (501) staff       (20)       32 2024-03-20 18:01:57.000000 eis-insurance-1.26.0/eis_insurance.egg-info/requires.txt
--rw-r--r--   0 ricard     (501) staff       (20)        4 2024-03-20 18:01:57.000000 eis-insurance-1.26.0/eis_insurance.egg-info/top_level.txt
--rw-r--r--   0 ricard     (501) staff       (20)      162 2024-03-20 18:01:58.109987 eis-insurance-1.26.0/setup.cfg
--rw-r--r--   0 ricard     (501) staff       (20)      996 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/setup.py
-drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-03-20 18:01:58.109403 eis-insurance-1.26.0/test/
--rw-r--r--   0 ricard     (501) staff       (20)      826 2024-03-20 18:00:00.000000 eis-insurance-1.26.0/test/test_activate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      943 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_activate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      883 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_calculate_custom_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1107 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_calculate_premium_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      996 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_calculate_product_fields_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      862 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_clone_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      848 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_bank_account_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      890 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_custom_application_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1115 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_dummy_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      862 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_lead_async_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1150 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1745 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      907 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      841 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_lead_status_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1013 2024-03-20 18:00:01.000000 eis-insurance-1.26.0/test/test_create_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      863 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_named_request_s3_data_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      942 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_payment_method_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1079 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      997 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      940 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_create_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      791 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_csv_product_factor_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      645 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_default_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      769 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_delete_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_delete_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      783 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_empty_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      987 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_insured_object_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      886 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      954 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_lead_status_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      954 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      864 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_policy_data_by_date_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      791 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      908 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      848 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      998 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1087 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_product_factor_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      877 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_product_factor_value_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1044 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_product_factor_value_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      920 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_product_factors_for_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1108 2024-03-20 18:00:02.000000 eis-insurance-1.26.0/test/test_get_product_factors_for_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      834 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_get_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      976 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_get_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      798 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_get_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      919 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_get_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      848 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_get_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      998 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_get_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_grouped_product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_grouped_product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1051 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_grouped_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1742 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_grpc_patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1749 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_grpc_update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      775 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_inline_response200.py
--rw-r--r--   0 ricard     (501) staff       (20)      775 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_inline_response503.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_insured_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      812 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_insured_object_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_insured_object_types_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1242 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_insured_objects_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      769 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_invoice_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      783 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_invoice_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      798 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_lead_bank_account_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1745 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_lead_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      762 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_lead_status_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1199 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_lead_statuses_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1790 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_leads_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1047 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_insured_object_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1001 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_insured_objects_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_lead_statuses_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      900 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_leads_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_named_ranges_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_policies_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1012 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_premium_formulas_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1001 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1036 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_product_field_types_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      990 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_product_fields_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      933 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_products_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      755 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_list_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      762 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_named_range_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1347 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_named_ranges_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1713 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_patch_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      900 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_patch_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1072 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_patch_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      922 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_patch_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     2054 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_policies_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      958 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_policy_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      776 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_policy_object_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      762 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      925 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_policy_premium_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      941 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_policy_premium_item_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      891 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_policy_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_premium_formula_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1606 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_premium_formulas_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      783 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_premium_override_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      972 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_premium_override_request_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      958 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_premium_override_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1011 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_product_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_product_factor_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1043 2024-03-20 18:00:03.000000 eis-insurance-1.26.0/test/test_product_factor_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_product_factor_value_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      891 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_product_factor_value_for_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1604 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_product_factors_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      776 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      805 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_product_field_type_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1543 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_product_fields_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_product_version_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      932 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_product_versions_api.py
--rw-r--r--   0 ricard     (501) staff       (20)     1453 2024-03-20 18:00:05.000000 eis-insurance-1.26.0/test/test_products_api.py
--rw-r--r--   0 ricard     (501) staff       (20)      705 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_sepa_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1193 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_shared_create_lead_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1025 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_shared_invoice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      834 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_shared_lead_policy_object_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_shared_product_field_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      884 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_shared_update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      912 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_shared_update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      992 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_store_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_store_product_factors_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_suspend_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      936 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_suspend_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      898 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_swap_premium_formulas_order_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      833 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_terminate_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      950 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_terminate_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1000 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_timeslice_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      862 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_insured_object_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1720 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_lead_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      907 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_lead_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      841 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_named_range_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      975 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_named_range_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)     1079 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_policy_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      929 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_policy_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_premium_formula_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_premium_formula_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      855 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_product_field_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      997 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_product_field_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      819 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_product_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      940 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_product_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      869 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_product_version_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_update_product_version_response_class.py
--rw-r--r--   0 ricard     (501) staff       (20)      790 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_uploaded_document_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)     1013 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_validate_product_factors_request_dto.py
--rw-r--r--   0 ricard     (501) staff       (20)      943 2024-03-20 18:00:04.000000 eis-insurance-1.26.0/test/test_withdraw_policy_response_class.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.850491 eis-insurance-1.30.0/
+-rw-r--r--   0 ricard     (501) staff       (20)      337 2024-04-18 15:36:21.850646 eis-insurance-1.30.0/PKG-INFO
+-rw-r--r--   0 ricard     (501) staff       (20)    23000 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/README.md
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.741298 eis-insurance-1.30.0/eis/
+-rw-r--r--   0 ricard     (501) staff       (20)        0 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/__init__.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.743991 eis-insurance-1.30.0/eis/insurance/
+-rw-r--r--   0 ricard     (501) staff       (20)      735 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/__init__.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.751109 eis-insurance-1.30.0/eis/insurance/api/
+-rw-r--r--   0 ricard     (501) staff       (20)      228 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)     5447 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/default_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     7612 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/insured_object_types_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    24476 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/insured_objects_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    23408 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/lead_statuses_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    55099 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/leads_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    30117 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/named_ranges_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    63708 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/policies_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    36321 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/premium_formulas_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    37917 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/product_factors_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    36949 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/product_fields_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13361 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/product_versions_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    37898 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api/products_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)    41662 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/api_client.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.751392 eis-insurance-1.30.0/eis/insurance/apis/
+-rw-r--r--   0 ricard     (501) staff       (20)     1207 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/apis/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)    16484 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/configuration.py
+-rw-r--r--   0 ricard     (501) staff       (20)     5074 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/exceptions.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.804803 eis-insurance-1.30.0/eis/insurance/model/
+-rw-r--r--   0 ricard     (501) staff       (20)      347 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11485 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/activate_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11862 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/activate_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12128 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/calculate_custom_premium_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12924 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/calculate_premium_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12318 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/calculate_product_fields_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12421 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/clone_product_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    18487 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/create_account_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11866 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/create_bank_account_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12564 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/eis/insurance/model/create_custom_application_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13015 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_dummy_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14361 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_insured_object_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12009 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_insured_object_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11606 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_async_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14927 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    21946 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11842 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11759 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_status_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11947 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_lead_status_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13809 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_named_range_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11949 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_named_range_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12316 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_named_request_s3_data_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_payment_method_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14081 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11864 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/eis/insurance/model/create_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15591 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12053 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    18650 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_field_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12403 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_field_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14404 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11896 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/create_product_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12383 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/csv_product_factor_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11462 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/delete_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11703 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/delete_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11700 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/empty_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12000 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_insured_object_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11938 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_lead_status_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11940 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_named_range_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11718 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_policy_data_by_date_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/eis/insurance/model/get_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11847 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11657 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12328 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12874 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factor_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12439 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11950 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12517 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11871 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11651 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_field_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12050 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_field_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12558 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11865 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12033 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12018 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/get_product_version_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12323 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12395 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_value_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11940 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/eis/insurance/model/grouped_product_factors_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    17245 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/grpc_patch_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    22171 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/grpc_update_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12817 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/inline_response200.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12817 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/inline_response503.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15814 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/insured_object_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13038 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/insured_object_type_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    16768 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/invoice_item_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12653 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/invoice_status_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11833 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/lead_bank_account_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    19631 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/lead_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12384 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/lead_status_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12158 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_insured_object_types_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12131 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_insured_objects_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12100 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_lead_statuses_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12674 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_leads_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11874 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_named_ranges_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12703 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_policies_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12265 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_premium_formulas_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12149 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_product_factors_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12283 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_product_field_types_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12121 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_product_fields_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12074 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_products_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12582 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/list_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14789 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/named_range_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    16739 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11811 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13591 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11851 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/patch_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    17937 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/policy_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13748 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/policy_object_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12867 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/eis/insurance/model/policy_object_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13319 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/policy_premium_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13714 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/policy_premium_item_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13763 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/policy_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15539 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_formula_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12952 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_override_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11971 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_override_request_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11905 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/premium_override_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15269 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14144 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14246 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_for_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13780 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_value_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12756 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_factor_value_for_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    18978 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_field_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12863 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_field_type_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13423 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/product_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11637 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/sepa_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14945 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_create_lead_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    18643 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_invoice_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12997 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_lead_policy_object_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    18996 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_product_field_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12804 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_update_named_range_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15971 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/shared_update_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12263 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/store_product_factors_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11884 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/store_product_factors_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11484 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/suspend_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11859 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/suspend_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11904 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12604 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/terminate_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11863 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/terminate_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    13994 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/timeslice_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14723 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_insured_object_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    21581 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11842 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12424 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_named_range_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11949 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_named_range_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14608 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11854 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    15591 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12029 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    19144 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_field_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12403 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_field_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12771 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11874 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12417 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12027 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/update_product_version_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11528 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/uploaded_document_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    12342 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/validate_product_factors_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)    11860 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model/withdraw_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)    82491 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/model_utils.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.805031 eis-insurance-1.30.0/eis/insurance/models/
+-rw-r--r--   0 ricard     (501) staff       (20)    12263 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/models/__init__.py
+-rw-r--r--   0 ricard     (501) staff       (20)    14277 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/eis/insurance/rest.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.805837 eis-insurance-1.30.0/eis_insurance.egg-info/
+-rw-r--r--   0 ricard     (501) staff       (20)      337 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/PKG-INFO
+-rw-r--r--   0 ricard     (501) staff       (20)    14232 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/SOURCES.txt
+-rw-r--r--   0 ricard     (501) staff       (20)        1 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/dependency_links.txt
+-rw-r--r--   0 ricard     (501) staff       (20)       32 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/requires.txt
+-rw-r--r--   0 ricard     (501) staff       (20)        4 2024-04-18 15:36:21.000000 eis-insurance-1.30.0/eis_insurance.egg-info/top_level.txt
+-rw-r--r--   0 ricard     (501) staff       (20)      162 2024-04-18 15:36:21.851008 eis-insurance-1.30.0/setup.cfg
+-rw-r--r--   0 ricard     (501) staff       (20)      996 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/setup.py
+drwxr-xr-x   0 ricard     (501) staff       (20)        0 2024-04-18 15:36:21.850303 eis-insurance-1.30.0/test/
+-rw-r--r--   0 ricard     (501) staff       (20)      826 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_activate_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      943 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_activate_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      883 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_calculate_custom_premium_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1107 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_calculate_premium_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      996 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_calculate_product_fields_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      862 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_clone_product_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_create_account_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      848 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_create_bank_account_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      890 2024-04-18 15:33:56.000000 eis-insurance-1.30.0/test/test_create_custom_application_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1115 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_dummy_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      862 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_insured_object_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_insured_object_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_async_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1150 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1745 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      907 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      841 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_status_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_lead_status_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1013 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_named_range_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_named_range_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      863 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_named_request_s3_data_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      942 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_payment_method_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1079 2024-04-18 15:33:57.000000 eis-insurance-1.30.0/test/test_create_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_premium_formula_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_field_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      997 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_field_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      940 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_create_product_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      791 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_csv_product_factor_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      645 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_default_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      769 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_delete_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_delete_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      783 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_empty_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      987 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_insured_object_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      886 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      954 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_lead_status_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      954 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_named_range_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      864 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_policy_data_by_date_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      791 2024-04-18 15:33:58.000000 eis-insurance-1.30.0/test/test_get_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      908 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      848 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      998 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_premium_formula_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1087 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factor_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      877 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factor_value_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1044 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factor_value_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      920 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factors_for_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1108 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_factors_for_version_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      834 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_field_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      976 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_field_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      798 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      919 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      848 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      998 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_get_product_version_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_grouped_product_factor_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_grouped_product_factor_value_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1051 2024-04-18 15:33:59.000000 eis-insurance-1.30.0/test/test_grouped_product_factors_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1742 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_grpc_patch_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1749 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_grpc_update_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      775 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_inline_response200.py
+-rw-r--r--   0 ricard     (501) staff       (20)      775 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_inline_response503.py
+-rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_insured_object_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      812 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_insured_object_type_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_insured_object_types_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1242 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_insured_objects_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      769 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_invoice_item_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      783 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_invoice_status_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      798 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_lead_bank_account_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1745 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_lead_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      762 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_lead_status_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1199 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_lead_statuses_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_leads_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1047 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_insured_object_types_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1001 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_insured_objects_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_lead_statuses_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      900 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_leads_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_named_ranges_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_policies_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1012 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_premium_formulas_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1001 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_product_factors_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1036 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_product_field_types_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      990 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_product_fields_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      933 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_products_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      755 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_list_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      762 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_named_range_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1347 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_named_ranges_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1713 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      900 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1072 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      922 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_patch_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     2054 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policies_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      958 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_policy_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      776 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_policy_object_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      762 2024-04-18 15:34:00.000000 eis-insurance-1.30.0/test/test_policy_object_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      925 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policy_premium_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      941 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policy_premium_item_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      891 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_policy_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_formula_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1606 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_formulas_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      783 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_override_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      972 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_override_request_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      958 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_premium_override_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1011 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1043 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_for_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_value_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      891 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factor_value_for_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1604 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_factors_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      776 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_field_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      805 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_field_type_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1543 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_fields_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_version_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      932 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_product_versions_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1453 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_products_api.py
+-rw-r--r--   0 ricard     (501) staff       (20)      705 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_sepa_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1193 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_create_lead_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1025 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_invoice_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      834 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_lead_policy_object_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_product_field_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      884 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_update_named_range_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      912 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_shared_update_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      992 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_store_product_factors_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1008 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_store_product_factors_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_suspend_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      936 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_suspend_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      898 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_swap_premium_formulas_order_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      833 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_terminate_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      950 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_terminate_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1000 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_timeslice_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      862 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_insured_object_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1720 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_lead_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      907 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_lead_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      841 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_named_range_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      975 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_named_range_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1079 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_policy_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      929 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_policy_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_premium_formula_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_premium_formula_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      855 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_field_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      997 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_field_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      819 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      940 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      869 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_version_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1019 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_update_product_version_response_class.py
+-rw-r--r--   0 ricard     (501) staff       (20)      790 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_uploaded_document_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)     1013 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_validate_product_factors_request_dto.py
+-rw-r--r--   0 ricard     (501) staff       (20)      943 2024-04-18 15:34:01.000000 eis-insurance-1.30.0/test/test_withdraw_policy_response_class.py
```

### Comparing `eis-insurance-1.26.0/README.md` & `eis-insurance-1.30.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # eis-insurance
 The EMIL InsuranceService API description
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0
-- Package version: 1.26.0
+- Package version: 1.30.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.emil.de](https://www.emil.de)
 
 ## Requirements.
 
 Python >=3.6
```

### Comparing `eis-insurance-1.26.0/eis/insurance/__init__.py` & `eis-insurance-1.30.0/eis/insurance/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0
     Contact: kontakt@emil.de
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.26.0"
+__version__ = "1.30.0"
 
 # import ApiClient
 from eis.insurance.api_client import ApiClient
 
 # import Configuration
 from eis.insurance.configuration import Configuration
```

### Comparing `eis-insurance-1.26.0/eis/insurance/api/default_api.py` & `eis-insurance-1.30.0/eis/insurance/api/default_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/insured_object_types_api.py` & `eis-insurance-1.30.0/eis/insurance/api/insured_object_types_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/insured_objects_api.py` & `eis-insurance-1.30.0/eis/insurance/api/insured_objects_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.delete_insured_object_endpoint = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/insuranceservice/v1/insured-objects/{id}',
                 'operation_id': 'delete_insured_object',
                 'http_method': 'DELETE',
                 'servers': None,
@@ -125,15 +125,15 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
-                        (str,),
+                        (float,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'authorization': 'Authorization',
                 },
@@ -141,15 +141,17 @@
                     'id': 'path',
                     'authorization': 'header',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.get_insured_object_endpoint = _Endpoint(
             settings={
                 'response_type': (GetInsuredObjectResponseClass,),
@@ -386,15 +388,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_insured_object(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str):
+            id (float):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -422,15 +424,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            None
+            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `eis-insurance-1.26.0/eis/insurance/api/lead_statuses_api.py` & `eis-insurance-1.30.0/eis/insurance/api/lead_statuses_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/leads_api.py` & `eis-insurance-1.30.0/eis/insurance/api/leads_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/named_ranges_api.py` & `eis-insurance-1.30.0/eis/insurance/api/named_ranges_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/policies_api.py` & `eis-insurance-1.30.0/eis/insurance/api/policies_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,43 +328,23 @@
                     'order',
                     'expand',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
-                    'filter',
-                    'order',
                     'expand',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
-                    ('filter',): {
-
-                        "CODE": "code",
-                        "LEADCODE": "leadCode",
-                        "POLICYNUMBER": "policyNumber",
-                        "ACCOUNTCODE": "accountCode",
-                        "STATUSES": "statuses",
-                        "PRODUCTNAME": "productName",
-                        "PRODUCTTYPE": "productType",
-                        "CREATEDAT": "createdAt",
-                        "POLICYSTARTDATE": "policyStartDate",
-                        "POLICYDATA": "policyData"
-                    },
-                    ('order',): {
-
-                        "POLICYNUMBER": "policyNumber",
-                        "CREATEDAT": "createdAt"
-                    },
                     ('expand',): {
 
                         "VERSIONS": "versions",
                         "PRODUCT": "product",
                         "TIMELINES": "timelines",
                         "PREMIUMS": "premiums",
                         "PREMIUMITEMS": "premiumItems",
@@ -828,15 +808,15 @@
     def create_policy(
         self,
         create_policy_request_dto,
         **kwargs
     ):
         """Create the policy  # noqa: E501
 
-        This will create a policy in the database. Policy creation is usually part      of a complex workflow that starts with lead creation. Creating directly a policy without prior knowledge     might result in an unusable policy. Look into lead creation for more information.  # noqa: E501
+        This will create a policy in the database. Policy creation is usually part     of a complex workflow that starts with lead creation. Creating directly a policy without prior knowledge     might result in an unusable policy. Look into lead creation for more information.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_policy(create_policy_request_dto, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -997,15 +977,15 @@
     def get_policy_data_by_date(
         self,
         code,
         **kwargs
     ):
         """Retrieve current policy version  # noqa: E501
 
-        This endpoint will return the current version of the policy. It is possible to filter the        response by a specific date and the system will return the valid data that was (or will be) at the        provided date.  # noqa: E501
+        This endpoint will return the current version of the policy. It is possible to filter the       response by a specific date and the system will return the valid data that was (or will be) at the       provided date.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_policy_data_by_date(code, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1093,17 +1073,17 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             authorization (str): Bearer Token: provided by the login endpoint under the name accessToken.. [optional]
             page_size (float): Page size.. [optional]
             page_token (str): Page token.. [optional]
-            filter (str): Filter the response by one or multiple fields. In general, fetching filtered responses will       conserve bandwidth and reduce response time.. [optional]
+            filter (str): Filter the response by one or multiple fields. In general, fetching filtered responses will       conserve bandwidth and reduce response time.<br/>       <br/>       <i>Allowed values: code, leadCode, policyNumber, holder, policyStartDate, productVersionId, productId, accountCode, productName, statuses, createdAt, policyData</i>. [optional]
             search (str): Search query.. [optional]
-            order (str): Order allowing you to specify the desired order of entities retrieved from the server.. [optional]
+            order (str): Order allowing you to specify the desired order of entities retrieved from the server.<br/>     <br/>     <i>Allowed values: id, policyNumber, createdAt, updatedAt, policyStartDate, productVersionId, productId</i>. [optional]
             expand (str): You can expand policy versions list in this endpoint. By default, versions will be an empty array.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
```

### Comparing `eis-insurance-1.26.0/eis/insurance/api/premium_formulas_api.py` & `eis-insurance-1.30.0/eis/insurance/api/premium_formulas_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/product_factors_api.py` & `eis-insurance-1.30.0/eis/insurance/api/product_factors_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/product_fields_api.py` & `eis-insurance-1.30.0/eis/insurance/api/product_fields_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
-                        (str,),
+                        (float,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'authorization': 'Authorization',
                 },
@@ -185,15 +185,15 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
-                        (str,),
+                        (float,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'authorization': 'Authorization',
                 },
@@ -401,15 +401,15 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
-                        (str,),
+                        (float,),
                     'update_product_field_request_dto':
                         (UpdateProductFieldRequestDto,),
                     'authorization':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
@@ -529,15 +529,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_product_field(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str):
+            id (float):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -613,15 +613,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_product_field(id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str):
+            id (float):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -868,15 +868,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_product_field(id, update_product_field_request_dto, async_req=True)
         >>> result = thread.get()
 
         Args:
-            id (str):
+            id (float):
             update_product_field_request_dto (UpdateProductFieldRequestDto):
 
         Keyword Args:
             authorization (str): Bearer Token. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
```

### Comparing `eis-insurance-1.26.0/eis/insurance/api/product_versions_api.py` & `eis-insurance-1.30.0/eis/insurance/api/product_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/api/products_api.py` & `eis-insurance-1.30.0/eis/insurance/api/products_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,20 +166,22 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
+                    'slug',
                     'authorization',
                     'expand',
                 ],
                 'required': [
                     'code',
                     'id',
+                    'slug',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -190,28 +192,32 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
                     'id':
                         (float,),
+                    'slug':
+                        (str,),
                     'authorization':
                         (str,),
                     'expand':
                         (str,),
                 },
                 'attribute_map': {
                     'code': 'code',
                     'id': 'id',
+                    'slug': 'slug',
                     'authorization': 'Authorization',
                     'expand': 'expand',
                 },
                 'location_map': {
                     'code': 'path',
                     'id': 'query',
+                    'slug': 'query',
                     'authorization': 'header',
                     'expand': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -232,19 +238,23 @@
                 'operation_id': 'get_product_by_identifier',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'code',
+                    'slug',
                     'authorization',
                     'expand',
                 ],
                 'required': [
                     'id',
+                    'code',
+                    'slug',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -253,26 +263,34 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (float,),
+                    'code':
+                        (str,),
+                    'slug':
+                        (str,),
                     'authorization':
                         (str,),
                     'expand':
                         (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
+                    'code': 'code',
+                    'slug': 'slug',
                     'authorization': 'Authorization',
                     'expand': 'expand',
                 },
                 'location_map': {
                     'id': 'query',
+                    'code': 'query',
+                    'slug': 'query',
                     'authorization': 'header',
                     'expand': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -594,28 +612,30 @@
             id
         return self.delete_product_endpoint.call_with_http_info(**kwargs)
 
     def get_product_by_code(
         self,
         code,
         id,
+        slug,
         **kwargs
     ):
         """Retrieve the product  # noqa: E501
 
         Retrieves the details of the product that was previously created. Supply the unique product code that was returned when you created it and Emil Api will return the corresponding product information.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_product_by_code(code, id, async_req=True)
+        >>> thread = api.get_product_by_code(code, id, slug, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Unique identifier for the object.
             id (float): Unique identifier referencing the product.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
 
         Keyword Args:
             authorization (str): Bearer Token: provided by the login endpoint under the name accessToken.. [optional]
             expand (str): Fields to expand response by. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -677,32 +697,38 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
+        kwargs['slug'] = \
+            slug
         return self.get_product_by_code_endpoint.call_with_http_info(**kwargs)
 
     def get_product_by_identifier(
         self,
         id,
+        code,
+        slug,
         **kwargs
     ):
         """Retrieve the product  # noqa: E501
 
         Retrieves the details of the product that was previously created. Supply the unique product code that was returned when you created it and Emil Api will return the corresponding product information.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_product_by_identifier(id, async_req=True)
+        >>> thread = api.get_product_by_identifier(id, code, slug, async_req=True)
         >>> result = thread.get()
 
         Args:
             id (float): Unique identifier referencing the product.
+            code (str): Unique identifier of the product that this object belongs to.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
 
         Keyword Args:
             authorization (str): Bearer Token: provided by the login endpoint under the name accessToken.. [optional]
             expand (str): Fields to expand response by. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -762,14 +788,18 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['id'] = \
             id
+        kwargs['code'] = \
+            code
+        kwargs['slug'] = \
+            slug
         return self.get_product_by_identifier_endpoint.call_with_http_info(**kwargs)
 
     def list_products(
         self,
         **kwargs
     ):
         """List products  # noqa: E501
```

### Comparing `eis-insurance-1.26.0/eis/insurance/api_client.py` & `eis-insurance-1.30.0/eis/insurance/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.26.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.30.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `eis-insurance-1.26.0/eis/insurance/apis/__init__.py` & `eis-insurance-1.30.0/eis/insurance/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/configuration.py` & `eis-insurance-1.30.0/eis/insurance/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.26.0".\
+               "SDK Package Version: 1.30.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `eis-insurance-1.26.0/eis/insurance/exceptions.py` & `eis-insurance-1.30.0/eis/insurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/activate_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/activate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/activate_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/activate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/calculate_custom_premium_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/calculate_custom_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/calculate_premium_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/calculate_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/calculate_product_fields_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/calculate_product_fields_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/clone_product_version_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/clone_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_account_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_bank_account_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_custom_application_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_dummy_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_dummy_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_insured_object_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_insured_object_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_lead_async_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_lead_async_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_lead_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_lead_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_lead_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_lead_status_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_lead_status_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_lead_status_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_named_range_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_named_range_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_named_request_s3_data_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_named_request_s3_data_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_payment_method_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_payment_method_request_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,18 +56,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'SEPA': "sepa",
-            'INVOICE': "invoice",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_premium_formula_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_request_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     }
 
     validations = {
         ('order',): {
             'inclusive_maximum': 10000,
             'inclusive_minimum': 0,
         },
+        ('variable_name',): {
+            'regex': {
+                'pattern': r'JS_VARIABLE_NAME_REGEX',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_premium_formula_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_product_field_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_product_field_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_product_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/create_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/create_product_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/create_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/csv_product_factor_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/csv_product_factor_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/delete_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/delete_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/delete_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/empty_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/empty_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_insured_object_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_lead_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_lead_status_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_named_range_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_policy_data_by_date_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_policy_data_by_date_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_premium_formula_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_premium_formula_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_factor_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_factor_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_factor_value_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_factor_value_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_factor_value_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_factors_for_version_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_factors_for_version_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_factors_for_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_field_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_field_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_request_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,16 +79,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (float,),  # noqa: E501
-            'code': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'slug': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'code': (str,),  # noqa: E501
+            'slug': (str,),  # noqa: E501
             'expand': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -108,16 +108,16 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, code, slug, *args, **kwargs):  # noqa: E501
         """GetProductRequestDto - a model defined in OpenAPI
 
         Args:
             id (float): Unique identifier referencing the product.
-            code ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Unique identifier of the product that this object belongs to.
-            slug ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
+            code (str): Unique identifier of the product that this object belongs to.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -202,16 +202,16 @@
 
     @convert_js_args_to_python_args
     def __init__(self, id, code, slug, *args, **kwargs):  # noqa: E501
         """GetProductRequestDto - a model defined in OpenAPI
 
         Args:
             id (float): Unique identifier referencing the product.
-            code ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Unique identifier of the product that this object belongs to.
-            slug ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
+            code (str): Unique identifier of the product that this object belongs to.
+            slug (str): A slug is a human-readable, unique identifier, used to identify a resource      instead of a less human-readable identifier like an id.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_version_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/get_product_version_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/get_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/grouped_product_factor_class.py` & `eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/grouped_product_factor_value_class.py` & `eis-insurance-1.30.0/eis/insurance/model/grouped_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/grouped_product_factors_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/grouped_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/grpc_patch_lead_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/grpc_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/grpc_update_lead_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/grpc_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/inline_response200.py` & `eis-insurance-1.30.0/eis/insurance/model/list_insured_object_types_response_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.insurance.model.insured_object_type_class import InsuredObjectTypeClass
+    globals()['InsuredObjectTypeClass'] = InsuredObjectTypeClass
 
-class InlineResponse200(ModelNormal):
+
+class ListInsuredObjectTypesResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'status': (str,),  # noqa: E501
-            'info': ({str: ({str: (str,)},)}, none_type,),  # noqa: E501
-            'error': ({str: ({str: (str,)},)}, none_type,),  # noqa: E501
-            'details': ({str: ({str: (str,)},)},),  # noqa: E501
+            'items': ([InsuredObjectTypeClass],),  # noqa: E501
+            'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'info': 'info',  # noqa: E501
-        'error': 'error',  # noqa: E501
-        'details': 'details',  # noqa: E501
+        'items': 'items',  # noqa: E501
+        'next_page_token': 'nextPageToken',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineResponse200 - a model defined in OpenAPI
+    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListInsuredObjectTypesResponseClass - a model defined in OpenAPI
+
+        Args:
+            items ([InsuredObjectTypeClass]): Products
+            next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (str,)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +196,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineResponse200 - a model defined in OpenAPI
+    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
+        """ListInsuredObjectTypesResponseClass - a model defined in OpenAPI
+
+        Args:
+            items ([InsuredObjectTypeClass]): Products
+            next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,18 +234,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (str,)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +263,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.items = items
+        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/inline_response503.py` & `eis-insurance-1.30.0/eis/insurance/model/sepa_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 
-class InlineResponse503(ModelNormal):
+class SepaDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,41 +78,40 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'status': (str,),  # noqa: E501
-            'info': ({str: ({str: (str,)},)}, none_type,),  # noqa: E501
-            'error': ({str: ({str: (str,)},)}, none_type,),  # noqa: E501
-            'details': ({str: ({str: (str,)},)},),  # noqa: E501
+            'iban': (str,),  # noqa: E501
+            'holder_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'info': 'info',  # noqa: E501
-        'error': 'error',  # noqa: E501
-        'details': 'details',  # noqa: E501
+        'iban': 'iban',  # noqa: E501
+        'holder_name': 'holderName',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """InlineResponse503 - a model defined in OpenAPI
+    def _from_openapi_data(cls, iban, *args, **kwargs):  # noqa: E501
+        """SepaDto - a model defined in OpenAPI
+
+        Args:
+            iban (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,18 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (str,)},)}): [optional]  # noqa: E501
+            holder_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,14 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.iban = iban
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,16 +189,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """InlineResponse503 - a model defined in OpenAPI
+    def __init__(self, iban, *args, **kwargs):  # noqa: E501
+        """SepaDto - a model defined in OpenAPI
+
+        Args:
+            iban (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,18 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (str): [optional]  # noqa: E501
-            info ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            error ({str: ({str: (str,)},)}, none_type): [optional]  # noqa: E501
-            details ({str: ({str: (str,)},)}): [optional]  # noqa: E501
+            holder_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.iban = iban
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/insured_object_class.py` & `eis-insurance-1.30.0/eis/insurance/model/insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/insured_object_type_class.py` & `eis-insurance-1.30.0/eis/insurance/model/insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/invoice_item_class.py` & `eis-insurance-1.30.0/eis/insurance/model/invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/invoice_status_class.py` & `eis-insurance-1.30.0/eis/insurance/model/invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/lead_bank_account_class.py` & `eis-insurance-1.30.0/eis/insurance/model/lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/lead_class.py` & `eis-insurance-1.30.0/eis/insurance/model/lead_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/lead_status_class.py` & `eis-insurance-1.30.0/eis/insurance/model/lead_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_insured_object_types_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_insured_objects_response_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.insurance.model.insured_object_type_class import InsuredObjectTypeClass
-    globals()['InsuredObjectTypeClass'] = InsuredObjectTypeClass
+    from eis.insurance.model.insured_object_class import InsuredObjectClass
+    globals()['InsuredObjectClass'] = InsuredObjectClass
 
 
-class ListInsuredObjectTypesResponseClass(ModelNormal):
+class ListInsuredObjectsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'items': ([InsuredObjectTypeClass],),  # noqa: E501
+            'items': ([InsuredObjectClass],),  # noqa: E501
             'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -106,18 +106,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListInsuredObjectTypesResponseClass - a model defined in OpenAPI
+        """ListInsuredObjectsResponseClass - a model defined in OpenAPI
 
         Args:
-            items ([InsuredObjectTypeClass]): Products
+            items ([InsuredObjectClass]): Insured objects
             next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -197,18 +197,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListInsuredObjectTypesResponseClass - a model defined in OpenAPI
+        """ListInsuredObjectsResponseClass - a model defined in OpenAPI
 
         Args:
-            items ([InsuredObjectTypeClass]): Products
+            items ([InsuredObjectClass]): Insured objects
             next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_insured_objects_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_product_fields_response_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.insurance.model.insured_object_class import InsuredObjectClass
-    globals()['InsuredObjectClass'] = InsuredObjectClass
+    from eis.insurance.model.product_field_class import ProductFieldClass
+    globals()['ProductFieldClass'] = ProductFieldClass
 
 
-class ListInsuredObjectsResponseClass(ModelNormal):
+class ListProductFieldsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'items': ([InsuredObjectClass],),  # noqa: E501
+            'items': ([ProductFieldClass],),  # noqa: E501
             'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -106,18 +106,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListInsuredObjectsResponseClass - a model defined in OpenAPI
+        """ListProductFieldsResponseClass - a model defined in OpenAPI
 
         Args:
-            items ([InsuredObjectClass]): Insured objects
+            items ([ProductFieldClass]): Product fields.
             next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -197,18 +197,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListInsuredObjectsResponseClass - a model defined in OpenAPI
+        """ListProductFieldsResponseClass - a model defined in OpenAPI
 
         Args:
-            items ([InsuredObjectClass]): Insured objects
+            items ([ProductFieldClass]): Product fields.
             next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_lead_statuses_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_lead_statuses_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_leads_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_leads_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_named_ranges_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_named_ranges_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_policies_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_policies_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_premium_formulas_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_premium_formulas_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_product_factors_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_product_field_types_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_product_field_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_product_fields_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/list_products_response_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.insurance.model.product_field_class import ProductFieldClass
-    globals()['ProductFieldClass'] = ProductFieldClass
+    from eis.insurance.model.product_class import ProductClass
+    globals()['ProductClass'] = ProductClass
 
 
-class ListProductFieldsResponseClass(ModelNormal):
+class ListProductsResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'items': ([ProductFieldClass],),  # noqa: E501
+            'items': ([ProductClass],),  # noqa: E501
             'next_page_token': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -106,18 +106,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductFieldsResponseClass - a model defined in OpenAPI
+        """ListProductsResponseClass - a model defined in OpenAPI
 
         Args:
-            items ([ProductFieldClass]): Product fields.
+            items ([ProductClass]): List of products.
             next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -197,18 +197,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductFieldsResponseClass - a model defined in OpenAPI
+        """ListProductsResponseClass - a model defined in OpenAPI
 
         Args:
-            items ([ProductFieldClass]): Product fields.
+            items ([ProductClass]): List of products.
             next_page_token (str): Next page token.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_products_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/suspend_policy_request_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.insurance.model.product_class import ProductClass
-    globals()['ProductClass'] = ProductClass
 
-
-class ListProductsResponseClass(ModelNormal):
+class SuspendPolicyRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,58 +63,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'items': ([ProductClass],),  # noqa: E501
-            'next_page_token': (str,),  # noqa: E501
+            '_from': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'items': 'items',  # noqa: E501
-        'next_page_token': 'nextPageToken',  # noqa: E501
+        '_from': 'from',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductsResponseClass - a model defined in OpenAPI
-
-        Args:
-            items ([ProductClass]): List of products.
-            next_page_token (str): Next page token.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SuspendPolicyRequestDto - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            _from (datetime): Terminate from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -174,16 +163,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,20 +183,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, items, next_page_token, *args, **kwargs):  # noqa: E501
-        """ListProductsResponseClass - a model defined in OpenAPI
-
-        Args:
-            items ([ProductClass]): List of products.
-            next_page_token (str): Next page token.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """SuspendPolicyRequestDto - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,14 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            _from (datetime): Terminate from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,16 +247,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.items = items
-        self.next_page_token = next_page_token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/list_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/named_range_class.py` & `eis-insurance-1.30.0/eis/insurance/model/named_range_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/patch_lead_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/patch_lead_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/patch_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/patch_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/patch_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/patch_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/patch_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/policy_class.py` & `eis-insurance-1.30.0/eis/insurance/model/policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/policy_object_class.py` & `eis-insurance-1.30.0/eis/insurance/model/policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/policy_object_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/policy_premium_class.py` & `eis-insurance-1.30.0/eis/insurance/model/policy_premium_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/policy_premium_item_class.py` & `eis-insurance-1.30.0/eis/insurance/model/policy_premium_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/policy_version_class.py` & `eis-insurance-1.30.0/eis/insurance/model/policy_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/premium_formula_class.py` & `eis-insurance-1.30.0/eis/insurance/model/premium_formula_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/premium_override_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/premium_override_request_class.py` & `eis-insurance-1.30.0/eis/insurance/model/premium_override_request_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/premium_override_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_factor_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_factor_for_version_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_factor_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_factor_value_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_factor_value_for_version_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_factor_value_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_field_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_field_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             'is_required': (bool,),  # noqa: E501
             'is_hidden': (bool,),  # noqa: E501
             'is_hidden_customer_portal': (bool,),  # noqa: E501
             'is_editable_customer_portal': (bool,),  # noqa: E501
             'is_system': (bool,),  # noqa: E501
             'is_unique': (bool,),  # noqa: E501
             'default_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'expression': (str,),  # noqa: E501
+            'expression': (str, none_type,),  # noqa: E501
             'min_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'max_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
@@ -151,15 +151,15 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str): Expression to calculate the field.
+            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -276,15 +276,15 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str): Expression to calculate the field.
+            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_field_type_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_field_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/product_version_class.py` & `eis-insurance-1.30.0/eis/insurance/model/product_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/sepa_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/uploaded_document_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 
-class SepaDto(ModelNormal):
+class UploadedDocumentDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,40 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'iban': (str,),  # noqa: E501
-            'holder_name': (str,),  # noqa: E501
+            'codes': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'iban': 'iban',  # noqa: E501
-        'holder_name': 'holderName',  # noqa: E501
+        'codes': 'codes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, iban, *args, **kwargs):  # noqa: E501
-        """SepaDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, codes, *args, **kwargs):  # noqa: E501
+        """UploadedDocumentDto - a model defined in OpenAPI
 
         Args:
-            iban (str):
+            codes ([str]): Uploaded document codes.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            holder_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,15 +165,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.iban = iban
+        self.codes = codes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +186,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, iban, *args, **kwargs):  # noqa: E501
-        """SepaDto - a model defined in OpenAPI
+    def __init__(self, codes, *args, **kwargs):  # noqa: E501
+        """UploadedDocumentDto - a model defined in OpenAPI
 
         Args:
-            iban (str):
+            codes ([str]): Uploaded document codes.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +223,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            holder_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +252,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.iban = iban
+        self.codes = codes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/shared_create_lead_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/shared_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/shared_invoice_class.py` & `eis-insurance-1.30.0/eis/insurance/model/shared_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/shared_lead_policy_object_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/shared_lead_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/shared_product_field_class.py` & `eis-insurance-1.30.0/eis/insurance/model/shared_product_field_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             'is_required': (bool,),  # noqa: E501
             'is_hidden': (bool,),  # noqa: E501
             'is_hidden_customer_portal': (bool,),  # noqa: E501
             'is_editable_customer_portal': (bool,),  # noqa: E501
             'is_system': (bool,),  # noqa: E501
             'is_unique': (bool,),  # noqa: E501
             'default_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'expression': (str,),  # noqa: E501
+            'expression': (str, none_type,),  # noqa: E501
             'min_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'max_value': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'created_at': (datetime,),  # noqa: E501
             'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
@@ -151,15 +151,15 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str): Expression to calculate the field.
+            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -276,15 +276,15 @@
             is_required (bool): Is field required?
             is_hidden (bool): Is field hidden on the booking funnel?
             is_hidden_customer_portal (bool): Is field hidden on the customer portal?
             is_editable_customer_portal (bool): Is field editable on the customer portal?
             is_system (bool): Is this a system field? - System fields can neither be deleted nor modified
             is_unique (bool): Should the field value be unique across policies?
             default_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Default value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
-            expression (str): Expression to calculate the field.
+            expression (str, none_type): Expression to calculate the field.
             min_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Minimum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             max_value ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): Maximum value of the field. For the field type date-time, it should be { \"templated\" : \"{{today}}\" }
             created_at (datetime): Time at which the object was created.
             updated_at (datetime): Time at which the object was updated.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/shared_update_named_range_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/shared_update_named_range_request_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,19 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'regex': {
+                'pattern': r'PYTHON_IDENTIFIER_NAME_REGEX',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/shared_update_premium_formula_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/shared_update_premium_formula_request_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     }
 
     validations = {
         ('order',): {
             'inclusive_maximum': 10000,
             'inclusive_minimum': 0,
         },
+        ('variable_name',): {
+            'regex': {
+                'pattern': r'JS_VARIABLE_NAME_REGEX',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/store_product_factors_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/store_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/store_product_factors_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/store_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/suspend_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/withdraw_policy_response_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.insurance.model.policy_class import PolicyClass
+    globals()['PolicyClass'] = PolicyClass
 
-class SuspendPolicyRequestDto(ModelNormal):
+
+class WithdrawPolicyResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            '_from': (datetime,),  # noqa: E501
+            'policy': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_from': 'from',  # noqa: E501
+        'policy': 'policy',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SuspendPolicyRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, policy, *args, **kwargs):  # noqa: E501
+        """WithdrawPolicyResponseClass - a model defined in OpenAPI
+
+        Args:
+            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime): Terminate from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.policy = policy
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SuspendPolicyRequestDto - a model defined in OpenAPI
+    def __init__(self, policy, *args, **kwargs):  # noqa: E501
+        """WithdrawPolicyResponseClass - a model defined in OpenAPI
+
+        Args:
+            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime): Terminate from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.policy = policy
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/suspend_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/suspend_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/swap_premium_formulas_order_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/terminate_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/terminate_policy_response_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.insurance.model.policy_class import PolicyClass
+    globals()['PolicyClass'] = PolicyClass
 
-class TerminatePolicyRequestDto(ModelNormal):
+
+class TerminatePolicyResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,50 +67,55 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            '_from': (datetime,),  # noqa: E501
+            'policy': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_from': 'from',  # noqa: E501
+        'policy': 'policy',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TerminatePolicyRequestDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, policy, *args, **kwargs):  # noqa: E501
+        """TerminatePolicyResponseClass - a model defined in OpenAPI
+
+        Args:
+            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +140,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime): Terminate from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.policy = policy
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """TerminatePolicyRequestDto - a model defined in OpenAPI
+    def __init__(self, policy, *args, **kwargs):  # noqa: E501
+        """TerminatePolicyResponseClass - a model defined in OpenAPI
+
+        Args:
+            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +229,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            _from (datetime): Terminate from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.policy = policy
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/terminate_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_policy_response_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 def lazy_import():
     from eis.insurance.model.policy_class import PolicyClass
     globals()['PolicyClass'] = PolicyClass
 
 
-class TerminatePolicyResponseClass(ModelNormal):
+class UpdatePolicyResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -104,15 +104,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, policy, *args, **kwargs):  # noqa: E501
-        """TerminatePolicyResponseClass - a model defined in OpenAPI
+        """UpdatePolicyResponseClass - a model defined in OpenAPI
 
         Args:
             policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -193,15 +193,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, policy, *args, **kwargs):  # noqa: E501
-        """TerminatePolicyResponseClass - a model defined in OpenAPI
+        """UpdatePolicyResponseClass - a model defined in OpenAPI
 
         Args:
             policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/timeslice_class.py` & `eis-insurance-1.30.0/eis/insurance/model/timeslice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_insured_object_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_lead_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_lead_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_named_range_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_named_range_request_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,19 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'regex': {
+                'pattern': r'PYTHON_IDENTIFIER_NAME_REGEX',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_named_range_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_policy_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_policy_request_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     allowed_values = {
         ('status',): {
             'ACTIVE': "ACTIVE",
             'WITHDRAWN': "WITHDRAWN",
             'TERMINATED': "TERMINATED",
             'SUSPENDED': "SUSPENDED",
+            'PENDING': "PENDING",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -99,14 +100,15 @@
             'policy_objects': ([PolicyObjectDto],),  # noqa: E501
             '_from': (datetime,),  # noqa: E501
             'to': (datetime,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'premium_override': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'lead_code': (str,),  # noqa: E501
             'policy_number': (str,),  # noqa: E501
+            'reason': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -114,14 +116,15 @@
         'policy_objects': 'policyObjects',  # noqa: E501
         '_from': 'from',  # noqa: E501
         'to': 'to',  # noqa: E501
         'status': 'status',  # noqa: E501
         'premium_override': 'premiumOverride',  # noqa: E501
         'lead_code': 'leadCode',  # noqa: E501
         'policy_number': 'policyNumber',  # noqa: E501
+        'reason': 'reason',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -166,14 +169,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             to (datetime): Date to which the policy should be updated. This will create a new timeline finishing at this date.. [optional]  # noqa: E501
             status (str): Policy status.. [optional]  # noqa: E501
             premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Premium Override. [optional]  # noqa: E501
             lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
             policy_number (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
+            reason (str): Policy status transition reason.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -262,14 +266,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             to (datetime): Date to which the policy should be updated. This will create a new timeline finishing at this date.. [optional]  # noqa: E501
             status (str): Policy status.. [optional]  # noqa: E501
             premium_override (bool, date, datetime, dict, float, int, list, str, none_type): Premium Override. [optional]  # noqa: E501
             lead_code (str): Unique identifier of the lead that this object belongs to.. [optional]  # noqa: E501
             policy_number (str): Unique identifier of the policy that this object belongs to.. [optional]  # noqa: E501
+            reason (str): Policy status transition reason.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_response_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from eis.insurance.model.policy_class import PolicyClass
-    globals()['PolicyClass'] = PolicyClass
+    from eis.insurance.model.premium_formula_class import PremiumFormulaClass
+    globals()['PremiumFormulaClass'] = PremiumFormulaClass
 
 
-class UpdatePolicyResponseClass(ModelNormal):
+class UpdatePremiumFormulaResponseClass(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,38 +84,38 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'policy': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'premium_formula': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'policy': 'policy',  # noqa: E501
+        'premium_formula': 'premiumFormula',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, policy, *args, **kwargs):  # noqa: E501
-        """UpdatePolicyResponseClass - a model defined in OpenAPI
+    def _from_openapi_data(cls, premium_formula, *args, **kwargs):  # noqa: E501
+        """UpdatePremiumFormulaResponseClass - a model defined in OpenAPI
 
         Args:
-            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
+            premium_formula (bool, date, datetime, dict, float, int, list, str, none_type): Premium formula.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.policy = policy
+        self.premium_formula = premium_formula
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, policy, *args, **kwargs):  # noqa: E501
-        """UpdatePolicyResponseClass - a model defined in OpenAPI
+    def __init__(self, premium_formula, *args, **kwargs):  # noqa: E501
+        """UpdatePremiumFormulaResponseClass - a model defined in OpenAPI
 
         Args:
-            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
+            premium_formula (bool, date, datetime, dict, float, int, list, str, none_type): Premium formula.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,15 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.policy = policy
+        self.premium_formula = premium_formula
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_premium_formula_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_premium_formula_request_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     }
 
     validations = {
         ('order',): {
             'inclusive_maximum': 10000,
             'inclusive_minimum': 0,
         },
+        ('variable_name',): {
+            'regex': {
+                'pattern': r'JS_VARIABLE_NAME_REGEX',  # noqa: E501
+            },
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_premium_formula_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/terminate_policy_request_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.insurance.model.premium_formula_class import PremiumFormulaClass
-    globals()['PremiumFormulaClass'] = PremiumFormulaClass
 
-
-class UpdatePremiumFormulaResponseClass(ModelNormal):
+class TerminatePolicyRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,66 +52,76 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('reason',): {
+            'TERMINATION_AT_RENEWAL': "termination_at_renewal",
+            'TERMINATION_AFTER_CLAIM': "termination_after_claim",
+            'TERMINATION_DUE_TO_UNDERWRITING': "termination_due_to_underwriting",
+            'TERMINATION_DUE_TO_DEFAULT_OF_INITIAL_PREMIUM': "termination_due_to_default_of_initial_premium",
+            'TERMINATION_DUE_TO_DEFAULT_OF_SUBSEQUENT_PREMIUM': "termination_due_to_default_of_subsequent_premium",
+            'TERMINATION_DUE_TO_DOUBLE_INSURANCE': "termination_due_to_double_insurance",
+            'TERMINATION_DUE_TO_LOSS_OF_RISK': "termination_due_to_loss_of_risk",
+            'TERMINATION_DUE_TO_BREACH_OF_DUTY': "termination_due_to_breach_of_duty",
+            'TERMINATION_DUE_TO_EXPIRY': "termination_due_to_expiry",
+            'WITHDRAWAL': "withdrawal",
+            'OTHER': "other",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'premium_formula': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            '_from': (datetime,),  # noqa: E501
+            'reason': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'premium_formula': 'premiumFormula',  # noqa: E501
+        '_from': 'from',  # noqa: E501
+        'reason': 'reason',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, premium_formula, *args, **kwargs):  # noqa: E501
-        """UpdatePremiumFormulaResponseClass - a model defined in OpenAPI
-
-        Args:
-            premium_formula (bool, date, datetime, dict, float, int, list, str, none_type): Premium formula.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TerminatePolicyRequestDto - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,14 +146,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            _from (datetime): Terminate from.. [optional]  # noqa: E501
+            reason (str): Policy termination reason.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +179,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.premium_formula = premium_formula
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +199,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, premium_formula, *args, **kwargs):  # noqa: E501
-        """UpdatePremiumFormulaResponseClass - a model defined in OpenAPI
-
-        Args:
-            premium_formula (bool, date, datetime, dict, float, int, list, str, none_type): Premium formula.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TerminatePolicyRequestDto - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,14 +233,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            _from (datetime): Terminate from.. [optional]  # noqa: E501
+            reason (str): Policy termination reason.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,15 +264,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.premium_formula = premium_formula
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_product_field_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_product_field_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_product_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_product_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_product_version_request_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/update_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/update_product_version_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/update_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/model/uploaded_document_dto.py` & `eis-insurance-1.30.0/eis/insurance/model/validate_product_factors_request_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from eis.insurance.model.csv_product_factor_dto import CsvProductFactorDto
+    globals()['CsvProductFactorDto'] = CsvProductFactorDto
 
-class UploadedDocumentDto(ModelNormal):
+
+class ValidateProductFactorsRequestDto(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,53 +67,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'codes': ([str],),  # noqa: E501
+            'product_version_id': (float,),  # noqa: E501
+            'product_factors': ([CsvProductFactorDto],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'codes': 'codes',  # noqa: E501
+        'product_version_id': 'productVersionId',  # noqa: E501
+        'product_factors': 'productFactors',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, codes, *args, **kwargs):  # noqa: E501
-        """UploadedDocumentDto - a model defined in OpenAPI
+    def _from_openapi_data(cls, product_version_id, product_factors, *args, **kwargs):  # noqa: E501
+        """ValidateProductFactorsRequestDto - a model defined in OpenAPI
 
         Args:
-            codes ([str]): Uploaded document codes.
+            product_version_id (float): Unique identifier referencing the Product version.
+            product_factors ([CsvProductFactorDto]): Factors
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.codes = codes
+        self.product_version_id = product_version_id
+        self.product_factors = product_factors
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,19 +196,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, codes, *args, **kwargs):  # noqa: E501
-        """UploadedDocumentDto - a model defined in OpenAPI
+    def __init__(self, product_version_id, product_factors, *args, **kwargs):  # noqa: E501
+        """ValidateProductFactorsRequestDto - a model defined in OpenAPI
 
         Args:
-            codes ([str]): Uploaded document codes.
+            product_version_id (float): Unique identifier referencing the Product version.
+            product_factors ([CsvProductFactorDto]): Factors
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,15 +263,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.codes = codes
+        self.product_version_id = product_version_id
+        self.product_factors = product_factors
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model/withdraw_policy_response_class.py` & `eis-insurance-1.30.0/eis/insurance/model/inline_response200.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from eis.insurance.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from eis.insurance.model.policy_class import PolicyClass
-    globals()['PolicyClass'] = PolicyClass
 
-
-class WithdrawPolicyResponseClass(ModelNormal):
+class InlineResponse200(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,55 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'policy': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'status': (str,),  # noqa: E501
+            'info': ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}, none_type,),  # noqa: E501
+            'error': ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}, none_type,),  # noqa: E501
+            'details': ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'policy': 'policy',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'info': 'info',  # noqa: E501
+        'error': 'error',  # noqa: E501
+        'details': 'details',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, policy, *args, **kwargs):  # noqa: E501
-        """WithdrawPolicyResponseClass - a model defined in OpenAPI
-
-        Args:
-            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """InlineResponse200 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,14 +137,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            status (str): [optional]  # noqa: E501
+            info ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}, none_type): [optional]  # noqa: E501
+            error ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}, none_type): [optional]  # noqa: E501
+            details ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +172,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.policy = policy
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, policy, *args, **kwargs):  # noqa: E501
-        """WithdrawPolicyResponseClass - a model defined in OpenAPI
-
-        Args:
-            policy (bool, date, datetime, dict, float, int, list, str, none_type): Policy
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """InlineResponse200 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,14 +226,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            status (str): [optional]  # noqa: E501
+            info ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}, none_type): [optional]  # noqa: E501
+            error ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}, none_type): [optional]  # noqa: E501
+            details ({str: ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,15 +259,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.policy = policy
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `eis-insurance-1.26.0/eis/insurance/model_utils.py` & `eis-insurance-1.30.0/eis/insurance/model_utils.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/models/__init__.py` & `eis-insurance-1.30.0/eis/insurance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis/insurance/rest.py` & `eis-insurance-1.30.0/eis/insurance/rest.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/eis_insurance.egg-info/SOURCES.txt` & `eis-insurance-1.30.0/eis_insurance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/setup.py` & `eis-insurance-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "eis-insurance"
-VERSION = "1.26.0"
+VERSION = "1.30.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `eis-insurance-1.26.0/test/test_activate_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_activate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_activate_policy_response_class.py` & `eis-insurance-1.30.0/test/test_activate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_calculate_custom_premium_request_dto.py` & `eis-insurance-1.30.0/test/test_calculate_custom_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_calculate_premium_request_dto.py` & `eis-insurance-1.30.0/test/test_calculate_premium_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_calculate_product_fields_request_dto.py` & `eis-insurance-1.30.0/test/test_calculate_product_fields_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_clone_product_version_request_dto.py` & `eis-insurance-1.30.0/test/test_clone_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_account_request_dto.py` & `eis-insurance-1.30.0/test/test_create_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_bank_account_request_dto.py` & `eis-insurance-1.30.0/test/test_create_bank_account_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_custom_application_request_dto.py` & `eis-insurance-1.30.0/test/test_create_custom_application_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_dummy_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_create_dummy_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_insured_object_request_dto.py` & `eis-insurance-1.30.0/test/test_create_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_insured_object_response_class.py` & `eis-insurance-1.30.0/test/test_create_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_lead_async_response_class.py` & `eis-insurance-1.30.0/test/test_create_lead_async_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_lead_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_lead_request_dto.py` & `eis-insurance-1.30.0/test/test_create_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_lead_response_class.py` & `eis-insurance-1.30.0/test/test_create_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_lead_status_request_dto.py` & `eis-insurance-1.30.0/test/test_create_lead_status_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_lead_status_response_class.py` & `eis-insurance-1.30.0/test/test_create_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_named_range_request_dto.py` & `eis-insurance-1.30.0/test/test_create_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_named_range_response_class.py` & `eis-insurance-1.30.0/test/test_create_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_named_request_s3_data_class.py` & `eis-insurance-1.30.0/test/test_create_named_request_s3_data_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_payment_method_request_dto.py` & `eis-insurance-1.30.0/test/test_create_payment_method_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_create_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_policy_response_class.py` & `eis-insurance-1.30.0/test/test_create_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_premium_formula_request_dto.py` & `eis-insurance-1.30.0/test/test_create_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_premium_formula_response_class.py` & `eis-insurance-1.30.0/test/test_create_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_product_field_request_dto.py` & `eis-insurance-1.30.0/test/test_create_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_product_field_response_class.py` & `eis-insurance-1.30.0/test/test_create_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_product_request_dto.py` & `eis-insurance-1.30.0/test/test_create_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_create_product_response_class.py` & `eis-insurance-1.30.0/test/test_create_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_csv_product_factor_dto.py` & `eis-insurance-1.30.0/test/test_csv_product_factor_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_default_api.py` & `eis-insurance-1.30.0/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_delete_request_dto.py` & `eis-insurance-1.30.0/test/test_delete_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_delete_response_class.py` & `eis-insurance-1.30.0/test/test_delete_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_empty_response_class.py` & `eis-insurance-1.30.0/test/test_empty_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_insured_object_response_class.py` & `eis-insurance-1.30.0/test/test_get_insured_object_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_lead_response_class.py` & `eis-insurance-1.30.0/test/test_get_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_lead_status_response_class.py` & `eis-insurance-1.30.0/test/test_get_lead_status_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_named_range_response_class.py` & `eis-insurance-1.30.0/test/test_get_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_policy_data_by_date_request_dto.py` & `eis-insurance-1.30.0/test/test_get_policy_data_by_date_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_get_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_policy_response_class.py` & `eis-insurance-1.30.0/test/test_get_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_premium_formula_request_dto.py` & `eis-insurance-1.30.0/test/test_get_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_premium_formula_response_class.py` & `eis-insurance-1.30.0/test/test_get_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_factor_response_class.py` & `eis-insurance-1.30.0/test/test_get_product_factor_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_factor_value_request_dto.py` & `eis-insurance-1.30.0/test/test_get_product_factor_value_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_factor_value_response_class.py` & `eis-insurance-1.30.0/test/test_get_product_factor_value_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_factors_for_version_request_dto.py` & `eis-insurance-1.30.0/test/test_get_product_factors_for_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_factors_for_version_response_class.py` & `eis-insurance-1.30.0/test/test_get_product_factors_for_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_field_request_dto.py` & `eis-insurance-1.30.0/test/test_get_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_field_response_class.py` & `eis-insurance-1.30.0/test/test_get_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_request_dto.py` & `eis-insurance-1.30.0/test/test_get_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_response_class.py` & `eis-insurance-1.30.0/test/test_get_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_version_request_dto.py` & `eis-insurance-1.30.0/test/test_get_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_get_product_version_response_class.py` & `eis-insurance-1.30.0/test/test_get_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_grouped_product_factor_class.py` & `eis-insurance-1.30.0/test/test_grouped_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_grouped_product_factor_value_class.py` & `eis-insurance-1.30.0/test/test_grouped_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_grouped_product_factors_response_class.py` & `eis-insurance-1.30.0/test/test_grouped_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_grpc_patch_lead_request_dto.py` & `eis-insurance-1.30.0/test/test_grpc_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_grpc_update_lead_request_dto.py` & `eis-insurance-1.30.0/test/test_grpc_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_inline_response200.py` & `eis-insurance-1.30.0/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_inline_response503.py` & `eis-insurance-1.30.0/test/test_inline_response503.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_insured_object_class.py` & `eis-insurance-1.30.0/test/test_insured_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_insured_object_type_class.py` & `eis-insurance-1.30.0/test/test_insured_object_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_insured_object_types_api.py` & `eis-insurance-1.30.0/test/test_insured_object_types_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_insured_objects_api.py` & `eis-insurance-1.30.0/test/test_insured_objects_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_invoice_item_class.py` & `eis-insurance-1.30.0/test/test_invoice_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_invoice_status_class.py` & `eis-insurance-1.30.0/test/test_invoice_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_lead_bank_account_class.py` & `eis-insurance-1.30.0/test/test_lead_bank_account_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_lead_class.py` & `eis-insurance-1.30.0/test/test_lead_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_lead_status_class.py` & `eis-insurance-1.30.0/test/test_lead_status_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_lead_statuses_api.py` & `eis-insurance-1.30.0/test/test_lead_statuses_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_leads_api.py` & `eis-insurance-1.30.0/test/test_leads_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_insured_object_types_response_class.py` & `eis-insurance-1.30.0/test/test_list_insured_object_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_insured_objects_response_class.py` & `eis-insurance-1.30.0/test/test_list_insured_objects_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_lead_statuses_response_class.py` & `eis-insurance-1.30.0/test/test_list_lead_statuses_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_leads_response_class.py` & `eis-insurance-1.30.0/test/test_list_leads_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_named_ranges_response_class.py` & `eis-insurance-1.30.0/test/test_list_named_ranges_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_policies_response_class.py` & `eis-insurance-1.30.0/test/test_list_policies_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_premium_formulas_response_class.py` & `eis-insurance-1.30.0/test/test_list_premium_formulas_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_product_factors_response_class.py` & `eis-insurance-1.30.0/test/test_list_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_product_field_types_response_class.py` & `eis-insurance-1.30.0/test/test_list_product_field_types_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_product_fields_response_class.py` & `eis-insurance-1.30.0/test/test_list_product_fields_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_products_response_class.py` & `eis-insurance-1.30.0/test/test_list_products_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_list_request_dto.py` & `eis-insurance-1.30.0/test/test_list_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_named_range_class.py` & `eis-insurance-1.30.0/test/test_named_range_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_named_ranges_api.py` & `eis-insurance-1.30.0/test/test_named_ranges_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_patch_lead_request_dto.py` & `eis-insurance-1.30.0/test/test_patch_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_patch_lead_response_class.py` & `eis-insurance-1.30.0/test/test_patch_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_patch_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_patch_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_patch_policy_response_class.py` & `eis-insurance-1.30.0/test/test_patch_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policies_api.py` & `eis-insurance-1.30.0/test/test_policies_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policy_class.py` & `eis-insurance-1.30.0/test/test_policy_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policy_object_class.py` & `eis-insurance-1.30.0/test/test_policy_object_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policy_object_dto.py` & `eis-insurance-1.30.0/test/test_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policy_premium_class.py` & `eis-insurance-1.30.0/test/test_policy_premium_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policy_premium_item_class.py` & `eis-insurance-1.30.0/test/test_policy_premium_item_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_policy_version_class.py` & `eis-insurance-1.30.0/test/test_policy_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_premium_formula_class.py` & `eis-insurance-1.30.0/test/test_premium_formula_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_premium_formulas_api.py` & `eis-insurance-1.30.0/test/test_premium_formulas_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_premium_override_dto.py` & `eis-insurance-1.30.0/test/test_premium_override_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_premium_override_request_class.py` & `eis-insurance-1.30.0/test/test_premium_override_request_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_premium_override_request_dto.py` & `eis-insurance-1.30.0/test/test_premium_override_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_class.py` & `eis-insurance-1.30.0/test/test_product_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_factor_class.py` & `eis-insurance-1.30.0/test/test_product_factor_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_factor_for_version_class.py` & `eis-insurance-1.30.0/test/test_product_factor_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_factor_value_class.py` & `eis-insurance-1.30.0/test/test_product_factor_value_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_factor_value_for_version_class.py` & `eis-insurance-1.30.0/test/test_product_factor_value_for_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_factors_api.py` & `eis-insurance-1.30.0/test/test_product_factors_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_field_class.py` & `eis-insurance-1.30.0/test/test_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_field_type_class.py` & `eis-insurance-1.30.0/test/test_product_field_type_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_fields_api.py` & `eis-insurance-1.30.0/test/test_product_fields_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_version_class.py` & `eis-insurance-1.30.0/test/test_product_version_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_product_versions_api.py` & `eis-insurance-1.30.0/test/test_product_versions_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_products_api.py` & `eis-insurance-1.30.0/test/test_products_api.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_sepa_dto.py` & `eis-insurance-1.30.0/test/test_sepa_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_shared_create_lead_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_shared_create_lead_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_shared_invoice_class.py` & `eis-insurance-1.30.0/test/test_shared_invoice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_shared_lead_policy_object_dto.py` & `eis-insurance-1.30.0/test/test_shared_lead_policy_object_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_shared_product_field_class.py` & `eis-insurance-1.30.0/test/test_shared_product_field_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_shared_update_named_range_request_dto.py` & `eis-insurance-1.30.0/test/test_shared_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_shared_update_premium_formula_request_dto.py` & `eis-insurance-1.30.0/test/test_shared_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_store_product_factors_request_dto.py` & `eis-insurance-1.30.0/test/test_store_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_store_product_factors_response_class.py` & `eis-insurance-1.30.0/test/test_store_product_factors_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_suspend_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_suspend_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_suspend_policy_response_class.py` & `eis-insurance-1.30.0/test/test_suspend_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_swap_premium_formulas_order_request_dto.py` & `eis-insurance-1.30.0/test/test_swap_premium_formulas_order_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_terminate_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_terminate_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_terminate_policy_response_class.py` & `eis-insurance-1.30.0/test/test_terminate_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_timeslice_class.py` & `eis-insurance-1.30.0/test/test_timeslice_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_insured_object_request_dto.py` & `eis-insurance-1.30.0/test/test_update_insured_object_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_lead_request_dto.py` & `eis-insurance-1.30.0/test/test_update_lead_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_lead_response_class.py` & `eis-insurance-1.30.0/test/test_update_lead_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_named_range_request_dto.py` & `eis-insurance-1.30.0/test/test_update_named_range_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_named_range_response_class.py` & `eis-insurance-1.30.0/test/test_update_named_range_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_policy_request_dto.py` & `eis-insurance-1.30.0/test/test_update_policy_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_policy_response_class.py` & `eis-insurance-1.30.0/test/test_update_policy_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_premium_formula_request_dto.py` & `eis-insurance-1.30.0/test/test_update_premium_formula_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_premium_formula_response_class.py` & `eis-insurance-1.30.0/test/test_update_premium_formula_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_product_field_request_dto.py` & `eis-insurance-1.30.0/test/test_update_product_field_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_product_field_response_class.py` & `eis-insurance-1.30.0/test/test_update_product_field_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_product_request_dto.py` & `eis-insurance-1.30.0/test/test_update_product_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_product_response_class.py` & `eis-insurance-1.30.0/test/test_update_product_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_product_version_request_dto.py` & `eis-insurance-1.30.0/test/test_update_product_version_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_update_product_version_response_class.py` & `eis-insurance-1.30.0/test/test_update_product_version_response_class.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_uploaded_document_dto.py` & `eis-insurance-1.30.0/test/test_uploaded_document_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_validate_product_factors_request_dto.py` & `eis-insurance-1.30.0/test/test_validate_product_factors_request_dto.py`

 * *Files identical despite different names*

### Comparing `eis-insurance-1.26.0/test/test_withdraw_policy_response_class.py` & `eis-insurance-1.30.0/test/test_withdraw_policy_response_class.py`

 * *Files identical despite different names*

