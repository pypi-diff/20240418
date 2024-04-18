# Comparing `tmp/focus_converter-0.7.1.dev8.tar.gz` & `tmp/focus_converter-0.7.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "focus_converter-0.7.1.dev8.tar", max compression
+gzip compressed data, was "focus_converter-0.7.1.dev9.tar", max compression
```

## Comparing `focus_converter-0.7.1.dev8.tar` & `focus_converter-0.7.1.dev9.tar`

### file list

```diff
@@ -1,209 +1,216 @@
--rw-r--r--   0        0        0     1074 2024-03-12 18:47:48.443540 focus_converter-0.7.1.dev8/LICENSE
--rw-r--r--   0        0        0     3819 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/README.md
--rw-r--r--   0        0        0        0 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/common/__init__.py
--rw-r--r--   0        0        0      974 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/common/cli_options.py
--rw-r--r--   0        0        0        0 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/configs/__init__.py
--rw-r--r--   0        0        0     7527 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/configs/base_config.py
--rw-r--r--   0        0        0      441 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/configs/string_transform_args.py
--rw-r--r--   0        0        0      922 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/0_dimension_dtypes_S001.yaml
--rw-r--r--   0        0        0     1267 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_charge_type_S001.yaml
--rw-r--r--   0        0        0      305 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_missing_dimension_line_item_net_unblended_cost_S001.yaml
--rw-r--r--   0        0        0      308 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_missing_dimension_reservation_reservation_a_r_n_S001.yaml
--rw-r--r--   0        0        0      291 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_reservation_reservation_arn_S001.yaml
--rw-r--r--   0        0        0      374 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_resource_type_S001.yaml
--rw-r--r--   0        0        0      372 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_resource_type_S002.yaml
--rw-r--r--   0        0        0      346 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_resource_type_S003.yaml
--rw-r--r--   0        0        0      293 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_savings_plan_savings_plan_arn_S001.yaml
--rw-r--r--   0        0        0      357 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/2_resource_name_S001.yaml
--rw-r--r--   0        0        0      165 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/availability_zone_S001.yaml
--rw-r--r--   0        0        0      317 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/billed_cost_S001.yaml
--rw-r--r--   0        0        0      153 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/billing_account_id_S001.yaml
--rw-r--r--   0        0        0      155 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/billing_currency_S001.yaml
--rw-r--r--   0        0        0      173 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/billing_period_end_S001.yaml
--rw-r--r--   0        0        0      181 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/billing_period_start_S001.yaml
--rw-r--r--   0        0        0      172 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/charge_description_S001.yaml
--rw-r--r--   0        0        0      340 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/charge_frequency_S001.yaml
--rw-r--r--   0        0        0      163 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/charge_period_end_S001.yaml
--rw-r--r--   0        0        0      171 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/charge_period_start_S001.yaml
--rw-r--r--   0        0        0      979 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/charge_sub_category_S001.yaml
--rw-r--r--   0        0        0      423 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/commitment_discount_category_S001.yaml
--rw-r--r--   0        0        0      386 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/commitment_discount_id_S001.yaml
--rw-r--r--   0        0        0      440 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/commitment_discount_type_S001.yaml
--rw-r--r--   0        0        0      991 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/effective_cost_S001.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/invoice_issuer_S001.yaml
--rw-r--r--   0        0        0      322 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/list_cost_S001.yaml
--rw-r--r--   0        0        0      160 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/list_unit_price_S001.yaml
--rw-r--r--   0        0        0     6355 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/mapping_files/aws_category_mapping.csv
--rw-r--r--   0        0        0      545 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/pricing_category_S001.yaml
--rw-r--r--   0        0        0      324 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/pricing_quantity_S001.yaml
--rw-r--r--   0        0        0      132 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/pricing_unit_S001.yaml
--rw-r--r--   0        0        0      130 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/provider_S001.yaml
--rw-r--r--   0        0        0      141 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/publisher_S001.yaml
--rw-r--r--   0        0        0      119 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/region_S001.yaml
--rw-r--r--   0        0        0      141 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/resource_id_S001.yaml
--rw-r--r--   0        0        0      326 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/service_category_S001.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/service_name_S001.yaml
--rw-r--r--   0        0        0      111 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/sku_id_S001.yaml
--rw-r--r--   0        0        0      269 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/sku_price_id_S001.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/usage_quantity_S001.yaml
--rw-r--r--   0        0        0      121 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/usage_unit_S001.yaml
--rw-r--r--   0        0        0     1281 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/0_dimension_dtypes_S001.yaml
--rw-r--r--   0        0        0     1249 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_charge_type_S001.yaml
--rw-r--r--   0        0        0      299 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_missing_dimension_line_item_net_unblended_cost_S001.yaml
--rw-r--r--   0        0        0      302 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_missing_dimension_reservation_reservation_a_r_n_S001.yaml
--rw-r--r--   0        0        0      372 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_resource_type_S001.yaml
--rw-r--r--   0        0        0      370 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_resource_type_S002.yaml
--rw-r--r--   0        0        0      346 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_resource_type_S003.yaml
--rw-r--r--   0        0        0      302 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_savings_plan_savings_plan_arn_S001.yaml
--rw-r--r--   0        0        0      355 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/2_resource_name_S001.yaml
--rw-r--r--   0        0        0      163 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/availability_zone_S001.yaml
--rw-r--r--   0        0        0      318 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/billed_cost_S001.yaml
--rw-r--r--   0        0        0      149 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/billing_account_id_S001.yaml
--rw-r--r--   0        0        0      151 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/billing_currency_S001.yaml
--rw-r--r--   0        0        0      169 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/billing_period_end_S001.yaml
--rw-r--r--   0        0        0      175 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/billing_period_start_S001.yaml
--rw-r--r--   0        0        0      169 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/charge_description_S001.yaml
--rw-r--r--   0        0        0      339 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/charge_frequency_S001.yaml
--rw-r--r--   0        0        0      157 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/charge_period_end_S001.yaml
--rw-r--r--   0        0        0      165 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/charge_period_start_S001.yaml
--rw-r--r--   0        0        0      974 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/charge_sub_category_S001.yaml
--rw-r--r--   0        0        0      423 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/commitment_discount_category_S001.yaml
--rw-r--r--   0        0        0      387 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/commitment_discount_id_S001.yaml
--rw-r--r--   0        0        0      440 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/commitment_discount_type_S001.yaml
--rw-r--r--   0        0        0      976 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/effective_cost_S001.yaml
--rw-r--r--   0        0        0      146 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/invoice_issuer_S001.yaml
--rw-r--r--   0        0        0      321 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/list_cost_S001.yaml
--rw-r--r--   0        0        0      157 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/list_unit_price_S001.yaml
--rw-r--r--   0        0        0      541 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/pricing_category_S001.yaml
--rw-r--r--   0        0        0      324 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/pricing_quantity_S001.yaml
--rw-r--r--   0        0        0      132 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/pricing_unit_S001.yaml
--rw-r--r--   0        0        0      130 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/provider_S001.yaml
--rw-r--r--   0        0        0      139 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/publisher_S001.yaml
--rw-r--r--   0        0        0      119 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/region_S001.yaml
--rw-r--r--   0        0        0      139 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/resource_id_S001.yaml
--rw-r--r--   0        0        0      324 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/service_category_S001.yaml
--rw-r--r--   0        0        0      145 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/service_name_S001.yaml
--rw-r--r--   0        0        0      111 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/sku_id_S001.yaml
--rw-r--r--   0        0        0      274 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/sku_price_id_S001.yaml
--rw-r--r--   0        0        0      145 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/usage_quantity_S001.yaml
--rw-r--r--   0        0        0      121 2024-03-12 18:47:48.531541 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/usage_unit_S001.yaml
--rw-r--r--   0        0        0      245 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/0_dimension_dtypes_S001.yaml
--rw-r--r--   0        0        0      178 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D0017_S001.yaml
--rw-r--r--   0        0        0      131 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D001_S001.yaml
--rw-r--r--   0        0        0      179 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D002_S001.yaml
--rw-r--r--   0        0        0      156 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D002_S002.yaml
--rw-r--r--   0        0        0      151 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D002_S003.yaml
--rw-r--r--   0        0        0      140 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D003_S001.yaml
--rw-r--r--   0        0        0      144 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D003_S002.yaml
--rw-r--r--   0        0        0      139 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D003_S003.yaml
--rw-r--r--   0        0        0      173 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D004_S001.yaml
--rw-r--r--   0        0        0      148 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D004_S002.yaml
--rw-r--r--   0        0        0      143 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D004_S003.yaml
--rw-r--r--   0        0        0      123 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D005_S001.yaml
--rw-r--r--   0        0        0      139 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D006_S001.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D007_S001.yaml
--rw-r--r--   0        0        0      131 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D008_S001.yaml
--rw-r--r--   0        0        0      138 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D009_S001.yaml
--rw-r--r--   0        0        0      328 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D010_S001.yaml
--rw-r--r--   0        0        0      126 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D012_S001.yaml
--rw-r--r--   0        0        0      150 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D013_S001.yaml
--rw-r--r--   0        0        0      142 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D014_S001.yaml
--rw-r--r--   0        0        0      140 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D015_S001.yaml
--rw-r--r--   0        0        0      122 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D016_S001.yaml
--rw-r--r--   0        0        0      138 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D017_S002.yaml
--rw-r--r--   0        0        0      149 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D017_S003.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D018_S001.yaml
--rw-r--r--   0        0        0      142 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D019_S001.yaml
--rw-r--r--   0        0        0      134 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D020_S001.yaml
--rw-r--r--   0        0        0      356 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D021_S001.yaml
--rw-r--r--   0        0        0      409 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D022_S001.yaml
--rw-r--r--   0        0        0      553 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D023_S001.yaml
--rw-r--r--   0        0        0      361 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D024_S001.yaml
--rw-r--r--   0        0        0      136 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D025_S001.yaml
--rw-r--r--   0        0        0      370 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D026_S001.yaml
--rw-r--r--   0        0        0      145 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D029_S001.yaml
--rw-r--r--   0        0        0    14015 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D030_S001.yaml
--rw-r--r--   0        0        0      134 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D031_S001.yaml
--rw-r--r--   0        0        0      440 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D033_S001.yaml
--rw-r--r--   0        0        0      158 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/commitment_discount_name_S001.yaml
--rw-r--r--   0        0        0     3459 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/mapping_files/azure_category_mapping.csv
--rw-r--r--   0        0        0      131 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/resource_id_S001.yaml
--rw-r--r--   0        0        0      133 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/usage_quantity_S001.yaml
--rw-r--r--   0        0        0      163 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/1_pricing_quantity_S001.yaml
--rw-r--r--   0        0        0       84 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/1_sku_id_S001.yaml
--rw-r--r--   0        0        0      141 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/1_sku_price_id_S001.yaml
--rw-r--r--   0        0        0      125 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/1_usage_quantity_S001.yaml
--rw-r--r--   0        0        0      113 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/1_usage_unit_S001.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D002_S001.yaml
--rw-r--r--   0        0        0      130 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D003_S001.yaml
--rw-r--r--   0        0        0      158 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D003_S002.yaml
--rw-r--r--   0        0        0      165 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D003_S003.yaml
--rw-r--r--   0        0        0      154 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D003_S004.yaml
--rw-r--r--   0        0        0      134 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D004_S001.yaml
--rw-r--r--   0        0        0      164 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D004_S002.yaml
--rw-r--r--   0        0        0      171 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D004_S003.yaml
--rw-r--r--   0        0        0      160 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D004_S004.yaml
--rw-r--r--   0        0        0      145 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D005_S001.yaml
--rw-r--r--   0        0        0      159 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D005_S002.yaml
--rw-r--r--   0        0        0      137 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D006_S001.yaml
--rw-r--r--   0        0        0      153 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D006_S002.yaml
--rw-r--r--   0        0        0      171 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D007_S001.yaml
--rw-r--r--   0        0        0      179 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D007_S002.yaml
--rw-r--r--   0        0        0      315 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D007_S003.yaml
--rw-r--r--   0        0        0      252 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D008_S001.yaml
--rw-r--r--   0        0        0      230 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D009_S001.yaml
--rw-r--r--   0        0        0      223 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D009_S002.yaml
--rw-r--r--   0        0        0      340 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D010_S001.yaml
--rw-r--r--   0        0        0      139 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D011_S001.yaml
--rw-r--r--   0        0        0      165 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D012_S001.yaml
--rw-r--r--   0        0        0      341 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D012_S002.yaml
--rw-r--r--   0        0        0      129 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D013_S001.yaml
--rw-r--r--   0        0        0      124 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D014_S001.yaml
--rw-r--r--   0        0        0      131 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/D016_S001.yaml
--rw-r--r--   0        0        0     3985 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/mapping_files/gcp_category_mapping.csv
--rw-r--r--   0        0        0      340 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/0_dimension_dtypes_S001.yaml
--rw-r--r--   0        0        0      163 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_availibility_zone_S001.yaml
--rw-r--r--   0        0        0      135 2024-03-12 18:47:48.535542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_billed_cost_S001.yaml
--rw-r--r--   0        0        0      149 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_billing_account_id_S001.yaml
--rw-r--r--   0        0        0      143 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_billing_currency_S001.yaml
--rw-r--r--   0        0        0      153 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_billing_period_end_S001.yaml
--rw-r--r--   0        0        0      159 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_billing_period_start_S001.yaml
--rw-r--r--   0        0        0      151 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_charge_description_S001.yaml
--rw-r--r--   0        0        0      158 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_charge_period_end_S001.yaml
--rw-r--r--   0        0        0      166 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_charge_period_start_S001.yaml
--rw-r--r--   0        0        0      127 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_effective_cost_S001.yaml
--rw-r--r--   0        0        0      147 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_pricing_unit_S001.yaml
--rw-r--r--   0        0        0      133 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_provider_S001.yaml
--rw-r--r--   0        0        0      119 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_region_S001.yaml
--rw-r--r--   0        0        0      135 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_resource_id_S001.yaml
--rw-r--r--   0        0        0      131 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_service_name_S001.yaml
--rw-r--r--   0        0        0      115 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_sku_id_S001.yaml
--rw-r--r--   0        0        0      137 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_sub_account_id_S001.yaml
--rw-r--r--   0        0        0      145 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_usage_quantity_S001.yaml
--rw-r--r--   0        0        0      143 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_configs/oci/1_usage_unit_S001.yaml
--rw-r--r--   0        0        0     1010 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/__init__.py
--rw-r--r--   0        0        0     4808 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/column_functions.py
--rw-r--r--   0        0        0     2833 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/datetime_functions.py
--rw-r--r--   0        0        0     5778 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/deferred_column_functions.py
--rw-r--r--   0        0        0     1176 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/lookup_function.py
--rw-r--r--   0        0        0     2439 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/sql_functions.py
--rw-r--r--   0        0        0     1382 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/string_functions.py
--rw-r--r--   0        0        0     6093 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_functions/validations.py
--rw-r--r--   0        0        0     7063 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/conversion_strategy.py
--rw-r--r--   0        0        0    12372 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/converter.py
--rw-r--r--   0        0        0        0 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/data_loaders/__init__.py
--rw-r--r--   0        0        0     1917 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/data_loaders/data_exporter.py
--rw-r--r--   0        0        0     2796 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/data_loaders/data_loader.py
--rw-r--r--   0        0        0     3518 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/data_loaders/provider_sensor.py
--rw-r--r--   0        0        0        1 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/exported_sample_data/aws_cur.csv
--rw-r--r--   0        0        0     5660 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/main.py
--rw-r--r--   0        0        0        0 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/models/__init__.py
--rw-r--r--   0        0        0     2900 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/models/focus_column_names.py
--rw-r--r--   0        0        0        0 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/utils/__init__.py
--rw-r--r--   0        0        0     4746 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/utils/export_conversion_rules.py
--rw-r--r--   0        0        0     2907 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/utils/export_converted_sample_data.py
--rw-r--r--   0        0        0     1820 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/utils/generate_per_provider_progress.py
--rw-r--r--   0        0        0     2124 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/focus_converter/utils/profiler.py
--rw-r--r--   0        0        0     1602 2024-03-12 18:47:48.539542 focus_converter-0.7.1.dev8/pyproject.toml
--rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 focus_converter-0.7.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-18 02:12:03.531411 focus_converter-0.7.1.dev9/LICENSE
+-rw-r--r--   0        0        0     3819 2024-04-18 02:12:03.611412 focus_converter-0.7.1.dev9/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/common/__init__.py
+-rw-r--r--   0        0        0      974 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/common/cli_options.py
+-rw-r--r--   0        0        0        0 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/configs/__init__.py
+-rw-r--r--   0        0        0     7527 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/configs/base_config.py
+-rw-r--r--   0        0        0      441 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/configs/string_transform_args.py
+-rw-r--r--   0        0        0      922 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/0_dimension_dtypes_S001.yaml
+-rw-r--r--   0        0        0     1267 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_charge_type_S001.yaml
+-rw-r--r--   0        0        0      305 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_missing_dimension_line_item_net_unblended_cost_S001.yaml
+-rw-r--r--   0        0        0      308 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_missing_dimension_reservation_reservation_a_r_n_S001.yaml
+-rw-r--r--   0        0        0      291 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_reservation_reservation_arn_S001.yaml
+-rw-r--r--   0        0        0      374 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_resource_type_S001.yaml
+-rw-r--r--   0        0        0      372 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_resource_type_S002.yaml
+-rw-r--r--   0        0        0      346 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_resource_type_S003.yaml
+-rw-r--r--   0        0        0      293 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_savings_plan_savings_plan_arn_S001.yaml
+-rw-r--r--   0        0        0      357 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/2_resource_name_S001.yaml
+-rw-r--r--   0        0        0      214 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/3_region_S001.yaml
+-rw-r--r--   0        0        0      165 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/availability_zone_S001.yaml
+-rw-r--r--   0        0        0      317 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/billed_cost_S001.yaml
+-rw-r--r--   0        0        0      153 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/billing_account_id_S001.yaml
+-rw-r--r--   0        0        0      155 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/billing_currency_S001.yaml
+-rw-r--r--   0        0        0      173 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/billing_period_end_S001.yaml
+-rw-r--r--   0        0        0      181 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/billing_period_start_S001.yaml
+-rw-r--r--   0        0        0      172 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/charge_description_S001.yaml
+-rw-r--r--   0        0        0      340 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/charge_frequency_S001.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/charge_period_end_S001.yaml
+-rw-r--r--   0        0        0      171 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/charge_period_start_S001.yaml
+-rw-r--r--   0        0        0      979 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/charge_sub_category_S001.yaml
+-rw-r--r--   0        0        0      423 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/commitment_discount_category_S001.yaml
+-rw-r--r--   0        0        0      386 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/commitment_discount_id_S001.yaml
+-rw-r--r--   0        0        0      440 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/commitment_discount_type_S001.yaml
+-rw-r--r--   0        0        0      991 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/effective_cost_S001.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/invoice_issuer_S001.yaml
+-rw-r--r--   0        0        0      322 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/list_cost_S001.yaml
+-rw-r--r--   0        0        0      160 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/list_unit_price_S001.yaml
+-rw-r--r--   0        0        0     6421 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/mapping_files/aws_category_mapping.csv
+-rw-r--r--   0        0        0      545 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/pricing_category_S001.yaml
+-rw-r--r--   0        0        0      324 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/pricing_quantity_S001.yaml
+-rw-r--r--   0        0        0      132 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/pricing_unit_S001.yaml
+-rw-r--r--   0        0        0      130 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/provider_S001.yaml
+-rw-r--r--   0        0        0      141 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/publisher_S001.yaml
+-rw-r--r--   0        0        0      300 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/region_S001.yaml
+-rw-r--r--   0        0        0      141 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/resource_id_S001.yaml
+-rw-r--r--   0        0        0      326 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/service_category_S001.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/service_name_S001.yaml
+-rw-r--r--   0        0        0      111 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/sku_id_S001.yaml
+-rw-r--r--   0        0        0      269 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/sku_price_id_S001.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/usage_quantity_S001.yaml
+-rw-r--r--   0        0        0      121 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/usage_unit_S001.yaml
+-rw-r--r--   0        0        0     1281 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/0_dimension_dtypes_S001.yaml
+-rw-r--r--   0        0        0     1249 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_charge_type_S001.yaml
+-rw-r--r--   0        0        0      299 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_missing_dimension_line_item_net_unblended_cost_S001.yaml
+-rw-r--r--   0        0        0      302 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_missing_dimension_reservation_reservation_a_r_n_S001.yaml
+-rw-r--r--   0        0        0      372 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_resource_type_S001.yaml
+-rw-r--r--   0        0        0      370 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_resource_type_S002.yaml
+-rw-r--r--   0        0        0      346 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_resource_type_S003.yaml
+-rw-r--r--   0        0        0      302 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_savings_plan_savings_plan_arn_S001.yaml
+-rw-r--r--   0        0        0      355 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/2_resource_name_S001.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/availability_zone_S001.yaml
+-rw-r--r--   0        0        0      318 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/billed_cost_S001.yaml
+-rw-r--r--   0        0        0      149 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/billing_account_id_S001.yaml
+-rw-r--r--   0        0        0      151 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/billing_currency_S001.yaml
+-rw-r--r--   0        0        0      169 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/billing_period_end_S001.yaml
+-rw-r--r--   0        0        0      175 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/billing_period_start_S001.yaml
+-rw-r--r--   0        0        0      169 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/charge_description_S001.yaml
+-rw-r--r--   0        0        0      339 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/charge_frequency_S001.yaml
+-rw-r--r--   0        0        0      157 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/charge_period_end_S001.yaml
+-rw-r--r--   0        0        0      165 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/charge_period_start_S001.yaml
+-rw-r--r--   0        0        0      974 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/charge_sub_category_S001.yaml
+-rw-r--r--   0        0        0      423 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/commitment_discount_category_S001.yaml
+-rw-r--r--   0        0        0      387 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/commitment_discount_id_S001.yaml
+-rw-r--r--   0        0        0      440 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/commitment_discount_type_S001.yaml
+-rw-r--r--   0        0        0      976 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/effective_cost_S001.yaml
+-rw-r--r--   0        0        0      146 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/invoice_issuer_S001.yaml
+-rw-r--r--   0        0        0      321 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/list_cost_S001.yaml
+-rw-r--r--   0        0        0      157 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/list_unit_price_S001.yaml
+-rw-r--r--   0        0        0      541 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/pricing_category_S001.yaml
+-rw-r--r--   0        0        0      324 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/pricing_quantity_S001.yaml
+-rw-r--r--   0        0        0      132 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/pricing_unit_S001.yaml
+-rw-r--r--   0        0        0      130 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/provider_S001.yaml
+-rw-r--r--   0        0        0      139 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/publisher_S001.yaml
+-rw-r--r--   0        0        0      119 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/region_S001.yaml
+-rw-r--r--   0        0        0      139 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/resource_id_S001.yaml
+-rw-r--r--   0        0        0      324 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/service_category_S001.yaml
+-rw-r--r--   0        0        0      145 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/service_name_S001.yaml
+-rw-r--r--   0        0        0      111 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/sku_id_S001.yaml
+-rw-r--r--   0        0        0      274 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/sku_price_id_S001.yaml
+-rw-r--r--   0        0        0      145 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/usage_quantity_S001.yaml
+-rw-r--r--   0        0        0      121 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/usage_unit_S001.yaml
+-rw-r--r--   0        0        0      245 2024-04-18 02:12:03.615412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/0_dimension_dtypes_S001.yaml
+-rw-r--r--   0        0        0      178 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D0017_S001.yaml
+-rw-r--r--   0        0        0      131 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D001_S001.yaml
+-rw-r--r--   0        0        0      179 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D002_S001.yaml
+-rw-r--r--   0        0        0      156 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D002_S002.yaml
+-rw-r--r--   0        0        0      151 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D002_S003.yaml
+-rw-r--r--   0        0        0      140 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D003_S001.yaml
+-rw-r--r--   0        0        0      144 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D003_S002.yaml
+-rw-r--r--   0        0        0      139 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D003_S003.yaml
+-rw-r--r--   0        0        0      173 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D004_S001.yaml
+-rw-r--r--   0        0        0      148 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D004_S002.yaml
+-rw-r--r--   0        0        0      143 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D004_S003.yaml
+-rw-r--r--   0        0        0      123 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D005_S001.yaml
+-rw-r--r--   0        0        0      139 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D006_S001.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D007_S001.yaml
+-rw-r--r--   0        0        0      131 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D008_S001.yaml
+-rw-r--r--   0        0        0      138 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D009_S001.yaml
+-rw-r--r--   0        0        0      328 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D010_S001.yaml
+-rw-r--r--   0        0        0      126 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D012_S001.yaml
+-rw-r--r--   0        0        0      150 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D013_S001.yaml
+-rw-r--r--   0        0        0      142 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D014_S001.yaml
+-rw-r--r--   0        0        0      140 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D015_S001.yaml
+-rw-r--r--   0        0        0      122 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D016_S001.yaml
+-rw-r--r--   0        0        0      138 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D017_S002.yaml
+-rw-r--r--   0        0        0      149 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D017_S003.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D018_S001.yaml
+-rw-r--r--   0        0        0      142 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D019_S001.yaml
+-rw-r--r--   0        0        0      134 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D020_S001.yaml
+-rw-r--r--   0        0        0      356 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D021_S001.yaml
+-rw-r--r--   0        0        0      409 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D022_S001.yaml
+-rw-r--r--   0        0        0      553 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D023_S001.yaml
+-rw-r--r--   0        0        0      361 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D024_S001.yaml
+-rw-r--r--   0        0        0      136 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D025_S001.yaml
+-rw-r--r--   0        0        0      370 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D026_S001.yaml
+-rw-r--r--   0        0        0      145 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D029_S001.yaml
+-rw-r--r--   0        0        0    14015 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D030_S001.yaml
+-rw-r--r--   0        0        0      134 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D031_S001.yaml
+-rw-r--r--   0        0        0      440 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D033_S001.yaml
+-rw-r--r--   0        0        0      158 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/commitment_discount_name_S001.yaml
+-rw-r--r--   0        0        0     3459 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/mapping_files/azure_category_mapping.csv
+-rw-r--r--   0        0        0      131 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/resource_id_S001.yaml
+-rw-r--r--   0        0        0      133 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/usage_quantity_S001.yaml
+-rw-r--r--   0        0        0      250 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/0_dimension_dtypes_S001.yaml
+-rw-r--r--   0        0        0      129 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_availibity_zone_S001.yaml
+-rw-r--r--   0        0        0      106 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billed_cost_S001.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_account_id_S001.yaml
+-rw-r--r--   0        0        0      124 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_currency_S001.yaml
+-rw-r--r--   0        0        0      130 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_end_S001.yaml
+-rw-r--r--   0        0        0      158 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_end_S002.yaml
+-rw-r--r--   0        0        0      165 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_end_S003.yaml
+-rw-r--r--   0        0        0      154 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_end_S004.yaml
+-rw-r--r--   0        0        0      134 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_start_S001.yaml
+-rw-r--r--   0        0        0      164 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_start_S002.yaml
+-rw-r--r--   0        0        0      171 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_start_S003.yaml
+-rw-r--r--   0        0        0      160 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_billing_period_start_S004.yaml
+-rw-r--r--   0        0        0      137 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_charge_period_end_S001.yaml
+-rw-r--r--   0        0        0      153 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_charge_period_end_S002.yaml
+-rw-r--r--   0        0        0      145 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_charge_period_start_S001.yaml
+-rw-r--r--   0        0        0      159 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_charge_period_start_S002.yaml
+-rw-r--r--   0        0        0      453 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_charge_type_S001.yaml
+-rw-r--r--   0        0        0      162 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_list_cost_S001.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_pricing_quantity_S001.yaml
+-rw-r--r--   0        0        0      129 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_pricing_unit_S001.yaml
+-rw-r--r--   0        0        0      139 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_provider_S001.yaml
+-rw-r--r--   0        0        0      252 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_publisher_S001.yaml
+-rw-r--r--   0        0        0      171 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_region_S001.yaml
+-rw-r--r--   0        0        0      179 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_region_S002.yaml
+-rw-r--r--   0        0        0      315 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_region_S003.yaml
+-rw-r--r--   0        0        0      131 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_resource_id_S001.yaml
+-rw-r--r--   0        0        0      125 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_resource_name_S001.yaml
+-rw-r--r--   0        0        0      165 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_service_category_S001.yaml
+-rw-r--r--   0        0        0      341 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_service_category_S002.yaml
+-rw-r--r--   0        0        0      135 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_service_name_S001.yaml
+-rw-r--r--   0        0        0       84 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_sku_id_S001.yaml
+-rw-r--r--   0        0        0      141 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_sku_price_id_S001.yaml
+-rw-r--r--   0        0        0      125 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_usage_quantity_S001.yaml
+-rw-r--r--   0        0        0      113 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/1_usage_unit_S001.yaml
+-rw-r--r--   0        0        0      233 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/2_effective_cost_S001.yaml
+-rw-r--r--   0        0        0      323 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/2_effective_cost_S002.yaml
+-rw-r--r--   0        0        0     3985 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/mapping_files/gcp_category_mapping.csv
+-rw-r--r--   0        0        0      340 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/0_dimension_dtypes_S001.yaml
+-rw-r--r--   0        0        0      163 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_availibility_zone_S001.yaml
+-rw-r--r--   0        0        0      135 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_billed_cost_S001.yaml
+-rw-r--r--   0        0        0      149 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_billing_account_id_S001.yaml
+-rw-r--r--   0        0        0      143 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_billing_currency_S001.yaml
+-rw-r--r--   0        0        0      153 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_billing_period_end_S001.yaml
+-rw-r--r--   0        0        0      159 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_billing_period_start_S001.yaml
+-rw-r--r--   0        0        0      151 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_charge_description_S001.yaml
+-rw-r--r--   0        0        0      158 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_charge_period_end_S001.yaml
+-rw-r--r--   0        0        0      166 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_charge_period_start_S001.yaml
+-rw-r--r--   0        0        0      127 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_effective_cost_S001.yaml
+-rw-r--r--   0        0        0      147 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_pricing_unit_S001.yaml
+-rw-r--r--   0        0        0      133 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_provider_S001.yaml
+-rw-r--r--   0        0        0      119 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_region_S001.yaml
+-rw-r--r--   0        0        0      135 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_resource_id_S001.yaml
+-rw-r--r--   0        0        0      131 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_service_name_S001.yaml
+-rw-r--r--   0        0        0      115 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_sku_id_S001.yaml
+-rw-r--r--   0        0        0      137 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_sub_account_id_S001.yaml
+-rw-r--r--   0        0        0      145 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_usage_quantity_S001.yaml
+-rw-r--r--   0        0        0      143 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_configs/oci/1_usage_unit_S001.yaml
+-rw-r--r--   0        0        0     1010 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/__init__.py
+-rw-r--r--   0        0        0     4808 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/column_functions.py
+-rw-r--r--   0        0        0     2833 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/datetime_functions.py
+-rw-r--r--   0        0        0     5778 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/deferred_column_functions.py
+-rw-r--r--   0        0        0     1176 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/lookup_function.py
+-rw-r--r--   0        0        0     2439 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/sql_functions.py
+-rw-r--r--   0        0        0     1382 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/string_functions.py
+-rw-r--r--   0        0        0     6093 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_functions/validations.py
+-rw-r--r--   0        0        0     7063 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/conversion_strategy.py
+-rw-r--r--   0        0        0    12515 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/converter.py
+-rw-r--r--   0        0        0        0 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/data_loaders/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/data_loaders/data_exporter.py
+-rw-r--r--   0        0        0     2911 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/data_loaders/data_loader.py
+-rw-r--r--   0        0        0     3518 2024-04-18 02:12:03.619412 focus_converter-0.7.1.dev9/focus_converter/data_loaders/provider_sensor.py
+-rw-r--r--   0        0        0        1 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/exported_sample_data/aws_cur.csv
+-rw-r--r--   0        0        0     6206 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/main.py
+-rw-r--r--   0        0        0        0 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/models/__init__.py
+-rw-r--r--   0        0        0     2900 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/models/focus_column_names.py
+-rw-r--r--   0        0        0        0 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/utils/__init__.py
+-rw-r--r--   0        0        0     4746 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/utils/export_conversion_rules.py
+-rw-r--r--   0        0        0     2907 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/utils/export_converted_sample_data.py
+-rw-r--r--   0        0        0     1820 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/utils/generate_per_provider_progress.py
+-rw-r--r--   0        0        0     2124 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/focus_converter/utils/profiler.py
+-rw-r--r--   0        0        0     1602 2024-04-18 02:12:03.623412 focus_converter-0.7.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 focus_converter-0.7.1.dev9/PKG-INFO
```

### Comparing `focus_converter-0.7.1.dev8/LICENSE` & `focus_converter-0.7.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/README.md` & `focus_converter-0.7.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/common/cli_options.py` & `focus_converter-0.7.1.dev9/focus_converter/common/cli_options.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/configs/base_config.py` & `focus_converter-0.7.1.dev9/focus_converter/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/0_dimension_dtypes_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/0_dimension_dtypes_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/1_charge_type_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/1_charge_type_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/charge_sub_category_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/charge_sub_category_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/effective_cost_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/effective_cost_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/mapping_files/aws_category_mapping.csv` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/mapping_files/aws_category_mapping.csv`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 AmazonSWF,Business Applications
 AmazonWAM,Business Applications
 AmazonWorkDocs,Business Applications
 AmazonWorkLink,Business Applications
 AmazonWorkMail,Business Applications
 AmazonWorkSpacesWeb,Business Applications
 Compute,Business Applications
+ComputeSavingsPlans,Compute
 ContactLensAmazonConnect,Business Applications
 CustomerProfiles,Business Applications
 AWSBudgets,Management and Governance
 AWSCostExplorer,Management and Governance
 Savings Plans*,Management and Governance
 AWSNetworkFirewall,Networking
 Reserved Instance (RI) Reporting*,Management and Governance
@@ -118,14 +119,15 @@
 AWSIoTThingsGraph,Internet of Things
 AWSIoT,Internet of Things
 IoTDeviceDefender,Internet of Things
 IoTDeviceManagement,Internet of Things
 IoTTwinMaker,Internet of Things
 AWSDeepRacer,AI and Machine Learning
 AmazonA2I,AI and Machine Learning
+AmazonBedrock,AI and Machine Learning
 AmazonCodeWhisperer,AI and Machine Learning
 AmazonDevOpsGuru,AI and Machine Learning
 AmazonEI,AI and Machine Learning
 AmazonForecast,AI and Machine Learning
 AmazonFraudDetector,AI and Machine Learning
 AmazonHealthLake,AI and Machine Learning
 AmazonKendra,AI and Machine Learning
```

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws/pricing_category_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws/pricing_category_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/0_dimension_dtypes_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/0_dimension_dtypes_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/1_charge_type_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/1_charge_type_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/charge_sub_category_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/charge_sub_category_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/effective_cost_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/effective_cost_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/aws-cur/pricing_category_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/aws-cur/pricing_category_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D023_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D023_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/D030_S001.yaml` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/D030_S001.yaml`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/azure/mapping_files/azure_category_mapping.csv` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/azure/mapping_files/azure_category_mapping.csv`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_configs/gcp/mapping_files/gcp_category_mapping.csv` & `focus_converter-0.7.1.dev9/focus_converter/conversion_configs/gcp/mapping_files/gcp_category_mapping.csv`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/__init__.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/column_functions.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/column_functions.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/datetime_functions.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/datetime_functions.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/deferred_column_functions.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/deferred_column_functions.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/lookup_function.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/lookup_function.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/sql_functions.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/sql_functions.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/string_functions.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_functions/validations.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_functions/validations.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/conversion_strategy.py` & `focus_converter-0.7.1.dev9/focus_converter/conversion_strategy.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/converter.py` & `focus_converter-0.7.1.dev9/focus_converter/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,26 +61,32 @@
 
     # column prefix used in source dataset
     __column_prefix__: Optional[str] = None
 
     # converted column prefix to be added to converted columns
     __converted_column_prefix__: Optional[str] = None
 
-    def __init__(self, column_prefix=None, converted_column_prefix=None):
+    __basename_template__: Optional[str] = None
+
+    def __init__(
+        self, column_prefix=None, converted_column_prefix=None, basename_template=None
+    ):
         self.__temporary_columns__ = []
         self.__column_prefix__ = column_prefix
         self.__converted_column_prefix__ = converted_column_prefix
 
         # ColumnValidator, used to validate column names in sql queries and transformations
         self.__column_validator__ = ColumnValidator()
         self.plans = {}
 
         # deferred column plans, these plans are applied after lazyframe is loaded
         self.__deferred_column_plans__ = DeferredColumnFunctions()
 
+        self.__basename_template__ = basename_template
+
     def load_provider_conversion_configs(self):
         plans = {}
 
         for provider in os.listdir(BASE_CONVERSION_CONFIGS):
             # collect all plans specific to vendor
             provider_plans: List[ConversionPlan] = []
```

### Comparing `focus_converter-0.7.1.dev8/focus_converter/data_loaders/data_exporter.py` & `focus_converter-0.7.1.dev9/focus_converter/data_loaders/data_exporter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 import multiprocessing
+import re
 from queue import Empty
 from typing import List
 
 import polars as pl
 import pyarrow.parquet as pq
+from pyarrow import Table
 
+from focus_converter.models.focus_column_names import FocusColumnNames
 
-def __writer_process__(export_path, queue: multiprocessing.Queue):
+
+def __writer_process__(
+    export_path, queue: multiprocessing.Queue, basename_template: str
+):
     while True:
         try:
-            df = queue.get(timeout=0.1)
+            table = queue.get()
         except Empty:
             continue
 
-        if not isinstance(df, pl.DataFrame):
+        if not isinstance(table, Table):
             break
 
         pq.write_to_dataset(
-            root_path=export_path, compression="snappy", table=df.to_arrow()
+            root_path=export_path,
+            compression="snappy",
+            table=table,
+            basename_template=basename_template,
         )
 
 
 class DataExporter:
     def __init__(
         self,
         export_path,
         export_include_source_columns: bool,
+        basename_template: str = None,
         process_count: int = multiprocessing.cpu_count(),
     ):
         self.__export_path__ = export_path
         self.__export_include_source_columns__ = export_include_source_columns
-
+        if basename_template and not re.search(r"-{i}\.parquet$", basename_template):
+            basename_template += "-{i}.parquet"
+        self.__basename_template__ = basename_template
         self.__queue__ = queue = multiprocessing.Queue(maxsize=process_count)
 
         self.__processes__ = processes = []
         for _ in range(process_count):
             p = multiprocessing.Process(
                 target=__writer_process__,
-                kwargs={"queue": queue, "export_path": self.__export_path__},
+                kwargs={
+                    "queue": queue,
+                    "export_path": self.__export_path__,
+                    "basename_template": self.__basename_template__,
+                },
             )
             processes.append(p)
 
         # start processes
         [p.start() for p in processes]
 
     def __del__(self):
@@ -56,15 +72,39 @@
             p.join()
             p.close()
 
         self.__queue__.close()
         del self.__queue__
         self.__queue__ = None
 
+    def __re_order_columns__(self):
+        """
+        Applies a new column ordering to allow easy reading
+        """
+        pass
+
     def collect(self, lf: pl.LazyFrame, collected_columns: List[str]):
         if not self.__export_include_source_columns__:
             # collect only applied columns
-            lf = lf.select(collected_columns)
+            sorted_column_list = [
+                focus_column.value
+                for focus_column in FocusColumnNames
+                if focus_column.value in collected_columns
+            ]
+        else:
+            # collect focus columns first
+            sorted_column_list = [
+                focus_column.value
+                for focus_column in FocusColumnNames
+                if focus_column.value in lf.columns
+            ]
+
+            # now collect all original provided columns
+            sorted_column_list += [
+                column for column in lf.columns if column not in sorted_column_list
+            ]
+
+        lf = lf.select(sorted_column_list)
 
         # compute final dataframe
         df: pl.DataFrame = lf.collect(streaming=True)
-        self.__queue__.put(df)
+        self.__queue__.put(df.to_arrow())
```

### Comparing `focus_converter-0.7.1.dev8/focus_converter/data_loaders/data_loader.py` & `focus_converter-0.7.1.dev9/focus_converter/data_loaders/data_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,19 @@
         )
 
         total_rows = dataset.count_rows()
 
         with tqdm(total=total_rows) as pobj:
             for batch in scanner.to_batches():
                 df = pl.from_arrow(batch)
+
+                # skip if number of rows empty
+                if df.shape[0] == 0:
+                    continue
+
                 yield df.lazy()
                 pobj.update(df.shape[0])
 
     def load_parquet_file(self) -> Iterable[pl.LazyFrame]:
         # reads parquet from data path and returns a lazy object
 
         yield pl.read_parquet(self.__data_path__).lazy()
```

### Comparing `focus_converter-0.7.1.dev8/focus_converter/data_loaders/provider_sensor.py` & `focus_converter-0.7.1.dev9/focus_converter/data_loaders/provider_sensor.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/main.py` & `focus_converter-0.7.1.dev9/focus_converter/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,21 @@
     validate: Annotated[
         bool,
         typer.Option(
             help="Validate generated data to match FOCUS spec.",
             rich_help_panel="Validation",
         ),
     ] = False,
+    basename_template: Annotated[
+        str,
+        typer.Option(
+            help="Specify a template string for output filename as opposed to guid-{i}.",
+            rich_help_panel="Data Export",
+        ),
+    ] = None,
 ):
     provider_sensor = ProviderSensor(base_path=data_path)
     provider_sensor.load()
 
     converter = FocusConverter(
         column_prefix=column_prefix, converted_column_prefix=converted_column_prefix
     )
@@ -66,14 +73,15 @@
         data_path=data_path,
         data_format=provider_sensor.data_format,
         parquet_data_format=provider_sensor.parquet_data_format,
     )
     converter.configure_data_export(
         export_path=export_path,
         export_include_source_columns=export_include_source_columns,
+        basename_template=basename_template,
     )
     converter.prepare_horizontal_conversion_plan(provider=provider_sensor.provider)
     converter.convert()
 
     if validate:
         for segment_file_name in os.listdir(export_path):
             file_path = os.path.join(export_path, segment_file_name)
@@ -112,14 +120,21 @@
     validate: Annotated[
         bool,
         typer.Option(
             help="Validate generated data to match FOCUS spec.",
             rich_help_panel="Validation",
         ),
     ] = False,
+    basename_template: Annotated[
+        str,
+        typer.Option(
+            help="Specify a template string for output filename as opposed to `guid-{i}`.",
+            rich_help_panel="Data Export",
+        ),
+    ] = None,
 ):
     # compute function for conversion
 
     if data_format == DataFormats.PARQUET and parquet_data_format is None:
         raise typer.BadParameter("parquet_data_format required")
 
     converter = FocusConverter(
@@ -130,14 +145,15 @@
         data_path=data_path,
         data_format=data_format,
         parquet_data_format=parquet_data_format,
     )
     converter.configure_data_export(
         export_path=export_path,
         export_include_source_columns=export_include_source_columns,
+        basename_template=basename_template,
     )
     converter.prepare_horizontal_conversion_plan(provider=provider)
     converter.convert()
 
     if validate:
         for segment_file_name in os.listdir(export_path):
             file_path = os.path.join(export_path, segment_file_name)
```

### Comparing `focus_converter-0.7.1.dev8/focus_converter/models/focus_column_names.py` & `focus_converter-0.7.1.dev9/focus_converter/models/focus_column_names.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/utils/export_conversion_rules.py` & `focus_converter-0.7.1.dev9/focus_converter/utils/export_conversion_rules.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/utils/export_converted_sample_data.py` & `focus_converter-0.7.1.dev9/focus_converter/utils/export_converted_sample_data.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/utils/generate_per_provider_progress.py` & `focus_converter-0.7.1.dev9/focus_converter/utils/generate_per_provider_progress.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/focus_converter/utils/profiler.py` & `focus_converter-0.7.1.dev9/focus_converter/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `focus_converter-0.7.1.dev8/pyproject.toml` & `focus_converter-0.7.1.dev9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "focus_converter"
-version = "0.7.1-dev8"
+version = "0.7.1-dev9"
 description = ""
 authors = ["Varun Mittal <varunmittal91@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "focus_converter" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-polars = "^0.20.6"
+polars = "0.20.10"
 pydantic = "^2.1.1"
 pandas = "^2.0.3"
 pyarrow = "^14"
 typer = "^0.9.0"
 rich = "^13.5.2"
 networkx = "^3.1"
 tqdm = "^4.66.1"
```

### Comparing `focus_converter-0.7.1.dev8/PKG-INFO` & `focus_converter-0.7.1.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: focus_converter
-Version: 0.7.1.dev8
+Version: 0.7.1.dev9
 Summary: 
 Author: Varun Mittal
 Author-email: varunmittal91@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: focus-validator
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
-Requires-Dist: polars (>=0.20.6,<0.21.0)
+Requires-Dist: polars (==0.20.10)
 Requires-Dist: pyarrow (>=14,<15)
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: sqlglot (>=18.7.0,<19.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

