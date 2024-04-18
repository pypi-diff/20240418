# Comparing `tmp/ecodev_model-0.0.1.tar.gz` & `tmp/ecodev_model-0.0.164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodev_model-0.0.1.tar", max compression
+gzip compressed data, was "ecodev_model-0.0.164.tar", max compression
```

## Comparing `ecodev_model-0.0.1.tar` & `ecodev_model-0.0.164.tar`

### file list

```diff
@@ -1,7 +1,93 @@
--rwxr-xr-x   0        0        0       88 2024-03-29 07:13:58.501498 ecodev_model-0.0.1/README.md
--rwxr-xr-x   0        0        0      381 2024-02-14 14:22:13.750000 ecodev_model-0.0.1/ecodev_model/__init__.py
--rwxr-xr-x   0        0        0      692 2024-02-14 14:22:13.320000 ecodev_model-0.0.1/ecodev_model/emission_type.py
--rwxr-xr-x   0        0        0     1261 2024-02-14 14:21:30.500000 ecodev_model-0.0.1/ecodev_model/sector.py
--rwxr-xr-x   0        0        0     1037 2024-02-14 14:22:13.310000 ecodev_model-0.0.1/ecodev_model/units.py
--rwxr-xr-x   0        0        0      498 2024-03-29 07:14:22.013456 ecodev_model-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 ecodev_model-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/README.md
+-rw-r--r--   0        0        0     6016 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/__init__.py
+-rw-r--r--   0        0        0     2003 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/commons.py
+-rw-r--r--   0        0        0     3326 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/constants.py
+-rw-r--r--   0        0        0     1263 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/company/__init__.py
+-rwxr-xr-x   0        0        0     2044 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/company/company.py
+-rw-r--r--   0        0        0     3108 2024-04-18 11:50:26.793011 ecodev_model-0.0.164/ecodev_model/db_model/company/company_directory.py
+-rw-r--r--   0        0        0     2163 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/company/company_emission.py
+-rw-r--r--   0        0        0     2475 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/company/company_financial_data.py
+-rw-r--r--   0        0        0     2189 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/db_model/company/company_info.py
+-rw-r--r--   0        0        0     3493 2024-04-18 11:49:17.077734 ecodev_model-0.0.164/ecodev_model/db_model/company/company_reduction_target.py
+-rw-r--r--   0        0        0     3215 2024-04-18 11:54:56.994150 ecodev_model-0.0.164/ecodev_model/db_model/company/company_target.py
+-rw-r--r--   0        0        0      528 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/company/nace_isic_link.py
+-rw-r--r--   0        0        0     2538 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/company/security_isin.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/emission_factor/__init__.py
+-rw-r--r--   0        0        0     3389 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/emission_factor/emission_factor.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/factset/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/factset/factset_entity_data.py
+-rw-r--r--   0        0        0     2559 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/factset/factset_financial_data.py
+-rw-r--r--   0        0        0     1536 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/db_model/factset/factset_structure_data.py
+-rw-r--r--   0        0        0     2475 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/company/__init__.py
+-rw-r--r--   0        0        0      919 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/company/cdp.py
+-rw-r--r--   0        0        0     1645 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/company/company_type.py
+-rw-r--r--   0        0        0      980 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/company/data_source.py
+-rw-r--r--   0        0        0    10364 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/domain_model/company/security_types.py
+-rw-r--r--   0        0        0     3515 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/company/targets.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/emission_factor/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/emission_factor/ef_datasources.py
+-rw-r--r--   0        0        0      692 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/emission_factor/emission_type.py
+-rw-r--r--   0        0        0     1260 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/emission_factor/sector.py
+-rw-r--r--   0        0        0     4701 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/geography.py
+-rw-r--r--   0        0        0     3363 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/scope.py
+-rw-r--r--   0        0        0     1037 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/domain_model/units.py
+-rw-r--r--   0        0        0     1297 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/insertors/__init__.py
+-rw-r--r--   0        0        0     3033 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/insertors/commons.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/company/__init__.py
+-rw-r--r--   0        0        0     3236 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/company/company_directory_insertor.py
+-rw-r--r--   0        0        0     4803 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/company/company_emission_insertor.py
+-rw-r--r--   0        0        0     5999 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/company/company_financial_data_insertor.py
+-rw-r--r--   0        0        0     6953 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/company/company_reduction_target_insertor.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/factset/__init__.py
+-rw-r--r--   0        0        0     1197 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/factset/factset_entity_insertor.py
+-rw-r--r--   0        0        0     4402 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/insertors/factset/factset_financial_data_insertor.py
+-rw-r--r--   0        0        0     2042 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/factset/factset_structure_insertor.py
+-rw-r--r--   0        0        0      934 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/insertors/nace_isic_insertor.py
+-rw-r--r--   0        0        0      560 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/__init__.py
+-rw-r--r--   0        0        0     1034 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/commons.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/__init__.py
+-rw-r--r--   0        0        0     3119 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/commons.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/company_directory/__init__.py
+-rw-r--r--   0        0        0     1042 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/company_directory/general_info_insertor.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/__init__.py
+-rw-r--r--   0        0        0     4871 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/cdp_emissions.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/cdp_emissions_modules/__init__.py
+-rw-r--r--   0        0        0     4630 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/cdp_emissions_modules/base_year_ghg.py
+-rw-r--r--   0        0        0    11106 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/cdp_emissions_modules/emissions.py
+-rw-r--r--   0        0        0     2491 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/cdp_emissions_modules/reporting_year.py
+-rw-r--r--   0        0        0     8554 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_emission/cdp_emissions_modules/verifications.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_info/__init__.py
+-rw-r--r--   0        0        0     7743 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/company_info/cdp.py
+-rw-r--r--   0        0        0     5115 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/company_info/company_info_insertor.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_reduction_target/__init__.py
+-rw-r--r--   0        0        0     7804 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_reduction_target/cdp_target.py
+-rw-r--r--   0        0        0     8845 2024-04-04 11:59:29.736492 ecodev_model-0.0.164/ecodev_model/methodo/company/company_reduction_target/commons.py
+-rw-r--r--   0        0        0     6090 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/company_reduction_target/sbt.py
+-rw-r--r--   0        0        0     2720 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/load_data.py
+-rw-r--r--   0        0        0     2481 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/company/search_companies.py
+-rw-r--r--   0        0        0     1146 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/methodo/database_test_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/methodo/factset/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/factset/commons.py
+-rw-r--r--   0        0        0     3575 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/methodo/factset/factset_entity_api.py
+-rw-r--r--   0        0        0     8538 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/factset/factset_fundamentals_api.py
+-rw-r--r--   0        0        0     2106 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/methodo/factset/factset_structure_api.py
+-rw-r--r--   0        0        0     1944 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/factset/financial_data_insertor.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/nlp/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/nlp/company_preprocessors.py
+-rw-r--r--   0        0        0     1309 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/nlp/stop_words/custom_stop_words.json
+-rw-r--r--   0        0        0    74443 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/nlp/stop_words/financial_stop_words.json
+-rw-r--r--   0        0        0     1915 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/methodo/nlp/text_preprocessors.py
+-rw-r--r--   0        0        0     2016 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/company/__init__.py
+-rw-r--r--   0        0        0     7997 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/retrievers/company/company_directory_retrievers.py
+-rw-r--r--   0        0        0     4571 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/company/company_emission_retrievers.py
+-rwxr-xr-x   0        0        0     1930 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/retrievers/company/company_info_retrievers.py
+-rw-r--r--   0        0        0     1686 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/company/company_reduction_target_retrievers.py
+-rwxr-xr-x   0        0        0     4593 2024-04-12 13:45:58.077144 ecodev_model-0.0.164/ecodev_model/retrievers/company/company_retrievers.py
+-rw-r--r--   0        0        0      389 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/company/nace_isic_retrievers.py
+-rw-r--r--   0        0        0     1778 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/company/security_isin_retrievers.py
+-rw-r--r--   0        0        0     1154 2024-04-04 11:59:29.740491 ecodev_model-0.0.164/ecodev_model/retrievers/factset/factset_fundamentals_data_retrievers.py
+-rw-r--r--   0        0        0      679 2024-04-18 12:09:23.877401 ecodev_model-0.0.164/pyproject.toml
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 ecodev_model-0.0.164/PKG-INFO
```

### Comparing `ecodev_model-0.0.1/ecodev_model/emission_type.py` & `ecodev_model-0.0.164/ecodev_model/domain_model/emission_factor/emission_type.py`

 * *Files identical despite different names*

### Comparing `ecodev_model-0.0.1/ecodev_model/sector.py` & `ecodev_model-0.0.164/ecodev_model/domain_model/emission_factor/sector.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from enum import Enum
 from enum import unique
 
 
 @unique
 class Sector(str, Enum):
     """
-    Ppossible emission factor sectors
+    Possible emission factor sectors
 
     NB: close but different from EcoInvent classification!
     see EcoInvent insertor for more details.
     """
     Electricity = 'Electricity'
     Goods_Purchase = 'Purchase of goods'
     Services_Purchase = 'Purchase of services'
```

### Comparing `ecodev_model-0.0.1/ecodev_model/units.py` & `ecodev_model-0.0.164/ecodev_model/domain_model/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module implemeening all unit enums
+Module implementing all unit enums
 """
 from enum import Enum
 from enum import unique
 
 
 @unique
 class BasicUnits(str, Enum):
```

